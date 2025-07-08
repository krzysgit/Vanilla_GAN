# Vanilla GAN Network

## Overview
A simple Vanilla GAN implementation for generating 28x28 grayscale images.

---

## Hyperparameters

| Parameter          | Value          | Description                          |
|--------------------|----------------|------------------------------------|
| `latent_dim`       | 100            | Dimension of input noise vector    |
| `batch_size`       | 64             | Number of samples per batch        |
| `lr`               | 0.0002         | Learning rate for optimizers       |
| `num_epochs`       | 101            | Number of training epochs          |
| `g_steps`          | 1              | Generator update steps per iteration |
| `image_size`       | 784 (28x28)    | Flattened image size                |
| `image_channels`   | 1              | Number of image channels (grayscale) |
| `hidden_dim_g`     | [512, 256, 128]| Generator hidden layer sizes       |
| `hidden_dim_d`     | [128, 256, 512]| Discriminator hidden layer sizes   |
| `dropout_rate`     | 0.3            | Dropout rate in discriminator      |
| `real_label_smooth`| 0.9            | Smoothed target label for real images |
| `fake_label_smooth`| 0.1            | Smoothed target label for fake images |

---

## Comments

My implementation does not achieve state of the art results. I suspect it to be down to the discriminator not being a Convolutional NN but a linear one. I would be very grateful if someone could comment on that
