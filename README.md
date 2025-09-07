# 📚 Online Quiz Portal

A comprehensive web-based examination system built with the MERN stack, designed to facilitate seamless online quiz administration and management for educational institutions.

## 🎯 Overview

The Online Quiz Portal is a full-stack web application that provides a complete solution for conducting online examinations. It offers separate interfaces for administrators and students, ensuring secure, efficient, and user-friendly exam management.

## ✨ Key Features

### 👨‍💼 Admin Features
- **Dashboard Management** - Comprehensive admin dashboard with analytics
- **Exam Creation** - Create and manage multiple choice questions
- **Category Management** - Organize exams by subjects/categories
- **Student Management** - View and manage registered students
- **Result Analytics** - Detailed performance reports with visualizations
- **Data Export** - Download results as Excel sheets

### 👨‍🎓 Student Features
- **User Registration & Login** - Secure authentication system
- **Exam Taking** - Interactive quiz interface with timer
- **Result Viewing** - Instant results with detailed feedback
- **Performance Tracking** - View exam history and progress
- **Responsive Design** - Works seamlessly on all devices

### 🔒 Security Features
- **JWT Authentication** - Secure token-based authentication
- **Password Encryption** - bcrypt hashing for password security
- **Role-based Access** - Separate permissions for admin and students
- **Session Management** - Secure user session handling

## 🛠️ Tech Stack

### Frontend
- **React.js** - User interface library
- **React Router** - Client-side routing
- **Axios** - HTTP client for API calls
- **React Bootstrap** - UI component library
- **CSS3** - Styling and responsive design

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Tokens for authentication
- **bcrypt** - Password hashing
- **CORS** - Cross-origin resource sharing

### Database
- **MongoDB** - NoSQL document database
- **MongoDB Atlas** - Cloud database service (optional)

### Additional Tools
- **Nodemailer** - Email notifications
- **Express Validator** - Input validation
- **Dotenv** - Environment variable management

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/online-quiz-portal.git
   cd online-quiz-portal
   ```

2. **Install dependencies**
   ```bash
   # Install backend dependencies
   npm install
   
   # Install frontend dependencies
   cd src
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory:
   ```env
   MONGO_URI=mongodb://localhost:27017/online-quiz-portal
   JWT_SECRET=your-super-secret-jwt-key-here
   PORT=5001
   REACT_APP_ADMIN_ROUTE=admin/dashbord
   ```

4. **Start the application**
   ```bash
   # Start the backend server
   npm start
   
   # Start the frontend (in a new terminal)
   cd src
   npm start
   ```

5. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5001
   - Admin Panel: http://localhost:3000/admin/login

## 📱 Usage

### For Students
1. Register a new account or login
2. Browse available courses and exams
3. Take exams with real-time timer
4. View results and performance history

### For Administrators
1. Login with admin credentials
2. Create and manage exam categories
3. Add questions and create exams
4. Monitor student performance
5. Export results and analytics

## 🔧 API Endpoints

### Authentication
- `POST /api/users/register` - User registration
- `POST /api/users/login` - User login
- `POST /adminlogin` - Admin login

### Exams
- `GET /api/exams` - Get all exams
- `POST /api/exams` - Create new exam
- `PUT /api/exams/:id` - Update exam
- `DELETE /api/exams/:id` - Delete exam

### Questions
- `GET /api/questions` - Get all questions
- `POST /api/questions` - Create new question
- `PUT /api/questions/:id` - Update question
- `DELETE /api/questions/:id` - Delete question

### Results
- `GET /api/results` - Get all results
- `POST /api/results` - Submit exam result
- `GET /api/results/:userId` - Get user results

## 📁 Project Structure

```
online-quiz-portal/
├── api/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   │   ├── userController.js
│   │   ├── examController.js
│   │   ├── questionController.js
│   │   └── resultController.js
│   ├── models/
│   │   ├── user.js
│   │   ├── exam.js
│   │   ├── question.js
│   │   └── result.js
│   └── routes/
│       └── courseRoutes.js
├── public/
│   └── assets/
├── src/
│   ├── components/
│   │   ├── Admin/
│   │   ├── Student/
│   │   ├── pages/
│   │   └── UIElements/
│   ├── App.js
│   └── index.js
├── server.js
└── package.json
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

