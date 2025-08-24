# Visual-Learning-Assistant-Framework-using-Text-To-Image-Diffusion-Models
**Text-to-Image Latent Diffusion Model for Educational Diagrams**

## 📌 Overview
* This project presents a specialized Latent Diffusion Model (LDM) pipeline designed to generate high-fidelity educational diagrams directly from text prompts. Unlike general-purpose diffusion models (e.g., Stable Diffusion), this lightweight approach is fine-tuned on structured educational datasets, producing curriculum-aligned, semantically accurate visuals to support learning and teaching.
* Built using PyTorch and Hugging Face Diffusers, the framework integrates:
  Fine-tuned Variational Autoencoder (VAE) for domain-specific latent representations.
  Text-conditioned U-Net (UNet2DConditionModel) with DDIM scheduler.
  Training optimizations: EMA, gradient accumulation, cosine LR scheduling, and noise augmentation.
* This system enables efficient inference on a single NVIDIA RTX 4090 GPU and supports further research on domain-specific diffusion models for education.

## Features
* Text-to-Diagram Generation: Create structured STEM visuals from natural language prompts.
* Domain-Specific VAE Fine-Tuning: Optimized latent representations for educational images.
* Lightweight & Efficient: Runs inference in under 2 seconds per sample on a single GPU.
* Quality Evaluation: Assessed with MSE, SSIM, and qualitative diagram clarity checks.
* Open Research Resource: All dataset preparation and training code provided.

## Tech Stack
* Frameworks: PyTorch, Hugging Face Diffusers
* GPU: NVIDIA RTX 4090 (24GB VRAM)
* Data Handling: Torchvision, NumPy, Pandas, Matplotlib
* Datasets: AI2D (4k+ annotated educational diagrams) & ScienceQA (21k+ diagram–question–answer pairs)

## Project Structure  

```text
Visual-Learning-Assistant-Framework-using-Text-To-Image-Diffusion-Models/
├── Dataset/                      # Data cleaning, preprocessing
├── Merging_AI2D_ScienceQA2/      # Dataset merging and preparation
├── VAE Implementation/           # Domain-specific VAE fine-tuning
├── LDM/                          # Latent Diffusion Model implementation
├── Inference/                    # Model inference and generation scripts
├── Results/                      # Evaluation metrics, visual outputs, qualitative results
├── README.md                     # Project documentation
```

## License
This project is for academic use only.

