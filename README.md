
# NLP - Data Preprocessing, Exploration, and Visualization (R)

## Task 1 ##
##  > FILES:
    Sentiment Analysis for Mental Health - Data Preprocessing, Exploration, Visualization.Rmd
    Sentiment Analysis for Mental Health - Data Preprocessing, Exploration, Visualization.pdf (Knitted)
### 1.1: Loaded and explored the dataset, removing redundant columns and checking/handling missing values
### 1.2: Balanced the class attribute (Status) by adjusting each class to match the median status count (3888)
### 1.3: Sampled the dataset by selecting 15% of the median value per class for consistency
### 1.4: Preprocessing text data
### 2.1, 2.2, 2.3: Applied NLP techniques, including identifying term frequency (TF), TF-IDF, and bigrams to analyze prominent words in each mental health status
##### *Sentiment Analysis for Mental Health - Barcharts.PDF is a document containing interactive barcharts visualizing the TF, TF-IDF, Bigram for each mental health status*(2.1, 2.2, 2.3)
    Sentiment Analysis for Mental Health - Barcharts.PDF
- Examples: Stress and Suicidal (for the other 5 statuses, see directly above)
<img src="https://github.com/user-attachments/assets/5d76a996-6c6d-42fc-a874-fd91d70edbcf" alt="stresstf" width="300" />
<img src="https://github.com/user-attachments/assets/c4ce7a29-c60c-47bf-aa6f-fe2d48fcaeee" alt="TFIDF Stress" width="300" />
<img src="https://github.com/user-attachments/assets/aa3c0960-86bf-4f3b-97c5-fb0b20e1a4bb" alt="Bigram Stress" width="300" />

<img src="https://github.com/user-attachments/assets/40143b84-50a7-46f8-9e88-953ab971cb46" alt="tfsuicidal" width="300" />
<img src="https://github.com/user-attachments/assets/232d8664-125b-40d0-b9b7-25b9a0ab85cb" alt="TFIDF Suicidal" width="300" />
<img src="https://github.com/user-attachments/assets/2db898db-c5e8-4389-b5a6-d33aba8940ff" alt="Bigram Suicidal" width="300" />

### 3.1: Function to search for a word in a particular status and return the count of occurrences
### 3.2: Function to search for the location of a word in a particular status
### 3.3: Function to calculate Cosine Similarity between 2 inputted sentences

## Task 2 ##
##  > FILES:
    Sentiment Analysis for Mental Health - Word Clouds.Rmd
    Sentiment-Analysis-for-Mental-Health---Word-Clouds.pdf (Knitted)
### Generated word clouds to illustrate key terms across the entire dataset and by individual status
***Includes Steps 1.1, 1.2, 1.3, 1.4***
#### Word Cloud - Every Status
![All](https://github.com/user-attachments/assets/58ccd470-d6c2-4808-974c-f67990f52f1c)
#### Word Cloud - Anxiety
![Anxiety](https://github.com/user-attachments/assets/44d9ede9-d201-414f-8777-dec9986bd18f)
#### Word Cloud - Bipolar
![Bipolar](https://github.com/user-attachments/assets/cb6d77bb-65dc-468f-b32b-1b7711a72e74)
#### Word Cloud - Depression
![Depression](https://github.com/user-attachments/assets/c09c265f-08cd-4a3c-9abd-d79340a29ffc)
#### Word Cloud - Normal
![Normal](https://github.com/user-attachments/assets/9d23ccd0-18f0-4775-a147-7d0f3c898252)
#### Word Cloud - Personality Disorder
![Personality Disorder](https://github.com/user-attachments/assets/798dcabb-1b47-46ba-9787-095b4687c9fd)
#### Word Cloud - Stress
![Stress](https://github.com/user-attachments/assets/02734738-99b4-4ac9-9ec9-e07666e1e6a2)
#### Word Cloud - Suicidal
![Suicidal](https://github.com/user-attachments/assets/a577836f-5590-4167-8565-a616e4211b87)











