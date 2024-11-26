# DEEP LEARNING USING DistillBERT

## Using R, Prepared Dataset for DistillBERT Training Through Light Preprocessing and Exported as CSV File
### > FILE: *Dataset preperation for DistillBERT.RMD*
#### Highlights:
- Check for missing values
- Balance Class Counts:
  - Equalize the count of each mental health status category by adjusting them to the median value (3888)
- Set Fixed Sample Size per Class:
  - Select a fixed sample size for each class, equivalent to 15% of the median value (15% of 3888 = ~583 samples per class)
- Light Text Preprocessing:
  - The text data undergoes minimal preprocessing, including:
    - Converting text to lowercase
    - Stripping extra whitespaces
    - Removing non-alphanumeric characters
    - Fixing specific encoding issues (e.g., replacing â€™ with ')
- Exporting Cleaned Data:
  - The cleaned dataset is exported as a CSV file (Cleaned_Statements_Less.csv) for model training with DistillBERT

## Loaded the Light Preprocessed Dataset and Trained a DistillBERT Model for Mental Health Status Classification
### > FILE: *DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb*
#### Highlights:
- Dataset Preparation:
  - Preprocessed and classified mental health status into 7 categories (e.g., Normal, Depression, Anxiety)
- DistillBERT Tokenization:
   - Applied DistilBertTokenizer for text tokenization
- Custom Dataset Class:
  - Organized tokenized data using a SentimentDataset class
- Model Training:
  - Fine-tuned DistilBertForSequenceClassification with Hugging Face Trainer API
- Hyperparameters:
  - Epochs: 8, Batch Size: 16 (Train) & 64 (Eval)
- Results:
  - Best model saved at /content/drive/MyDrive/results/best_model

## Developed Functions to Evaluate the Model Using Confusion Matrices and Visualized Its Performance
### > FILE: *DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb*
#### Highlights:
- Metrics Calculation:
  - Accuracy: 
    - **0.8005%**
  - Precision (Weighted): 
    - **0.8193%**
  - Recall (Weighted):
    - **0.8005%**
  - Specificity: 
    - **0.7665%**
- Confusion Matrix
  - Generated and visualized a confusion matrix using Seaborn's heatmap to display the distribution of predictions vs. actual labels
![confusion matrix](https://github.com/user-attachments/assets/c3c9c4bf-dda5-4dbc-a05c-57e1d23a3a5e)
![pic](https://github.com/user-attachments/assets/c0179f20-64f5-4ecf-8200-767b629aa63b)

## Implemented a Real-Time Prediction System That Classifies New Statements and Provides a Confidence Score for Each Mental Health Status Through the Trained DistillBERT Model
### > FILE: *DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb*
#### Highlights:





