# Classifying Wine Varieties Based on The Provided Wine Expert Descriptions in The Wine Reviews Dataset using DistilBERT as the Language Model

# Project Description
This project implements a wine variety classification system based on textual descriptions provided by wine experts. Using DistilBERT, a lighter and faster version of BERT, the model aims to classify wine varieties based on detailed descriptions of their taste, aroma, and other characteristics.

# Problem Statement:
With the vast diversity in wine types, distinguishing between varieties based on expert descriptions can be challenging for consumers. To aid in wine selection, this project seeks to build a model that can automatically classify wine varieties based on the text reviews associated with each wine.

# Methodology:
**Dataset:**

- The dataset used in this project is sourced from Kaggle’s Wine Reviews dataset, which contains detailed reviews of different wines.
- After performing Exploratory Data Analysis (EDA), the focus was narrowed down to the four most frequent wine varieties in the dataset.
![image](https://github.com/user-attachments/assets/490c28cc-18ef-4dac-8315-1930dd735e98)


**Preprocessing:**

- Only the relevant columns, "description" (containing the text) and "variety" (representing the wine type), were retained.
- Tokenization was done using the tokenizer from the DistilBERT model to convert text data into input IDs and attention masks.
![image](https://github.com/user-attachments/assets/38e722a6-1e98-4cd0-a1ba-5f90d6c1739e)


**Modeling:**

- DistilBERT (uncased) was used as the base model for text classification, with the classification head fine-tuned to output predictions for wine varieties.
- The model was fine-tuned and evaluated using hyperparameters such as learning rate, batch size, dropout rate, and the number of epochs.

**Parameter Tuning:**

Hyperparameters were tuned to find the optimal values for model performance, with manual adjustments made to the learning rate, epoch, dropout, and other model parameters.
![image](https://github.com/user-attachments/assets/1e6da46f-561b-41c7-b602-6c951f6c3cdf)


**Results:**

- The model achieved an accuracy of 91%, indicating strong performance in classifying wines based on the expert descriptions.
- Performance across classes was consistent, with the Chardonnay class showing the best results in terms of precision, recall, and F1 score.
![Uploading image.png…]()


# Conclusion:
The use of DistilBERT proved effective for the task of classifying wine varieties based on textual descriptions, offering a smaller, faster model with a performance level close to the original BERT model.


Link Dataset : https://www.kaggle.com/datasets/zynicide/wine-reviews
