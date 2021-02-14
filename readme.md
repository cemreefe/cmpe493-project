# CMPE 493 Term Project

Cemre Efe Karakaş - 2016400153
Eylül Yalçınkaya - 2017400039



## Contents

There are five  Jupyter notebooks:

1. TfIdf_Vectorizer
2. Gensim_Doc2Vec
3. HuggingFace_Bert
4. Spacy
5. NeuralNetwork

​    We used Google Colab environment for our collaborative development process, all notebooks have the data preparation part in common for Colab environment. When you run the notebook in your own Colab environment, it will require you to mount your Google Drive and download the dataset in your drive. All libraries are installed within the notebook as well.

​    To run the notebooks, open them in your Colab environment and follow the instructions on the notebooks.

​    These five notebooks correspond to five different methods we experimented for our information retrieval task.

**TfIdf_Vectorizer**: This is the baseline method we used and presented at the progress presentation. `sklearn`'s TfIdfVectorizer is used to vectorize documents and topics. Then, cosine similarity is used to calculate a relevance score.

**Gensim_Doc2Vec**: `gensim`'s `Doc2Vec` model is trained using the documents. Then, both documents and topics are vectorized and cosine similarity is used to calculate a relevance score.

**HuggingFace_Bert**: 3 pretrained BERT models are used to calculate a relevance score between documents and topics.

**Spacy**: `spacy`'s pretrained model is used to vectorize documents and topics and cosine similarity is used to calculate a relevance score.

**NeuralNetwork**: Statistical features such as mean, standard deviation, their absolute valued counterparts for individual vectors, as well as the cosine similarity, euclidean distance and manhattan distance between document and topic embedding vectors are calculated. These numerical features are then fed into a neural network to predict the judgement value for a given topic, document pair. We can take into account both the vectors generated by spacy and gensim models.


