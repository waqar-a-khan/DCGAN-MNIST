# **DCGAN for MNIST Digit Generation** 🎨🔢  

This repository contains a **Deep Convolutional Generative Adversarial Network (DCGAN)** trained on the **MNIST dataset** to generate realistic handwritten digits. The model uses **convolutional and transposed convolutional layers** to generate high-quality 28×28 grayscale digits from random noise.  

## **✨ Features**  
✅ **Uses DCGAN architecture** (Conv & Transposed Conv layers)  
✅ **LeakyReLU for stable training**  
✅ **BatchNorm to improve convergence**  
✅ **Tanh activation to generate realistic digits**  
✅ **Visualizes generated digits during training**  

## **📌 Dataset**  
- **MNIST Dataset**: Handwritten digit images (0-9)  
- Images are **normalized to (-1,1)** for GAN training  

## **🚀 Training Details**  
- **Discriminator:** Learns to classify real vs. fake images  
- **Generator:** Creates fake images to fool the Discriminator  
- **Loss Function:** Binary Cross-Entropy (BCE)  
- **Optimizer:** Adam (lr=0.0002, β1=0.5)  
- **Training for 50 epochs**  

## **📂 Repository Structure**  
```
📦 DCGAN-MNIST  
 ├── 📄 dcgan_mnist.ipynb   # Jupyter Notebook for training in Google Colab  
 ├── 📂 data/               # MNIST dataset (downloaded automatically)  
 ├── 📂 generated/          # Generated images saved during training  
 ├── 📄 README.md           # Project documentation  
 ├── 📄 requirements.txt    # Required libraries  
```

## **🔧 Setup & Usage (Run on Google Colab)**  
1️⃣ Open the notebook in Google Colab:  
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/DCGAN-MNIST/blob/main/dcgan_mnist.ipynb)

2️⃣ Install dependencies:  
```python
!pip install torch torchvision matplotlib
```  
3️⃣ Run the cells in `dcgan_mnist.ipynb` to train the model.  

## **📊 Sample Results**  
Generated MNIST Digits after 50 epochs:  
![Generated Digits](https://user-images.githubusercontent.com/example/generated_digits.png)  

---
### **🔗 References**  
- [DCGAN Paper (Radford et al., 2015)](https://arxiv.org/abs/1511.06434)  
- [PyTorch DCGAN Tutorial](https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html)  

🚀 **Happy Training!**

