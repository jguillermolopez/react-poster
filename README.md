# React Poster

A full-stack React.js application for creating and viewing short posts. This project features a modern frontend built with Vite and React Router, and a lightweight Express.js backend for storing posts in a local JSON file. Styling is handled using module.css.

## 🚀 Features

- 🧭 Routing with React Router
- 💬 Create, view, and list posts
- 🎨 Modal interface for post creation and details
- 🧩 Component-based UI
- 🗃️ Node.js backend with file-based storage
- 📦 Built with Vite for fast development

## 🛠️ Technologies

### Frontend

- React.js (via Vite)
- React Router
- CSS Modules
- React Icons

### Backend

- Node.js
- Express.js
- fs/promises for file storage

## 🧱 Project Structure

react-poster/
├── backend/
│ ├── app.js
│ ├── posts.json
│ └── data/
│ └── posts.js
├── frontend/
│ ├── index.html
│ ├── package.json
│ ├── vite.config.js
│ └── src/
│ ├── components/
│ │ ├── MainHeader.jsx
│ │ ├── MainHeader.module.css
│ │ ├── Modal.jsx
│ │ ├── Modal.module.css
│ │ ├── Post.jsx
│ │ ├── Post.module.css
│ │ ├── PostList.jsx
│ │ └── PostList.module.css
│ ├── routes/
│ │ ├── RootLayout.jsx
│ │ ├── Posts.jsx
│ │ ├── NewPost.jsx
│ │ ├── NewPost.module.css
│ │ ├── PostDetails.jsx
│ │ └── PostDetails.module.css
│ ├── main.jsx
│ └── index.css

## 📦 Installation & Setup

### 📁 Clone the Repository

```bash
git clone https://github.com/your-username/react-poster.git
cd react-poster
```

### 📱 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend runs on http://localhost:5173

### 🌐 Backend Setup

```bash
cd backend
npm install
node app.js
```

## 🔄 API Endpoints

| Method | Endpoint     | Description         |
| ------ | ------------ | ------------------- |
| GET    | `/posts`     | Fetch all posts     |
| GET    | `/posts/:id` | Fetch a single post |
| POST   | `/posts`     | Create a new post   |

## 🧪 How It Works

- Users create posts using a modal form.
- Posts are stored in posts.json via the backend.
- Each post is dynamically fetched and rendered.
- Modal-based routing handles both form submission and detail view.

## ✅ Requirements

- Node.js v16+
- npm v8+
- Modern browser (Chrome, Firefox, Edge, etc.)

## 📂 Example `posts.json`

```json
{
  "posts": [
    {
      "id": "abc123",
      "author": "Jane Doe",
      "body": "This is a test post"
    }
  ]
}
```

## 🧹 Future Improvements

- Edit/Delete post features
- Persistent storage using a real database
- Authentication & User system
- Production deployment instructions

## 📄 License

This project is licensed under the MIT License.

## 👤 Author

Made with ❤️ by Jose Lopez
