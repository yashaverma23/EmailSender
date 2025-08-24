# 📧 Cold Email Sender

A simple, professional **Streamlit web app** to send personalized cold emails to recruiters with your resume attached.  

The email body is stored in `templates/email.docx` (so you can edit it without touching code), and placeholders like `[Company Name]` and `[Recruiter’s Name]` are auto-filled from inputs in the app.  

---

## 🚀 Features
- Uses your **email.docx** as a template  
- Placeholders auto-replaced with company & recruiter details  
- Attach **Resume.pdf** (from `templates/` or upload a custom one)  
- **Preview email** before sending  
- One-click **Send** button  
- 🌙 **Light/Dark theme toggle** at the top-right  
- Credentials stored securely in **Streamlit secrets**  

---

## 📂 Project Structure
EmailSender/
│
├── app.py # Main Streamlit app
├── requirements.txt # Python dependencies
├── README.md # Project docs
├── .gitignore # Ignore venv, secrets, etc.
│
├── templates/ # Email template + Resume
│ ├── email.docx
│ └── Resume.pdf
│
└── .streamlit/
└── secrets.toml # 🔒 Email + password (ignored by git)


---

## 🔒 Setup Secrets
Create a file: **`.streamlit/secrets.toml`**

```toml
EMAIL = "your_email@gmail.com"
EMAIL_PASSWORD = "your_16_char_app_password"

git clone https://github.com/<your-username>/EmailSender.git
cd EmailSender
pip install -r requirements.txt
streamlit run app.py

EMAIL = "your_email@gmail.com"
EMAIL_PASSWORD = "your_16_char_app_password"


Application for Data Analyst Role at [Company Name]

Hi [Recruiter’s Name],

I am writing to express my interest in the Data Analyst position at [Company Name]...

Best regards,  
Yash Verma  
📞 +91 7383507341  
✉️ yashaverma20@gmail.com



---

✅ This version is **ready to copy-paste** into your repo.  

Do you also want me to prepare a matching **`.gitignore` file** so your secrets and venv never get pushed to GitHub?
