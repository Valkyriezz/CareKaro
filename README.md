# CareKaro

Low-Tech Pregnancy Care Assistant
A maternal health companion for underserved communities, combining SMS and a simple web portal to improve prenatal care access.

## 📖 Overview

In rural and economically disadvantaged areas, many pregnant women lack smartphones or internet access. As a result, they miss out on essential checkups, health tips, and supplements during pregnancy. This project aims to solve that with a low-tech approach: an SMS-based reminder system backed by a mobile-first web portal.

---

## 🚀 Features

### 👩‍🍼 For Pregnant Women
- Register via phone number (self or assisted by NGO/health worker)
- Automatically track pregnancy stage based on due date
- Receive weekly SMS reminders:
  - Health tips and nutrition advice
  - Supplement and vaccine alerts (e.g., Iron, Calcium, TT)
  - Free checkup camp notifications

### 🧑‍⚕️ For NGOs / Health Workers
- Web dashboard to:
  - Register and manage women by location
  - View pregnancy stages and SMS logs
  - Identify high-risk cases
  - Schedule local checkup camps and send notifications

---

## 🛠 Tech Stack (Web-Only)

| Layer         | Technologies Used                            |
|---------------|-----------------------------------------------|
| Frontend      | React.js (mobile-first responsive UI)         |
| Backend       | Node.js (Express.js)                          |
| Database      | MongoDB (via Mongoose)                        |
| SMS Gateway   | Twilio / Nexmo API                            |
| Scheduling    | `node-cron` for weekly SMS reminders          |
| Deployment    | Vercel (frontend) + Render / Railway (backend)|

---

## 🧪 MVP Features

- ✅ Phone number registration and validation
- ✅ Pregnancy week calculator
- ✅ Weekly SMS system with Twilio
- ✅ Admin dashboard for NGOs
- 🔜 Location-based checkup notifications

---

## 💡 Impact

- Improves access to prenatal care for women without smartphones
- Encourages consistent health checkups and supplement intake
- Enables NGOs to track and support women more effectively

---

## 🧩 Future Extensions

- Voice call reminders (IVR) for illiterate users
- Integration with government health databases
- PWA support for offline use by health workers
- ML-based risk detection (missed visits, age, comorbidities)

---

## 🛠️ Local Development Setup

```bash
# Clone the repo
git clone https://github.com/your-username/low-tech-pregnancy-assistant.git
cd low-tech-pregnancy-assistant

# Install backend dependencies
cd backend
npm install

# Set up .env file with MongoDB URI and Twilio keys

# Run backend
npm run dev

# In a new terminal: setup frontend
cd ../frontend
npm install
npm start
