# 🎬 QuickShow - Movie Ticket Booking Website

## 📌 Overview

**QuickShow** is a modern, full-stack web application built using the **MERN** stack that enables users to explore movies, book tickets with live seat selection, and enjoy a seamless booking experience. Admins can manage movies and view bookings, while the system handles user sessions, background jobs, email notifications, and payment failure fallbacks smartly.

🚀 **Live Demo**: [https://quick-show-client-alpha.vercel.app/](https://quick-show-client-alpha.vercel.app/)  
📂 **GitHub Repo**: [QuickShow Repository](https://github.com/balmukund18/QuickShow-FullStack/tree/main)

---

## 🎯 Key Features

### 🧑‍💻 For Users
- **Signup/Login** using Clerk with support for Email, Phone, and Social logins
- **Explore Movies** with show details, posters, and timings
- **Real-Time Seat Selection** using an interactive interface
- **Secure Online Payments** with Stripe
- **Multi-session Login** (e.g. multiple accounts, easy switch)
- **Background Email Notifications** for:
  - Booking confirmations
  - Reminders before movie start
  - New movie announcements
- **Auto-Hold Seats** for 10 minutes post payment failure to allow retry

### 🛠️ For Admins
- **Admin Dashboard** with authentication
- **Add & Manage Movies**
- **View All Bookings**
- **Trigger Email Campaigns** (via Inngest and Brevo)
- **Theming and UI Controls**

---

## 🧪 Tech Stack

| Layer       | Technology                        |
|-------------|-----------------------------------|
| **Frontend**  | React.js, Tailwind CSS, Clerk Auth |
| **Backend**   | Node.js, Express.js              |
| **Database**  | MongoDB (with Atlas)             |
| **Auth**      | Clerk (with Webhooks & Multi-login) |
| **Emails**    | Brevo (Transactional)            |
| **Jobs**      | Inngest (Background + Scheduler) |
| **Payments**  | Stripe                           |
| **API Source**| TMDB API                         |
| **Hosting**   | Vercel (Frontend), Render/Other (Backend) |

---

## 🛠️ Installation Guide

### 🔧 Backend Setup (Server)

```bash
# Clone the repository
git clone https://github.com/balmukund18/QuickShow-FullStack.git

# Navigate to the server directory
cd QuickShow-FullStack/server

# Install backend dependencies
npm install

# Create a .env file in the /server folder and add the following environment variables:
# - MONGODB_URI
# - CLERK_SECRET_KEY
# - INNGEST_EVENT_KEY
# - BREVO_SMTP_KEY
# - STRIPE_SECRET_KEY
# - Other required API keys (TMDB, etc.)

# Start the backend server
npm run server
```

### 🎨 Frontend Setup (Client)

```bash
# Navigate to the client directory
cd QuickShow-FullStack/client

# Install frontend dependencies
npm install

# Create a .env file in the /client folder and add:
# - VITE_CLERK_PUBLISHABLE_KEY
# - VITE_BACKEND_URL

# Start the React development server
npm run dev
```

## 👥 Contributors

Feel free to contribute! Open a pull request or report issues to help improve the project.

## 📜 License

This project is open-source under the [MIT License](LICENSE).

## 📞 Contact

For queries, suggestions, or collaborations, feel free to reach out:

- 📧 Email: [sm1370530@gmail.com](mailto:sm1370530@gmail.com)
- 🔗 GitHub: [@balmukund18](https://github.com/balmukund18)

Open to feedback, issues, or contributions! 🤝
