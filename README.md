# ImageBoost

**ImageBoost** is an end-to-end deep learning pipeline that denoises, enhances, and classifies low-quality images. The goal is to demonstrate how restoring visual fidelity improves downstream classification performance—and to explore how these tasks can be unified into a single, optimized pipeline.

## Project Overview
## Module Interaction & Data Flow

The ImageBoost pipeline flows through three sequential modules, each transforming the image to improve overall classification accuracy:

1. **Denoising Module**
   - Removes synthetic or real-world noise from input images
   - Input: Noisy image (`256x256`, RGB)
   - Output: Denoised image (`256x256`, RGB)

2. **Enhancement Module**
   - Applies super-resolution or sharpening to improve clarity
   - Input: Denoised image
   - Output: Enhanced image (`512x512`, RGB or same size)

3. **Classification Module**
   - Classifies the enhanced image into a category
   - Input: Enhanced image
   - Output: Class label (e.g., "cat", "car", "flower")

Each stage saves outputs to shared folders for the next module to use:
- `data/denoising_outputs/`
- `data/enhancement_outputs/`

All images are saved in `.png` format to ensure compatibility across modules.

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
