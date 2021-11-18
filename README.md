# Sartorius - Kaggle Competition
### Lachlan Dryburgh 2021
[Kaggle Competition](https://www.kaggle.com/c/sartorius-cell-instance-segmentation) labelling neuroglioblastoma pixels in microscope images. 

Using Tensorflow 2.7 to implement a u-net style convolutional neural network, trained using [SH-SY5Y](https://en.wikipedia.org/wiki/SH-SY5Y) line glioblastoma cells against normal astrocytes and cortical neurons.

The addition of a class-box image clasifier after the downstack half of the u-net allows transfer learning where images are labelled but no pixel annotations are available. 

## Cell Images and Annotation Masks

![types](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/cell_types.png?raw=true)

## CNN Design
### Downstack - Class Box

![downstack](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/downstack.png?raw=true)

### Full Model

![full](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/full_model.png?raw=true)


## Training Downstack
Initial training of downstack using semi supervised dataset which is just labeled with cell types but lack pixel annotations.

![training_class](https://github.com/LachlanD/Glioblastoma-Detection-Kaggle/blob/main/img/down_loss.png?raw=true)

## Training Full Network after pre-training Downstack

![training_pixel](https://github.com/LachlanD/Glioblastoma-Detection-Kaggle/blob/main/img/pretrained_loss.png?raw=true)

## Validation Set Predictions

![pred1](https://github.com/LachlanD/Glioblastoma-Detection-Kaggle/blob/main/img/prediction1.png?raw=true)
![pred2](https://github.com/LachlanD/Glioblastoma-Detection-Kaggle/blob/main/img/prediction2.png?raw=true)
![pred3](https://github.com/LachlanD/Glioblastoma-Detection-Kaggle/blob/main/img/prediction3.png?raw=true)
