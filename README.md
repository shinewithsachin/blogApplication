# Blog Application

A full-featured blog application built using **Node.js**, **Express.js**, **EJS**, **Multer**, and **MongoDB**. This application allows users to create blog posts, as well as upload images to accompany their posts.

## Features

- **Create Blog Posts**: Users can create new blog posts, update existing ones, and delete posts.
- **Image Upload**: Supports uploading images for blog posts using **Multer**.
- **Responsive UI**: Built with **EJS** templates to serve dynamic content and present it in a clean, responsive layout.
- **MongoDB Integration**: Blog posts and images are stored and retrieved from a **MongoDB** database.
- **User Authentication**: (Optional) Extend the application to include user authentication and authorization.

## Technologies Used

- **Node.js**: Server-side JavaScript runtime environment.
- **Express.js**: Framework for building the backend API.
- **EJS**: Templating engine to dynamically render HTML pages.
- **Multer**: Middleware for handling file uploads (images).
- **MongoDB**: NoSQL database for storing blog posts and user data.

## Installation

### Prerequisites

- Node.js (v14 or later)
- MongoDB

### Setup

1. **Clone the repository**:
    ```bash
    git clone https://github.com/shinewithsachin/blog-app.git
    cd blog-app
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Set up environment variables**:
    Create a `.env` file in the root directory and add the following:
    ```bash
    MONGO_URL = mongodb://localhost:27017/blogify
    PORT = 8000
    ```

4. **Run the application**:
    ```bash
    npm start
    ```

5. **Visit the application**:
    Open your browser and navigate to `http://localhost:8000`.

## Usage

- **Home Page**: Displays all blog posts.
- **Create Post**: Navigate to the "Create Post" page to create a new blog with an image.
- **Upload Image**: When creating a new post, you can upload an image using the provided form.

## File Structure

```
blog-app/
│
├── models/
│   └── Post.js        # Mongoose schema for blog posts
│
├── public/
│   └── uploads/       # Stores uploaded images
│
├── routes/
│   └── index.js       # Routes for handling blog operations
│
├── views/
│   ├── index.ejs      # Homepage (list of blog posts)
│   ├── create.ejs     # Form to create a new post
│   └── partials/      # Reusable components (e.g., header, footer)
│
├── app.js             # Main application file
├── .env               # Environment variables
├── package.json       # Project dependencies and scripts
└── README.md          # Project documentation
```

## Dependencies

- **express**: Web framework for Node.js.
- **ejs**: Template engine for rendering HTML.
- **multer**: Middleware for handling file uploads.
- **mongoose**: ODM for MongoDB.
- **dotenv**: Loads environment variables from a `.env` file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
