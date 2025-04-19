# Forever - Ecommerce Platform

A full-stack ecommerce platform with user and admin interfaces built using React, Node.js, and MongoDB.

## Features

### Customer Features
- Browse product catalog with filtering and search
- User authentication and account management 
- Shopping cart functionality
- Multiple payment options (Stripe, Razorpay, COD)
- Order tracking
- Responsive design for all devices

### Admin Features
- Product management (Add/Remove products)
- Order management with status updates
- Secure admin authentication
- Image upload with Cloudinary integration
- Sales tracking and monitoring

## Tech Stack

### Frontend
- React.js with Vite
- React Router for navigation
- TailwindCSS for styling
- Axios for API calls
- React Toastify for notifications

### Backend
- Node.js & Express
- MongoDB with Mongoose
- JWT for authentication
- Cloudinary for image storage
- Stripe & Razorpay payment gateways

## Project Structure
```
ecomm project/
├── frontend/           # Customer facing application
├── admin/             # Admin dashboard application  
└── backend/           # API server
```

## Getting Started

1. Clone the repository
2. Install dependencies for each component:
```bash
# Install frontend dependencies
cd frontend
npm install

# Install admin dependencies
cd ../admin
npm install

# Install backend dependencies
cd ../backend
npm install
```

3. Configure environment variables:

Create `.env` files in each directory with the following variables:

Backend:
```
JWT_SECRET=your_jwt_secret
MONGODB_URI=your_mongodb_uri
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret
CLOUDINARY_NAME=your_cloudinary_name
STRIPE_SECRET_KEY=your_stripe_secret
RAZORPAY_KEY_SECRET=your_razorpay_secret
RAZORPAY_KEY_ID=your_razorpay_key
```

Frontend:
```
VITE_BACKEND_URL=http://localhost:4000
VITE_RAZORPAY_KEY_ID=your_razorpay_key
```

Admin:
```
VITE_BACKEND_URL=http://localhost:4000
```

4. Start the applications:

```bash
# Start backend server
cd backend
npm run server

# Start frontend application
cd frontend
npm run dev

# Start admin application
cd admin
npm run dev
```

## Default Ports
- Backend: 4000
- Frontend: 5173
- Admin: 5174

## Admin Access
Default admin credentials:
- Email: admin@example.com
- Password: greatstack123

## Contributing
Feel free to submit issues and pull requests.

## License
MIT License