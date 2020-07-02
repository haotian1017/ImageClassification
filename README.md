# Final Project
## Welcome to the final project of Deep Learning!

- Hongxu Hao (hh2302)
- Haotian Guan (hg1580)


##Here we present several deep learning method to help medical community identify the existence of Intracranial Hemorrhage from CT scans of head.
Please refer to Intracranial Hemorrhage Detection Final Paper.pdf for details of each model. Code of each section is also included here. 





## File1.Visualization from a radiologist perspective.ipynb:
This file use window function to visualize the CT images, which have four windows:Default window, Brain Window and Subdural window.


## File2. train_label.ipynb
This file includes deleting images with irregular shape. Initial split of data is also included, 
as well as downsampling. CSV files of meta data is included, but the original image data is not listed here due to incredibly large data size. 
The compressed file of image data is 180 GB, while the uncompressed file is about 366 GB. 
The down-sampled data contains about 100000 images, and 70% are in training set, 15% are in validation set, 15% are in test set. 

## File3. transfer_dcm_data.py
This file extract information from dcm format images and transfer dcm format images into png format for later training


## File4.SRGAN final version
This file built a Super resolution GAN architecture and trained it to fix the blurring part of the CT images. 
We will use the images processed by SRGAN for later detection task. 

## File5. DenseNet169.ipynb
This file contains all code needed for running densenet169 with window function applied.Best performance models are saved into pickle files for reusing. 

## File6. Resnet18.ipynb 
This file contains all code needed for running Resnet18 with window function applied. 

## File7. Vgg and Efficient.ipynb
This file contains code for running baseline model vgg16 and model EfficientNet-b7 as well as 
their result. The result of baseline model include accuracy and loss for training, validation and test set.
The result for EfficientNet-b7 include accuracy and loss for training, validation and test set, plus its auc
for test set.

## File8. resnet_best_out2.pickle
This file contains the trained parameters of  Resnet18

## File9. densenet_best_out2.pickle
This file contains the trained parameters of best performance model DenseNet169

## File10. IH_final.zip
This is the csv files of stage1 and stage2 label after being cleaned and split

## File11. train_metadata.csv
This is the meta data for patients including patient ID

## Detailed informations and guidelines are shown in our project paper. Thank you for reading our paper!







