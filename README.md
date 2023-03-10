
# Improving Accuracy of Liquid-Based Pap Test Diagnosis using Pre-trained CNN Models and Fine-Tuning Techniques

According to the World Health Organization, cervical cancer is a significant health concern for women worldwide. The Papanicolaou or pap test is an effective tool for early detection of the disease, which can help prevent deaths. However, the process of analyzing pap test results, which involves a pathologist examining images of the cells, is time-consuming and prone to human error. In developing countries, doctors often rely on manual examination with microscopes, resulting in a shortage of available services.

To address this issue, this paper proposes a methodology that focuses on finding an effective convolutional neural network (CNN) model for analyzing digital pap smears. The approach involves two stages . In the first stage, different pre-trained models such as DenseNet, EfficientNet, ResNet, and VGG19 are used to classify four classes of cervical cells on high-resolution 
 cell images belonging to 460 patients. In the second stage, the best previous model is selected, and through fine-tuning techniques, the best hyperparameters are selected. This study uses different performance metrics for high-resolution classification, such as accuracy, sensitivity, precision, and specificity.

This project is based on the classification of cancer cell images into 4 different types using transfer learning and fine tuning process:

* Negative intraepithelial lesion (NIL).
* Low-grade squamous intraepithelial lesion (LSIL).
* High-grade squamous intraepithelial lesion (HSIL).
* Squamous cell carcinoma (SCC). The trainings were performed in Google Colab in its free version. The steps that
 
 ## Obtain the  [dataset](https://drive.google.com/drive/folders/1tzuhemvmCR94rbQK4_CZd_HoEq_mJQLU?usp=share_link).

## Description of the Files

This repository contain 3 directories.

# replication_of_results
In this directory are the code for replicate the results of the paper Liquid-Based Pap Test Analysis Using Two-Stage CNNs https://doi.org/10.1016/j.ypmed.2004.03.040 

# fine_tuning
Code for the fine tuning process with the Resnet152 pretrained architecture. This was the best model found for this task. Before choosing the best model,resnet152, VGG16, efficienetb0, efficienetb3 and DenseNet201 were tested.

# train_model_afer_finetuning

Corresponding code to train the after model to obtain the best combination of parameters with fine tuning.
