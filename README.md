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
    - **0.8369%**
  - Precision (Weighted): 
    - **0.8380%**
  - Recall (Weighted):
    - **0.8369%**
  - Specificity: 
    - **0.8106%**
- Confusion Matrix
  - Generated and visualized a confusion matrix using Seaborn's heatmap to display the distribution of predictions vs. actual labels
![er](https://github.com/user-attachments/assets/d62bbe61-e3f7-43d1-9e5e-d2a06889b0a2)
![cm](https://github.com/user-attachments/assets/fb4aa9df-42c6-466e-90e6-50821bc51bd4)



## Implemented a Real-Time Prediction System That Classifies New Statements and Provides a Confidence Score for Each Mental Health Status Through the Trained DistilBERT Model
### > FILE: 
    - DistilBERT_Sentiment_Analysis_NLP_Deep_Learning.ipynb
#### Highlights:
- Label Mapping
- Prediction Function: predict_statement
- Returned Values
  - The mental health status with the highest predicted probability is returned

![pred2](https://github.com/user-attachments/assets/f93549f7-d63f-478d-8ddf-b730711df0f6)
![pred](https://github.com/user-attachments/assets/9bd84c58-22c4-4baa-9996-6226535c2412)




