# Generative-AI-work

## Diffusion Model for Image Generation (MNIST)

This project implements and trains a U-Net-based diffusion model capable of generating handwritten digits from scratch using the MNIST dataset.

🧠 **Key Concepts**:
- Forward and reverse diffusion process
- U-Net architecture
- Image denoising and reconstruction
- PyTorch implementation
- Generative AI fundamentals

📦 **Dataset**: MNIST (28x28 grayscale digits)  
🛠️ **Frameworks**: PyTorch, torchvision, einops  
💻 **Hardware**: Tested on GPU (CUDA-enabled), supports CPU fallback  

## 🚀 Project Highlights

- Trained for 30 epochs on 80/20 train-validation split
- Added print checkpoints for real-time debugging and validation
- Final generated samples resemble real handwritten digits

## 📊 Results

<img src="images/generated_samples.png" width="500"/>

> 📝 *Note: Above image is generated after training using the reverse diffusion process on a noisy latent.*

- Images to come... 

## 🛠️ Troubleshooting Approach

To ensure reliable execution, we included `print()` statements after key steps:
- GPU/CPU checks
- Dataset loading and splitting
- Image preprocessing validation
- Diffusion process monitoring

This helped catch shape mismatches and ensure all stages of the pipeline executed correctly.

## 🧪 Try It Yourself

You can open the notebook in Google Colab or run it locally with:

```bash
pip install torch torchvision einops matplotlib
