# Implementation-of-an-application-to-classify-relations-according-to-the-context
This project is based on Deep Learning and NLP (Team Project)

keywords : unstructured text document, context, semantic relationship



DataSet(labeled : Text , Topic) : 

  - Manually 600 unstructured Texts collected from wikipedia  .
  
  - Topics were manually extracted .



Description :


Today, and thanks to the Web, the use of information technology has
led to an explosion in the volume of data exchanged between individuals,
companies, etc. and even led to a profound change in all aspects
economic, political and social. This growth
constant of heterogeneous data volume leads to greater complexity
in information retrieval and knowledge extraction.
It’s in that context that we’re talking about. We’re talking about extraction.
information from textual documents. More specifically, we
we are interested in extracting relationships between named entities and their
context classification.
Our objective is to develop an application whose realization is made in
two parts: the first part is devoted to the improvement of extraction
of context from an unstructured text document. This step
is based on “deep learning”.


![protocole expérimental](https://user-images.githubusercontent.com/78451998/184122796-20251534-5a2c-423c-9cf0-4ca07720f1e8.png)



Steps: 

1- Extract Keywors(important words) from unstructured text documents : used deveral keyword extraction tools : 

TF-IDF/KeyBert/LDA/TextRank - chosed the best tool comparing to the giving


![graphe](https://user-images.githubusercontent.com/78451998/184121932-aad0c026-caa6-44b5-ad3d-192613ff578e.png)

F1-score results for each one.



2- Training our model using :

 2-1 Word2Vec to vectorize our sentence and create sentence embeddings
 
 2-2 Training our Model using LSTM
 
 2-3 Training a 2nd Model using GRU
 
 2-3 chosing the best architecture according to the giving accuracy in our case ==> LSTM
 
 
 
3- Extracting the context using Markov chains (trained on our Dataset)/LSTM Model/Python code 

![try1](https://user-images.githubusercontent.com/78451998/184121900-fc557de1-9423-4794-ad49-5aee70bcdb12.PNG)



4- Compare the givin context with the one figured in our dataset using ROUGE matric.

Read More about ROUGE metric : https://medium.com/nlplanet/two-minutes-nlp-learn-the-rouge-metric-by-examples-f179cc285499
