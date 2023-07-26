# BUS-UNet++ Ensemble for Nodule Segmentation

This repository contains the implementation of the BUS-UNet++ ensemble, a combination of the ConvLSTM up-sampling architecture from BUS-UNet and skip connections in aggregation blocks from UNet++ models. The model is designed for the task of nodule segmentation in CT images. The dataset for this study is collected from the Lung Image Database Consortium Image Database Resource Initiative (LIDC-IDRI).

## Dataset

The dataset used for this study is the LIDC-IDRI dataset. Due to data access restrictions, we cannot provide the raw data. However, you can access the dataset at <YOUR_DATASET_LINK>.

To preprocess the dataset and obtain the Region of Interest (RoI) containing nodule masks and images, you can use the `preprocess_dataset()` function provided in the `data_preprocessing.py` file.

## Model Architecture

The BUS-UNet++ model is designed using ConvLSTM up-sampling blocks from the BUS-UNet architecture and skip connections in aggregation blocks from UNet++. The implementation of the model can be found in the `bus_unet_plusplus.py` file.

## Model Training

To train the BUS-UNet++ ensemble, you can use the `train_model()` function provided in the `train.py` file. The model will be trained using the Adam optimizer. After training, the accuracy achieved, Intersection over Union (IoU), and Dice Score Coefficient (DSC) will be computed and printed.


