# 🚀 Self-Healing Application

## 📌 Project Overview

The **Self-Healing Application** is a Python-based intelligent monitoring and recovery system that leverages Machine Learning and Streamlit to detect anomalies in application logs and automatically perform corrective actions.

Built using a **Random Forest Machine Learning algorithm**, the system analyzes application log patterns, identifies abnormal activities, and triggers automated recovery mechanisms to minimize manual intervention.

This project demonstrates the concepts of self-monitoring, self-diagnosis, and self-recovery to improve application reliability, fault detection, and system availability.

## ✨ Features

- 🤖 **Machine Learning-Based Anomaly Detection:** Uses a Random Forest classifier to analyze application logs and identify abnormal patterns.
- 🔧 **Automated Self-Healing:** Automatically triggers predefined corrective actions when anomalies are detected.
- 📊 **Interactive Dashboard:** Built with Streamlit to visualize application logs, anomaly predictions, and healing activities.
- 📝 **Activity Logging:** Maintains CSV-based records of application activity and automated recovery actions.
- ⚡ **System Monitoring:** Provides an interactive view of system activities and detected anomalies.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core application development |
| Machine Learning | Anomaly detection |
| Random Forest | Classification algorithm |
| Scikit-learn | Model training and prediction |
| Pandas | Data processing |
| Joblib | Model serialization |
| Streamlit | Interactive dashboard |
| CSV | Log storage and tracking |

## 📂 Project Structure

```text
Self-Healing-Applications/
│
├── dashboard.py        # Streamlit monitoring dashboard
├── self_healing.py     # Core self-healing mechanism
├── train_model.py      # Random Forest model training
├── model.joblib        # Trained ML model
├── logs.csv            # Sample application log data
├── actions_log.csv     # Automated healing action records
├── requirements.txt    # Project dependencies
└── __pycache__/        # Python cache files
```

## ⚙️ Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/dhanushn113-ai/Self-Healing-Applications.git

cd Self-Healing-Applications
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

**Windows:**

```bash
venv\Scripts\activate
```

**Mac/Linux:**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Alternatively, install the required packages manually:

```bash
pip install scikit-learn pandas joblib streamlit
```

### 4. Train the Machine Learning Model

```bash
python train_model.py
```

This generates the trained `model.joblib` file, which is used for anomaly detection.

### 5. Run the Self-Healing System

```bash
python self_healing.py
```

### 6. Launch the Streamlit Dashboard

```bash
streamlit run dashboard.py
```

Open your browser and navigate to:

**http://localhost:8501**

## 🔄 System Workflow

1. **Log Collection:** Collects application log data.
2. **Data Processing:** Processes log patterns using Python and Pandas.
3. **Anomaly Detection:** The Random Forest model predicts whether log patterns are normal or anomalous.
4. **Self-Healing:** Triggers predefined corrective actions when anomalies are detected.
5. **Activity Tracking:** Records detected anomalies and healing actions in CSV files.
6. **Visualization:** Displays logs, predictions, and recovery activities through the Streamlit dashboard.

## 📊 Log Management

The application maintains two CSV files to track system activities:

- **logs.csv:** Contains sample application log data used for training and testing.
- **actions_log.csv:** Stores records of corrective actions performed by the self-healing system.

## 🚀 Future Enhancements

- Support for real-time application log streaming.
- Implementation of advanced anomaly detection algorithms.
- Docker-based containerization and deployment.
- Integration with monitoring platforms such as Prometheus and Grafana.
- Advanced automated recovery and notification mechanisms.

## 🤝 Contributing

Contributions are welcome!

1. Fork this repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch to your repository.
5. Submit a Pull Request.

## 📜 License

This project is licensed under the MIT License.

---

<div align="center">

### ⭐ If you find this project useful, consider giving it a star!

**Made with ❤️ by [Dhanush N](https://github.com/dhanushn113-ai)**

</div>
