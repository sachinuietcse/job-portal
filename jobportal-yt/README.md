# Job Portal - Full Stack Application

A modern, responsive job portal application built with the MERN stack (MongoDB, Express.js, React, Node.js) that connects job seekers with employers.

## 🚀 Features

### For Job Seekers
- **User Registration & Authentication**: Secure signup/login system with JWT authentication
- **Profile Management**: Complete profile creation with resume upload
- **Job Search & Filter**: Advanced job filtering by category, location, and company
- **Job Applications**: Apply to jobs with one-click application system
- **Application Tracking**: View and manage all job applications
- **Company Browsing**: Explore companies and their job openings

### For Employers/Admin
- **Company Management**: Create and manage company profiles
- **Job Posting**: Post new job opportunities with detailed descriptions
- **Applicant Management**: View and manage job applications
- **Admin Dashboard**: Comprehensive dashboard for managing jobs and applications
- **Protected Routes**: Secure admin-only areas

### General Features
- **Responsive Design**: Beautiful, mobile-friendly UI built with Tailwind CSS
- **Real-time Notifications**: Toast notifications for user actions
- **Image Upload**: Cloudinary integration for profile pictures and company logos
- **State Management**: Redux Toolkit for efficient state management
- **Modern UI Components**: Radix UI components with custom styling

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern React with hooks
- **Vite** - Fast build tool and development server
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Accessible UI components
- **Redux Toolkit** - State management
- **React Router** - Client-side routing
- **Axios** - HTTP client
- **Framer Motion** - Animations
- **Lucide React** - Icons

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB ODM
- **JWT** - Authentication
- **bcryptjs** - Password hashing
- **Cloudinary** - Image storage
- **Multer** - File upload handling

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **MongoDB** (local installation or MongoDB Atlas)
- **Cloudinary Account** (for image uploads)

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone <repository-url>
cd jobportal-yt
```

### 2. Backend Setup

Navigate to the backend directory:
```bash
cd backend
```

Install dependencies:
```bash
npm install
```

Create a `.env` file in the backend directory:
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
PORT=8000
```

Start the backend server:
```bash
npm run dev
```

The backend server will run on `http://localhost:8000`

### 3. Frontend Setup

Open a new terminal and navigate to the frontend directory:
```bash
cd frontend
```

Install dependencies:
```bash
npm install
```

Start the frontend development server:
```bash
npm run dev
```

The frontend will run on `http://localhost:5173`

## 📁 Project Structure

```
jobportal-yt/
├── backend/
│   ├── controllers/          # Request handlers
│   ├── middlewares/          # Custom middleware
│   ├── models/              # Database models
│   ├── routes/              # API routes
│   ├── utils/               # Utility functions
│   ├── index.js             # Server entry point
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── hooks/           # Custom React hooks
│   │   ├── redux/           # Redux store and slices
│   │   ├── utils/           # Utility functions
│   │   ├── App.jsx          # Main App component
│   │   └── main.jsx         # Entry point
│   ├── public/              # Static assets
│   └── package.json
└── README.md
```

## 🔐 Environment Variables

### Backend (.env)
```env
MONGO_URI=mongodb://localhost:27017/jobportal
JWT_SECRET=your_super_secret_jwt_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
PORT=8000
```

## 🚀 API Endpoints

### Authentication
- `POST /api/v1/user/register` - User registration
- `POST /api/v1/user/login` - User login
- `POST /api/v1/user/logout` - User logout

### User Management
- `GET /api/v1/user/profile` - Get user profile
- `POST /api/v1/user/profile/update` - Update user profile

### Company Management
- `GET /api/v1/company` - Get all companies
- `POST /api/v1/company/register` - Register new company
- `GET /api/v1/company/:id` - Get company by ID
- `PUT /api/v1/company/:id` - Update company

### Job Management
- `GET /api/v1/job` - Get all jobs
- `POST /api/v1/job/post` - Post new job
- `GET /api/v1/job/:id` - Get job by ID
- `GET /api/v1/job/admin` - Get admin jobs

### Applications
- `POST /api/v1/application/apply/:id` - Apply to job
- `GET /api/v1/application` - Get user applications
- `GET /api/v1/application/:id/applicants` - Get job applicants

## 🎨 Features in Detail

### User Authentication
- Secure JWT-based authentication
- Password hashing with bcryptjs
- Protected routes for authenticated users
- Persistent login state with Redux Persist

### File Upload
- Cloudinary integration for image storage
- Profile picture and resume upload
- Company logo upload
- Optimized image delivery

### Responsive Design
- Mobile-first approach
- Modern UI with Tailwind CSS
- Accessible components with Radix UI
- Smooth animations with Framer Motion

### State Management
- Redux Toolkit for global state
- Separate slices for different features
- Async actions with createAsyncThunk
- Persistent state across sessions

## 🧪 Development

### Frontend Development
```bash
cd frontend
npm run dev     # Start development server
npm run build   # Build for production
npm run preview # Preview production build
```

### Backend Development
```bash
cd backend
npm run dev     # Start with nodemon
```

## 🚀 Deployment

### Frontend (Netlify/Vercel)
1. Build the project: `npm run build`
2. Deploy the `dist` folder to your hosting platform

### Backend (Railway/Render/Heroku)
1. Set environment variables
2. Deploy the backend folder
3. Update CORS origin in backend to match frontend URL

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/new-feature`
3. Commit your changes: `git commit -m 'Add new feature'`
4. Push to the branch: `git push origin feature/new-feature`
5. Submit a pull request

## 📝 License

This project is licensed under the ISC License.

## 👥 Authors

- **Developer Name** - Initial work

## 🙏 Acknowledgments

- React team for the amazing framework
- Tailwind CSS for the utility-first CSS framework
- Radix UI for accessible components
- MongoDB team for the database
- All open-source contributors

## 📞 Support

For support, email your-email@example.com or create an issue in the repository.

---

**Happy Coding! 🚀**
