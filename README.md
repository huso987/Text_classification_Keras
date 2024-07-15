# Text Classification with Keras
This project demonstrates how to build a text classification model using Keras. The dataset used for this project is the "fake_job_postings" dataset, which aims to classify job postings as fraudulent or not.

## Dataset
The dataset used in this project is the "fake_job_postings" dataset. It contains the following columns:

telecommuting: Indicates whether the job allows telecommuting (int).
has_company_logo: Indicates whether the job posting has a company logo (int).
has_questions: Indicates whether the job posting has screening questions (int).
required_experience: Specifies the required experience for the job (object).
fraudulent: Indicates whether the job posting is fraudulent (int).
text: Combined text column from various job description fields (object).

## Data Cleaning and Preprocessing
Remove Irrelevant Columns: Columns like salary_range and job_id are removed as they are not needed for text classification.
Handle Missing Values: Fill missing values with an empty string.
Combine Text Columns: Combine relevant text columns into a single column.
Text Cleaning: Remove HTML tags, special characters, stopwords, and perform lemmatization.

## Feature Extraction
TF-IDF Vectorization: Convert the cleaned text data into numerical features using TF-IDF vectorization.

## Model Training
Train-Test Split: Split the dataset into training and testing sets.
Neural Network Model: Build and train a neural network model using Keras with the following architecture:
Dense layer with 512 units and ReLU activation
Dense layer with 256 units and ReLU activation
Dense layer with 128 units and ReLU activation
Output layer with 1 unit and sigmoid activation

## Result

Test Accuracy: 98.04%
