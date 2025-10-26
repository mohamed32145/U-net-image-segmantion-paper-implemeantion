#  U-Net: Convolutional Networks for Biomedical Image Segmentation

This repository contains a PyTorch implementation and experiment replications of the **U-Net** architecture, as proposed in the paper:  
> *Olaf Ronneberger, Philipp Fischer, Thomas Brox, “U-Net: Convolutional Networks for Biomedical Image Segmentation,” MICCAI 2015.*

---

##  Repository Structure

| File | Description |
|------|--------------|
| `DLfinal1.ipynb` | U-Net implementation and training pipeline (model, dataset, loss function, and training loop). |
| `DLfinal2.ipynb` | Experimental results, evaluation, and visualization of predictions on biomedical images. |

---

##  Project Overview

U-Net is a fully convolutional neural network designed for **biomedical image segmentation**, enabling pixel-level prediction with limited training data.

This project aims to:
- Reproduce the original U-Net architecture.
- Train and test it on biomedical segmentation datasets (e.g., ISBI 2012, Cell images, etc.).
- Visualize model outputs (segmentation masks, predictions vs. ground truth).

---

##  Architecture Overview

The U-Net consists of:
- **Encoder (Contracting path):** captures context using convolution and pooling.
- **Decoder (Expanding path):** enables precise localization using transposed convolutions and skip connections.
- **Skip connections:** merge encoder and decoder feature maps for high-resolution segmentation.

<img width="867" height="504" alt="image" src="https://github.com/user-attachments/assets/9e2db21c-ed87-45d0-a632-632ca98833a3" />


---

##  Requirements

Before running the notebooks, install dependencies:

```bash
pip install torch torchvision torchaudio
pip install numpy matplotlib scikit-image tqdm

