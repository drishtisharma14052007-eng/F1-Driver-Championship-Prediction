# 🏎️ F1 Champion Predictor
### Formula 1 Driver Champion Classification Using Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange" />
  <img src="https://img.shields.io/badge/Status-Completed-success" />
  <img src="https://img.shields.io/badge/Platform-Google%20Colab-yellow?logo=googlecolab" />
</p>

## 🏁 About the Project

**F1 Champion Predictor** is a machine learning classification project that analyzes historical Formula 1 driver statistics to classify drivers into two categories:

- 🏆 **Champion** – Drivers who have won at least one championship.
- 🏎️ **Non-Champion** – Drivers who have not won a championship.

The project explores how different driver performance metrics, including race wins, podiums, pole positions, fastest laps, and points, can be used to identify championship-winning drivers.

Four machine learning algorithms are implemented and evaluated to compare their classification performance.

## 🎯 Project Objectives

- Analyze historical Formula 1 driver performance data.
- Perform data preprocessing and exploratory data analysis (EDA).
- Identify important numerical features using correlation analysis.
- Build and train multiple machine learning classification models.
- Evaluate model performance using accuracy, precision, recall, F1-score, and confusion matrices.
- Compare different algorithms to identify the best-performing model.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine learning models and evaluation |
| Google Colab | Development environment |

## 📊 Dataset & Features

The project uses a Formula 1 driver statistics dataset (`F1Drivers_Dataset.csv`).

The following features are used for model training:

| Feature | Description |
|---|---|
| Race_Wins | Total race victories |
| Pole_Positions | Number of pole positions |
| Fastest_Laps | Fastest laps achieved |
| Podiums | Total podium finishes |
| Win_Rate | Race win rate |
| Pole_Rate | Pole position rate |
| Points | Driver points |
| Points_Per_Entry | Average points per entry |
| FastLap_Rate | Fastest lap rate |
| Podium_Rate | Podium rate |
| Race_Starts | Total race starts |

**Target Variable:** `Champion`

- `1` → Champion
- `0` → Non-Champion

## ⚙️ Project Workflow

The project follows these steps:

**1. Data Loading**
- Import the dataset using Pandas.
- Inspect dataset structure and available columns.

**2. Data Preprocessing**
- Examine missing values and dataset information.
- Remove the Championship Years feature.
- Convert the Seasons feature into a numerical count.

**3. Exploratory Data Analysis (EDA)**
- Correlation heatmap.
- Champion vs Non-Champion distribution.
- Race wins distribution.
- Pairwise feature relationships.

**4. Feature Selection**
- Analyze correlations between numerical features and championships.
- Select performance-related features for model development.

**5. Data Splitting & Scaling**
- Split the dataset into 80% training and 20% testing.
- Use stratified sampling.
- Apply StandardScaler to numerical features.

**6. Model Training**
Train four different classification algorithms.

**7. Model Evaluation**
Compare classification reports, confusion matrices, and accuracy scores.

**8. New Driver Classification**
Test the trained models on a sample set of new driver statistics.

## 🤖 Machine Learning Models

The following algorithms are implemented:

1. **K-Nearest Neighbors (KNN)** – Classifies drivers based on nearby data points.
2. **Logistic Regression** – Uses a logistic function for binary classification.
3. **Decision Tree** – Uses decision-based splits to classify drivers.
4. **Random Forest** – Combines multiple decision trees to improve classification performance.

## 📈 Model Performance

Based on the recorded notebook outputs:

| Model | Accuracy |
|---|---:|
| KNN | 98.85% |
| Logistic Regression | 97.70% |
| Decision Tree | 98.85% |
| Random Forest | 99.43% |

🏆 **Best Performing Model: Random Forest**

Random Forest achieved the highest recorded accuracy of approximately **99.43%** on the test dataset.

*Note: The test set contains significantly more Non-Champion than Champion samples. Accuracy alone may therefore overstate performance, so precision, recall, F1-score, and class-wise results should also be considered.*

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/F1ChampPredictor.git
cd F1ChampPredictor
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Add the Dataset

Place `F1Drivers_Dataset.csv` in your Google Drive and update the dataset path in the notebook if required.

### 4. Run the Notebook

Open `F1ChampPredictor.ipynb` in Google Colab or Jupyter Notebook.

Run the cells sequentially to perform preprocessing, visualization, model training, evaluation, and classification.

## 🔮 Future Improvements

- Incorporate additional historical and seasonal Formula 1 data.
- Address class imbalance using suitable resampling techniques.
- Perform hyperparameter tuning to optimize model performance.
- Add feature importance analysis.
- Develop a user-friendly interface for driver classification.
- Extend the project towards predicting championship outcomes using season-specific data.

## 📌 Key Learnings

Through this project, I explored:

- Data preprocessing and exploratory data analysis.
- Feature selection using correlation analysis.
- Binary classification using Scikit-learn.
- Feature scaling and train-test splitting.
- Training and comparing multiple ML algorithms.
- Evaluating models using classification metrics.
- Applying trained models to new input data.

## 👩‍💻 Author

**Drishti Sharma**

B.Tech Computer Science and Engineering

Interested in Machine Learning, Artificial Intelligence, and Software Development.

- GitHub: [@drishtisharma14052007-eng](https://github.com/drishtisharma14052007-eng)
- LinkedIn: [Drishti Sharma](https://www.linkedin.com/in/drishti-sharma-a26b88374/)

---

⭐ If you find this project interesting, consider giving the repository a star!

*Built as a hands-on machine learning project exploring Formula 1 driver performance statistics.*
