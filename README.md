# Text-Generation-using-LSTM-and-GloVe-Model

This project focuses on building a text generation system using an LSTM (Long Short-Term Memory) network enhanced with GloVe word embeddings. The goal is to train a deep learning model capable of understanding language patterns and generating coherent text when given a starting phrase. By combining sequential learning with semantic-rich vectors, the model produces meaningful and context-aware sentences.

The dataset used for training comes from the file ArticlesApril2017.csv, which contains news articles. These articles undergo preprocessing that includes text cleaning, tokenization, and the creation of input sequences used to teach the model how to predict the next word.

The model architecture begins with an embedding layer initialized using pre-trained GloVe vectors. This allows the network to start with strong semantic understanding. It is followed by an LSTM layer that captures long-term dependencies and patterns across sequences of words. A final dense layer with softmax activation predicts the most likely next word in the sequence. The model is trained using categorical cross-entropy loss and optimized to improve prediction accuracy.

To run the project, you can clone the GitHub repository and install the necessary dependencies. GloVe embeddings are required, and if they are not included, they can be downloaded separately from the Stanford NLP website. After setting up the environment, the entire workflow—from data preprocessing to model training and text generation—can be executed through the provided Jupyter Notebook.

This system is capable of generating text based on a provided seed phrase. For example, starting with a phrase like “global market,” the model can continue with a realistic and context-driven sentence. Although the current implementation is effective, future improvements may include using a BiLSTM architecture, integrating beam search for higher-quality text generation, working with larger datasets, or deploying the model as a web application.

This project is completely open-source and can be used freely for learning, experimentation, or research purposes.
