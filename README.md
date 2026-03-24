# 🌦️ Toronto Weather Prediction

> A machine learning project that analyzes historical weather data from Toronto, Ontario to build predictive models for weather forecasting.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Academic%20Project-blueviolet)

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Project Structure](#-project-structure)
- [Workflow](#-workflow)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Notebooks](#running-the-notebooks)
- [Data](#-data)
- [Analysis](#-analysis)
- [Prediction Models](#-prediction-models)
- [Tech Stack](#-tech-stack)
- [Results](#-results)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📌 Overview

This project applies machine learning techniques to **historical weather data from Toronto, Ontario** to understand patterns and build predictive models for key weather variables such as temperature and precipitation. The full pipeline — from raw data ingestion to model evaluation — is implemented in interactive **Jupyter Notebooks**.

This was developed as part of an academic assignment (Assignment 4) and demonstrates end-to-end data science skills including data cleaning, exploratory analysis, feature engineering, and supervised learning.

---

## 🗂️ Project Structure

```
Toronto_Weather_Prediction/
│
├── 📁 Analysis/              # Exploratory Data Analysis (EDA) notebooks & plots
├── 📁 Data/                  # Raw and processed Toronto weather datasets
├── 📁 Prediction/            # ML model training, evaluation & prediction notebooks
├── 📁 notebooks/
│   └── Assignment-4.ipynb   # Main assignment notebook (full pipeline)
└── requirements.txt          # Python dependencies
```

### Folder Breakdown

| Folder | Purpose |
|--------|---------|
| `Analysis/` | Data exploration, visualizations, trend analysis, and correlation studies |
| `Data/` | Raw CSV/dataset files with historical Toronto weather records |
| `Prediction/` | Feature engineering, model training, evaluation metrics, and output plots |
| `notebooks/` | End-to-end Jupyter notebook combining all steps |
| `requirements.txt` | All required Python libraries for reproducibility |

---

## 🔄 Workflow

```
Raw Data  ──►  Data Cleaning  ──►  EDA & Visualization  ──►  Feature Engineering
                                                                      │
                                                                      ▼
                                              Model Training  ◄──  Data Split
                                                      │
                                                      ▼
                                              Model Evaluation  ──►  Predictions
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- Python **3.8+**
- pip
- Jupyter Notebook or JupyterLab

### Installation

**1. Clone the repository:**

```bash
git clone https://github.com/kirmanioussema12/Toronto_Weather_Prediction.git
cd Toronto_Weather_Prediction
```

**2. (Recommended) Create a virtual environment:**

```bash
python -m venv venv
source venv/bin/activate        # On macOS/Linux
venv\Scripts\activate           # On Windows
```

**3. Install dependencies:**

```bash
pip install -r requirements.txt
```

### Running the Notebooks

```bash
jupyter notebook
```

Then navigate to one of the following in your browser:

| Notebook | Description |
|----------|-------------|
| `notebooks/Assignment-4.ipynb` | Full pipeline: data loading → EDA → modeling → evaluation |
| `Analysis/` | Individual EDA notebooks |
| `Prediction/` | Model-specific notebooks |

---

## 📊 Data

The `Data/` folder contains historical weather records for **Toronto, Ontario**. Typical features include:

| Feature | Description |
|---------|-------------|
| `Date` | Observation date |
| `Max Temp (°C)` | Daily maximum temperature |
| `Min Temp (°C)` | Daily minimum temperature |
| `Mean Temp (°C)` | Daily mean temperature |
| `Total Precip (mm)` | Total precipitation |
| `Snow on Grnd (cm)` | Snow on ground |
| `Speed of Max Gust (km/h)` | Wind gust speed |

> 📌 Data may be sourced from [Environment and Climate Change Canada (ECCC)](https://climate.weather.gc.ca/), which provides free historical climate data.

---

## 🔍 Analysis

The `Analysis/` folder covers:

- Distribution and histogram plots for all weather variables
- Seasonal trends (temperature, precipitation across months/years)
- Correlation heatmaps between features
- Missing value detection and handling
- Outlier detection and treatment

---

## 🤖 Prediction Models

The `Prediction/` folder and `notebooks/Assignment-4.ipynb` include:

- **Data preprocessing** — encoding, scaling, train/test split
- **Feature engineering** — lag features, rolling statistics
- **Model training** — one or more of the following:
  - Linear Regression
  - Decision Tree Regressor / Classifier
  - Random Forest
  - Gradient Boosting / XGBoost
- **Model evaluation** using metrics:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
  - R² Score
  - Accuracy / F1 (for classification tasks)
- **Visualizations** of predictions vs. actual values

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `Python 3.8+` | Core language |
| `Jupyter Notebook` | Interactive development |
| `Pandas` | Data manipulation and wrangling |
| `NumPy` | Numerical computations |
| `Matplotlib` | Data visualization |
| `Seaborn` | Statistical plotting |
| `Scikit-learn` | Machine learning models & evaluation |

> Check `requirements.txt` for exact versions.

---

## 📈 Results

Model performance results are documented inside the notebooks. Key takeaways:

- Temperature prediction shows strong regression performance due to seasonal patterns
- Precipitation is inherently noisier and harder to predict precisely
- Ensemble methods (Random Forest, Gradient Boosting) generally outperform linear baselines

---

## 🤝 Contributing

Contributions and suggestions are welcome! To contribute:

1. Fork the repository
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add: your descriptive message"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a **Pull Request**

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Oussema Kirmani**
- GitHub: [@kirmanioussema12](https://github.com/kirmanioussema12)

---

> 💡 *This project was developed as part of an academic assignment focusing on data science and machine learning applied to real-world climate data.*
