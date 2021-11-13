# Sartorius
 Kaggle Competition labelling neuroglioblastoma pixels in microscope images

Using Tensorflow 2.7 to implement a u-net style convolutional neural network.

The addition of a class-box image clasifier after the downstack half of the u-net allows transfer learning where images are labelled but no pixel annotations are available. 

## Downstack - Class Box

![downstack](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/downstack.png?raw=true)

## Full Model

![full](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/full_model.png?raw=true)
