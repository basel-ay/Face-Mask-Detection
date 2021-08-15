# Face-Mask-Detection

# **Introduction**


Face mask detection has a range of applications from capturing the movement of the face to facial recognition which at first requires the face to be detected with very good precision. Face detection is more relevant today as it is not only used on images, but also in video applications like real-time surveillance and face detection in videos.

High precision image classification is now possible with advances in convolutional networks. Pixel level information is often needed after face detection, which most face detection methods do not provide.

Obtaining pixel-level detail has been a difficult part of semantic segmentation. Semantic segmentation is the process of assigning a label to each pixel in the image.

![](https://www.logmask.com/images/mask-detection-sample.jpg)

# **Approach**

* Extract face data for training.
* Train the classifier to classify faces in mask or labels without a mask.
* Detect faces while testing data using SSD face detector.
* Using the trained classifier, classify the detected faces.

In the third step of the above process, you have to think about what is the SSD face detector? Well, the **SSD is a Single Shot Multibox Detector**. This is a technique used to detect objects in images using a single deep neural network.

It is used for the detection of objects in an image. Using a basic architecture of the VGG-16 architecture, the SSD can outperform other object detectors such as YOLO and Faster R-CNN in terms of speed and accuracy.

![](https://www.researchgate.net/profile/Adam_Nowosielski/publication/332948824/figure/fig5/AS:767146284036100@1559913335810/The-model-of-Single-Shot-MultiBox-Detector-SSD-25.ppm)

Datasets :
* Face Mask Detection Dataset : https://www.kaggle.com/wobotintelligence/face-mask-detection-dataset
* Caffe Face Detector (OpenCV Pre-trained Model) : https://www.kaggle.com/sambitmukherjee/caffe-face-detector-opencv-pretrained-model
