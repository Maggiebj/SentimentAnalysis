# Sentiment Analysis Project
#### Project Summary
In this project, we built sentiment prediction models with textCNN. We implemented with two methods of conv1d textcnn and conv2d textcnn.
Both have achieved more than 76% accuracy after only 5 epoches training. It's promising it will have better performance if we train on more epoches. 
Conv1d textCNN has slightly better accuracy and less test loss than the other one.

We also built textcnn model with different embedding layers. We built and tested three implementations of embedding layer. 
The first one has single glove embedding layer with parameters training.
The second one has concatenating glove embedding with normal initialized embedding layer , setting glove embedding parameters constant. 
The third one has single glove embedding layer with constant embedding parameters. 

The models with single glove embedding have better accuracy than concatenating embedding layer model. 
The model with embedding parameters training tends to overfit in the earlier epoches.
The single glove embedding model with constant embedding parameters beat the two counterpartners with the best performance and less training time. 



## File Descriptions
There are 2 notebook files in the product.

sentiment_textcnn.ipynb--Built and trained CNN models with two implementation, conv1d cnn and conv2d cnn.

sentiment_testcnn_glove.ipynb--Built, trained and compared the textcnn model with different embedding layers of glove embedding and concatenating glove embedding with normal initialized embedding.


# Licensing, Authors, Acknowledgements:

Conv2d textcnn idea from (https://github.com/Shawn1993/cnn-text-classification-pytorch/blob/master/model.py)

Conv1d textcnn idea from the book of "Dive Into DEEP Learning".
