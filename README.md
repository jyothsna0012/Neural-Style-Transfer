# Neural-Style-Transfer


# 🎨 Neural Style Transfer using VGG19 (PyTorch)

This project implements **Neural Style Transfer (NST)** using a pre-trained **VGG19** network in **PyTorch**.  
It generates a stylized image by combining the **content of one image** with the **artistic style of another**.

---

## 📌 Project Description

Neural Style Transfer is a deep learning technique that:
- Preserves the **content structure** of a content image
- Transfers **artistic textures and patterns** from a style image
- Uses **Gram Matrices** to represent style information
- Optimizes a target image using **content loss + style loss**

---

## 🧠 Concepts Used

- Convolutional Neural Networks (CNN)
- Pre-trained **VGG19**
- Feature extraction from convolutional layers
- Gram Matrix for style representation
- Gradient-based optimization
- PyTorch autograd

---

## 🛠️ Technologies Used

- Python  
- PyTorch  
- Torchvision  
- Matplotlib  
- PIL (Image Processing)

---

## 📂 Project Structure


---

## ⚙️ How It Works

### 1️⃣ Feature Extraction
- Uses convolutional layers of **VGG19**
- Extracts content features (e.g., `conv4_2`)
- Extracts style features (e.g., `conv1_1`, `conv2_1`, `conv3_1`, etc.)

### 2️⃣ Style Representation
- Style is captured using **Gram Matrices**
- Gram matrices represent texture correlations in feature maps

### 3️⃣ Loss Functions
- **Content Loss**: Difference between target and content features
- **Style Loss**: Difference between Gram matrices of target and style
- **Total Loss** = Content Loss + Style Loss

### 4️⃣ Optimization
- The target image is optimized directly
- Uses **Adam optimizer**
- Runs for multiple iterations to improve stylization
