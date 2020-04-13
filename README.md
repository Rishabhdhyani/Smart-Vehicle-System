# Smart-Vehicle-System

This project deals with the problem of overspeeding in our country by finding the culprit and taking immediate action against them by issuing E-challan. This project uses trio method to provide efficient method of alarming the driver about speed in that particular road. 

The implementation can be divided in three parts:-

1) Deep Learning model
2) Raspberry pi
3) RF Module

Currently, we are done with our first implementation. I am going to mention the implementation details.

1) I have used SVHN( Street View House Numbers ) data as the training set and implemented it using keras-retinanet. The project is implemented in Ubuntu 18.04 and works well in it. It is advised to use separate environment for this particular project.

## Requirements

- python 3.6
- tensorflow 1.10.0
- keras 2.2.4
- keras-retinanet 0.5.0
                                 
Then, download the data set from this link http://ufldl.stanford.edu/housenumbers/train.tar.gz. Now you need to train your model by running main.py.

After training the model, run infer.py to test images in folder samples. In the file output.txt, you will get the json object which give you speed limit.

Note- Further implementation will be uploaded soon. Bash file automate.sh will be used to integrate the trio system and it will be done with the help of python sockets. 
