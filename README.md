# PoliMi ***Artificial Neural Networks and Deep Learning*** 2021 course challenges

## Challenge 1: Image Classification

Welcome to the first Homework of the Artificial Neural Networks and Deep Learning course! You have the opportunity to test what you learned during the course. We set up a competition to make things more fun! 😎

In this homework you are required to classify images of leafs, which are divided into categories according to the species of the plant to which they belong. Being a classification problem, given an image, the goal is to predict the correct class label.

### Dataset Details:
Image size: 256x256

Color space: RGB (read as 'rgb' in ImageDataGenerator.flow_from_directory ('color_mode' attribute) or use PIL.Image.open('imgname.jpg').convert('RGB'))

File Format: JPG

Number of classes: 14
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
Development| 0.9623 | 0.9556 | 0.9200 | 0.8889 | 1.0000 | 0.9778 | 0.9600 | 1.0000 | 0.9556 | 0.9778 | 1.0000 | 0.9200 | 0.9200 | 0.9778 | 0.9778 | 0.9964 | 1.0000 | 0.7286 |
Final| 0.9434 | 1.0000 | 0.9200 | 0.8667 | 1.0000 | 1.0000 | 0.8800 | 0.9333 | 0.9556 | 0.9333 | 1.0000 | 0.8000 | 0.8400 | 0.9556 | 1.0000 | 0.9893 | 0.9889 | 0.6429 |

## Challenge 2: Time Series Forecasting

In this homework, you are required to predict future samples of a multivariate time series. The goal is to design and implement forecasting models to learn how to exploit past observations in the input sequence to correctly predict the future. 


### Dataset Details:
We provide a training multivariate time series with the following characteristics

Length of the time series (number of samples in the training set):   68528

Number of features: 7

Name of the features: 'Sponginess', 'Wonder level', 'Crunchiness', 'Loudness on impact', 'Meme creativity', 'Soap slipperiness', 'Hype root'

The provided time series has a uniform sampling rate.

Please notice that no automatic validation set is provided.

The provided dataset is in '.csv' format and can be downloaded [here](https://drive.google.com/drive/folders/14YIaBj7Hm9wjqc8notvB0gW4V8PHO8mR?usp=sharing).

### Results
 RMSE  | MAE  | Sponginess RMSE  | Wonder Level RMSE | Crunchiness RMSE | Loudness on Impact RMSE | Meme Creativity RMSE | Soap Slipperiness RMSE | Hype Root RMSE | First Quarter RMSE | Second Quarter RMSE | Third Quarter RMSE | Fourth Quarter RMSE |
 |-|-|-|-|-|-|-|-|-|-|-|-|-|
 3.7042 | 2.3823  | 1.9088  | 1.8086  | 6.4420  | 1.3604  | 0.7890  | 2.6788 | 6.1630 | 3.7786  | 3.5216  | 3.8056  | X  | 
