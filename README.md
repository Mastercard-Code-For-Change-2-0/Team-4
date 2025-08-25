# 🎯 **Donation Management System**

A comprehensive full-stack donation management platform built with modern web technologies.

## 🚀 **Features**

### **🔒 Authentication System**
- Separate donor and receiver authentication
- JWT-based session management
- Role-based access control

### **💝 Donation Management**
- Multi-category donation system (clothes, stationary, food, furniture, electronics)
- Image upload with Cloudinary integration
- Real-time status tracking
- Automatic request-donation matching

### **📋 Request Management**
- Request creation and tracking
- Automatic fulfillment detection
- Status management (pending, approved, fulfilled, rejected)

### **👨‍💼 Admin Panel**
- Real-time dashboard with statistics
- Complete donation and request history
- Status management for matched donations
- Comprehensive reporting

## 🛠️ **Tech Stack**

### **Backend**
- **Node.js** with Express.js
- **MongoDB** with Mongoose ODM
- **JWT** for authentication
- **Multer** + **Cloudinary** for file uploads
- **bcrypt** for password hashing

### **Frontend**
- **React** with Vite
- **Tailwind CSS** for styling
- **Axios** for API calls
- **React Router** for navigation

### **Admin Panel**
- **React** with modern UI components
- **Lucide React** for icons
- **Responsive design** with Tailwind CSS

## 📁 **Project Structure**

```
MasterCard CFC/
├── Backend/
│   ├── Controllers/          # Business logic
│   ├── Models/              # Database schemas
│   ├── Routes/              # API endpoints
│   ├── Config/              # Passport configuration
│   ├── Middlewares/         # Authentication middleware
│   ├── Services/            # Business services
│   ├── Utils/               # Utility functions
│   └── index.js             # Server entry point
├── Frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── hooks/           # Custom hooks
│   │   └── assets/          # Static assets
│   └── package.json
├── admin/
│   ├── src/
│   │   ├── components/      # Admin UI components
│   │   ├── pages/           # Admin pages
│   │   ├── services/        # API services
│   │   └── utils/           # Helper functions
│   └── package.json
└── README.md
```

## 🚀 **Getting Started**

### **Prerequisites**
- Node.js (v14 or higher)
- MongoDB
- Cloudinary account (for image uploads)

### **Backend Setup**
1. Navigate to Backend directory:
   ```bash
   cd Backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create `.env` file with:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

4. Start the server:
   ```bash
   npm start
   ```

### **Frontend Setup**
1. Navigate to Frontend directory:
   ```bash
   cd Frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start development server:
   ```bash
   npm run dev
   ```

### **Admin Panel Setup**
1. Navigate to admin directory:
   ```bash
   cd admin
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start development server:
   ```bash
   npm run dev
   ```

## 🌐 **API Endpoints**

### **Authentication**
- `POST /api/donor/signup` - Donor registration
- `POST /api/donor/signin` - Donor login
- `POST /api/receiver/signup` - Receiver registration
- `POST /api/receiver/signin` - Receiver login

### **Donations**
- `POST /api/donation/donate` - Create donation
- `GET /api/donation/all` - Get all donations

### **Requests**
- `POST /api/request/create` - Create request
- `GET /api/request/all` - Get all requests

### **Admin**
- `GET /api/admin/dashboard` - Dashboard statistics
- `GET /api/admin/history` - Complete history
- `GET /api/admin/matched-donations` - Matched donations
- `PUT /api/admin/donations/:id/status` - Update donation status

## 🎯 **Key Features**

### **Automatic Matching**
- Smart algorithm matches donations with requests
- Real-time status updates
- Automatic fulfillment detection

### **File Upload**
- Secure image uploads to Cloudinary
- Category-based file organization
- Image optimization and transformation

### **Admin Dashboard**
- Real-time statistics and analytics
- Complete transaction history
- Status management interface

## 🔐 **Security Features**

- JWT token-based authentication
- Password hashing with bcrypt
- Protected API routes
- Input validation and sanitization
- CORS configuration

## 🎨 **UI/UX Features**

- Responsive design for all screen sizes
- Modern and intuitive interface
- Loading states and error handling
- Smooth animations and transitions
- Accessibility considerations

## 🤝 **Contributing**

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 **License**

This project is licensed under the MIT License.

## 🙏 **Acknowledgments**

- Built for MasterCard CFC (Code for Change) initiative
- Inspired by the need for efficient donation management systems
- Thanks to all contributors and supporters

---

**Happy Coding! 🚀**
