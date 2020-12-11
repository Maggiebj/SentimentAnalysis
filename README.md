# Sentiment Analysis Project
#### Project Summary
In this project, we built sentiment prediction models with two different textCNN, Conv1d cnn and Conv2d cnn.
Both have achieved more than 76% accuracy after only 5 epoches training.  
Conv1d textCNN has slightly better accuracy and less test loss than Conv2d textCNN.

We also built the same textcnn model with different embedding layers. 
The first one has single glove embedding layer with parameters training.
The second one has concatenating glove embedding with normal initialized embedding layer, setting glove embedding parameters constant. 
The third one has single glove embedding layer with constant embedding parameters. 

The models with single glove embedding have better accuracy than concatenating embedding layer model. 
The model with embedding parameters training tends to overfit in the earlier epoches.
The single glove embedding model with constant embedding parameters beat the two counterpartners with the best performance and less training time. 



## File Descriptions
There are 2 notebook files in the product.

sentiment_textcnn.ipynb--Built and trained CNN models with two implementation, conv1d cnn and conv2d cnn.

sentiment_textcnn_glove.ipynb--Built, trained the same textcnn model with different embedding layers of glove embedding and concatenating embedding layers.


# Licensing, Authors, Acknowledgements:

Conv2d textcnn idea from (https://github.com/Shawn1993/cnn-text-classification-pytorch/blob/master/model.py)

Conv1d textcnn idea from the book of "Dive Into DEEP Learning".
