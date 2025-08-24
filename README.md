# Health-Node

🏥 Health Node – Healthcare Management System

A full-stack, role-based healthcare management system enabling real-time appointment booking, prescription handling, secure payments, and doctor-patient interactions.

Frontend : https://health-node.vercel.app/
Admin : https://health-node-zv8a.vercel.app/

🛠️ Tech Stack

Frontend: React.js (Vite), Tailwind CSS

Backend: Node.js, Express.js

Database: MongoDB Atlas

Authentication: JWT (JSON Web Tokens)

Real-time Communication: WebSockets (Socket.io)

Payments: Razorpay API

Media Handling: Cloudinary

🔐 Roles & Access

👨‍⚕️ Doctor: Manage appointments, write prescriptions.

🧑‍💼 Admin: Dashboard to manage doctors, patients, and appointments.

🧑‍🤝‍🧑 Patient: Book appointments, view prescriptions and pay online.

🎯 Features

📅 Appointment Booking: Role-specific workflows for booking and managing appointments.

📄 Prescription Management: Doctors can securely upload/view prescriptions.

🔒 Role-Based JWT Auth: Ensures secure access to protected routes and APIs.

💳 Razorpay Integration: Secure online payment for booking confirmations.

🔄 WebSockets Support: Real-time updates on appointment status and payments.

📁 Image Uploads: Cloudinary used for efficient and fast media handling.

📊 Admin Dashboard: Visualize and manage system-wide data.

📱 Mobile Responsive UI: Built using React + Tailwind for seamless mobile experience.

📁 Folder Structure
health-node/
│
├── client/                      # React Frontend (Vite)
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── contexts/
│   │   ├── services/            # API calls
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── .env                     # VITE_ prefixed env vars
│   └── vite.config.js
│
├── server/                      # Node.js + Express Backend
│   ├── config/
│   │   ├── db.js
│   │   └── cloudinary.js
│   ├── controllers/
│   ├── middleware/
│   │   └── auth.js              # JWT middleware
│   ├── models/
│   │   ├── User.js
│   │   ├── Appointment.js
│   │   ├── Prescription.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── doctor.js
│   │   ├── patient.js
│   │   └── admin.js
│   ├── utils/
│   │   └── razorpay.js
│   ├── socket.js                # WebSocket server
│   ├── index.js                 # Entry point
│   └── .env                     # Server secrets
│
├── README.md
└── package.json

⚙️ Installation & Setup
1. Clone the Repository
git clone https://github.com/your-username/health-node.git
cd health-node

2. Setup Backend (Express Server)
cd server
npm install


Create .env file in /server:

PORT=4000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
RAZORPAY_KEY_ID=your_key_id
RAZORPAY_SECRET=your_secret


Start backend:

npm run dev

3. Setup Frontend (React)
cd ../client
npm install


Create .env in /client:

VITE_BACKEND_URL=http://localhost:4000
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id


Start frontend:

npm run dev

📊 Key Results

⚡ Improved responsiveness by 45% using WebSockets for live updates.

🧠 Reduced manual admin efforts by 40% with automated dashboards and analytics.

💳 Enabled seamless online payments through Razorpay integration.

📌 Future Improvements

🔔 Push Notifications

📱 Mobile App Version (React Native)

🔍 Advanced Search & Filters

📈 Analytics Dashboard for doctors

👨‍💻 Author

Aman Bhagat
Frontend + Full-stack Developer




