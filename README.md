# ImageBoost

**ImageBoost** is an end-to-end deep learning pipeline that denoises, enhances, and classifies low-quality images. The goal is to demonstrate how restoring visual fidelity improves downstream classification performance—and to explore how these tasks can be unified into a single, optimized pipeline.

## Project Overview

Real-world images often suffer from noise, low resolution, or degradation, which impacts tasks like classification and detection. Our solution integrates three key components:

1. **Image Denoising**  
   Removes noise artifacts from low-quality images using convolutional autoencoders (e.g., DnCNN, UNet).

2. **Super-Resolution / Enhancement**  
   Upscales and enhances image quality using models like SRCNN or GAN-based approaches (e.g., SRGAN).

3. **Image Classification**  
   Applies deep learning models (e.g., ResNet, EfficientNet) to classify the restored images with improved accuracy.

## Team Roles

| Name         | Role               | Responsibility                     |
|--------------|--------------------|-------------------------------------|
| Person A     | Denoising Lead     | Image noise removal + pipeline input |
| Person B     | Enhancement Lead   | Super-resolution & enhancement     |
| Person C     | Classification Lead| Image labeling & final prediction  |

## Repository Structure

The repository is organized as follows:
- **denoising/**: Contains code and models for noise removal, including a README.
- **enhancement/**: Contains super-resolution and enhancement models, along with its README.
- **classification/**: Contains image classification models and a corresponding README.
- **data/**: Stores input/output image samples, with subfolders like `denoising_outputs/`.
- **utils/**: Contains shared scripts and utilities used across the project.
- **notebooks/**: Contains the final integrated Jupyter notebooks.
- **media/**: Contains pipeline diagrams and presentation assets.
- **README.md**: This project description file.

## Status

- Project proposal submitted (April 7 deadline)
- Week 1: Dataset selection, repo setup, and model planning
- Model implementation + experimentation (April–May)

## Timeline

| Phase                     | Dates              |
|---------------------------|--------------------|
| Proposal Submission       | ✅ April 7, 2025   |
| Model Development         | April 8 – May 1    |
| Final Submission          | May 8, 2025        |

## Contact

For any questions or collaboration inquiries, please contact the team via GitHub Issues or by email.
