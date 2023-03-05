
# Improving Accuracy of Liquid-Based Pap Test Diagnosis using Pre-trained CNN Models and Fine-Tuning Techniques
This project tries to find a model based on pre-trained networks for the classification of cancer cell images into 4 different types:
* Negative intraepithelial lesion (NIL).
* Low-grade squamous intraepithelial lesion (LSIL).
* High-grade squamous intraepithelial lesion (HSIL).
* Squamous cell carcinoma (SCC).
This project proposes a methodology that focuses on finding an effective convolutional neural network (CNN) model for analyzing digital pap smears. The approach involves two stages. In the first stage, different pre-trained models such as DenseNet, EfficientNet, ResNet, and VGG19 are used to classify four classes of cervical cells. In the second stage, the best previous model is selected, and through fine-tuning techniques, the best hyperparameters are selected. This study uses different performance metrics for high-resolution classification, such as accuracy, sensitivity, precision, and specificity

 The trainings were performed in Google Colab in its free version. The steps are:
 
 ## Obtain the dataset
In order to obtain the data you have to click [here](https://drive.google.com/drive/folders/1tzuhemvmCR94rbQK4_CZd_HoEq_mJQLU?usp=share_link).
tant to mention that for the code to work you must download the dataset and load it on a drive. In addition, some changes must be made to the code, some lines in the code which will be mentioned later.
## Description of the Files

TThis repository contains three .ypynb files. Which are used to obtain the results of our research.

# Replication of results
In this file are the code for replicate the results of the paper Liquid-Based Pap Test Analysis Using Two-Stage CNNs https://doi.org/10.1016/j.ypmed.2004.03.040 
In the DATA PREPROCESSING section you must specify the path where the above mentioned dataset is located. After that you only have to execute the code and it will work correctly.

# Fine tuning
Code for the fine tuning process with the Resnet152 pretrained architecture. This was the best model found for this task. Before choosing the best model,resnet152, VGG16, efficienetb0, efficienetb3 and DenseNet201 were tested.

# Train model afer finetuning

Corresponding code to train the after model to obtain the best combination of parameters with fine tuning.
