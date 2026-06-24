# 🚢 Hackathon ML — Titanic Survival Prediction

[![Solution Kylian](https://img.shields.io/badge/Python-solution__kylian.py%20(CatBoost)-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/Kycks912004/hackathon-ml-2025/blob/main/hackathon-ml-2025-groupe-16-cargo-main/solution_kylian.py)
[![GitHub](https://img.shields.io/badge/GitHub-Code%20Source-181717?style=for-the-badge&logo=github)](https://github.com/Kycks912004/hackathon-ml-2025)

## 🏆 Résultats

| Métrique | Score |
|----------|-------|
| **Meilleure précision** | **80.68 %** |
| Algorithme | CatBoostClassifier |
| Split | 84% train / 16% validation |
| Seed | 42 |

**Soumission finale** — extrait de `soumission_finale.csv` :

| PassengerId | Survived |
|------------|----------|
| 892 | 0 |
| 893 | 0 |
| 894 | 0 |
| 895 | 0 |
| 896 | 1 |
| … | … |

**Features engineering utilisées :**
- Extraction du titre (`Mr`, `Miss`, `Rare`…)
- Indicateur `Est_enfant` (Titre + Age < 18)
- Nb de mots dans le nom
- Première lettre de la cabine
- Remplacement des NaN (médiane / catégorie `X`)

---

Welcome to the Titanic Survival Prediction challenge! This is a classic data science problem and a perfect way to practice your skills in data exploration, feature engineering, and machine learning.

## The Challenge

The goal is to use machine learning to create a model that predicts which passengers survived the Titanic shipwreck. You will be working with a dataset of real passenger information.

For the full competition details, rules, and data description, please visit the official Kaggle page:
[https://www.kaggle.com/c/titanic](https://www.kaggle.com/c/titanic)

## 📂 Project Structure

This project is designed to be completed **entirely within the `titanic_analysis.ipynb` Jupyter Notebook**. The structure is simple:

.
├── data/ <br/>
│&nbsp;&nbsp;&nbsp;&nbsp;├── train.csv <br/>
│&nbsp;&nbsp;&nbsp;&nbsp;└── test.csv <br/>
├── .gitignore <br/>
├── README.md <br/>
├── requirements.txt <br/>
├── submission.csv <br/>
└── titanic_analysis.ipynb <br/>

## 🚀 Getting Started

Follow these steps to set up your project. You'll need to have **Anaconda** or **Miniconda** installed.

1.  **Clone the Repository:**
    ```bash
    git clone titanic-hackathon
    cd titanic-hackathon
    ```

2.  **Create a Conda Environment:**
    ```bash
    # Create a new conda environment named "titanic-env"
    conda create --name titanic-env python=3.10

    # Activate the new environment
    conda activate titanic-env
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Download the Data:**
    Download `train.csv` and `test.csv` from the [Kaggle data page](https://www.kaggle.com/c/titanic/data) and place them inside the `data/` folder.

5.  **Start Your Work in VS Code:**
    Open the entire project folder in VS Code with a single command.
    ```bash
    code .
    ```
    Once VS Code opens, open the `titanic_analysis.ipynb` file. In the top-right corner, click "Select Kernel." A dropdown will appear; be sure to choose the Python interpreter from your **`titanic-env`** Conda environment.


## 📝 Your Task: A Workflow for Your Notebook

All of your work—from exploration to final model training—should be done inside `titanic_analysis.ipynb`. Use the pre-made Markdown cells to structure your work with clear headings for each step.

1.  **Import Libraries and Load Data:**
    * Start by importing all the necessary libraries (`pandas`, `seaborn`, `scikit-learn`, etc.).
    * Load `train.csv` and `test.csv` into pandas DataFrames.

2.  **Exploratory Data Analysis (EDA):**
    * Inspect the data. Ask questions: How many people survived? What is the distribution of age, sex, and class? How do these features correlate with survival?
    * Use `matplotlib` and `seaborn` to create visualizations to answer your questions.

3.  **Data Cleaning & Feature Engineering:**
    * **Handle Missing Values:** Identify and fill missing data.
    * **Convert Categorical Features:** Transform columns like `Sex` and `Embarked` into numbers.
    * **Create New Features:** Engineer new features from existing ones.

4.  **Model Training and Evaluation:**
    * Choose a classification model from `scikit-learn`.
    * Split your training data to evaluate your model's performance before submitting.
    * Train your model.

5.  **Create Your Submission:**
    * In the final section of your notebook, use your trained model to make predictions on the test data.
    * Generate the `submission.csv` file directly from a code cell. The file must have exactly two columns: `PassengerId` and `Survived`.

## 🏆 Leaderboard

The leaderboard is scored based on **accuracy**—the percentage of passengers you correctly predict.

Good luck, and have fun!
