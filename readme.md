# Personal Portfolio - NextJS Backend

[![API Status](https://img.shields.io/badge/API-Online-brightgreen)](https://portfolio-nextjs-backend.vercel.app/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-blue)](https://github.com/Rakesh01999/portfolio-nextjs-backend)

## 📌 Overview

This is the backend API for my personal portfolio website built with Node.js, Express, and MongoDB. It provides a comprehensive set of REST APIs to manage all content displayed on both the user-facing and admin portions of the portfolio.

## ✨ Features

- **RESTful API** - Well-structured endpoints following REST principles
- **Authentication & Authorization** - JWT-based secure access with role management
- **Database Integration** - MongoDB with Mongoose for data modeling
- **File Uploads** - Support for images and document uploads
- **Validation** - Comprehensive request validation
- **API Documentation** - Auto-generated API documentation
- **Error Handling** - Robust error handling mechanism

## 🔌 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new admin (protected)
- `POST /api/auth/login` - Admin login
- `GET /api/auth/me` - Get current user profile

### Profile Management
- `GET /api/profile` - Get profile information
- `PUT /api/profile` - Update profile information
- `PUT /api/profile/resume` - Update resume/CV

### Education
- `GET /api/education` - Get all education entries
- `POST /api/education` - Add new education entry
- `PUT /api/education/:id` - Update education entry
- `DELETE /api/education/:id` - Delete education entry

### Experience
- `GET /api/experience` - Get all experience entries
- `POST /api/experience` - Add new experience entry
- `PUT /api/experience/:id` - Update experience entry
- `DELETE /api/experience/:id` - Delete experience entry

### Skills
- `GET /api/skills` - Get all skills
- `POST /api/skills` - Add new skill
- `PUT /api/skills/:id` - Update skill
- `DELETE /api/skills/:id` - Delete skill

### Projects
- `GET /api/projects` - Get all projects
- `GET /api/projects/:id` - Get project details
- `POST /api/projects` - Add new project
- `PUT /api/projects/:id` - Update project
- `DELETE /api/projects/:id` - Delete project
- `POST /api/projects/upload` - Upload project images

### Blog
- `GET /api/blogs` - Get all blog posts
- `GET /api/blogs/:id` - Get blog post details
- `POST /api/blogs` - Create new blog post
- `PUT /api/blogs/:id` - Update blog post
- `DELETE /api/blogs/:id` - Delete blog post
- `POST /api/blogs/upload` - Upload blog images

### Contact
- `POST /api/contact` - Submit contact form
- `GET /api/contact` - Get all contact submissions (protected)
- `DELETE /api/contact/:id` - Delete contact submission (protected)

## 🛠️ Technology Stack

- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT (JSON Web Tokens)
- **File Storage**: Cloudinary/AWS S3/Local Storage
- **Validation**: Joi/Express Validator
- **Documentation**: Swagger/OpenAPI
- **Testing**: Jest and Supertest
- **Logging**: Winston/Morgan

## 📦 Database Schema

The MongoDB database includes collections for:
- Users (Admin credentials)
- Profile (Personal information)
- Education
- Experience
- Skills
- Projects
- Blog Posts
- Contact Submissions

## 🚀 Installation & Setup

### Prerequisites
- Node.js 18+ installed
- MongoDB installed locally or connection to MongoDB Atlas

### Installation

1. Clone the repository
```bash
git clone https://github.com/Rakesh01999/portfolio-nextjs-backend
cd portfolio-nextjs-backend
```

2. Install dependencies
```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Configure environment variables
```bash
cp .env.example .env
```
Then edit `.env` with your configuration:
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/portfolio
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRE=30d
NODE_ENV=development
CLOUD_NAME=your_cloudinary_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
```

4. Run the development server
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

5. The API will be available at [http://localhost:5000](http://localhost:5000)

## 📝 API Documentation

API documentation is automatically generated and available at `/api-docs` endpoint when the server is running.

## 🧪 Testing

```bash
# Run tests
npm test
# or
yarn test
```

## 📦 Build & Deployment

```bash
# Build the application
npm run build
# or
yarn build

# Start production server
npm start
# or
yarn start
```

## 🔗 Related Repositories

- [Portfolio - NextJS User Frontend](https://github.com/Rakesh01999/portfolio-nextjs-user-frontend)
- [Portfolio - NextJS Admin Frontend](https://github.com/Rakesh01999/portfolio-nextjs-admin-frontend)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 👨‍💻 Author

Rakesh Biswas - [My Website's -server](https://portfolio-nextjs-backend.vercel.app/)