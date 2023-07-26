# BUS-UNet++ Ensemble for Nodule Segmentation

This repository contains the implementation of the BUS-UNet++ ensemble, a combination of the ConvLSTM up-sampling architecture from BUS-UNet and skip connections in aggregation blocks from UNet++ models. The model is designed for the task of nodule segmentation in CT images. The dataset for this study is collected from the Lung Image Database Consortium Image Database Resource Initiative (LIDC-IDRI).

## Dataset

The dataset used for this study is the LIDC-IDRI dataset. Due to data access restrictions, we cannot provide the raw data. However, you can access the dataset at [https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=1966254].

To preprocess the dataset and obtain the Region of Interest (RoI) containing nodule masks and images, you can check the `dataset.py` file.

## Model Architecture

The BUS-UNet++ model is designed using ConvLSTM up-sampling blocks from the BUS-UNet architecture and skip connections in aggregation blocks from UNet++. The implementation of the model can be found in the `bus_unet++.py` file.

## Model Training
The model will be trained using the Adam optimizer. After training, the accuracy achieved, Intersection over Union (IoU), and Dice Score Coefficient (DSC) will be computed and printed.


