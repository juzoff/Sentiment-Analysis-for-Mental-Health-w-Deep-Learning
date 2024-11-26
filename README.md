
# Sentiment-Analysis-for-Mental-Health-w-Deep-Learning

### Note: This project is organized into multiple branches on GitHub, each correlating with a different portion of the assignment. To explore specific sections, please select the branch that corresponds to the task or analysis you are interested in. 
## Branches: 
### >NLP - Data Preprocessing, Exploration, and Visualization (R) ###
- Loaded and explored the dataset, removing redundant columns and handling missing values
- Balanced the class attribute (Status) by adjusting each class to match the median status count (3888)
- Sampled the dataset by selecting 15% of the median value per class for consistency
- Applied NLP techniques, including term frequency (TF), word clouds, and TF-IDF, to analyze prominent words in each mental health status
- Calculated bigrams and created functions to count words and locate specific terms in the dataset
- Visualization (R):
  - Created interactive barcharts to visualize the TF, TF-IDF, Bigram for each mental health status
  - Generated word clouds to illustrate key terms across the entire dataset and by individual status

### >Deep Learning using DistillBERT (Using Python on Google Colab) ###
- Using R, prepared dataset for DistillBERT training through light preprocessing and exporting as CSV file
- Loading the light preprocessed dataset and trained a DistillBERT model for mental health status classification
- Developed functions to evaluate the model using confusion matrices and visualized its performance
- Implemented a real-time prediction system that classifies new statements and provides a confidence score for each mental health status through the trained DistillBERT model
## 
The project involved extensive data preprocessing, deep learning, and text analysis techniques to build a model capable of classifying mental health statuses based on textual statements. The goal was to build a model capable of identifying key mental health statuses such as Depression, Anxiety, Stress, Suicidal tendencies, Bipolar disorder, and Personality Disorders based on various types of text, including social media posts, forum conversations, and personal statements. By leveraging natural language processing (NLP) and deep learning techniques, this project allowed me to gain insights into mental health trends.

The dataset used for this project is a combination of several Kaggle datasets, including the 3k Conversations Dataset for Chatbots, Depression Reddit Cleaned, Human Stress Prediction, Bipolar and Suicidal Mental Health Datasets, and others. Each data entry is labeled with one of seven mental health statuses: Normal, Depression, Suicidal, Anxiety, Stress, Bipolar, or Personality Disorder. This diverse dataset provided a strong foundation for training models to classify mental health conditions based on text data.
