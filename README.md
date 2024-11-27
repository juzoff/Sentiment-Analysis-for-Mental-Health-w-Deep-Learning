# DEEP LEARNING USING DistilBERT

## Using R, Prepared Dataset for DistilBERT Training Through Light Preprocessing and Exported as CSV File
### > FILE: 
    - Dataset preperation for DistilBERT.Rmd
    - Dataset preperation for DistilBERT.pdf (Knitted)
#### Highlights:
- Check for missing values
- Balance Class Counts:
  - Equalize the count of each mental health status category by adjusting them to the median value (3888)
- Set Fixed Sample Size per Class:
  - Select a fixed sample size for each class, equivalent to 25% of the median value (25% of 3888 = ~972 samples per class)
- Light Text Preprocessing:
  - The text data undergoes minimal preprocessing, including:
    - Converting text to lowercase
    - Stripping extra whitespaces
    - Removing non-alphanumeric characters
    - Fixing specific encoding issues (e.g., replacing â€™ with ')
- Exporting Cleaned Data:
  - The cleaned dataset is exported as a CSV file (Cleaned_Statements_Less.csv) for model training with DistilBERT

## Loaded the Light Preprocessed Dataset and Trained a DistilBERT Model for Mental Health Status Classification
### > FILE: 
    - DistilBERT_Sentiment_Analysis_Deep_Learning.ipynb
#### Highlights:
- Dataset Preparation:
  - Preprocessed and classified mental health status into 7 categories (e.g., Normal, Depression, Anxiety)
- DistilBERT Tokenization:
   - Applied DistilBertTokenizer for text tokenization
- Custom Dataset Class:
  - Organized tokenized data using a SentimentDataset class
- Model Training:
  - Fine-tuned DistilBertForSequenceClassification with Hugging Face Trainer API
- Hyperparameters:
  - Epochs: 16, Batch Size: 16 (Train) & 64 (Eval)
- Results:
  - Best model saved at /content/drive/MyDrive/results/best_model

## Developed Functions to Evaluate the Model Using Confusion Matrices and Visualized Its Performance
### > FILE: 
    - DistilBERT_Sentiment_Analysis_NLP_Deep_Learning.ipynb
#### Highlights:
- Metrics Calculation:
  - Accuracy: 
    - **0.8229%**
  - Precision (Weighted): 
    - **0.8274%**
  - Recall (Weighted):
    - **0.8229%**
  - Specificity: 
    - **0.7945%**
- Confusion Matrix
  - Generated and visualized a confusion matrix using Seaborn's heatmap to display the distribution of predictions vs. actual labels
![confusion matrix](https://github.com/user-attachments/assets/af971b9b-8d5e-4d6b-8d27-e3951c0b2b4d)
![output](https://github.com/user-attachments/assets/4591fdcb-678c-41d8-a27c-f5ed112f3784)


## Implemented a Real-Time Prediction System That Classifies New Statements and Provides a Confidence Score for Each Mental Health Status Through the Trained DistilBERT Model
### > FILE: 
    - DistilBERT_Sentiment_Analysis_NLP_Deep_Learning.ipynb
#### Highlights:
- Label Mapping
- Prediction Function: predict_statement
- Returned Values
  - The mental health status with the highest predicted probability is returned
![PREDICTION](https://github.com/user-attachments/assets/1b719e61-0193-40c3-93e6-844448f01af4)
![prediction2](https://github.com/user-attachments/assets/b76d56de-ce4b-4d82-9165-9b8baf449433)




