# 🍕 Food Delivery App - MERN Stack

A full-stack food delivery application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) featuring Stripe payment integration, real-time order management, and a comprehensive admin panel.

## 🌟 Features

### 🛒 Frontend (Customer App)
- **Modern UI/UX** - Clean, responsive design with modern styling
- **User Authentication** - Secure login/register system with JWT tokens
- **Food Menu** - Browse categorized food items with detailed descriptions
- **Smart Cart** - Add/remove items with quantity management
- **Multiple Payment Methods**:
  - 💳 Credit/Debit Card (Stripe integration)
  - 📱 UPI Payment (Coming soon)
  - 💵 Cash on Delivery (COD)
- **Order Tracking** - Real-time order status updates
- **Location Services** - Get current location for delivery
- **Order History** - View past orders and their status

### 🔧 Admin Panel
- **Order Management** - View, update, and track all orders
- **Real-time Updates** - Auto-refresh every 10 seconds
- **Food Management** - Add, edit, and delete food items
- **Status Updates** - Change order status (Processing → Out for Delivery → Delivered)
- **Order Analytics** - Total orders count and payment status
- **Notification System** - Alert sounds and visual indicators for new orders

### 🚀 Backend API
- **RESTful API** - Clean API endpoints for all operations
- **JWT Authentication** - Secure user authentication
- **Stripe Integration** - Secure payment processing
- **MongoDB Database** - Efficient data storage and retrieval
- **File Upload** - Image upload for food items
- **Order Verification** - Payment verification system

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI library
- **React Router** - Navigation
- **Axios** - HTTP client
- **CSS3** - Styling
- **Vite** - Build tool

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM
- **JWT** - Authentication
- **Stripe** - Payment processing
- **Multer** - File uploads
- **bcrypt** - Password hashing
- **CORS** - Cross-origin requests

## 📁 Project Structure

```
food-del/
├── 📱 frontend/          # React customer app
│   ├── src/
│   │   ├── components/   # Reusable components
│   │   ├── pages/        # Page components
│   │   ├── context/      # React context
│   │   └── assets/       # Images and static files
│   └── package.json
├── 🔧 admin/            # React admin panel
│   ├── src/
│   │   ├── components/   # Admin components
│   │   ├── pages/        # Admin pages
│   │   └── assets/       # Admin assets
│   └── package.json
├── 🖥️ backend/          # Node.js API server
│   ├── controllers/      # Route controllers
│   ├── models/          # Database models
│   ├── routes/          # API routes
│   ├── middleware/      # Custom middleware
│   ├── config/          # Database config
│   ├── uploads/         # Uploaded images
│   └── package.json
├── 📚 README.md         # Project documentation
├── 🚀 start.sh          # Quick start script
├── ⚡ QUICK_START.md    # Quick setup guide
└── 💳 STRIPE_SETUP.md   # Stripe integration guide
```

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud)
- Stripe account (for payments)

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/food-delivery-app.git
cd food-delivery-app
```

### 2. Environment Setup
Create `.env` file in the `backend` directory:
```env
# JWT Secret for authentication
JWT_SECRET="your_jwt_secret_key"

# MongoDB connection string
MONGODB_URI="mongodb+srv://username:password@cluster.mongodb.net/food-delivery"

# Stripe Secret Key (get from https://dashboard.stripe.com/apikeys)
STRIPE_SECRET_KEY="sk_test_your_stripe_secret_key"
```

### 3. Install Dependencies & Start
```bash
# Make start script executable
chmod +x start.sh

# Run the complete application
./start.sh
```

**Or start manually:**

```bash
# Backend
cd backend
npm install
npm run server

# Frontend (new terminal)
cd frontend
npm install
npm run dev

# Admin Panel (new terminal)
cd admin
npm install
npm run dev
```

### 4. Access the Application
- **Frontend**: http://localhost:5173
- **Admin Panel**: http://localhost:5174
- **Backend API**: http://localhost:4000

## 💳 Payment Integration

### Stripe Setup
1. Create account at [Stripe Dashboard](https://dashboard.stripe.com/)
2. Get your API keys from "Developers" → "API Keys"
3. Add the secret key to your `.env` file
4. Use test cards for development:
   - **Success**: `4242 4242 4242 4242`
   - **Decline**: `4000 0000 0000 0002`
   - **Expiry**: Any future date
   - **CVC**: Any 3 digits

### Payment Flow
1. **Card Payment**: Redirects to Stripe's secure checkout
2. **COD**: Processes order immediately
3. **Verification**: Confirms payment and updates order status

## 📱 API Endpoints

### Authentication
```
POST /api/user/register    # User registration
POST /api/user/login       # User login
```

### Food Items
```
GET  /api/food/list        # Get all food items
POST /api/food/add         # Add new food item (admin)
POST /api/food/remove      # Remove food item (admin)
```

### Orders
```
POST /api/order/place      # Place order with Stripe
POST /api/order/place-cod  # Place COD order
POST /api/order/verify     # Verify payment
POST /api/order/userorders # Get user orders
GET  /api/order/list       # Get all orders (admin)
POST /api/order/status     # Update order status (admin)
```

### Cart
```
POST /api/cart/add         # Add to cart
POST /api/cart/remove      # Remove from cart
POST /api/cart/get         # Get cart items
```

## 🔄 Real-time Features

### Admin Panel Auto-refresh
- Orders refresh every 10 seconds automatically
- Visual and audio notifications for new orders
- Manual refresh button available
- Order count tracking

### Order Status Flow
1. **Food Processing** (default)
2. **Out for Delivery**
3. **Delivered**

## 🎨 UI Features

### Customer App
- Responsive design for all devices
- Interactive cart with quantity controls
- Payment method selection
- Order summary before checkout
- Order history with status tracking

### Admin Panel
- Real-time order notifications
- Sortable order list (newest first)
- Order details with customer information
- Payment status indicators
- Quick status updates

## 🧪 Testing

### Test User Accounts
Create test accounts through the registration process or use:
- Email: `test@example.com`
- Password: `password123`

### Test Orders
1. Add items to cart
2. Fill delivery information
3. Select payment method
4. Place order
5. Check admin panel for order appearance

### Test Payments
Use Stripe test cards:
- Success: `4242 4242 4242 4242`
- Failure: `4000 0000 0000 0002`

## 🔧 Configuration

### Database Models

#### User Model
```javascript
{
  name: String,
  email: String (unique),
  password: String (hashed),
  cartData: Object
}
```

#### Food Model
```javascript
{
  name: String,
  description: String,
  price: Number,
  image: String,
  category: String
}
```

#### Order Model
```javascript
{
  userId: String,
  items: Array,
  amount: Number,
  address: Object,
  status: String,
  date: Date,
  payment: Boolean
}
```

## 🚀 Deployment

### Backend Deployment (e.g., Heroku)
1. Set environment variables
2. Update MongoDB URI for production
3. Replace Stripe test keys with live keys
4. Deploy using git

### Frontend Deployment (e.g., Netlify/Vercel)
1. Update API URLs for production
2. Build the project: `npm run build`
3. Deploy the `dist` folder

### Important for Production
- Use HTTPS for secure payments
- Set up proper CORS policies
- Enable Stripe webhooks for reliable payment processing
- Set up proper error logging
- Configure rate limiting

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow ES6+ standards
- Use meaningful commit messages
- Test your changes thoroughly
- Update documentation as needed
