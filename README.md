# Sentiment Analysis Project
#### Project Summary
In this project, we build sentiment prediction models with textCNN. We implement with two methods of conv1d cnn and conv2d cnn.
Both have achieved more than 76% accuracy after only 5 epoches training. It's promising it will have better performance if we train more epoches. 
Conv1d textCNN has slightly better accuracy and less test loss than the other one.

We also build textcnn model with different embedding layer. We built and tested three implementations of embedding layer. 
The first one has single glove embedding layer with parameters training.
The second one has concatenating glove embedding with normal initialized embedding layer , setting glove embedding parameters constant. 
The third one has single glove embedding layer with constant embedding parameters. 

The models with single glove embedding have better accuracy than concatenating embedding layer model. 
The model with embedding parameters training tends to overfit in the earlier epoches.
The single glove embedding model with constant embedding parameters beat the two counterpartners with the best performance and less training time. 



## File Descriptions
There are 2 notebook files in the product.

sentiment_textcnn.ipynb--Built and train CNN models with two implementation, conv1d cnn and conv2d cnn.

sentiment_testcnn_glove.ipynb--Built, train and compare the textcnn model with different embedding layer of glove embedding and concatenating glove and normal initialized embedding.


# Licensing, Authors, Acknowledgements:

Conv2d cnn idea from (https://github.com/Shawn1993/cnn-text-classification-pytorch/blob/master/model.py)
Conv1d cnn idea from the book of <Dive Into DEEP Learning>
