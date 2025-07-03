# 🍕 Food Delivery App - MERN Stack

A full-stack food delivery application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) featuring Stripe payment integration, real-time order management, and a comprehensive admin panel.


## 🌐 Live Demo

| Component | Live URL | Description |
|-----------|----------|-------------|
| 🛒 **Customer App** | [https://kaleidoscopic-dolphin-f2171b.netlify.app](https://kaleidoscopic-dolphin-f2171b.netlify.app) | Main food ordering application |
| 🔧 **Admin Panel** | [https://capable-rolypoly-60bb52.netlify.app](https://capable-rolypoly-60bb52.netlify.app) | Restaurant management dashboard |
| 🚀 **Backend API** | [https://foodiegoo.onrender.com](https://foodiegoo.onrender.com) | RESTful API server |

> **✅ All services deployed successfully!** - Frontend, Admin, and Backend are all live.

### 🎯 Quick Test
- **Customer App**: Browse menu, add items to cart, and place orders
- **Admin Panel**: Manage orders, add food items, and track deliveries
- **Test Payments**: Use Stripe test cards (4242 4242 4242 4242)

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

## 📸 Screenshots

<div align="center">
  <img src="frontend/src/assets/logo.png" alt="FoodieGoo Logo" width="120" style="margin-bottom: 20px; opacity: 0.8;"/>
  <h3>🍕 Application Showcase</h3>
</div>

This project includes comprehensive screenshots showcasing all three main components:

---

### 🛒 Frontend (Customer App)

#### 🏠 Home Page & Menu
<table align="center">
<tr>
<td align="center" width="50%">
<img src="ScreenShots/frontend/home.png" alt="Home Page" width="100%"/>
<br/><em>Modern homepage with hero section and categories</em>
</td>
<td align="center" width="50%">
<img src="ScreenShots/frontend/menu.png" alt="Menu Page" width="100%"/>
<br/><em>Comprehensive food menu with filtering</em>
</td>
</tr>
</table>

#### 🔐 Authentication System
<table align="center">
<tr>
<td align="center" width="50%">
<img src="ScreenShots/frontend/login.png" alt="Login Page" width="100%"/>
<br/><em>Secure login form with validation</em>
</td>
<td align="center" width="50%">
<img src="ScreenShots/frontend/signup.png" alt="Signup Page" width="100%"/>
<br/><em>User registration with form validation</em>
</td>
</tr>
</table>

#### 🛒 Shopping & Order Flow
<table align="center">
<tr>
<td align="center" width="33%">
<img src="ScreenShots/frontend/dishes.png" alt="Food Items" width="100%"/>
<br/><em>Food items with add to cart</em>
</td>
<td align="center" width="33%">
<img src="ScreenShots/frontend/cart_page.png" alt="Cart Page" width="100%"/>
<br/><em>Shopping cart management</em>
</td>
<td align="center" width="33%">
<img src="ScreenShots/frontend/placeorder_page.png" alt="Place Order" width="100%"/>
<br/><em>Checkout and payment selection</em>
</td>
</tr>
</table>

#### 📦 Order Tracking & Site Footer
<table align="center">
<tr>
<td align="center" width="50%">
<img src="ScreenShots/frontend/orders_page.png" alt="Orders Page" width="100%"/>
<br/><em>Real-time order status tracking</em>
</td>
<td align="center" width="50%">
<img src="ScreenShots/frontend/footer.png" alt="Footer" width="100%"/>
<br/><em>Site footer with social links</em>
</td>
</tr>
</table>

---

### 🔧 Admin Panel

#### 📊 Dashboard & Order Management
<table align="center">
<tr>
<td align="center" width="50%">
<img src="ScreenShots/admin/admin_mainpage.png" alt="Admin Dashboard" width="100%"/>
<br/><em>Admin dashboard with navigation</em>
</td>
<td align="center" width="50%">
<img src="ScreenShots/admin/admin_orderlist.png" alt="Order Management" width="100%"/>
<br/><em>Real-time order management system</em>
</td>
</tr>
</table>

#### 🍕 Food Item Management
<div align="center">
<img src="ScreenShots/admin/admin_itemlist.png" alt="Food Items Management" width="80%"/>
<br/><em>Add, edit, and manage food items with image uploads</em>
</div>

---

### 🖥️ Backend & Database

#### 💾 MongoDB Database Collections
<table align="center">
<tr>
<td align="center" width="50%">
<img src="ScreenShots/backend/mongodb_users_database.png" alt="Users Database" width="100%"/>
<br/><em>User collection with authentication data</em>
</td>
<td align="center" width="50%">
<img src="ScreenShots/backend/mongodb_orders_Database.png" alt="Orders Database" width="100%"/>
<br/><em>Orders collection with payment status</em>
</td>
</tr>
</table>

#### 🔧 API Testing & Payment Integration
<table align="center">
<tr>
<td align="center" width="50%">
<img src="ScreenShots/backend/postman_client_backend.png" alt="API Testing" width="100%"/>
<br/><em>RESTful API endpoints via Postman</em>
</td>
<td align="center" width="50%">
<img src="ScreenShots/backend/stripe_backend.png" alt="Stripe Integration" width="100%"/>
<br/><em>Secure payment processing with Stripe</em>
</td>
</tr>
</table>

---

<div align="center">
  <img src="frontend/src/assets/logo.png" alt="FoodieGoo" width="80" style="opacity: 0.5; margin: 20px 0;"/>
  <br/>
  <em>🍕 FoodieGoo - Complete Food Delivery Solution 🚀</em>
</div>

## �🛠️ Tech Stack

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
FoodieGoo/
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

## 📱 API Endpoints (POSTMAN)

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
