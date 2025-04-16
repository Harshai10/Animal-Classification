# Animal-Classification

# Animal Classification Project

## Description
This project implements an image classification system to identify various animal species using deep learning techniques. It explores both a custom Convolutional Neural Network (CNN) and transfer learning approaches using pre-trained models like MobileNetV2 and VGG16.

## Installation
To run this project, you need to have Python installed along with the required libraries. You can set up a virtual environment and install the dependencies using the following commands:

```bash
# Create a virtual environment
python -m venv myenv

# Activate the virtual environment
# On Windows
myenv\Scripts\activate
# On macOS/Linux
source myenv/bin/activate

# Install required packages
pip install -r requirements.txt
```

## Usage
1. Place your dataset in the `dataset/` directory, organized into subfolders for each class.
2. Open `animalclassification.ipynb` in Jupyter Notebook or any compatible environment.
3. Run the cells sequentially to preprocess the data, train the models, and evaluate their performance.

## Dataset Information
The dataset consists of images of various animal classes organized in folders, each representing a class. The images are preprocessed and augmented to improve model generalization.

## Model Architecture
### Custom CNN Model
A custom CNN model is built with convolutional layers, batch normalization, and max pooling layers, followed by dense layers for classification.

### Transfer Learning
Two transfer learning models are implemented:
- **MobileNetV2**: A lightweight model pre-trained on ImageNet, fine-tuned for animal classification.
- **VGG16**: A deeper model also pre-trained on ImageNet, used for comparison.

## Training Instructions
The models are trained using the `fit` method with early stopping and learning rate reduction callbacks to optimize performance. Training parameters such as batch size and number of epochs can be adjusted in the notebook.

## Evaluation
After training, the models are evaluated on a validation set, and performance metrics such as accuracy, loss, confusion matrix, and classification report are generated.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

---

Feel free to contribute to this project or use it as a reference for your own animal classification tasks!
