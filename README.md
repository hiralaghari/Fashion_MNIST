# Fashion MNIST Classification with Transfer Learning

This project explores image classification on the Fashion MNIST dataset using transfer learning. It serves as an introduction to transfer learning techniques, using the pre-trained ResNet50 model to classify images of clothing items.

## Project Overview

The Fashion MNIST dataset consists of 70,000 grayscale images in 10 categories, with 60,000 images for training and 10,000 for testing. The goal is to classify each image into one of the 10 categories.

In this project, we utilized the ResNet50 model, pre-trained on the ImageNet dataset, and adapted it for the Fashion MNIST dataset through transfer learning. The key steps involved resizing the images, modifying the model architecture, and fine-tuning the model to achieve high accuracy on this new task.

## Key Steps

1. **Data Preprocessing**: 
   - Loaded and preprocessed the Fashion MNIST dataset.
   - Resized the images from 28x28 to 224x224 pixels to match the input size required by ResNet50.

2. **Model Selection**:
   - Used the ResNet50 model, pre-trained on ImageNet, with its top layers removed.
   - Added custom dense layers on top of ResNet50 to adapt it to the Fashion MNIST classification task.

3. **Transfer Learning**:
   - The convolutional base of ResNet50 was frozen, preserving the pre-trained weights.
   - The added custom layers were trained on the Fashion MNIST dataset.

4. **Training**:
   - Fine-tuned the model on the Fashion MNIST dataset.
   - Monitored performance using validation data.

## Results

The final model demonstrated strong performance on the Fashion MNIST dataset, leveraging the power of transfer learning to quickly achieve high accuracy.



## Conclusion

This project provided hands-on experience with transfer learning, demonstrating how a pre-trained model like ResNet50 can be adapted to a new task with minimal effort. The techniques learned here can be applied to various other image classification problems, particularly when dealing with smaller datasets.

## Acknowledgments

- [Keras Documentation](https://keras.io/api/applications/resnet/#resnet50-function)
- [Fashion MNIST Dataset](https://github.com/zalandoresearch/fashion-mnist)

