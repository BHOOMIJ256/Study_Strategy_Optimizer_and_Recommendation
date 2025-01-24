# Study_Strategy_Optimizer_and_Recommendation

**Problem Statement :** In Today's Educational system, students often struggle to optimize their study strategies due to the lack of personalized guidance tailored to their unique academic strengths, weaknesses, and time constraints.This challenge is particularly pronounced when juggling multiple subjects, limited resources, and varying levels of parental support and test preparation.

Traditional study plans are typically generalized and fail to account for individual learning patterns, leading to suboptimal performance and wasted effort. Furthermore, factors such as weak subject areas, test preparation effectiveness, and available study hours are not adequately analyzed or utilized to maximize academic outcomes.

## Project Objective:Study Strategy Optimizer and Recommendations⌛

The Student Study Strategy Optimizer aims to bridge this gap by leveraging data science and deep learning to create a personalized study strategy for each student. By analyzing historical performance data, demographic factors, and study habits, this solution will:

1. Identify weak subjects that require additional focus.
2. Recommend an optimal allocation of study hours for each subject based on available student data.
3. Suggest necessary guidelines and tips for enhanced and better outcomes.

## Table of Contents
- [Reading the Data](#ReadingtheData)
- [Data Cleaning and Preprocessing](#DataCleaningandPreprocessing)
- [Exploratory Data Analysis](#ExploratoryDataAnalysis).
- [Feature Engineering](#FeatureEngineering).
- [Model Development & Evaluation](#ModelDevelopment&Evaluation)
- [Tech Stack Used](#TechStackUsed).
  
## Reading the Data
The above dataset is Student Performance dataset with 10,000 unique values from <a href ="https://www.kaggle.com/datasets/nadeemajeedch/students-performance-10000-clean-data-eda/data"> kaggle </a>

The dataset conatins 12 Attributes/features:
1. **Roll_No** : Represent the roll number of the student.
2. **Gender**: Analyzing performance differences between male and female students.
3. **Race_Ethinicity** :Allows analysis of academic performance trends across different racial or ethnic groups.
4. **Parental Level of Education**: Indicates the educational background of the student's family.
5. **Lunch**: Shows whether students receive a free or reduced lunch, which is often a socioeconomic indicator.
6. **Test Preparation Course**: This tells whether students completed a test prep course, which could impact their performance.
7. **Math Score**: Provides a measure of each student’s performance in math, used to calculate averages or trends across various demographics.
8. **Science Score**: Evaluates students' Science knowledge, which can be analyzed to assess overall scentific knowledge of the student.
9. **Reading Score**: Measures performance in reading, allowing for insights into literacy and comprehension levels among students.
10. **Writing Score**: Evaluates students' writing skills, which can be analyzed to assess overall literacy and expression.
11. **Total Score:** Shows the total number achieved by the student out of 400.
12. **Grade:** Grade achieved by the student. "A" grade if Total marks >= 320, "B" grade if Total marks >= 250, "C" grade if Total marks >= 200, "D" grade if Total marks >= 150 and Fail if <150.

## Data Cleaning and Preprocessing 
1. Checking **Sum of Null** Values.
2. Checking **Sum of Duplicated** Values
3. Conversion of **float values** to **numeric values** for better interpretability
4. Imputation of null values by **mean, median or mode**

## Exploratory Data Analysis
1. Performed **Univariate analysis** on different variables/attributes, through **bar charts, histograms**.
2. Utilized **pie-charts** to showcase distributions among variable values.
3. Performed **correlation on attributes** to display relationship between them. **Scatter plots** for total score with math_score, science_score, reading_score and writing_score.
4. **Correlation heatmap** on all 4 score variables.
 
## Feature Engineering 
1. Dropped **irrelevant columns** for further analysis.
2. **Identified weak subjects** along with **average scores** and **score variability** between subjects.
3. **Label Encoding** for categorical variables.
4. Formulated **key performance indicators** like **High Performance or Low Performance** based on threshold value.
5. **Scaled all numerical** features by min-max scaling.

## Model Development & Evaluation
1. Developed a **simple sequential perceptron** with 4 layers.
2. Utilized the **Relu** and **Sigmoid** activation functions with 50 epochs.
3. Attained **99% test accuracy**.
4. Saved and loaded the model for further usuage and predictions as per user input.
5. Created a **time allocation and recommendations system** based on user inputs.

## Tech Stack Used 
> **Programming language** : Python

> **Libraries** : Numpy, Pandas, Seaborn, Matplotlib, scikit-learn, tensorflow/keras.

> **Platform** : Google Colab



