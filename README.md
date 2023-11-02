<div align="center">
  <a href="https://www.kaggle.com/competitions/uw-madison-gi-tract-image-segmentation">
    <img src="cover.png" alt="Logo" width="" height="200">
  </a>

<h1 align="center">Medica Image Segmentation</h1>
</div>

## 1. Problem Statement
Gastrointestinal cancer patients often undergo radiotherapy as part of their treatment regimen. This therapeutic approach is designed to deliver precisely targeted radiation to tumors while sparing healthy tissues, such as the stomach and intestines. However, the challenge arises from the daily variations in tumor and organ positions, which necessitate the manual delineation of these organs by medical professionals.

This manual segmentation process is not only time-consuming and labor-intensive but also extends the duration of treatment sessions. For patients already coping with the challenges of cancer, the added treatment time can be physically and emotionally taxing.

To address this issue, there is a compelling need to automate the segmentation process in medical images, particularly for identifying the stomach and intestines. Deep learning methods offer a promising solution to enhance the efficiency and accuracy of this critical step in radiotherapy. By automating the identification and delineation of these organs, deep learning can significantly reduce the time required for this process, ultimately shortening treatment sessions and improving the overall experience for patients battling gastrointestinal cancer.

The provided image showcases a compelling example of the need for deep learning-based segmentation. Within this image, the stomach and intestines are distinguishable, but the complex contours and variations in shape pose a formidable challenge for manual delineation.

![1](https://github.com/royasotude/medical-image-segmentation/assets/118993192/0573eaae-f61a-437b-a559-5e1b915211ca)



                
     


## 2. Related Works
In the dynamic realm of medical image segmentation, several noteworthy contributions have significantly advanced the field. One of the most influential developments is the U-Net architecture, which introduced a highly effective convolutional neural network (CNN) framework for biomedical image segmentation. This innovation has been instrumental in various applications, from the precise delineation of organs in radiological images to the segmentation of individual cells in microscopic images.

DeepLab, another seminal work, stands out for its role in semantic image segmentation. It has been widely adopted in medical imaging to achieve detailed object recognition and localization, allowing for a deeper understanding of the structures within medical images.

Moreover, the 3D U-Net model has addressed the unique challenges associated with volumetric medical data. With its ability to segment three-dimensional images, it has been applied to tasks like tumor and organ delineation, providing critical support for medical diagnosis and treatment planning.

These related works represent a strong foundation upon which medical image segmentation continues to build. They have significantly enhanced our ability to extract meaningful information from complex medical images, ultimately benefiting healthcare professionals and researchers in their quest to improve diagnostics and treatment outcomes.


## 3. The Proposed Method
For the task of intestines and stomach segmentation in medical images, my proposed method is based on the U-Net architecture. U-Net, in this context, is constructed using convolutional layers and tailored to the specific needs of gastrointestinal organ segmentation.

The U-Net architecture comprises a contracting path and an expanding path. The contracting path begins with the input medical image and is composed of a series of convolutional layers followed by pooling layers. These convolutional layers progressively reduce the spatial dimensions while increasing the number of feature channels. This step extracts features relevant to intestines and stomach in various scales and complexities.

The expanding path, or decoder, consists of transposed convolutional layers. This path gradually restores the spatial dimensions to generate the final segmentation masks for intestines and stomach. Importantly, the architecture includes skip connections, which directly link encoder layers to their corresponding decoder layers. These skip connections enable the network to maintain both fine-grained spatial information and high-level semantic context, ensuring precise localization and segmentation of the gastrointestinal organs. This customized U-Net architecture, designed for intestines and stomach segmentation, takes advantage of its ability to capture intricate details and localize specific structures within medical images.

![image](https://github.com/royasotude/medical-image-segmentation/assets/118993192/0bdf80fb-acba-4f3a-ac7d-2cc221cb345e)


## 4. Implementation
This section delves into the practical aspects of the project's implementation.

### 4.1. Dataset
Under this subsection, you'll find information about the dataset used for the medical image segmentation task. It includes details about the dataset source, size, composition, preprocessing, and loading applied to it.
[Dataset](https://drive.google.com/file/d/1-2ggesSU3agSBKpH-9siKyyCYfbo3Ixm/view?usp=sharing)

### 4.2. Model
In this subsection, the architecture and specifics of the deep learning model employed for the segmentation task are presented. It describes the model's layers, components, libraries, and any modifications made to it.

### 4.3. Configurations
This part outlines the configuration settings used for training and evaluation. It includes information on hyperparameters, optimization algorithms, loss function, metric, and any other settings that are crucial to the model's performance.

### 4.4. Train
Here, you'll find instructions and code related to the training of the segmentation model. This section covers the process of training the model on the provided dataset.

### 4.5. Evaluate
In the evaluation section, the methods and metrics used to assess the model's performance are detailed. It explains how the model's segmentation results are quantified and provides insights into the model's effectiveness.

