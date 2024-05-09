MRI Brain Tumor Segmentation with UNet and ResUNet

1. Project Overview

This project explores the application of deep learning for automatic brain tumor segmentation in Magnetic Resonance Imaging (MRI) scans. It leverages two prominent architectures, UNet and ResUNet, to segment tumor regions within MRI images. By effectively identifying and isolating tumor areas, this project contributes to the field of medical image analysis, potentially aiding in early diagnosis, treatment planning, and disease monitoring.

2. Dataset

Source: The Cancer Imaging Archive (TCIA) - a publicly available repository of cancer imaging data.
Description: An elaborate dataset comprising real MRI scans of patients. The dataset selection process is crucial to ensure model generalizability and real-world effectiveness.
3. Methodology

Image Segmentation: This project tackles the task of semantic segmentation, aiming to classify each pixel in the MRI image as either belonging to the tumor region or the background.
UNet Model: A widely used convolutional neural network architecture specifically designed for image segmentation. Its U-shaped structure with skip connections facilitates efficient feature extraction and localization.
ResUNet Model: An extension of UNet that incorporates residual connections from ResNet architecture. These connections enhance the model's ability to learn complex patterns and improve gradient flow during training.
4. Evaluation

Dice Loss and Jaccard Loss: These metrics were employed to assess the performance of the UNet and ResUNet models.
Dice Loss: Measures the overlap between the predicted tumor segmentation and the ground truth (actual tumor region). A lower Dice loss indicates better segmentation accuracy.
Jaccard Loss (Intersection-over-Union): Similar to Dice loss, it calculates the ratio of the intersection between predicted and ground truth regions to their union. Lower Jaccard loss signifies better segmentation.
5. Results

UNet Evaluation Loss: 0.01130
ResUNet Evaluation Loss: 0.01140
Both models achieved very low evaluation losses, suggesting effective tumor segmentation. While UNet performed slightly better in this experiment, it's important to consider other factors like training time and model complexity when selecting the optimal approach for a specific application.
6. Future Work

Hyperparameter Tuning: Further refine model performance by optimizing hyperparameters (e.g., learning rate, optimizer, number of epochs) specific to the chosen architecture and dataset.
Ensemble Learning: Explore the potential benefits of combining the predictions of UNet and ResUNet for potentially improved segmentation accuracy by leveraging the strengths of both models.
Visualization: Implement techniques to visualize segmentation results, aiding in interpreting model behavior and identifying areas for improvement.
Clinical Validation: Conduct validation studies with medical professionals to assess the model's effectiveness in a real-world clinical setting.
