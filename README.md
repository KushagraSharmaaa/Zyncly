# 🌟 Zyncly - Advanced MERN B2B Teams Project Management SaaS

A powerful and scalable multi-tenancy project management system built with **Node.js**, **MongoDB**, and **React**. Designed for real-world B2B needs, this project delivers features like Google Sign-In, workspace management, project tracking, task collaboration, role-based permissions, and more.

---

## 🌟 Key Features

- 🔐 **Authentication** (Google Sign-In, Email, Password)
- 🏢 **Create & Manage Multiple Workspaces**
- 📊 **Projects & Epics Management**
- ✅ **Tasks** (CRUD, Status, Priority, Assignee)
- 👥 **Roles & Permissions** (Owner, Admin, Member)
- ✉️ **Invite Members to Workspaces**
- 🔍 **Filters & Search** (Status, Priority, AssignedTo)
- 📈 **Analytics Dashboard**
- 📅 **Pagination & Load More**
- 🔒 **Cookie Session Management**
- 🚪 **Logout & Session Termination**
- 🌱 **Seeding** for Test Data
- 💾 **Mongoose Transactions** for Robust Data Integrity
- 🌐 **Built with MERN Stack** (Node.js, MongoDB, React, TypeScript)

---

## 🚀 Tools & Technologies

This project leverages the latest tools and frameworks for modern development:

- **Node.js**: Scalable backend architecture
- **React.js**: Dynamic frontend framework
- **MongoDB & Mongoose**: Flexible and scalable database solutions
- **Google OAuth**: Seamless Google Sign-In integration
- **TypeScript**: For a type-safe codebase
- **TailwindCSS & Shadcn UI**: Beautiful, responsive design
- **Vite.js**: Lightning-fast frontend development

---

## 🔄 Getting Started

### 1. Set Up Environment Variables

Create a `.env` file in the backend directory and configure these variables:

```plaintext
PORT=8000
NODE_ENV=development
MONGO_URI="mongodb+srv://<username>:<password>@<>.mongodb.net/zyncly_db"

SESSION_SECRET="session_secret_key"

GOOGLE_CLIENT_ID=<your-google-client-id>
GOOGLE_CLIENT_SECRET=<your-google-client-secret>
GOOGLE_CALLBACK_URL=http://localhost:8000/api/auth/google/callback

FRONTEND_ORIGIN=http://localhost:5173
FRONTEND_GOOGLE_CALLBACK_URL=http://localhost:5173/auth/google/callback
```

Create a `.env` file in the client directory:

```plaintext
VITE_API_BASE_URL=http://localhost:8000/api
```

### 2. Install Dependencies

**Backend:**
```bash
cd backend
npm install
```

**Frontend:**
```bash
cd client
npm install
```

### 3. Seed the Database

Run the role seeder to create necessary roles:

```bash
npx ts-node backend/src/seeders/role.seeder.ts
```

### 4. Run the Application

**Start Backend:**
```bash
cd backend
npm run dev
```

**Start Frontend:**
```bash
cd client
npm run dev
```

Access the application at `http://localhost:5173`.

---

## 🌐 Deployment

### Backend Deployment
1. Set up environment variables on your hosting platform
2. Deploy to platforms like Heroku, Railway, or Render
3. Update frontend API base URL to point to your deployed backend

### Frontend Deployment
1. Update the API base URL in your environment variables
2. Deploy to platforms like Vercel, Netlify, or GitHub Pages

---

## 📁 Project Structure

```
├── backend/                 # Backend API (Node.js + Express)
│   ├── src/
│   │   ├── controllers/    # Route controllers
│   │   ├── models/         # Database models
│   │   ├── routes/         # API routes
│   │   ├── services/       # Business logic
│   │   ├── middlewares/    # Custom middlewares
│   │   └── utils/          # Utility functions
├── client/                  # Frontend (React + TypeScript)
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── hooks/          # Custom hooks
│   │   ├── pages/          # Page components
│   │   └── lib/            # Utility libraries
```

---

## 🔧 Development

### Backend Development
- Built with Express.js and TypeScript
- Uses MongoDB with Mongoose for data modeling
- Implements role-based access control
- Supports Google OAuth authentication

### Frontend Development
- Built with React 18 and TypeScript
- Uses Vite for fast development
- Implements responsive design with TailwindCSS
- Uses React Query for state management

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

**Built with ❤️ by Kushagra Sharma using the MERN stack**

