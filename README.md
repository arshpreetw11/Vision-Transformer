#Vision Transformer (ViT) Replication using PyTorch
Project Overview

This project presents an implementation and replication of the Vision Transformer (ViT) architecture using PyTorch. The model is developed from scratch to understand the internal working of transformer-based image classification models and later compared with a pretrained Vision Transformer model.

The project demonstrates image patch embedding, positional encoding, multi-head self-attention, transformer encoder blocks, and training workflows for image classification tasks.

Features
Implementation of Vision Transformer (ViT) from scratch
Image patch creation and embedding generation
Positional embedding and learnable class token
Multi-Head Self-Attention mechanism
Transformer Encoder block implementation
Custom MLP block construction
Training and evaluation pipeline
Transfer learning using pretrained ViT-B/16
Model comparison between custom and pretrained approaches
Dataset

The project uses the Pizza, Steak, Sushi image classification dataset.

Classes included:

Pizza
Steak
Sushi

Dataset source:
PyTorch Deep Learning dataset repository.

Technologies Used
Python
PyTorch
Torchvision
Matplotlib
Torchinfo
Jupyter Notebook
Project Structure
replicating_project.ipynb      # Main notebook containing complete implementation
models/                        # Saved trained models
data/                          # Dataset directory
Model Architecture

The custom Vision Transformer implementation contains:

Patch Embedding Layer
Converts input images into fixed-size patches.
Uses convolutional projection for embedding generation.
Class Token
Learnable token added to the patch sequence.
Positional Embeddings
Preserves spatial information across image patches.
Multi-Head Self-Attention (MHSA)
Enables contextual understanding among patches.
MLP Block
Feed-forward neural network for representation learning.
Transformer Encoder Stack
Combines attention and MLP blocks with residual connections.
Classification Head
Produces final class predictions.
Training

The model is trained using:

Optimizer: Adam
Loss Function: Cross-Entropy Loss
Image Size: 224 × 224
Patch Size: 16 × 16

Training includes both:

Custom Vision Transformer implementation
Pretrained Vision Transformer fine-tuning
Results

The project evaluates:

Training loss
Testing loss
Training accuracy
Testing accuracy

Loss curves are plotted for performance analysis.

Installation

Clone the repository:

git clone https://github.com/arshpreetw11/Vision%20Transformer.git
cd "Vision Transformer"

Install dependencies:

pip install torch torchvision matplotlib torchinfo
Usage

Run the notebook:

jupyter notebook replicating_project.ipynb

Execute cells sequentially to:

Load dataset
Create patch embeddings
Build Vision Transformer architecture
Train custom ViT
Fine-tune pretrained ViT
Evaluate performance
Future Improvements
Hyperparameter tuning
Experimentation with larger datasets
Advanced augmentation techniques
Performance benchmarking with CNN architectures
Model deployment integration
References
Dosovitskiy et al. — An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale
PyTorch Documentation
Torchvision Model Documentation
Author
Arshpreet Walia
Git-Hub : arshpreetw11
