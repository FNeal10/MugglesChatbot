Mental Health Chatbot
Overview
This project is an advanced conversational AI designed to assist users with mental health-related inquiries. The chatbot is fine-tuned on a dataset specifically curated for mental health FAQs, ensuring that it is well-versed in common concerns and therapeutic insights. The model offers supportive and understanding responses, helping users feel heard and valued.

Dataset
Our dataset is sourced from Kaggle and contains 3 features and 100 rows with no missing values. The pre-processing steps include:

Remove Punctuation: All punctuation marks are removed to ensure clean and uniform text data.
Remove Non-ASCII Characters: Characters that are not in the standard ASCII range are removed.
Remove Extra Whitespace: Any extra spaces are eliminated to maintain consistency.
Text Lowering and Tokenization: The text is converted to lowercase and split into individual words (tokens).
Remove Stopwords: Common words that do not add significant meaning (like "and", "the", "is") are removed.
Filter Short Tokens: Words with a length of less than three characters are excluded to focus on meaningful terms.
Lemmatization and Stemming: Words are converted to their base forms using lemmatization and further reduced to their root forms using stemming.
Combine Tokens: The processed words are reassembled into a single string.
We employed Bag of Words and TF-IDF (Term Frequency-Inverse Document Frequency) along with cosine similarity to further process and analyze the text data. These techniques help in quantifying the text and measuring the similarity between different text documents, enhancing the chatbot's ability to understand and generate relevant responses.

Implementation
Data Collection and Preprocessing:
The dataset is collected from Kaggle, ensuring it is clean and complete.
Preprocessing steps are applied to standardize and prepare the text data for further analysis.
Feature Extraction:
Using Bag of Words and TF-IDF, the text data is transformed into numerical vectors that represent the importance of each word in the context of the dataset.
Cosine Similarity Calculation:
This method is used to measure the similarity between text documents, allowing the chatbot to find the most relevant responses to user queries based on the processed data.
Model Training:
The processed and transformed data is used to train the chatbot model, enabling it to understand and generate responses to various mental health-related questions.
Deployment:
The trained chatbot is deployed using Google Colab and Python NLP, ensuring a scalable and robust implementation that can interact with users effectively.
Conclusion
Our chatbot leverages advanced text preprocessing techniques, Bag of Words, TF-IDF, and cosine similarity to deliver accurate and empathetic responses to mental health-related queries. By utilizing a well-curated dataset from Kaggle and employing state-of-the-art natural language processing methods, we have developed a robust and reliable tool that can assist users in navigating their mental health concerns. The model's deployment in Google Colab using Python NLP ensures that it is both scalable and efficient, providing valuable support to those in need.

Dependencies
Python 3.8+
NLTK
Scikit-learn
Flask
Re
NumPy
Pandas
Acknowledgements
The dataset is sourced from Kaggle.
