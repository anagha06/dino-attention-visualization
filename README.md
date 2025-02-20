# DINO Self-Attention Visualizations

This repository contains a notebook that visualizes self-attention patterns of Vision Transformers (ViTs) pre-trained using the DINO (Distillation with No Labels) method. DINO is a self-supervised learning method that allows Vision Transformers to segment objects in images without being explicitly trained to do so. This behavior is particularly interesting because it is not observed in traditional convolutional models like ResNets.

## Overview

The DINO paper demonstrates that Vision Transformers, when pre-trained using a self-supervised learning approach, are able to segment and identify objects within images. This is done without relying on supervised annotations, making it a significant advancement over traditional methods. The self-attention mechanism in ViTs allows the model to attend to different parts of an image, and through this notebook, we visualize how the model focuses on various regions during its decision-making process.

Key concepts explored in this notebook:
- **Self-Attention in ViTs**: The attention mechanism helps the model determine which parts of an image are most important by assigning higher attention weights to certain regions.
- **DINO Method**: DINO uses self-distillation to create robust representations of images without labels. This is done by maximizing similarity between different augmentations of the same image, encouraging the model to learn meaningful features that help with object segmentation.
- **Object Segmentation**: Unlike classical convolutional models, ViTs trained with DINO are able to naturally segment objects within an image, highlighting the power of self-supervised learning.

## Features

- **Self-Attention Visualization**: Visualize attention maps from different layers and heads in the ViT model.
- **Exploration of DINO's Impact**: Understand how DINO's self-supervised learning method enables object segmentation in ViTs.
- **Comparison to Convolutional Models**: Contrast the attention patterns in ViTs to traditional CNNs like ResNets, showing the advantages of transformer-based architectures for certain tasks.

## Requirements

- Python 3.x
- PyTorch
- Matplotlib (for visualization)
- NumPy

@inproceedings{caron2021emerging,
  title={Emerging Properties in Self-Supervised Vision Transformers},
  author={Caron, Mathilde and Touvron, Hugo and Misra, Ishan and Chen, Xie and Cord, Matthieu and Douze, Matthijs and Jégou, Hervé},
  booktitle={NeurIPS 2021},
  year={2021}
}
