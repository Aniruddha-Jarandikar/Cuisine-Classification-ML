# Restaurant Cuisine Classification

## Project Overview

This project focuses on classifying restaurants into their primary cuisine categories using Machine Learning classification algorithms. The objective is to predict the cuisine type of a restaurant based on features such as location, pricing, ratings, customer votes, and service-related attributes.

## Dataset

The dataset contains restaurant information including:

- Country Code
- City
- Average Cost for Two
- Price Range
- Aggregate Rating
- Votes
- Has Table Booking
- Has Online Delivery
- Is Delivering Now
- Cuisines

For classification, the first cuisine listed for each restaurant was extracted as the **Primary Cuisine**.

## Data Preprocessing

The following preprocessing steps were performed:

- Removed records with missing cuisine values.
- Extracted the primary cuisine from multi-cuisine entries.
- Selected the top 10 most frequent cuisine categories.
- Encoded categorical variables using Label Encoding.
- Converted binary Yes/No attributes into numerical values.
- Split the dataset into training and testing sets.

## Machine Learning Models

The following classification algorithms were trained and evaluated:

1. Logistic Regression
2. Random Forest Classifier

## Model Performance

| Model | Accuracy |
|---------|---------:|
| Logistic Regression | 45.47% |
| Random Forest | 41.77% |

### Best Performing Model

**Logistic Regression** achieved the highest classification accuracy and was selected as the final model.

## Feature Importance

The most influential features for cuisine prediction included:

- Aggregate Rating
- Votes
- Average Cost for Two
- City
- Price Range

These features contributed significantly to distinguishing between cuisine categories.

## Challenges and Biases

Several challenges were identified during the project:

- Significant class imbalance among cuisine categories.
- North Indian cuisine dominated the dataset.
- Minority cuisines had fewer samples, reducing prediction performance.
- Similar cuisines often shared overlapping characteristics such as pricing and ratings.

## Future Improvements

Potential enhancements include:

- Applying SMOTE for class balancing.
- Using NLP techniques on restaurant names and cuisine descriptions.
- Experimenting with advanced models such as XGBoost and Neural Networks.
- Incorporating additional restaurant attributes for improved classification accuracy.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Author

**Aniruddha Jarandikar**

Machine Learning Internship Project – Cognifyz Technologies
