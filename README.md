# Cartoon Character Detector
This project is a machine learning solution for detecting specific cartoon characters in images. It leverages a supervised learning model to recognize seven well-known cartoon characters. Given an image input, the model outputs the character's name if it's among the predefined list. The current version of the model is trained to recognize:

- Donald Duck
- Mickey Mouse
- Minion
- Olaf
- Pooh
- Powerpuff Girls
- Pumba

This project aims to demonstrate how to preprocess, train, and evaluate a model for cartoon character recognition and can serve as a foundation for expanding to other characters or image classification tasks.

## Project Structure
The project is structured in a Jupyter notebook that contains the following main sections:

### Analysis:

Defines the problem and objectives, detailing the characters that the model can recognize and the dataset's structure.
Describes the approach of using supervised learning and the types of evaluations used.
### Data Preprocessing:

Loads and preprocesses images, including resizing, normalization, and label encoding to ensure consistency for model input.
Applies data augmentation techniques to improve the model's generalization by simulating variations in image orientation, lighting, etc.
### Model Development:

Several models were developed and compared, including:
1. K-Nearest Neighbors (KNN): Configured with 15 neighbors using the Manhattan distance metric. Evaluated with 5-fold cross-validation.
3. Support Vector Classifier (SVC): Various kernels and hyperparameters were tested using grid search to find the best configuration.
4. Random Forest Classifier: An ensemble learning method that constructs multiple decision trees during training, which then vote to predict the final output. Cross-validation was used to assess its accuracy.
5. Convolutional Neural Network (CNN): A deep learning model with multiple convolutional, pooling, and dropout layers for feature extraction and classification.
### Evaluation:

Evaluates the model’s performance using:

**Accuracy Score:** Measures the model's ability to classify images correctly.

**Confusion Matrix:** Provides a breakdown of predictions to show areas of high accuracy and misclassifications.

**Visual Evaluation:** Shows example predictions to enable human review of the results and confirmation of the model’s performance.
