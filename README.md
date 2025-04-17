# Diffusion-based-Image-Generation-with-U-Net Architecture

Overview:
This project demonstrates a diffusion-based image restoration technique using a U-Net architecture to remove noise from images. The model leverages the forward and reverse diffusion process to progressively add and remove noise, generating high-quality images from noisy inputs. The core idea is based on the denoising process in diffusion models, which can be trained to predict and reverse noise added to the images.

Key Features:

Image Generation & Denoising: Generates images from random noise and progressively refines them by removing noise during training.

U-Net Architecture: A powerful convolutional neural network (CNN) model designed for image-to-image tasks, particularly for denoising.

Reverse Diffusion: Utilizes a reverse diffusion model to restore original images starting from noisy inputs.

Image Restoration: Trains the model to predict the noise at each step and restore images through progressive denoising.

PROJECT STRUCTURE:

1. Image Preprocessing:
   
    -Load and preprocess input images.

    -Convert images into tensors for training and testing.

2. Diffusion Process:
   
    -Forward Diffusion: Gradually adds noise to the image.

    -Reverse Diffusion: Removes noise at each step to recover the original image.

3. U-Net Architecture:
   
    -Encoder-Decoder architecture designed for image restoration tasks, with skip connections for better information flow.

5. Training the Model:
   
   -The model is trained using MSE (Mean Squared Error) loss to predict noise at each timestep and refine the image.

7. Image Restoration:
   
   -Use the reverse diffusion process to restore images starting from noisy inputs.
