# Social Media Analytics Project

## Project Overview
This project uses **Apache Spark** and other big data tools to analyze social media data and gain insights into user behavior, trends, and sentiment. Data from platforms like Twitter, Facebook, and LinkedIn is processed to uncover popular topics, brand discussions, and user engagement patterns.

## Problem Statement
The goal is to analyze social media data to determine:
- Popular or trending topics
- Sentiment towards specific brands or products
- Patterns of user engagement with social media content

## Steps Involved
### 1. Data Collection
- Collected social media data using APIs and third-party tools.
- Stored data in **CSV format**, with 6844 records.
- Focused on `review_text` and `review_rating` for further analysis.

### 2. Data Preparation
- Cleaned the dataset by removing duplicates and null values.
- Extracted relevant features like `review_text` and `review_rating`.
- Filtered out non-numeric values in the `review_rating` column and categorized ratings as negative, neutral, or positive.

### 3. Data Analysis
- Used **NLP** techniques to tokenize and remove stop words from `review_text`.
- Converted words into vectors for model input.
- Applied **Logistic Regression** to classify sentiment as positive, negative, or neutral.
- Split the dataset into 70% training and 30% testing data.

### 4. Model Evaluation
- Evaluated model accuracy using metrics like **accuracy**, **precision**, **recall**, and **F1 score**.
- Experimented with different class groupings (binary and multiclass classification) to improve accuracy.

### 5. Data Visualization
- Used histograms to visualize the distribution of ratings.
- Created bar charts to compare evaluation metrics between the training and testing datasets.

## Findings
- The dataset is **imbalanced**, leading to lower accuracy in sentiment classification.
- The best results were obtained using a **multiclass classification** approach, grouping ratings into negative (1-2), neutral (3), and positive (4-5).

## Tools and Technologies
- **Apache Spark**
- **PySpark**
- **NLP**
- **Logistic Regression**

## How to Run
1. Install the required packages (e.g., PySpark, NLP libraries).
2. Run the Jupyter Notebook to preprocess the data and train the model.
3. View the visualizations for model performance analysis.
