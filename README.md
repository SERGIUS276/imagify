
# 🎨 Imagify SaaS – AI Image Generation Web App

**Imagify** is a full-stack SaaS web application for generating and transforming images using AI. It includes user authentication, optional payment integration, and a powerful backend/frontend structure built with modern technologies.

---

## 🚀 Features

- ✨ AI-powered image generation  
- 🔐 User authentication system  
- 💳 Optional payment integration (Stripe / Razorpay)  
- 🛢️ MongoDB database (hosted via Atlas)  
- ⚙️ Built with Node.js + React (Vite)  

---

## 🛠️ Tech Stack

| Layer     | Tech              |
|-----------|-------------------|
| Frontend  | React + Vite      |
| Backend   | Node.js + Express |
| Database  | MongoDB (Atlas)   |
| API       | ClipDrop          |
| Payments  | Stripe / Razorpay (optional) |

---

## 📁 Project Structure

```
Imagify_Saas/
├── client        # React frontend (port 5173)
└── server        # Node.js backend (port 4000)
```

---

## ⚙️ How to Run the Project

### ✅ Prerequisites

- Node.js installed  
- MongoDB Atlas account  
- ClipDrop API key  
- (Optional) Stripe or Razorpay account  

---

### 🧪 Backend Setup (Server – Port `4000`)

1. Open the project in your code editor.  
2. Open a terminal in the `server` folder.  
3. Run:

   ```bash
   npm install
   ```

4. Create a `.env` file in the `server` directory and paste the following:

   ```env
   CLIPDROP_API_KEY=your_clipdrop_key
   MONGODB_URI=your_mongo_uri_without_trailing_slash
   STRIPE_SECRET_KEY=your_stripe_key        # optional
   RAZORPAY_SECRET_KEY=your_razorpay_secret # optional
   RAZORPAY_KEY_ID=your_razorpay_key_id     # optional
   ```

   **⚠️ Notes:**  
   - Avoid using `@` in your MongoDB password.  
   - Do **not** add a trailing `/` in the MongoDB URI.  

5. Start the backend server:

   ```bash
   npm run server
   ```

6. The backend will be running at:

   ```
   http://localhost:4000
   ```

---

### 💻 Frontend Setup (Client – Port `5173`)

> ⚠️ **Make sure the backend server is already running!**

1. Open a terminal in the `client` folder.  
2. Run:

   ```bash
   npm install
   ```

3. Start the frontend:

   ```bash
   npm run dev
   ```

4. Open the app in your browser:

   ```
   http://localhost:5173
   ```

---

## 📌 Notes

- ✅ Ensure all `.env` variables are set correctly before running the project.  
- 🔁 Always start the **backend before the frontend**.  
- 💳 Payment integration is **optional** and can be skipped during development/testing.  
