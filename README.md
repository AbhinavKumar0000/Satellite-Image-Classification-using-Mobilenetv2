# Satellite-Image-Classification-using-Mobilenetv2

Land Cover Classification with Deep Learning
This repository contains the code for a dissertation project focused on leveraging deep learning techniques for satellite imagery analysis. The project implements a lightweight Convolutional Neural Network (MobileNetV2) to classify land use and land cover from Sentinel-2 satellite images using the EuroSAT dataset.

Project Overview
The primary goal of this research was to develop an efficient and accurate model for automated Land Use and Land Cover (LULC) classification. This is a foundational step in monitoring environmental changes like deforestation, urbanization, and agricultural expansion. By using a computationally efficient model, this project demonstrates a practical approach that can be executed in resource-constrained environments.

Key Features
Model: MobileNetV2, pre-trained on ImageNet.

Dataset: EuroSAT (Sentinel-2 satellite images).

Framework: PyTorch.

Performance: Achieved ~98% accuracy on the validation set.

Results
The model demonstrated exceptional performance, correctly classifying most land cover types. The main challenge identified was distinguishing between visually similar sub-categories (e.g., 'AnnualCrop' vs. 'Pasture').

Classification Report
Confusion Matrix
Example Predictions
The model correctly identifies the class in most cases. Misclassifications typically occur between similar classes.

How to Run the Code
1. Clone the Repository
git clone <your-repository-url>
cd <repository-name>

2. Install Dependencies
It is recommended to use a virtual environment.

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt

3. Run the Training Script
The script will automatically download the EuroSAT dataset, split it, and begin training. The best-performing model will be saved as best_eurosat_model.pth.

python train.py
