# GAN Image Generator using PyTorch

## Project Overview

This project implements a Generative Adversarial Network (GAN) using PyTorch to generate synthetic images based on the CIFAR-10 dataset.

The project explores generative deep learning through two competing neural networks: a Generator and a Discriminator.

The Generator learns to produce synthetic images, while the Discriminator learns to distinguish generated images from real dataset samples.

## Technologies Used

- Python
- PyTorch
- Torchvision
- Google Colab
- Jupyter Notebook
- CIFAR-10 Dataset

## Model Architecture

The implementation follows a Deep Convolutional GAN (DCGAN-style) architecture.

**1. Generator**
- Takes random noise as input.
- Uses transposed convolutional layers.
- Applies Batch Normalization and ReLU activation.
- Generates synthetic RGB images.

**2. Discriminator**
- Receives real and generated images.
- Uses convolutional layers.
- Applies LeakyReLU activation.
- Predicts whether an image is real or generated.

## Training Configuration

| Parameter | Value |
|---|---|
| Dataset | CIFAR-10 |
| Image Size | 64 × 64 |
| Latent Dimension | 100 |
| Batch Size | 128 |
| Epochs | 10 |
| Optimizer | Adam |
| Learning Rate | 0.0002 |
| Loss Function | Binary Cross Entropy |

## Training Process

The model follows an adversarial training process:

1. Load and preprocess the CIFAR-10 dataset.
2. Initialize the Generator and Discriminator.
3. Train the Discriminator using real and generated images.
4. Train the Generator to produce images that fool the Discriminator.
5. Monitor training losses.
6. Generate and visualize synthetic images during training.

## Project Structure

```text
GAN_Image_Generator/
│
├── GAN_Image_Generator.ipynb
└── README.md
```

## Results and Observations

The model produces synthetic image samples during training.

The generated images demonstrate the initial learning capabilities of the adversarial network, although image quality and object clarity remain areas for improvement.

Training for additional epochs and experimenting with model architecture and hyperparameters could improve generation quality.

## Learning Outcomes

Through this project, I explored:

- Generative Adversarial Networks.
- Convolutional neural networks.
- PyTorch model implementation.
- Adversarial training.
- Image preprocessing.
- Neural network optimization.
- Monitoring generative model training.

## Future Improvements

- Extend training duration.
- Experiment with different hyperparameters.
- Implement model checkpointing.
- Improve training visualization.
- Explore quantitative GAN evaluation metrics.
- Experiment with alternative GAN architectures.

## Author

**Gyang Shedrach Emmanuel**

Computer Science | Machine Learning | Deep Learning | Data Science

GitHub: [@GyangShady](https://github.com/GyangShady)

LinkedIn: [Gyang Shedrach](https://www.linkedin.com/in/gyang-shedrach-70a37226a/)
