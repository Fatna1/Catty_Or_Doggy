# Catty_Or_Doggy 🐱🐶
 

A deep learning image classifier that distinguishes between cats and dogs with **98.64% test accuracy** using a fine-tuned ResNet18 architecture.

## 📊 Model Performance
- **Test Accuracy**: 98.64%
- **Training Time**: 3 epochs
- **Model**: ResNet18 (pretrained on ImageNet)
- **Framework**: PyTorch

## 🏗️ Architecture
- Base model: ResNet18 with transfer learning
- Modified final fully connected layer for binary classification (cat/dog)
- Optimizer: Adam (learning rate: 0.0001)
- Loss function: Cross-Entropy Loss

## 📁 Dataset
The model was trained on the [Dog and Cat Classification Dataset](https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset) from Kaggle, containing:
- Total images: ~25,000 (original dataset)
- Training split: 70%
- Validation split: 15%
- Test split: 15%

## 🚀 Quick Start

### Install dependencies
pip install -r requirements.txt

### Run the Notebook
1. Clone this repository
2. Open cat-dog-classification.ipynb in Jupyter Notebook or any Notebook editor
4. Run all cells to train the model or use the pre-trained weights

### 🎯 Data Preprocessing
Images are transformed using:
-Resize to 224×224 pixels
-Random horizontal flipping (data augmentation)
-Normalization using ImageNet stats (mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])

### Training Results:
<img width="731" height="78" alt="Screenshot 2026-04-28 150150" src="https://github.com/user-attachments/assets/543cd81b-6657-48e1-b83f-be8900a58811" />

## 🛠️ Technologies Used
-PyTorch: Deep learning framework
-TorchVision: Pre-trained models and transforms
-PIL: Image processing
-NumPy: Numerical operations

## Examples:
-🐱Cat Prediction:
_image1:_
<img width="270" height="148" alt="download" src="https://github.com/user-attachments/assets/c270ef78-3979-4713-bf2c-79ba3f369cb5" />
Output:
<img width="398" height="194" alt="Screenshot 2026-04-28 193723" src="https://github.com/user-attachments/assets/f45a5c64-9956-4c3d-9ab2-b16d428bccea" />
_image2:_
<img width="273" height="185" alt="5" src="https://github.com/user-attachments/assets/754ef890-1594-4f7b-a42d-b632c2506222" />
Ouput:
<img width="383" height="186" alt="image" src="https://github.com/user-attachments/assets/51930e48-3674-4d2d-a449-2cd0cfe59c34" />

-🐶 Dog Prediction
_image1_
<img width="1344" height="1012" alt="4" src="https://github.com/user-attachments/assets/8034a5b9-00c1-473e-ab38-be354bf29761" />
Output:
<img width="371" height="181" alt="image" src="https://github.com/user-attachments/assets/985bd654-8935-4c51-98c7-64f6d35dbc86" />
_image2_:
<img width="541" height="350" alt="2" src="https://github.com/user-attachments/assets/1bc90121-6d05-47cb-9bfc-f5d3d3f5ab13" />
Output:
<img width="341" height="183" alt="image" src="https://github.com/user-attachments/assets/00bdc541-82f4-48c7-883f-aa6fda993c84" />
_image3:_
<img width="660" height="370" alt="3" src="https://github.com/user-attachments/assets/883fdb14-9135-40a6-8139-639256b3404d" />
Output:
<img width="453" height="183" alt="image" src="https://github.com/user-attachments/assets/535cebc9-49be-4ffe-b69b-662d028afa43" />







