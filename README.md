# DEEP LEARNING USING DistillBERT

## Using R, Prepared Dataset for DistillBERT Training Through Light Preprocessing and Exported as CSV File
### > FILE: 
    - Dataset preperation for DistillBERT.RMD
    - Dataset preperation for DistilBERT Training.pdf
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
  - The cleaned dataset is exported as a CSV file (Cleaned_Statements_Less.csv) for model training with DistillBERT

## Loaded the Light Preprocessed Dataset and Trained a DistillBERT Model for Mental Health Status Classification
### > FILE: 
    - DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb
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
  - Epochs: 16, Batch Size: 16 (Train) & 64 (Eval)
- Results:
  - Best model saved at /content/drive/MyDrive/results/best_model

## Developed Functions to Evaluate the Model Using Confusion Matrices and Visualized Its Performance
### > FILE: 
    - DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb
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


## Implemented a Real-Time Prediction System That Classifies New Statements and Provides a Confidence Score for Each Mental Health Status Through the Trained DistillBERT Model
### > FILE: 
    - DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb
#### Highlights:





