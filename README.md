# OIBSIP_Data-science_task4
# Objective of the Task
The objective of this project is to build a spam classifier that can distinguish between spam and ham (non-spam) emails using machine learning. The model is trained on a labeled SMS dataset and uses text preprocessing, TF-IDF vectorization, and a Naive Bayes classifier to make predictions.

# Steps Performed
1. Data Loading & Cleaning
Loaded the dataset (spam.csv) and retained only relevant columns (label, text).
Mapped textual labels: "ham" → 0, "spam" → 1.
2. Text Preprocessing
Converted text to lowercase.
->Removed:
Numbers
Punctuation
Extra whitespaces
Created a new clean_text column with preprocessed data using a custom cleaning function.
3. Model Pipeline
Used TF-IDF Vectorizer to convert text into numerical features.
Trained a Multinomial Naive Bayes classifier within a Pipeline for efficiency.
4. Model Training and Evaluation
Split the dataset into training and testing sets (80/20 split).
->Evaluated model using:
Accuracy Score
Classification Report
Confusion Matrix (Heatmap)
5. Model Saving and User Interaction
Saved the trained model using joblib as spam_detector_model.pkl.
Implemented a CLI-based classifier to take user input and predict whether it's spam or not.

# Tools & Technologies Used
1. Language: Python 🐍
2. Libraries:
pandas, numpy – Data manipulation
matplotlib, seaborn – Visualization
scikit-learn – Machine Learning pipeline, TF-IDF, Naive Bayes, model evaluation
joblib – Saving/loading the trained model
re, string – Text preprocessing

# Outcome / Results
✅ Achieved high accuracy in classifying spam vs. ham emails.
🔍 The model is lightweight and efficient, ideal for real-time applications.
🧠 Trained model supports live prediction from user input through the command line.
💾 Final model saved as: spam_detector_model.pkl
