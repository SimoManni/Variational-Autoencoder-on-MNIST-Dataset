# Variational Autoencoder on MNIST Dataset

This repository contains the step-by-step implementation of a Variational Autoencoder (VAE), a simple deep generative network, on the MNIST dataset. 

## Overview
Variational Autoencoders (VAEs) are a type of generative model that learn to encode input data into a latent space, then decode it back to the original data. This implementation demonstrates how to build and train a VAE using the MNIST dataset, which consists of handwritten digit images.

The notebook motivates the switch from normal autoencoders to variational autoencoders by discussing the limitations of standard autoencoders in terms of generating new data. Normal autoencoders can compress and reconstruct data but lack a structured approach to sampling new data points from the latent space.

To address these limitations, the notebook introduces the concept of VAEs, which incorporate a probabilistic approach to the latent space representation. This is achieved by modeling the latent variables as distributions and using techniques such as the Kullback-Leibler (KL) divergence to measure the difference between the learned latent distribution and a prior distribution (typically a Gaussian). The KL divergence term in the VAE loss function encourages the learned latent space to be continuous and well-formed, enabling meaningful sampling and generation of new data.

Furthermore, the notebook provides a detailed explanation of how VAEs optimize the balance between reconstruction loss and the KL divergence, ensuring the encoded latent space is useful for generating new, coherent data samples.


## Features

- Implementation of the encoder and decoder networks
- Training process for the VAE on the MNIST dataset
- Visualization of the latent space
- Generation of new handwritten digits

## Results
The following video shows the latent space of the VAE and the generative capabilities of the network. 

<p align="center">
  <img src="https://github.com/SimoManni/Variational-Autoencoder-on-MNIST-Dataset/assets/151052936/e787c954-a1db-4ffc-9e60-10f9e31fae8e" alt="VAE Video" width="600">
</p>

