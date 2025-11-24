# 🧼 Image Denoising Using Convolutional Autoencoders

This project demonstrates how a **Convolutional Autoencoder (CAE)** can be used to remove noise from images.
Using the **MNIST handwritten digits dataset**, the model learns to reconstruct clean images from noisy inputs by learning meaningful spatial features.

---

## 🚀 Overview

The project workflow includes:

* Loading MNIST dataset
* Adding Gaussian noise to the images
* Training a Convolutional Autoencoder to remove noise
* Evaluating results using **PSNR** and **SSIM**
* Visualizing and comparing:

  * Original images
  * Noisy images
  * Denoised output predictions

---

## 🧠 Model Architecture

The autoencoder consists of:

* **Encoder**: Convolution + MaxPooling layers to compress image features
* **Decoder**: Convolution + Upsampling layers to reconstruct clean images

The network learns to map noisy inputs → clean output.

---

## 📦 Requirements

Make sure the following libraries are installed:

```
TensorFlow
NumPy
Matplotlib
scikit-image
```

You can install dependencies with:

```bash
pip install tensorflow numpy matplotlib scikit-image
```

---

## ▶️ How to Run

```bash
python denoising_autoencoder.py
```

After training completes, the script will display visual results comparing:

* Noisy Input
* Denoised Output
* Ground Truth Image

---

## 📊 Evaluation Metrics

The model performance is evaluated using:

| Metric   | Meaning                                                              |
| -------- | -------------------------------------------------------------------- |
| **PSNR** | Measures reconstruction quality (higher = better)                    |
| **SSIM** | Measures similarity to original image based on structure & luminance |

---

## 🖼 Sample Output

✔️ Before vs After denoising plots are generated to visually compare model performance.

---

## 📁 Dataset

* Dataset used: **MNIST (60,000 train / 10,000 test handwritten digits)**
* Automatically downloaded via `TensorFlow/Keras`

---

## ✨ Future Improvements

* Apply CAE to real-world noisy images
* Experiment with UNet or Diffusion-based denoisers
* Hyperparameter tuning for better reconstruction

---

## 👤 Author

**Neema J Rai**

