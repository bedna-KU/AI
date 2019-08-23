# AI
My notes about AI

# Codes

## Face detector

What’s the Difference Between Haar-Feature Classifiers and Convolutional Neural Networks? https://towardsdatascience.com/whats-the-difference-between-haar-feature-classifiers-and-convolutional-neural-networks-ce6828343aeb

https://github.com/ipazc/mtcnn

## YOLO

YOLO object detection with OpenCV https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/

YOLO — ‘You only look once’ for Object Detection explained https://medium.com/diaryofawannapreneur/yolo-you-only-look-once-for-object-detection-explained-6f80ea7aaa1e

## Keras

Keras Mask R-CNN https://www.pyimagesearch.com/2019/06/10/keras-mask-r-cnn/

## Dlib

Object tracking with dlib https://www.pyimagesearch.com/2018/10/22/object-tracking-with-dlib/

## Real-Time Object Detection

Liveness Detection with OpenCV https://www.pyimagesearch.com/2019/03/11/liveness-detection-with-opencv/

## Online test TensorFlow 2.0

https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/r2/tutorials/quickstart/beginner.ipynb#scrollTo=0trJmd6DjqBZ

Beginner’s Guide to Retrain GPT-2 (117M) to Generate Custom Text Content https://medium.com/@ngwaifoong92/beginners-guide-to-retrain-gpt-2-117m-to-generate-custom-text-content-8bb5363d8b7f

#

# Interesting

Detecting Parkinson’s Disease with OpenCV, Computer Vision, and the Spiral/Wave Test https://www.pyimagesearch.com/2019/04/29/detecting-parkinsons-disease-with-opencv-computer-vision-and-the-spiral-wave-test/

# Streaming video

Live video streaming over network with OpenCV and ImageZMQ https://www.pyimagesearch.com/2019/04/15/live-video-streaming-over-network-with-opencv-and-imagezmq/

# Datasets

Coco datataset for object detection 91 categories http://cocodataset.org/#home

# HW

## Rpi ...

Building a Raspberry Pi security camera with OpenCV https://www.pyimagesearch.com/2019/03/25/building-a-raspberry-pi-security-camera-with-opencv/

# Developers

Adrian Rosebrock

# Additional

## Instalation & compiling

### Install TensorFlow over conda

conda install tensorflow

### Install Conda for Debian like distro

curl https://repo.anaconda.com/pkgs/misc/gpgkeys/anaconda.asc | gpg --dearmor > conda.gpg

install -o root -g root -m 644 conda.gpg /etc/apt/trusted.gpg.d/

echo "deb [arch=amd64] https://repo.anaconda.com/pkgs/misc/debrepo/conda stable main" > /etc/apt/sources.list.d/conda.list

apt install conda

## Auxiliary functions

### Convert video to frames

ffmpeg -i video.mp4 -r 3 -f image2 image-%3d.jpeg

### Resize images (no aspect ratio)

onvert tmp/IMG_4408.jpg -resize 224x224\! tmp/IMG_4408_res.jpg
