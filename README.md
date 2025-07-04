# 🔐 Keylogger Detection – APLab Project

This repository contains a Jupyter Notebook (`aplab.ipynb`) that implements a full machine-learning pipeline to detect keylogger activity using the `Keylogger_Detection.csv` dataset. The workflow includes data cleaning, feature preprocessing, classification, and result visualization.

---

## 🧠 Project Overview

Keyloggers are spyware that covertly record keystrokes, posing serious security threats. This project trains ML models to classify system activity into two classes: **Benign** and **Keylogger** :contentReference[oaicite:1]{index=1}.

A companion Kaggle notebook by Ammar N. Alhajali explores this same dataset using CNNs in an IoT intrusion detection context :contentReference[oaicite:2]{index=2}, which inspired parts of the data exploration and modeling approach.

---

## 🗄️ Dataset Description

- **Link:** https://www.kaggle.com/code/ammarnassanalhajali/iot-intrusion-detection-keylogging-cnn-img?select=Keylogger_Detection.csv
- **Labels:**  
  - `Benign` – normal system activity  
  - `Keylogger` – presence of keylogging behavior
- **Features:** Numeric system-level statistics (e.g., CPU usage, I/O counts, memory metrics).

---

## 🛠️ Data Processing and Workflow

The notebook follows these steps:

1. **Loading and Exploratory Analysis** – Read CSV, inspect feature distributions and missing values.
2. **Label Encoding** – Convert text labels to binary: `0` = Benign, `1` = Keylogger.
3. **Null/Constant Handling** – Remove missing records and features with no variance.
4. **Balancing & Sampling** – Uniform sampling to maintain performance with large datasets.
5. **Feature Scaling** – Normalize inputs for robust model training.
6. **Train/Test Split** – 80% training, 20% testing partition.

---

## 🧪 Model Training & Evaluation

- Implements classification models to detect keylogger presence.
- Includes metrics like **accuracy**, **precision**, **recall**, and **F1-score**.
- Provides visualizations: confusion matrices, ROC curves, and training-loss plots using **matplotlib** and **seaborn**.

---

## 📦 Installation

Ensure you have Python 3.8+, then:

```bash
pip install -r requirements.txt
```

▶️ Running the Notebook

    Place Keylogger_Detection.csv alongside aplab.ipynb.

    Launch the notebook:

jupyter notebook aplab.ipynb

    Follow the sequential cells to preprocess data, train models, and view results.

📁 Project Structure

aplab-project/

├── main.ipynb

├── requirements.txt

├── LICENSE

├── README.md

└── .gitignore

📄 License

This project is released under the MIT License.

👤 Author

Shourja Dutta

B.Tech, Computer Science & System Engineering

KIIT University (Batch of 2026)

🤝 Contributions

Pull requests are welcome! For significant changes, please open an issue first to discuss your ideas.
