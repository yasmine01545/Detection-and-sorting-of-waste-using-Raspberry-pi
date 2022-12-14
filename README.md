# Detection-and-sorting-of-waste-using-Raspberry-pi
 # Description  

This end-of-year project in artificial intelligence focuses on the computer vision technique for the classification of waste into recycling categories, which could be an effective way to treat waste.
The libraries used to develop machine learning methods are Keras and tensorflow.
The objective of this project is to use a convolutional neural network (CNN) model to take images and classify them into six classes consisting of glass, paper, metal, plastic, cardboard and trash.
We also create a dataset containing approximately 400 to 500 images collected via the internet.

The system consists of sorting the waste received on a conveyor belt and classifying it according to 5 categories:
namely plastic, glass, paper, steel and other waste (vegetable, food, etc.).
As shown in Figure 1, this system includes a camera that captures images of the waste present on the treadmill. These images will then be analyzed and analyzed in real time through a Raspberry Pi 4 card on which is deposited automatic image processing software based on deep neural networks (deep learning). This software makes it possible to classify the images and to control the scrapers to direct and properly route the waste to the various reception bins (plastic, glass, paper, metal and others).
![image](https://user-images.githubusercontent.com/80918787/195158441-d92a7542-a121-4b7d-ad96-f62abfac044e.png)

## needs
1. Jupyter Notebook 
2.	Putty 
3. WinSCP
4. VNC viewer
5.	Camera pi
6. Raspberry Pi

## Model building
We used a set of image data downloaded from the internet ”github”
Here is the download link:
[https://github.com/garythung/trashnet/blob/master/data/dataset-resized.zip
](https://github.com/garythung/trashnet/tree/master/data)
After the download phase, we extracted the images.
There are 5 steps in the deep learning process:
- Load data


First, we need to extract the contents of "dataset-resized.zip"



This repository contains the dataset that we collected. The dataset spans six classes: glass, paper, cardboard, plastic, metal, and trash. Currently, the dataset consists of 2527 images:

- 501 glass
- 594 paper
- 403 cardboard
- 482 plastic
- 410 metal
- 137 trash

The pictures were taken by placing the object on a white posterboard and using sunlight and/or room lighting. The pictures have been resized down to 512 x 384,

- Define the model. Sequential model

- Compile the model by calling the compile() function
- Fit the model with the training dataset. And test the model on test data by calling the model through the fit() function.
![image](https://user-images.githubusercontent.com/80918787/195160912-6f83ffab-3ed0-497a-8af1-82aa9d561bff.png)

After defining the model and compiling it, we need to make predictions by running the model on the same data. Here we specify the epochs (epochs are the number of iterations for the training process to run in the dataset and the batch size is a number of instances that are evaluated before updating the weight)

-  Make a prediction by calling the evaluation or prediction() function.


![image](https://user-images.githubusercontent.com/80918787/195161300-38bee4e9-be16-44c2-b077-3d647e3c9612.png)

![image](https://user-images.githubusercontent.com/80918787/195161357-cb8a41f5-17b4-40ba-bcbf-111069094577.png)


## Installation

```bash
source tflite-env/bin/activate
```

```bash
sudo apt -y install libjpeg-dev libtiff5-dev libjasper_dev libpng12-dev libavcoder-dev libavformat-dev libswscle-dev
```

```bash
sudo apt -y install qt4-dev-tools libatlas-base-devlibhdf5-103
```
```bash

python -m pip install of rib-python==4.1.0.25
```
![image](https://user-images.githubusercontent.com/80918787/195163424-3e01a001-5c60-4392-919f-940903c413fd.png)


## Resultat

https://user-images.githubusercontent.com/80918787/195164025-fee2f841-d755-47b9-b254-51cf2cdf87de.mp4

