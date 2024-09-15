# Variational Auto-Encoders (VAE) - Advanced Course on Deep Generative Models

## Overview
This repository contains the solution for **Exercise 5: Variational Auto-Encoders (VAE)** from the Advanced Course on Deep Generative Models, Spring 2024. The assignment focuses on implementing a VAE model and training it on the MNIST dataset. The notebook includes ELBO computation, training, sampling, and latent traversals.

## Assignment Details

- **Instructor**: Dan Rosenbaum
- **Due Date**: 30 June 2024
- **Main File**: `main.ipynb`

### Key Tasks
1. **Implement ELBO Calculation**: Implement the `calc_elbo` function to compute the Evidence Lower Bound (ELBO) for training, evaluation, and testing. This includes:
   - Reconstruction log-likelihood
   - KL divergence between the approximate posterior and the prior.
   
2. **Sample Generation**: Implement the `sample` function to generate samples from the VAE. Use a standard Gaussian as the prior and generate samples from the decoder output.

3. **Encoder and Decoder Architecture**: 
   - The **encoder** uses several convolutional layers followed by fully connected layers to map inputs to the latent space.
   - The **decoder** uses fully connected layers followed by transposed convolutions to reconstruct the input image.

4. **MNIST Training**: Train the model on the MNIST dataset, log the ELBO, reconstruction likelihood, and KL divergence during training. Generate image samples and report ELBO results on the test set.

5. **Latent Traversals**: Visualize the learned latent space by interpolating between two latent representations of different digits. Generate and display the resulting transformation.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/vae-assignment.git
   cd vae-assignment
2. Open the main.ipynb notebook in Google Colab or Jupyter Notebook.

3. Run all cells to:
    * Train the VAE model on the MNIST dataset.
    * Generate image samples from the trained VAE.
    * Perform latent traversals between two different digit representations.
