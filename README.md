# 🛡️ Malicious URL Detection Using Machine Learning 🔍💻

📌 **Problem Statement**  
This project aims to proactively detect **malicious URLs** using machine learning techniques. With the rise in phishing, scams, and malware threats through URLs, an intelligent system is needed to classify web links as *safe* or *malicious*. This system helps individuals and organizations protect against potential cybersecurity threats.

---

🎯 **Objectives**

- Detect whether a URL is malicious or benign using ML.
- Extract key lexical features from URLs for predictive modeling.
- Build a user-friendly web interface for real-time classification.
- Store user access and predictions securely in a MongoDB database.

---

✅ **Steps Followed**

🔹 **Step 1: Feature Engineering**

- Parsed URLs to extract meaningful lexical features like:
  - Length of the URL
  - Count of `.`, `/`, and `-`
- Created a feature matrix using NumPy.

🔹 **Step 2: Model Building**

- Trained multiple models: Random Forest, XGBoost, LightGBM
- **Selected LightGBM** for its high accuracy and low latency.
- Serialized the final model using `joblib`.

🔹 **Step 3: Backend Integration (Flask)**

- Built a Flask app for:
  - User registration and login
  - URL submission form
  - Prediction result rendering
- Integrated **MongoDB** for user data and session handling.

🔹 **Step 4: Frontend Development**

- Developed HTML templates:
  - `home.html` - Landing page
  - `register.html` - Registration form
  - `login.html` - Login page
  - `index.html` - URL prediction form
- Styled using **CSS** with a clean, responsive layout.

---

📊 **Dashboards / Screens**

📌 **Screen 1: Landing Page**

- Welcome message and app description
- Buttons: Login | Register
- "How it Works" explanation section


📸 Snapshot:
![Image](https://github.com/user-attachments/assets/8ac63895-4ff3-455a-a735-5291d378393a)

📌 **Screen 2: Register/Login Page**

- Form to register a new user or login to the system
- Session-based redirection to the prediction page

📸 Snapshot:
![Image](https://github.com/user-attachments/assets/b50a3c4b-4fe3-4146-b17f-405e3a301ac5)

📌 **Screen 3: Prediction Interface**

- Input field to enter URL
- "Check URL" button
- Real-time classification result (Benign ✅ or Malicious ❌)
📸 Snapshot:
![Image](https://github.com/user-attachments/assets/f2328d70-97d4-4858-ba4e-b6d5ef8e5ec4)

📸 Snapshot:
![Image](https://github.com/user-attachments/assets/18741ce1-01b6-475b-9545-f72f6855cc41)
![Image](https://github.com/user-attachments/assets/d0cdf468-56e3-4842-98ce-620ba5553168)

📌 **Screen 4: Real-Time Dashboard**

- Visual summary of total URL checks, malicious vs. benign counts
- Pie chart showing safe vs. malicious URL distribution
- Cards displaying:
  - Total URLs scanned
  - Total malicious URLs
  - Total benign URLs
- Dynamically updated from MongoDB data for admin or user overview

📸 Snapshot:
 ![Image](https://github.com/user-attachments/assets/263f157e-a1b4-46dc-9f52-14bf189bb413)
🧠 **Key Features & Insights**

- Simple, fast URL classification with real-time feedback
- ML-powered backend with LightGBM classifier
- Secured user login and session handling
- Modular code with clean separation of concerns (frontend/backend)
- Realtime dashboard for usage analytics and trends

---

💻 **Tools & Technologies Used**

| Component      | Tool/Library            |
|----------------|--------------------------|
| Language       | Python                   |
| Web Framework  | Flask                    |
| Machine Learning | LightGBM, joblib       |
| Database       | MongoDB (local)          |
| Frontend       | HTML5, CSS3              |
| Hosting        | Localhost (127.0.0.1)    |

---



