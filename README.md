
# Delete User Account API

Production-ready Flask API for безопасной регистрации и удаления пользователей через REST API.  
Includes rate-limiting, Docker, clean modular structure — всё для продакшена и продажи.

---

👉 [Buy it on Gumroad](https://talabov.gumroad.com/)

## 🚀 Features

- Registration and instant user deletion via API
- Secure password hashing (no plain passwords)
- SQLite by default, easy to switch DB in .env
- Rate limiting (anti-abuse)
- Docker-ready, clean project structure
- Simple integration (Postman, curl, любой front-end)
- Health-check endpoint
- Logging for audits and debugging

---

## 📦 Endpoints

### POST \`/register\`

**Request (JSON):**
\`\`\`json
{
  "email": "user@mail.com",
  "password": "password123"
}
\`\`\`
**Response:**
\`\`\`json
{
  "message": "User registered."
}
\`\`\`

---

### POST \`/delete\`

**Request (JSON):**
\`\`\`json
{
  "email": "user@mail.com",
  "password": "password123"
}
\`\`\`
**Response:**
\`\`\`json
{
  "message": "User deleted."
}
\`\`\`

---

### GET \`/health\`

Always returns
\`\`\`json
{"status": "ok"}
\`\`\`

---

## ⚡ Quick Start

### Docker (recommended)
\`\`\`bash
docker build -t delete-user-account-api .
docker run -d -p 5000:5000 --env-file .env delete-user-account-api
\`\`\`

### Local
\`\`\`bash
pip install -r requirements.txt
cp .env.example .env
python app.py
\`\`\`

---

## 🖼️ Screenshots

![Server Logs](server_logs.png)
![Server Startup](start_server.png)
![Delete User in Postman](delete_user_account.png)

---

> 💡 See real examples on Gumroad or in this README.

---

## 💼 Ready-to-Use Version

You can get a ZIP version with all files, setup instructions, \`.env.example\`, and more:

👉 [Buy it on Gumroad](https://talabov.gumroad.com/)

---

## 📬 Contact

**Need this in another stack (Node.js, Go, etc)?**  
Contact: talabov.ali72@gmail.com  
Telegram: [@talabovali](https://t.me/talabovali)

*Note: Pricing may vary depending on complexity and target stack.*

---

**Ready for production and monetization. 100% tested.**
