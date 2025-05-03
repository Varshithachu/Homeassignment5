# Homeassignment5
# Implementing a Basic GAN on MNIST Dataset
# Overview
This code demonstrates the implementation of a simple Generative Adversarial Network (GAN) using PyTorch.
* Defining a Generator and Discriminator architecture
* Training them alternately in an adversarial setup
* Generating handwritten digit images using the MNIST dataset
# Dataset
Dataset Used: MNIST handwritten digits dataset.
The dataset is loaded directly using PyTorch’s torchvision.datasets.
No manual or external dataset required.
# Requirements
Running on Google Colab
PyTorch and torchvision are pre-installed.
No additional setup needed.
If necessary, install using:
!pip install torch torchvision
Install packages:
pip install torch torchvision matplotlib
# Output
Image Samples
Images generated at Epoch 0, 25, and 50 showing the GAN’s progress in creating digits.
# Observations
GAN Adversarial Training:
Generator improves over time in making realistic digits.
Discriminator tries to correctly distinguish real and fake digits.
Loss Behavior:
Generator and Discriminator losses fluctuate due to adversarial competition.
Generated Images:
Initially noisy, but get sharper and more digit-like after more epochs.

# Data Poisoning Simulation on Sentiment Classifier
# Overview
This code simulates a basic data poisoning attack on a sentiment classifier using an expanded small dataset. The main focus is:
Training a baseline sentiment classifier on movie reviews.
Poisoning the training data by flipping labels for sentences mentioning "UC Berkeley".
Comparing model performance before and after poisoning.
# Dataset
Manually created dataset with 20 sentences (positive and negative sentiment).
Includes multiple sentences mentioning "UC Berkeley".
Balanced distribution of positive and negative labels.
# Installation & Requirements
Running on Google Colab
Required libraries are usually pre-installed.
!pip install scikit-learn pandas matplotlib seaborn
Running on Local System
pip install scikit-learn pandas matplotlib seaborn
Running the Script
# Output
Graphs and Visualizations
Bar chart comparing model accuracy before and after poisoning.
Heatmaps of confusion matrices showing classification results.
Observations
Model accuracy drops after data poisoning.
Confusion matrix shows an increase in misclassifications.
Flipping labels for "UC Berkeley" sentences causes confusion in the model, demonstrating the effectiveness of the data poisoning attack.
