# A.I. Breast Cancer Detection - A Tool To Assist Oncologists

### A convolutional neural network approach to detecting malignant tumors in breast cancer tissue. 
##### Developed by Ravish Rawal at Columbia University.

\
Despite incredible advances in imaging technology, breast cancer can be difficult to detect in tissue slides with the unaided human eye. The CAMELYON16 dataset provides a small set of cancerous breast tissue slides, annotated by oncologists to show malignant areas.

This project adopts a sliding window approach to:

1. Extract patches
2. Classify patches
3. Train a classifier using this labelled dataset
4. Fine tune the classifier
5. Generate a heatmap to predict and display cancerous regions


#### Predictions:

The algorithm catches areas that were lazily annotated and others that may have been missed. 

![alt text](https://github.com/ravishrawal/breast-cancer-detection/blob/main/prediction.png?raw=true)
![alt text](https://github.com/ravishrawal/breast-cancer-detection/blob/main/mask.png?raw=true)

#### Metrics:

* Precision:  95.16 %
* Recall:  93.65 %
![alt text](https://github.com/ravishrawal/breast-cancer-detection/blob/main/confusion_matrix.png?raw=true)


#### Future Work:

Due to GPU and storage constraints, the slides had to be downsampled from 40x to 10x zoom. The algorithm can be improved by using the 40x magnification for training and prediction.
