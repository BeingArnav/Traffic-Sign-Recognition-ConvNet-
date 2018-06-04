## Project:  Traffic-Sign-Recognition(ConvNet)
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)
### Overview

This is the implementation of Traffic Sign Recognition Project deep neural networks and convolutional neural networks to classify traffic signs. The model is trained, visualized and explored for better understanding of the pictorial data of traffic signs from natural images by using the [Traffic Sign Dataset](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/581faac4_traffic-signs-data/traffic-signs-data.zip).

### Dependencies

This project requires **Python 3.5** and the following Python libraries installed:

- [Opencv2](https://docs.opencv.org/3.0-beta/doc/py_tutorials/py_tutorials.html)
- [Jupyter](http://jupyter.org/)
- [NumPy](http://www.numpy.org/)
- [Pickle](https://docs.python.org/2/library/pickle.html)
- [scikit-learn](http://scikit-learn.org/)
- [TensorFlow](http://tensorflow.org)
- [Matplotlib](http://matplotlib.org/)
- [Pandas](http://pandas.pydata.org/) (Optional)
- [Keras](https://keras.io/)


 Final CNN Architecture :

 Layer (type)                 Output Shape              Param #   
 =================================================================
 conv2d_1 (Conv2D)            (None, 28, 28, 32)        2432      
 _________________________________________________________________
 activation_1 (Activation)    (None, 28, 28, 32)        0         
 _________________________________________________________________
 conv2d_2 (Conv2D)            (None, 24, 24, 32)        25632     
 _________________________________________________________________
 activation_2 (Activation)    (None, 24, 24, 32)        0         
 _________________________________________________________________
 max_pooling2d_1 (MaxPooling2 (None, 12, 12, 32)        0         
 _________________________________________________________________
 conv2d_3 (Conv2D)            (None, 8, 8, 64)          51264     
 _________________________________________________________________
 activation_3 (Activation)    (None, 8, 8, 64)          0         
 _________________________________________________________________
 conv2d_4 (Conv2D)            (None, 4, 4, 64)          102464    
 _________________________________________________________________
 activation_4 (Activation)    (None, 4, 4, 64)          0         
 _________________________________________________________________
 max_pooling2d_2 (MaxPooling2 (None, 2, 2, 64)          0         
 _________________________________________________________________
 dropout_1 (Dropout)          (None, 2, 2, 64)          0         
 _________________________________________________________________
 flatten_1 (Flatten)          (None, 256)               0         
 _________________________________________________________________
 dense_1 (Dense)              (None, 1024)              263168    
 _________________________________________________________________
 activation_5 (Activation)    (None, 1024)              0         
 _________________________________________________________________
 dropout_2 (Dropout)          (None, 1024)              0         
 _________________________________________________________________
 dense_2 (Dense)              (None, 43)                44075     
 _________________________________________________________________
 activation_6 (Activation)    (None, 43)                0     


### Dataset

1. [Download the dataset](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/581faac4_traffic-signs-data/traffic-signs-data.zip). This is a pickled dataset in which we've already resized the images to 32x32.
2. Clone the project and start the notebook.
```
git clone https://github.com/BeingArnav/Traffic-Sign-Recognition-ConvNet-
cd Traffic-Sign-Recognition-ConvNet-
jupyter notebook Traffic_Signs_Recognition.ipynb
```
3. Hurry ,begin your task !!
