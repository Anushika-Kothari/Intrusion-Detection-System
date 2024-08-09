## Project Overview: Lightweight Intrusion Detection System for Edge Computing

This project introduces a novel **Intrusion Detection System (IDS)** designed for edge computing environments. The system leverages a combination of **Convolutional Neural Networks (CNNs)** and **Random Forest** for feature reduction, focusing on anomaly detection to identify potential cybersecurity threats efficiently.

### Key Features

- **Dataset Selection**: Utilizes the CICIDS 2017 dataset, which includes 79 features and 1 label, providing a comprehensive representation of both normal and attack scenarios in network traffic.
  
- **Feature Reduction**: Implements a Random Forest algorithm to reduce the number of features from 79 to 21, optimizing the dataset for more efficient processing.
  
- **Data Transformation**:
  - **Quantile Transformation**: Applied to enhance the interpretability of the dataset.
  - **Image Generation and Normalization**: Transforms data into an optimized image dataset to be used by CNN models.
  
- **CNN Classification Models**:
  - Multiple CNN architectures including VGG16, VGG19, Xception, Inception, and Inception-ResNet are used for classification.
  - These models are trained to detect anomalies in network traffic that may indicate cyber-attacks.
  
- **Ensembling**:
  - Top 3 performing CNN models are selected and ensembled using techniques such as probability averaging, bagging, and concatenation to enhance detection accuracy.
  
- **Quantization**:
  - Quantization techniques are applied to the ensembled model to reduce its size by 50%, making it more suitable for deployment on resource-constrained edge devices.
  - Despite the reduction in model size, the system achieves an accuracy of 98.13%, maintaining robust detection capabilities.

### Summary of Results

- **Accuracy**: The ensembled model achieved a detection accuracy of 98.13% after quantization.
- **Size Reduction**: The model size was reduced by 50% through quantization techniques, making it efficient for deployment in resource-limited environments.
- **Performance**: The system effectively balances computational efficiency with high detection performance, making it a promising solution for edge-deployable cybersecurity technologies.

### Future Work

- **Advanced Quantization Techniques**: Further exploration of quantization methods to optimize model size without compromising accuracy.
- **Adaptability**: Investigating the model’s adaptability across different edge computing environments and real-world scenarios.
- **Expansion**: Refining and expanding the applicability of the IDS for broader use in diverse cybersecurity settings.

This project demonstrates a significant advancement in developing lightweight yet powerful IDS solutions suitable for modern edge computing environments.
