# Paragraph Layout Recognition
Comparative Analysis between GCN and LSTM 

There is often a need to convert a document-based image such as historical texts, hospital records, financial documents into machine readable data for editing, transferring, and cloud storage. This is a challenge since different documents are structured differently. When scanned, the document comes as a block of information; 
The machine then has to recognize the paragraphs, images etc. within the document. The problem has evolved from recognising just the text to identifying the structure of the text and discern images, paragraphs, tables etc. from it. 

Most machine and deep learning algorithms effectively capture patterns in data in Euclidean.
There is an increasing number of applications where data is represented in the form of a Graph and lack a grid-like regularity.
In this project, we address the problem of identifying paragraphs from layout of unstructured document images. 
We have made an attempt in comparing two of the most popular neural network models, GCN and LSTM.

We have made use of the PubLayNet dataset which contains a rich set of more than 1M document images for the purpose training and testing out models.

This project includes the code that we have worked on converting the dataset(1/8th of the total dataset) into desired form to fit our models and the code for developing the models.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Data Preprocessing

For LSTM and GRU

We have downloaded the val.json file that is provided with the PubLayNet dataset, it contains the details of the each document image in the set. We have used this file to get the bounding box details and category details of all the different structures in the document.
We created a csv file from this data which gave us around 120761 rows.

DataPreprocessing_LSTMGRU.ipynb contains the code for the datapreprocessing. It gets it input from val.json which is in the input folder.

This code was developed on Google Colab and uses the libraries that are already present. To run this file one has to just place the val.json in the drive or content folder and give its path. 

Transfer Learning doesn't need any preprocessing of the data as it uses pre trained models.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# LSTM and GRU







