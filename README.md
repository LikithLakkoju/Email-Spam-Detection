# Email Spam Detection with Machine Learning

This project demonstrates a simple spam detection system using Logistic Regression with text preprocessing through `TfidfVectorizer`. The system classifies emails as "spam" or "ham" (not spam) based on their content.

## Features
- **Data Preprocessing**: Cleans and prepares the dataset by removing unnecessary columns and handling missing values.
- **Feature Extraction**: Converts text into TF-IDF features for better model performance.
- **Model Training**: Uses Logistic Regression for training on labeled email data.
- **Evaluation**: Provides accuracy metrics on both training and test datasets.
- **Prediction**: Allows prediction of whether a given email is spam or ham.

## Dataset
The dataset used in this project is a CSV file with labeled email messages, where:
- `v1` column contains labels (`spam` or `ham`).
- `v2` column contains the email text.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo-name/email-spam-detection.git
   cd email-spam-detection
2. **Install Dependencies**:
   ```bash
   pip install numpy pandas scikit-learn
3. **Download the Dataset**: Ensure spam1.csv is in the project directory or update the code with the path to your dataset.

## Code Overview
- **Data Loading and Cleaning**: Loads spam1.csv, removes unused columns, and fills missing values.
- **Label Encoding**: Encodes "spam" as 0 and "ham" as 1.
- **Train-Test Split**: Splits the dataset into training and testing sets.
- **TF-IDF Vectorization**: Transforms the email content into numerical features using TfidfVectorizer.
- **Model Training**: Trains a Logistic Regression model on the transformed data.
- **Prediction and Evaluation**: Outputs accuracy scores on both the training and test data. Allows for custom email classification.

## Usage
1. **Train the Model**: Run the script to train the model on the dataset. The model's accuracy will be displayed on both training and test data.
2. **Predict Email Classification**: Use the input_mail variable in the script to input an email text. The model will output whether the email is classified as spam or ham.

## Example Output

The code will display accuracy results and classify sample emails as spam or ham. For example:
```python
input_mail = ["Even my brother is not like to speak with me. They treat me like aids patent."]
```````
This will output:
```
Ham Mail

