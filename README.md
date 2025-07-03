Project 4: Application of Computer Vision

Overview:

This project explores the application of Convolutional Neural Networks (CNNs) for image classification using the CIFAR-10 dataset with the Keras library. The primary goal is to demonstrate the effectiveness of CNNs in recognizing and classifying images.

Key Components:

  CNN Architecture: Utilizes convolutional layers, ReLU activations, pooling layers, and fully connected layers to extract and classify image features.
  Dataset: The CIFAR-10 dataset, consisting of 60,000 32x32 color images across 10 classes.
  Frameworks: Keras for building and training models and TensorFlow as the backend for scalability and deployment.

Methodology:

  Data Acquisition: Loading and normalizing the CIFAR-10 dataset.
  Model Implementation: Constructing a CNN using Keras' Sequential API, including convolutional, pooling, and dense layers.
  Training: Employing gradient-based optimization (Adam optimizer) and learning rate scheduling to train the model.
  Performance Evaluation: Assessing model performance using metrics like accuracy, loss, and F1 score; visualizing training and validation accuracy/loss.

Results:

  The model demonstrates significant improvement in training accuracy over epochs.
  Validation metrics indicate the need for further tuning to prevent overfitting or underfitting.

Conclusion:

The project successfully showcases the power of CNNs in image classification tasks and provides insights into model optimization techniques for better performance on the CIFAR-10 dataset.

Demo: https://www.youtube.com/watch?v=TtrxSdNe6R8

## Azure Pipeline Mapping

| Pipeline Step       | What I Did                                                | Azure Equivalent              |
|---------------------|-----------------------------------------------------------|-------------------------------|
| Data Ingestion      | Loaded CIFAR-10 dataset from Keras                        | Azure Data Factory (linked dataset) |
| Processing          | Normalized, augmented, and reshaped image data            | Azure Databricks (Python pipeline)  |
| Modeling/Analysis   | Built and trained CNN using Keras/TensorFlow              | Azure Databricks ML Runtime         |
| Evaluation          | Measured accuracy, loss, F1 score                         | DBT (metrics layer)                 |
| Automation          | Could simulate with scheduled training script             | Azure Logic Apps / Pipelines        |
| Versioning          | Used GitHub for model updates and performance tracking    | Azure DevOps Git                    |

