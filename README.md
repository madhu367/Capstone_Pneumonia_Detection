<h2>Objective
<h6>The objective of the Capstone project is to build a Pneumonia Detection system to detect a visual signal for pneumonia in medical images. The visual signal is in the in the form of inflammation in the Chest X-Ray images. In particular, the need is to construct a deep learning model to automatically locate lung opacities on chest radiographs. The model achieves this by learning the bounding boxes around the affected area from the training image set. Subsequently, the model is applied on test images to predict bounding boxes around lung opacities.

<h2>Data Set
<h6>The data set consists of Chest X-Ray images stored in a special format called DICOM files (*.dcm). They contain a combination of header metadata as well as underlying raw image arrays for pixel data. The images are provided in two folders namely stage_2_train_images and stage_2_test_images. The dataset is sourced from https://www.kaggle.com/c/rsna-pneumonia-detection-challenge/data

<h2>Process Overview
<h6>

* Perform Exploratory Data Analysis
* Prepare and pre-process dataset
* Choose Performance Metric (IOU)
* Finalize Model Architecture Options
* Augment images (ImgAug, Albumentations, PIL, OpenCV)
* Choose Performance Visualization tools (wandb.ai)
* Configure and tune Hyperparameters
* Evaluate Models iteratively
* Observe and Report performance

The following models are compared

* Mask R-CNN, based on Matterport Implementation - Model1_MRCNN_Pneumonia_Detection_MRCNN.ipynb
* Semantic Segmentation Model using a custom network architecture with an Encoder/Decoder Network )(Model2_SSED_Pneumonia_Detection_Custom.ipynb)
* Semantic Segmentation Model using a DenseNet backbone with Encoder/Decoder network (Model3_DNSED_Pneumonia_Detection_DenseNet.ipynb)
