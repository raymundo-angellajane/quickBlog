# quickBlog

## Description

Quickblog is a full-stack blog application designed for creating, managing, and sharing blog posts. It features a modern, responsive frontend built with React and Vite, along with a robust backend powered by Node.js and Express. The application supports user authentication, blog post creation and editing, comment management, and an admin dashboard for content oversight.

### Key Features

- **Blog Management**: Create, edit, delete, and publish blog posts with rich text editing using Quill.
- **User Authentication**: Secure login system for admin users using JWT tokens.
- **Comments System**: Allow readers to leave comments on blog posts.
- **Admin Dashboard**: Comprehensive dashboard for managing blogs, comments, and analytics.
- **Image Upload**: Integrated with ImageKit for seamless image uploads and management.
- **Responsive Design**: Mobile-friendly UI built with TailwindCSS and enhanced with Motion for animations.
- **Markdown Support**: Render blog content using Marked for Markdown parsing.
- **Real-time Notifications**: Toast notifications for user feedback using React Hot Toast.

### Tech Stack

#### Frontend
- **React**: Component-based UI library for building the user interface.
- **Vite**: Fast build tool and development server.
- **TailwindCSS**: Utility-first CSS framework for styling.
- **React Router**: Client-side routing for navigation.
- **Axios**: HTTP client for API requests.
- **Quill**: Rich text editor for blog content creation.
- **Motion**: Animation library for smooth UI transitions.
- **Marked**: Markdown parser for rendering blog posts.

#### Backend
- **Node.js**: JavaScript runtime for server-side logic.
- **Express**: Web framework for building RESTful APIs.
- **MongoDB**: NoSQL database for storing blog data, comments, and user information.
- **Mongoose**: ODM for MongoDB to manage data models.
- **JWT**: JSON Web Tokens for authentication.
- **Multer**: Middleware for handling file uploads.
- **ImageKit**: Image management and optimization service.
- **Google Generative AI**: Integrated for potential AI-powered features (e.g., content suggestions).
- **CORS**: Cross-origin resource sharing for API access.

### Project Structure

- **client/**: Frontend React application.
- **server/**: Backend Node.js/Express API server.
- **README.md**: Project documentation.

### Getting Started

#### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- ImageKit account for image uploads
- Google Generative AI API key (optional)

#### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd quickBlog
   ```

2. **Install server dependencies**:
   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies**:
   ```bash
   cd ../client
   npm install
   ```

4. **Set up environment variables**:
   - Create a `.env` file in the `server` directory with the following variables:
     ```
     MONGODB_URI=<your-mongodb-connection-string>
     JWT_SECRET=<your-jwt-secret>
     IMAGEKIT_PUBLIC_KEY=<your-imagekit-public-key>
     IMAGEKIT_PRIVATE_KEY=<your-imagekit-private-key>
     IMAGEKIT_URL_ENDPOINT=<your-imagekit-url-endpoint>
     GOOGLE_API_KEY=<your-google-generative-ai-api-key>
     ```

5. **Start the backend server**:
   ```bash
   cd server
   npm run server
   ```

6. **Start the frontend development server**:
   ```bash
   cd ../client
   npm run dev
   ```

7. **Access the application**:
   - Frontend: http://localhost:5173 (default Vite port)
   - Backend API: http://localhost:4000 (or configured port)

### Usage

- **Admin Login**: Access the admin dashboard at `/admin/login` to manage blogs and comments.
- **Creating Blogs**: Use the rich text editor to create and publish new blog posts.
- **Viewing Blogs**: Browse published blogs on the home page and individual blog pages.
- **Comments**: Readers can leave comments on blog posts (requires implementation of user authentication for comments if desired).

### Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

### License

This project is licensed under the ISC License.
