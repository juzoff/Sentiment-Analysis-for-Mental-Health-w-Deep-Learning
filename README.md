# DEEP LEARNING USING DistillBERT

## Using R, Prepared Dataset for DistillBERT Training Through Light Preprocessing and Exported as CSV File
#### - FILE: *Dataset preperation for DistillBERT.RMD*
#### Highlights:
- Light Text Preprocessing:
  - The text data undergoes minimal preprocessing, including:
    - Converting text to lowercase
    - Stripping extra whitespaces
    - Removing non-alphanumeric characters
    - Fixing specific encoding issues (e.g., replacing â€™ with ')
- Exporting Cleaned Data:
  - The cleaned dataset is exported as a CSV file (Cleaned_Statements_Less.csv) for model training with DistillBERT

## Loaded the Light Preprocessed Dataset and Trained a DistillBERT Model for Mental Health Status Classification
#### - FILE: *DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb*
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
  - Epochs: 8, Batch Size: 16 (Train) & 64 (Eval), Warmup Steps: 500, Weight Decay: 0.01, Metric: Accuracy
- Results:
  - Training completed in {trainer.state.global_step} steps
  - Best model saved at /content/drive/MyDrive/results/best_model

## Developed Functions to Evaluate the Model Using Confusion Matrices and Visualized Its Performance
#### - FILE: *DistillBERT_Sentiment_Analysis_Deep_Learning.ipynb*




## Implemented a Real-Time Prediction System That Classifies New Statements and Provides a Confidence Score for Each Mental Health Status Through the Trained DistillBERT Model





