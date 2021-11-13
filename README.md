# Sartorius - Kaggle Competition
### Lachlan Dryburgh 2021
 Kaggle Competition labelling neuroglioblastoma pixels in microscope images. 

Using Tensorflow 2.7 to implement a u-net style convolutional neural network, trained using [SH-SY5Y](https://en.wikipedia.org/wiki/SH-SY5Y) line glioblastoma cells against normal astrocytes and cortical neurons.

The addition of a class-box image clasifier after the downstack half of the u-net allows transfer learning where images are labelled but no pixel annotations are available. 

## Cell Images and Annotation Masks

![types](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/cell_types.png?raw=true)

## CNN Design
### Downstack - Class Box

![downstack](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/downstack.png?raw=true)

### Full Model

![full](https://github.com/LachlanD/Kaggle-Glioblastoma/blob/main/img/full_model.png?raw=true)
