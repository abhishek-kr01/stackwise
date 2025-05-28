# 🧠 Stackwise - Developer Q&A Platform

**Stackwise** is a full-stack, modern web application designed as a community-driven platform where developers can **ask questions**, **post answers**, **comment**, and **vote** on content — inspired by the functionality of Stack Overflow. Built with **Next.js**, **TypeScript**, and powered by **Appwrite** as the backend-as-a-service (BaaS), this project demonstrates a modular, scalable, and maintainable codebase suitable for both personal and professional development use.

---

## 📸 Preview

> Add a screenshot or GIF here

---

## 🚀 Features

- ✅ User Authentication (Register & Login)
- 🧾 Ask Questions & Submit Answers
- 👍 Upvote / Downvote System for Answers and Questions
- 💬 Commenting System
- 📝 Rich Text Editor for better question formatting
- 🔄 Pagination for questions and answers
- 🔐 Protected Routes with Middleware
- 💡 Modular Component-based Architecture
- 📦 API route management via Next.js (`/api`)
- ☁️ Fully Integrated with Appwrite (Auth, DB, Storage)

---

## 🛠️ Tech Stack

### 📌 Frontend

- [Next.js](https://nextjs.org/) – App framework
- [React](https://react.dev/) – UI library
- [TypeScript](https://www.typescriptlang.org/) – Static typing
- CSS Modules – Scoped and modular styles

### 📌 Backend & Services

- [Appwrite](https://appwrite.io/) – Open-source backend-as-a-service for authentication, database, and storage
- REST-like API routes (`/src/app/api`) for backend logic

### 📌 Additional Tools

- [React Hook Form](https://react-hook-form.com/) – Form handling
- Rich Text Editor (custom or package-based)
- ESLint + Prettier – Linting & formatting
- Vercel (Optional) – Deployment

---

## 📁 Project Structure Overview

src/
├── auth/ # Authentication pages
│ ├── login/
│ │ └── page.tsx
│ └── register/
│ └── page.tsx
│ └── layout.tsx

├── app/ # Main app routing and layout
│ ├── api/ # API routes
│ │ ├── answer/route.ts
│ │ └── vote/route.ts
│ ├── layout.tsx
│ ├── page.tsx

├── components/ # Reusable UI components
│ ├── magiciui/ # Custom UI components (folder-based)
│ └── ui/ # Form components like input, label, etc.

├── lib/ # Utility functions and helpers
│ └── utils.ts

├── models/
│ ├── client/config.ts # Appwrite client-side config
│ └── server/ # Server-side Appwrite setup
│ ├── dbSetup.ts
│ ├── question.collection.ts
│ ├── answer.collection.ts
│ ├── comment.collection.ts
│ └── vote.collection.ts

├── store/ # Global state (e.g., auth state)
│ └── Auth.ts

├── middleware.ts # Middleware for route protection
├── globals.css # Global styles
├── .env.sample # Sample env file

---

## 🔐 Environment Setup

### 1. Clone the Repository

```bash
git clone https://github.com/abhishek-kr01/stackwise.git
cd stackwise

2. Install Dependencies
npm install

3. Create and Configure .env File
Rename .env.sample to .env and add your Appwrite project configuration:

NEXT_PUBLIC_APPWRITE_HOST_URL=https://cloud.appwrite.io/v1

NEXT_PUBLIC_APPWRITE_PROJECT_ID=your_project_id
APPWRITE_API_KEY=your_api_key

4. Run Development Server
npm run dev

Visit: http://localhost:3000


🧪 Functional Modules Overview
Module	    Description
auth	    Handles user registration and login using Appwrite Auth
questions	Post new questions with rich formatting support
answers	    Submit answers to questions
comments	Add comments to both questions and answers
votes	    Upvote/downvote logic with backend integration
pagination	Load more questions or answers dynamically
middleware	Protects routes from unauthenticated access

🧠 Future Improvements
🔍 Search and filter functionality

📈 View count per question

🏷️ Tags and categories

🧾 Markdown editor with preview

👥 User profiles and contributions tracking

🗂️ Admin panel for moderation

```

🤝 Contributing
Contributions are welcome!

Fork the repository

Create a new branch (git checkout -b feature/YourFeature)

Commit your changes (git commit -m 'Add new feature')

Push to the branch (git push origin feature/YourFeature)

Open a Pull Request

🙏 Acknowledgements

Appwrite — for providing a robust open-source BaaS

Next.js — for a seamless developer experience

Stack Overflow — for inspiration
