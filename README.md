# RCNN-from-scratch
This is the implementation of the famous RCNN paper using PyTorch.

Object Detection.
Object Detection is a process of not only detecting an object in the image but also giving the location of the object mostly in terms of bounding boxes.

RCNN.
RCNN (Region - Convolutional Neural Network) is an object detection technique which gives the classes of the objects present in an image and also their locations. There are primarily three steps in the RCNN, they are getting region proposals from the region proposal algorithm (Selective Search in our case). Then, we pass the region proposals through the pretrained network (RESNET18 in our case). The last step includes passing the feature vectors obtained from the last layer of the pretrained network to the class specific SVMs (Support Vector Machine) for classfication.

In this project, we have tried to implement the full RCNN paper, obviously with some modifications to suit our dataset. The modifications include not transforming the bounding box coordinates to any other space but using the raw predictions, not dilating the image before passing it through the pretrained the network.
