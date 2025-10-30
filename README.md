# VAE-MNIST-Generator
In this project i tried to build a unsupervised Handwritten digit generator using Variational Autoencoder while doing my CSE425 Neural Network Course. The model trained on MNIST dataset and generate new, realistic digit images and it learns patterns directly from the data without any labels. 
## Objective :
- Compress images into a small latent space
- Reconstruct the original images accurately
- Generate new handwritten digit samples
- Show smooth transitions between digits

## VAE Explanation :
VAE is a deep learning model. It encodes images into a compact latent vector. It adds randomness to encourage diverse output and decodes the vector back into an image. It trains by balancing image quality and latent space structure. This helps not just copy, but create new images.
## Model Design

Encoder:
Convolution layers → flatten → produces mean + variance values

Reparameterization:
Added controlled noise to sample latent vector

Decoder:
Upsampling layers to reconstruct images from latent vector
Epochs	15
Batch Size	128

##Results
Quantitative:
- Low reconstruction error, MSE = 0.0223
- KL Divergence = 3.7078
- Latent Std = 1.015 

Qualitative:
- Reconstructed images look close to originals
- Generated digits look realistic; a few are blurry
- Smooth interpolation between digits
##Future Improvements:
- Train more epochs for sharper digits
- Will try β VAE to control disentanglement
- Experiment with CIFAR-10 or Fashion-MNIST
- add attention or deeper convolution blocks

## How To Run:
- open in google Colab
- Run locally in jupyter Notebook



