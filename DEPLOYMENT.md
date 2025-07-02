# 🚀 Deployment Guide

This guide will help you deploy your Food Delivery App to live servers.

## 📋 Prerequisites

1. **GitHub Account** - To store your code
2. **Vercel Account** - For frontend and admin panel deployment
3. **Railway/Render Account** - For backend deployment
4. **MongoDB Atlas** - For database hosting
5. **Stripe Account** - For payment processing

## 🔧 Environment Variables Setup

### Backend (.env)
```env
MONGODB_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_jwt_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
PORT=4000
FRONTEND_URL=https://your-frontend-domain.vercel.app
ADMIN_URL=https://your-admin-domain.vercel.app
```

### Frontend (.env)
```env
VITE_BACKEND_URL=https://your-backend-domain.railway.app
VITE_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
```

### Admin (.env)
```env
VITE_BACKEND_URL=https://your-backend-domain.railway.app
```

## 🚀 Step-by-Step Deployment

### 1. Deploy Backend (Railway/Render)

#### Option A: Railway Deployment
1. Go to [Railway](https://railway.app/)
2. Connect your GitHub repository
3. Select the `backend` folder
4. Add environment variables in Railway dashboard
5. Deploy!

#### Option B: Render Deployment
1. Go to [Render](https://render.com/)
2. Create new Web Service
3. Connect your GitHub repository
4. Set build command: `npm install`
5. Set start command: `npm start`
6. Add environment variables
7. Deploy!

### 2. Deploy Frontend (Vercel)

1. Go to [Vercel](https://vercel.com/)
2. Import your GitHub repository
3. Select the `frontend` folder
4. Add environment variables
5. Deploy!

### 3. Deploy Admin Panel (Vercel)

1. Create another Vercel project
2. Import the same GitHub repository
3. Select the `admin` folder
4. Add environment variables
5. Deploy!

## 📱 Live URLs

After deployment, you'll get these URLs:
- **Frontend**: `https://your-app-name.vercel.app`
- **Admin Panel**: `https://your-admin-name.vercel.app`
- **Backend API**: `https://your-backend-name.railway.app`

## 🔐 Security Checklist

- [ ] All environment variables are set correctly
- [ ] CORS is configured for your domains
- [ ] JWT secret is secure and unique
- [ ] MongoDB database is properly secured
- [ ] Stripe webhooks are configured (if using)

## 🎯 Testing Deployment

1. Test API endpoints: `https://your-backend-url/api/food`
2. Test frontend functionality
3. Test admin panel operations
4. Test payment flow (use Stripe test cards)

## 📞 Support

If you encounter any issues during deployment, check:
1. Build logs in deployment platform
2. Environment variables are correctly set
3. API endpoints are accessible
4. Database connection is working

---

Happy Deploying! 🚀
