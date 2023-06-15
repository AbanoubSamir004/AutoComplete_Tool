# AutoComplete_Tool


Implemented a Sentence AutoComplete Tool by integrating a word2vec pretrained model and LSTM. The project encompassed the following steps:

1. Loading Data: The Enron Sent Corpus Dataset was used as the training data. It was downloaded and loaded into the project, and the necessary tokenization and preprocessing techniques were applied to prepare the data.

2. Preprocessing the Data: The loaded data underwent preprocessing steps such as removing stopwords, handling punctuation, and performing any necessary data cleaning or normalization.

3. Train-Test Split: The preprocessed data was divided into training and validation sets. The training data consisted of enronsent00 to enronsent10, while the validation data included enronsent11 to enronsent15.

4. Splitting Data into Time Steps: To prepare the data for the LSTM model, the paragraphs were split into fixed time steps or sequences. Each sequence contained a certain number of words or tokens, allowing the model to learn the context and predict the next word effectively.

5. Word Embedding: A pretrained word2vec model was downloaded and used as an embedding layer in the LSTM model. This embedding layer mapped each word to a dense vector representation, capturing semantic relationships between words.

6. LSTM Model: The LSTM model was built using the Keras or PyTorch framework. It incorporated the word2vec embedding layer and additional LSTM layers to learn the patterns and relationships in the sequential data. The model was trained using the training data, and hyperparameters were fine-tuned to optimize the prediction accuracy.

7. Testing the Model: Users could enter sentences word by word, and the model would predict the next word based on the provided input. Users would verify the correctness of the prediction, and the model would continue predicting subsequent words until the user terminated the loop.

   - **Case 1:**
   
        ![Case 1 Screenshot](https://github.com/AbanoubSamir004/AutoComplete_Tool/assets/60902991/5e075f70-76c8-4094-bf47-5aafd600f36f)

   - **Case 2:**
   
        ![Case 2 Screenshot](https://github.com/AbanoubSamir004/AutoComplete_Tool/assets/60902991/694d067e-1926-4668-bc40-49da4adeeca2)

   - **Case 3:** 
  
        ![Case 3 Screenshot](https://github.com/AbanoubSamir004/AutoComplete_Tool/assets/60902991/357265b5-f7a6-406f-81f4-7d61672d66ff)
