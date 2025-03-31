# Human Segmentation with U-Net

## Introduction
This project implements **U-Net**, a deep learning architecture for semantic image segmentation, specifically for human segmentation. U-Net has proven to be highly effective for various segmentation tasks, including human body segmentation.

## Dataset
The model is trained using a dataset that includes full-body images along with corresponding segmentation masks. A custom PyTorch dataset class (`FullBodyDataset`) is used to load and preprocess the images and masks. The dataset pipeline includes:
- Defining dataset paths and loading sample images.
- Creating a dataset class that handles image-mask pair loading.
- Applying transformations to prepare the data for training.

## Model Architecture
The **U-Net** model consists of:
1. **Encoder (Contracting Path):** A series of convolutional and pooling layers that extract features from the input image.
2. **Bottleneck:** The lowest-resolution representation of the image, capturing high-level features.
3. **Decoder (Expanding Path):** Transposed convolutions and skip connections that reconstruct the segmentation mask.

## Framework
This implementation is built using **PyTorch** and leverages its deep learning capabilities for training and inference.

## Results
Sample outputs include segmented images showing detected human regions. Performance metrics and qualitative results will be added based on training outcomes.

<p align="center">
  <img src="https://github.com/HanaNabhan/Human_segmentation/blob/main/output.png" width="900"/>
</p>
