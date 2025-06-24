# verimail

# 📧 VeriMail – Email Verification Microservice

VeriMail is a lightweight Python microservice built with Flask that handles secure **email verification** using a one-time code (OTP). It collects a user's email, sends a 6-digit code to their inbox, and verifies the code through a simple UI.

---

## ✨ Features

- 🔐 One-time 6-digit verification code
- 📬 Sends code via SMTP (e.g., Gmail, Mailgun)
- 🕓 5-minute expiration for security
- ✅ Simple verification UI
- 🧠 Easy to integrate into any app

---

## 🚀 Demo

```bash
git clone https://github.com/YOUR_USERNAME/verimail.git
cd verimail
pip install -r requirements.txt
python app.py
````

Open your browser at:
👉 `http://localhost:5000`

---

## ⚙️ Configuration

In `app.py`, update your email credentials:

```python
app.config['MAIL_SERVER'] = 'smtp.gmail.com'
app.config['MAIL_PORT'] = 587
app.config['MAIL_USE_TLS'] = True
app.config['MAIL_USERNAME'] = 'your_email@gmail.com'
app.config['MAIL_PASSWORD'] = 'your_password_or_app_password'
```

🔐 Use an App Password if you're using Gmail:
👉 [How to Generate Gmail App Password](https://support.google.com/mail/answer/185833)

---

## 📂 Folder Structure

```
verimail/
├── app.py                  # Main Flask app
├── requirements.txt        # Python dependencies
├── templates/              # HTML templates
│   ├── email_form.html
│   ├── verify.html
│   ├── success.html
│   └── failure.html
└── README.md
```

---

## ✅ Usage Flow

1. User enters their email address
2. App generates and emails a 6-digit code
3. User is redirected to a verification page
4. If correct and not expired → ✅ success

---

## 💡 Ideas for Improvement

* ⏱ Resend code with cooldown
* 📱 SMS code support (Twilio)
* 🌐 REST API version
* 🐳 Docker container for deployment
* 🧪 Unit tests and CI workflow

---

## 📜 License

MIT © 2025 [Your Name](https://github.com/YOUR_USERNAME)

````

---
