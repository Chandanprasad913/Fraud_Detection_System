💳 Fraud Detection System using Machine Learning

A Machine Learning–powered Fraud Detection System built using LightGBM and deployed with Streamlit.
The system predicts whether a transaction is Fraudulent or Legitimate based on real-time transaction inputs and geolocation distance.

🚀 Live Features

🔍 Real-time fraud prediction

🤖 Trained LightGBM classification model

📍 Distance calculation using latitude & longitude

🧠 Pre-trained label encoders for categorical data

🖥️ Interactive Streamlit web interface

🔐 Privacy-safe credit card hashing

🛠️ Tech Stack
Category	Tools
Language	Python
ML Model	LightGBM
Frontend	Streamlit
Data Handling	Pandas, NumPy
Distance Calc	Geopy (Haversine)
Model Storage	Joblib
📂 Project Structure
Fraud_Detection_System/
│
├── app.py                     # Streamlit application
├── dataset.csv                # Dataset used for training
├── fraud_detection_model.jb   # Trained LightGBM model
├── label_encoders.jb          # Saved encoders for categorical features
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation

📥 Input Parameters

The application takes the following transaction details:

Merchant Name

Category

Transaction Amount

User Latitude & Longitude

Merchant Latitude & Longitude

Transaction Time (Hour, Day, Month)

Gender

Credit Card Number

📍 Distance between user & merchant is automatically calculated.

⚙️ Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/your-username/fraud-detection-system.git
cd fraud-detection-system

2️⃣ (Optional) Create Virtual Environment
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate  # Linux / Mac

3️⃣ Install Dependencies
pip install -r requirements.txt

▶️ Run the Application
streamlit run app.py


Open in browser:

http://localhost:8501

🧠 How It Works

User enters transaction details

Distance is calculated using Haversine formula

Categorical data is encoded using saved encoders

Credit card number is hashed for privacy

LightGBM model predicts fraud probability

Output:

❌ Fraudulent Transaction

✅ Legitimate Transaction

📊 Dataset

File: dataset.csv

Contains historical transaction records

Used for training the LightGBM model

Includes categorical, numerical & geolocation features

📈 Future Enhancements

📊 Transaction analytics dashboard

☁️ Cloud deployment (Streamlit Cloud / AWS)

🔐 User authentication

🧪 Model performance metrics visualization

👨‍💻 Author

Prasad Chandankumar Someshwar
🎓 MCA | AI/ML Enthusiast

📧 Email: prasadchandan913@gmail.com

🔗 GitHub: Chandanprasad913

⭐ Support

If you found this project helpful, please ⭐ star the repository and share it!
