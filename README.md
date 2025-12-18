💳 Fraud Detection System using Machine Learning

A Streamlit-based Fraud Detection System that predicts whether a financial transaction is Fraudulent or Legitimate using a trained LightGBM model.
The application takes transaction details as input, performs feature engineering (including distance calculation), and displays real-time predictions.


🚀 Features

🔍 Real-time fraud prediction

🤖 Machine Learning model (LightGBM)

📍 Distance calculation using latitude & longitude (Haversine via Geopy)

🧠 Encoded categorical features using pre-trained label encoders

🖥️ Interactive UI built with Streamlit

📊 Supports multiple transaction attributes


🛠️ Tech Stack

Frontend: Streamlit

Backend / ML: Python, LightGBM

Libraries: Pandas, NumPy, Joblib, Geopy

Model Serialization: Joblib

'''
📂 Project Structure
Fraud_Detection_System/
│
├── app.py                     # Streamlit application
├── dataset.csv                # Dataset used for training the model
├── fraud_detection_model.jb   # Trained LightGBM model
├── label_encoders.jb          # Saved label encoders
├── requirements.txt           # Required dependencies
└── README.md                  # Project documentation
'''

📥 Input Parameters

The system requires the following transaction details:

Merchant Name

Category

Transaction Amount

User Latitude & Longitude

Merchant Latitude & Longitude

Transaction Hour, Day, Month

Gender

Credit Card Number

The distance between user and merchant is automatically calculated.

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/fraud-detection-system.git
cd fraud-detection-system

2️⃣ Create Virtual Environment (Optional but Recommended)
python -m venv venv
venv\Scripts\activate   # For Windows
source venv/bin/activate # For Linux/Mac

3️⃣ Install Dependencies
pip install -r requirements.txt

▶️ Run the Application
streamlit run app.py

Then open your browser and visit:
http://localhost:8501


🧠 Prediction Logic

Categorical features are encoded using saved label encoders.

Unseen categories are handled safely.

Credit card number is hashed for privacy.

LightGBM model predicts:

Fraudulent Transaction

Legitimate Transaction


📊 Output
After clicking "Check For Fraud", the system displays:

✅ Legitimate Transaction
❌ Fraudulent Transaction

📌 Future Improvements

Add transaction history visualization

Improve handling of unseen categories

Deploy on cloud (AWS / Streamlit Cloud)

Add authentication & logging

👨‍💻 Author

Prasad Chandankumar Someshwar
MCA | AI/ML Enthusiast
📧 Email: prasadchandan913@gmail.com
🔗 GitHub: https://github.com/Chandanprasad913
