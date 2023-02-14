# PoliMi **Artificial Neural Networks and Deep Learning** 2022 course challenges

## Challenge 1: Image Classification

Welcome to the first Homework of the Artificial Neural Networks and Deep Learning course! You have the opportunity to test what you learned during the course. We set up a competition to make things more fun! 😎

In this homework you are required to classify images of leafs, which are divided into categories according to the species of the plant to which they belong. Being a classification problem, given an image, the goal is to predict the correct class label.

### Dataset Details:
Image size: 256x256
Color space: RGB (read as 'rgb' in ImageDataGenerator.flow_from_directory ('color_mode' attribute) or use PIL.Image.open('imgname.jpg').convert('RGB'))
File Format: JPG
Number of classes: 14
Classes:
- 0: "Apple"
- 1: "Blueberry"
- 2: "Cherry"
- 3: "Corn"
- 4: "Grape"
- 5: "Orange"
- 6: "Peach"
- 7: "Pepper"
- 8: "Potato"
- 9: "Raspberry"
- 10: "Soybean"
- 11: "Squash"
- 12: "Strawberry"
- 13: "Tomato"

Dataset Structure: Single folder.

Training: containing 17728 images already divided in sub-folders, based on their class.

Training images per class:
- Apple : 988, 
- Blueberry : 467
- Cherry : 583
- Corn : 1206
- Grape : 1458
- Orange : 1748
- Peach : 977
- Pepper : 765
- Potato : 716
- Raspberry : 264
- Soybean : 1616
- Squash : 574
- Strawberry : 673
- Tomato : 5693


The provided dataset ([download](https://drive.google.com/file/d/11iZ3AZ1OrUU4TimBlFVneV0e7-_HrWgu/view?usp=sharing)) is in zip format. 

We provide a sample notebook in the starting_kit to load the zip file (for people using Colab).

We suggest to use the ImageDataGenerator as we have seen during lessons to load images from directory (flow_from_directory).

Please notice that no automatic validation set is provided.


## Results
 Phase| Mean Accuracy| Apple Mean Accuracy| Blueberry Mean Accuracy| Cherry Mean Accuracy| Corn Mean Accuracy| Grape Mean Accuracy| Orange Mean Accuracy| Peach Mean Accuracy| Pepper Mean Accuracy| Potato Mean Accuracy| Raspberry Mean Accuracy| Soybean Mean Accuracy| Squash Mean Accuracy| Strawberry Mean Accuracy| Tomato Mean Accuracy| Healthy Mean Accuracy| Unhealthy Mean Accuracy| Wild Mean Accuracy|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
Development| 0.9623 (2)| 0.9556 (3)| 0.9200 (2)| 0.8889 (5)| 1.0000 (1)| 0.9778 (2)| 0.9600 (2)| 1.0000 (1)| 0.9556 (3)| 0.9778 (2)| 1.0000 (1)| 0.9200 (3)| 0.9200 (3)| 0.9778 (2)| 0.9778 (2)| 0.9964 (2)| 1.0000 (1)| 0.7286 (2)|
Final| 0.9434 (5)| 1.0000 (1)| 0.9200 (3)| 0.8667 (5)| 1.0000 (1)| 1.0000 (1)| 0.8800 (4)| 0.9333 (3)| 0.9556 (2)| 0.9333 (4)| 1.0000 (1)| 0.8000 (6)| 0.8400 (4)| 0.9556 (3)| 1.0000 (1)| 0.9893 (4)| 0.9889 (3)| 0.6429 (5)|

## Challenge 2: Time Series Prediction
