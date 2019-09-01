# AI
My notes about AI

# Neural Netorks

darknet https://pjreddie.com/darknet/

# Articles

21 Must-Know Open Source Tools for Machine Learning you Probably Aren’t Using (but should!) https://www.analyticsvidhya.com/blog/2019/07/21-open-source-machine-learning-tools/

Turning a MacBook into a Touchscreen with $1 of Hardware https://www.anishathalye.com/2018/04/03/macbook-touchscreen/?fbclid=IwAR05JSy6XJcPNjBxR0IiNEGB7_tAuf0Z1bTQnDI2QR7oa2N218agjYc1bYE

Image classification with Keras and deep learning https://www.pyimagesearch.com/2017/12/11/image-classification-with-keras-and-deep-learning/

Python | Image Classification using keras https://www.geeksforgeeks.org/python-image-classification-using-keras/

How to Perform Object Detection With YOLOv3 in Keras https://machinelearningmastery.com/how-to-perform-object-detection-with-yolov3-in-keras/

Detection Objects in a webcam image stream https://github.com/TannerGilbert/Tutorials/blob/master/Tensorflow%20Object%20Detection/detect_object_in_webcam_video.ipynb

Near Real Time CPU Face detection using deep learning https://github.com/iitzco/faced

Building powerful image classification models using very little data https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html

Simple Image Classification using Convolutional Neural Network — Deep Learning in python. https://becominghuman.ai/building-an-image-classifier-using-deep-learning-in-python-totally-from-a-beginners-perspective-be8dbaf22dd8

## Face detector

What’s the Difference Between Haar-Feature Classifiers and Convolutional Neural Networks? https://towardsdatascience.com/whats-the-difference-between-haar-feature-classifiers-and-convolutional-neural-networks-ce6828343aeb

https://github.com/ipazc/mtcnn

## YOLO

Live Object Detection https://towardsdatascience.com/live-object-detection-26cd50cceffd

YOLO object detection with OpenCV https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/

YOLO — ‘You only look once’ for Object Detection explained https://medium.com/diaryofawannapreneur/yolo-you-only-look-once-for-object-detection-explained-6f80ea7aaa1e

## Keras

Keras Mask R-CNN https://www.pyimagesearch.com/2019/06/10/keras-mask-r-cnn/

Training and Detecting Objects with YOLO3 https://github.com/jbrownlee/keras-yolo3

## Real-Time Object Detection

## 

## Online test Python code

https://colab.research.google.com

# Interesting

Detecting Parkinson’s Disease with OpenCV, Computer Vision, and the Spiral/Wave Test https://www.pyimagesearch.com/2019/04/29/detecting-parkinsons-disease-with-opencv-computer-vision-and-the-spiral-wave-test/

# Streaming video

Live video streaming over network with OpenCV and ImageZMQ https://www.pyimagesearch.com/2019/04/15/live-video-streaming-over-network-with-opencv-and-imagezmq/

# Datasets

Coco datataset for object detection 91 categories http://cocodataset.org/#home

Internet Archive https://archive.org/about/

# Pretrained models

VGG-16 Pre-trained Model for Keras https://www.kaggle.com/keras/vgg16

# HW

## Rpi ...

Building a Raspberry Pi security camera with OpenCV https://www.pyimagesearch.com/2019/03/25/building-a-raspberry-pi-security-camera-with-opencv/

# Developers

https://github.com/Tony607

https://github.com/anujshah1003

https://github.com/ipazc

https://github.com/pjreddie

https://machinelearningmastery.com/about/

https://github.com/TannerGilbert

# Additional

## Instalation & compiling

### Install TensorFlow over conda

conda install tensorflow

### Install Conda for Debian like distro

curl https://repo.anaconda.com/pkgs/misc/gpgkeys/anaconda.asc | gpg --dearmor > conda.gpg

install -o root -g root -m 644 conda.gpg /etc/apt/trusted.gpg.d/

echo "deb [arch=amd64] https://repo.anaconda.com/pkgs/misc/debrepo/conda stable main" > /etc/apt/sources.list.d/conda.list

apt install conda

# Auxiliary functions

### Convert video to images (3frames per second)

ffmpeg -i video.mp4 -r 3 -f image2 image-%3d.jpeg

### Resize video (to 1600x1200)

ffmpeg -i input.ogv -vf scale=1600:1200 output.avi

### Video to half speed

ffmpeg -i input.mkv -filter:v "setpts=2*PTS" output.mkv

## Video - remove noise

ffmpeg -i <input_file> -af "highpass=f=200, lowpass=f=3000" <output_file>

### Resize images (no aspect ratio)

convert '*.jpg[224x224!]' resized%03d.png
