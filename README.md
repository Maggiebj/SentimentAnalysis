# Sentiment Analysis Project
#### Project Summary
In this project, we built sentiment prediction models with two different textCNN, Conv1d cnn and Conv2d cnn.
Both have achieved more than 76% accuracy after only 5 epoches training.  
Conv1d textCNN has slightly better accuracy and less test loss than Conv2d textCNN.

We also built the same textcnn model with different embedding layers. 
The first one has single glove embedding layer with parameters training.(accuracy 80.2%)
The second one has concatenating glove embedding with normal initialized embedding layer, setting glove embedding parameters constant. (accuracy 76.0%) 
The third one has single glove embedding layer with constant embedding parameters. (accuracy 80.9%)


Update: Added sentiment analysis with machine learning.  Logisticregression model with tfidf got 88.47% accuracy --2020.12.31

## File Descriptions
There are 3 notebook files in the product.

sentiment_textcnn.ipynb--Built and trained CNN models with two implementation, conv1d cnn and conv2d cnn.

sentiment_textcnn_glove.ipynb--Built, trained the same textcnn model with different embedding layers of glove embedding and concatenating embedding layers.

sentiment_ml.ipynb--Built, trained machine learning model of logisticregression and multinomialNB with countvectorizer and tfidf. 


# Licensing, Authors, Acknowledgements:

Conv2d textcnn idea is from (https://github.com/Shawn1993/cnn-text-classification-pytorch/blob/master/model.py)

Conv1d textcnn idea is from the book of "Dive Into DEEP Learning".
