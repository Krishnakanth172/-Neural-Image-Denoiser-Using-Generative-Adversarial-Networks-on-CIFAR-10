Project Overview
This project implements a Generative Adversarial Network (GAN) to denoise images from the CIFAR-10 dataset. The model adds Gaussian noise to images, 
and the generator learns to reconstruct the original clean images from the noisy ones. The discriminator evaluates the authenticity of the denoised images,
distinguishing between real and generated images.

Introduction
Image denoising is crucial in image processing tasks to restore original, clean images from noisy data.
This project explores the use of GANs to remove noise from images by using the CIFAR-10 dataset. The GAN is composed of:

A Generator that generates clean images from random noise.
A Discriminator that distinguishes between original clean images and denoised images.

Dataset
The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 different classes, with 50,000 training images and 10,000 test images. 
For this project, Gaussian noise is added to the images to simulate noisy inputs.

Prerequisites
To run this project, you will need:
Python 3.7 or higher
TensorFlow 2.x
NumPy
Matplotlib

Installation
Clone the repository:
git clone https://github.com/yourusername/cifar10_denoising_gan.git
cd cifar10_denoising_gan

Install the required dependencies:
pip install -r requirements.txt

How to Run
Train the GAN: Run the following command to start training the GAN on noisy CIFAR-10 images.
python gan.py
Evaluate the GAN: After training, you can evaluate the model on test images and visualize the results:
python evaluate.py

Results
During the training, the generator learns to reconstruct denoised images from the noisy inputs. Here's a sample of the results:
Noisy Image vs. Denoised Image vs. Original Image

References
CIFAR-10 Dataset: https://www.cs.toronto.edu/~kriz/cifar.html
GAN Paper: https://arxiv.org/abs/1406.2661
