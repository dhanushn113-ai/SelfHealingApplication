A Python + Streamlit project that uses a Random Forest Machine Learning model to detect anomalies in application logs and perform automated self-healing actions.
This system demonstrates how applications can self-monitor, self-diagnose, and recover automatically without manual intervention.

🚀 Features
Machine Learning (Random Forest): Trains a model to classify log patterns and detect anomalies.
Self-Healing Logic: Automatically triggers corrective actions when anomalies are detected.
Interactive Dashboard (Streamlit): Visualizes logs, predictions, and healing actions in real time.
Logging: Maintains CSV logs of both raw system activity and healing actions.
📂 Project Structure
├── dashboard.py # Streamlit dashboard for monitoring

├── self_healing.py # Core self-healing logic (uses Random Forest model)

├── train_model.py # Script to train the Random Forest model

├── model.joblib # Saved trained model

├── logs.csv # Sample log data used for training

├── actions_log.csv # Records of performed healing actions

└── pycache/ # Auto-generated Python cache files

yaml Copy code

⚙️ Getting Started
1. Clone the Repository
git clone https://github.com/balakrishnabadri25/Self-Healing-Applications.git
cd Self-Healing-Applications
2. Create and Activate a Virtual Environment
python -m venv venv
Windows

venv\Scripts\activate
Mac/Linux

source venv/bin/activate
3. Install Dependencies
pip install -r requirements.txt
If requirements.txt is missing, install manually:

pip install scikit-learn pandas joblib streamlit
4. Train the Model
python train_model.py
This creates model.joblib which will be used for anomaly detection.
5. Run the Self-Healing System
python self_healing.py
6. Launch the Streamlit Dashboard

streamlit run dashboard.py
The dashboard will open in your browser (default: http://localhost:8501).

Simple Setup:
-> Install dependencies like python scikit-learn streamlit -> python -m streamlit run dashboard.py

📊 Logs
logs.csv → Input log data used for training/testing.

actions_log.csv → Record of actions performed by the self-healing system.

🛠 Future Enhancements
Support for real-time streaming logs.

More advanced ML models for anomaly detection.

Containerization with Docker for easier deployment.

Integration with external monitoring tools (e.g., Prometheus, Grafana).

🤝 Contributing
Contributions are welcome!

Fork the repo

Create a feature branch

Commit changes

Open a pull request

📜 License
This project is licensed under the MIT License.
