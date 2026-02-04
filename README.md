🌞 Solar Energy Forecasting Dashboard

A professional, interactive Solar Energy Prediction system built using Streamlit and Machine Learning.
The application allows users to manually input solar and environmental parameters and instantly predict AC power output with rich visualizations.

This project is designed to run smoothly in Google Colab, locally, or via ngrok, making it ideal for college projects, hackathons, and demonstrations.

🚀 Features

🔮 Live Solar Power Prediction

🧠 Machine Learning Models

Random Forest Regressor

Gradient Boosting Regressor

📊 Interactive Visualizations

Irradiation vs AC Power

DC Power vs AC Power

Feature Importance Chart

🎛 Manual Input Interface

Solar Irradiation

Ambient Temperature

Module Temperature

DC Power

💻 Modern Streamlit Dashboard UI

⚡ Fast & Stable Execution (No PySpark JVM issues)

🛠 Tech Stack
Layer	Technology
Frontend	Streamlit
ML Models	Scikit-learn
Visualization	Plotly
Language	Python
Deployment	Google Colab / ngrok / Local
📂 Project Structure
solar-energy-forecasting/
│
├── app.py               # Main Streamlit application
├── README.md            # Project documentation
└── requirements.txt     # Python dependencies (optional)

📊 Dataset

This project uses a synthetic solar dataset generated inside the application.

The data simulates real-world solar plant behavior:

Non-linear relation between irradiation, temperature, DC power, and AC output.

No external CSV file is required.

🔧 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/solar-energy-forecasting.git
cd solar-energy-forecasting

2️⃣ Install Dependencies
pip install streamlit scikit-learn plotly pandas numpy

3️⃣ Run the Application Locally
streamlit run app.py


Open in browser:

http://localhost:8501

☁️ Run in Google Colab (Recommended for Demos)
!pip install streamlit pyngrok scikit-learn plotly

from pyngrok import ngrok
ngrok.set_auth_token("YOUR_NGROK_TOKEN")
public_url = ngrok.connect(8501)
print(public_url)

streamlit run app.py --server.port 8501 --server.address 0.0.0.0


Open the ngrok public URL in a new browser tab.

🧪 How It Works

User enters solar and environmental parameters.

ML model predicts AC Power Output.

Dashboard displays:

Predicted power

Efficiency

Generation level

Interactive graphs

Users can switch ML models from the sidebar to compare results.

📸 Screenshots

Add screenshots here after deploying the app
Example:

/screenshots/prediction_panel.png
/screenshots/visualization.png

🎯 Use Cases

🎓 College Mini / Major Projects

⚡ Renewable Energy Analytics

🤖 Machine Learning Demonstrations

🏆 Hackathons

📊 Data Visualization Practice

🔮 Future Enhancements

Real-world solar datasets integration

Time-series forecasting (LSTM)

Model accuracy comparison dashboard

Export predictions as CSV/PDF

Cloud deployment (Streamlit Cloud / HuggingFace Spaces)

👨‍💻 Author

Shaik Naveed Ahamed
AI & ML Enthusiast | Big Data | Streamlit Developer

⭐ Support

If you find this project helpful, please ⭐ the repository on GitHub.
