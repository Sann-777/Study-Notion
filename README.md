# StudyNotion - Legacy Monolithic Application

This folder contains the original monolithic version of the StudyNotion EdTech platform.

## 📁 Structure

```
monolithic-legacy/
├── src/                    # React frontend source code
│   ├── components/         # React components
│   ├── pages/             # Page components
│   ├── services/          # API services
│   ├── utils/             # Utility functions
│   ├── App.jsx            # Main App component
│   └── index.js           # Entry point
├── server/                # Express.js backend
│   ├── controllers/       # Route controllers
│   ├── models/           # MongoDB models
│   ├── routes/           # API routes
│   ├── middleware/       # Custom middleware
│   ├── config/           # Configuration files
│   └── index.js          # Server entry point
├── public/               # Static assets
├── package.json          # Dependencies and scripts
└── README.md            # This file
```

## 🚀 Running the Legacy Application

### Prerequisites
- Node.js v16+
- MongoDB running locally or connection string
- npm or yarn

### Setup & Run
```bash
# Install dependencies
npm install

# Start both frontend and backend
npm run dev

# Or run separately:
npm start          # Frontend only (port 3000)
npm run server     # Backend only (port 4000)
```

### Environment Variables
Create a `.env` file in the `server/` directory:
```env
MONGODB_URI=mongodb://localhost:27017/studynotion
JWT_SECRET=your-jwt-secret
MAIL_HOST=smtp.gmail.com
MAIL_USER=your-email@gmail.com
MAIL_PASS=your-app-password
CLOUD_NAME=your-cloudinary-name
API_KEY=your-cloudinary-key
API_SECRET=your-cloudinary-secret
RAZORPAY_KEY=your-razorpay-key
RAZORPAY_SECRET=your-razorpay-secret
```

## 🔄 Migration to Microservices

This legacy application has been migrated to a microservices architecture. The new implementation can be found in:
- `../frontend-microservice/` - Modern React frontend with TypeScript
- `../microservices/` - Backend microservices

## 📝 Notes

- This is the original monolithic implementation
- Kept for reference and backward compatibility
- New development should use the microservices architecture
- This version may not receive active updates

## 🆘 Support

For issues with the legacy application, please refer to the main project documentation or create an issue in the repository.
