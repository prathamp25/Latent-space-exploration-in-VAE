# Latent-space-exploration-in-VAE
A Variational Autoencoder (VAE) using PyTorch and trains it on the Fashion MNIST dataset.

The VAE compresses images into a 2D latent space and reconstructs them, learning meaningful representations.

It defines an encoder that compresses 28×28 grayscale images into a latent space of size 2, where it learns a probabilistic distribution (mean and log variance). A reparameterization trick is used to sample from this distribution, ensuring differentiability. The decoder then reconstructs the images from the latent representation. The model is trained using a combination of reconstruction loss (Binary Cross-Entropy) and KL divergence, which regularizes the latent space. The optimizer used is Adam, and the data is loaded in batches with transformations applied. The goal of this VAE is to learn a meaningful lower-dimensional representation of the Fashion MNIST images while ensuring smooth latent space transitions for generative purposes.
