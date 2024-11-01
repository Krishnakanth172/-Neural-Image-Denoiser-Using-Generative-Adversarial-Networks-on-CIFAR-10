Project Overview
This project applies a Generative Adversarial Network to restore noisy images in the CIFAR-10 dataset. The model injects some Gaussian noise to the image,
and the generator would learn to restore the clean original images from the noise. To validate the power of the generator, it has to cross-check from the
discriminator that whether those images are actual or are generated.
The paper on this research will explore the uses of GANs while restoring noisy images based on CIFAR-10. GAN divides into
A generator that will generate clean images from noising.
A discriminator that will differentiate between clean original images and noisy images.

Dataset
This dataset consists of 60,000 32x32 color images in ten classes with 50,000 training images and 10,000 testing images.
Noisy inputs for this project are simulated by adding Gaussian noise to the images.

Requirements
To run this project, you will need:
Python 3.7 or higher
TensorFlow 2.x
NumPy
Matplotlib

Setup
Clone the repository:
 git clone https://github.com/yourusername/cifar10_denoising_gan.git
 cd cifar10_denoising_gan

Install required dependencies:
 pip install -r requirements.txt

How to Run
Train the GAN: To train the GAN on noisy CIFAR-10 images, you should run.
 python gan.py
Evaluate the GAN: After the training has finished, you can evaluate the model on test images and visualize the results:
 python evaluate.py

Results
In the training process, the generator learns to reconstruct the denoised images from the noisy inputs. Some sample results are as follows:
Noisy Image vs. Denoised Image vs. Original Image

References
CIFAR-10 Dataset: https://www.cs.toronto.edu/~kriz/cifar.html
GAN Paper: https://arxiv.org/abs/1406.2661
