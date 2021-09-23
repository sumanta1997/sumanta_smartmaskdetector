# sumanta_smartmaskdetector
During COVID-19 pandemic, we all know how much essential it is wear to mask to prevent further spread of novel corona virus. Here is a smart AI solution of detection of face mask. I've trained a resnet18 model to classify among people who are wearing mask from people who are not wearing mask. It has designed to run nVIDIA Jetson platform. 

! [] (New video.gif)

## Guidelines 
Folowing guidelines have to be followed for using it:

I'm assuming JetPack,PyTorch,TensorRT and dustynv's Hello AI setup are done.

Steps to use it after opening the terminal are as follows:

Step 1. You have to clone from github repository

command: git clone https://github.com/sumanta1997/sumanta_smartmaskdetector.git

Step 2. Change directory to jetson-inference 

command: cd jetson-inference

Step 3. Run the docker with assigning the cloned directory as user volume

command: docker/run.sh --volume ~/sumanta_smartmaskdetector:/sumanta_smartmaskdetector

Step 4. Change directory to sumanta_smartmask detector

command:cd /sumanta_smartmaskdetector

Step 5. Run the inference by running mask-detector.py with usb webcam as input

command: python3 mask-detector.py /dev/video0

That's it
