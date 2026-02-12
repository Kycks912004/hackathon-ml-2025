[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/guIftrs1)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=21087737&assignment_repo_type=AssignmentRepo)
# Titanic: Predicting Survival - Hackathon Challenge 🚢

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
