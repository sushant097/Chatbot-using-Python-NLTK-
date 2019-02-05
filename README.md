# Chatbot-using-Python-NLTK
This is the Chatbot made with NLTK in python with Term Frequency-Inverse Document Frequencyn(TF-IDF) and Cosine Similarity. 

There are several way to create a ChatBot. Some are:
- Bag of Words
- TF-IDF Approach
- Cosine Similarity

## Bag of Words
 The bag-of-words is a representation of text that describes the occurrence of words within a document. It involves two things:
 - A vocabulary of known words.
 - A measure of the presence of known words.
 
 This is called as **Bag of words** since any information about the order or structure of words in the document is discarded and the model is only concerned with whether the known words occur in the document, not where they occur in the document.
The main logic behind the Bag of words is that documents should be similar if they contain similar content.

For Example, if the dictionary contains words {Chatbot, is, developing, better, than, yesterday} and need to vectorize the text "Chatbot is better", we would have the following vector: {1,1,0,1,0,0}

A problem with the Bag of Words approach is that highly frequent words start to dominate in the document (e.g. larger score), but may not contain as much “informational content”. Also, it will give more weight to longer documents than shorter documents.

## TF-IDF Approach
Another approach is to rescale the frequency of words by how often they appear in all documents so that the scores for frequent words. This approach is called Term Frequency-Inverse Document Frequency, or TF-IDF for short, where:

**Term Frequency**: is a scoring of the frequency of the word in the current document.
`TF = (Number of times term t appears in a document)/(Number of terms in the document)`

**Inverse Document Frequency**: is a scoring of how rare the word is across documents.

`IDF = 1+log(N/n), where, N is the number of documents and n is the number of documents a term t has appeared in.`

Tf-idf weight is a weight often used in information retrieval and text mining. This weight is a statistical measure used to evaluate how important a word is to a document in a collection or corpus
## Description
-  Use text file corpus to build Chatbot Knowledge.
-  You can build robust by making text corpus including all information needed to it.
-  You can also use web crawling eg: Build Chatbot about what is happening right now in this world by crawling news website like: BBC, CNN etc. The reference to **Beautiful Soup** web crawler found [here](https://github.com/sushant097/Text-Summarizer-in-Python-v1/blob/master/urlTextReader.py)

## References
-[TF-IDF versus Cosine Similarity]( https://stats.stackexchange.com/questions/140557/tf-idf-versus-cosine-similarity-in-document-search)
- [Cosine Similarity using TF-IDF weighting  Kaggle Post](https://www.kaggle.com/antriksh5235/cosine-similarity-using-tfidf-weighting)
