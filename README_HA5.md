# Assignment: GAN & Data Poisoning Simulation

## Student Info
**Name**: Damodar Goud Ediga  
**Student ID**: 700755572  

---

## Question 3: Basic GAN Implementation (MNIST)

### Overview
This project implements a simple Generative Adversarial Network (GAN) using PyTorch to generate handwritten digits from the MNIST dataset.

### Architecture
- **Generator**: 100-dim noise → Fully connected layers → 784-dim image
- **Discriminator**: 784-dim image → Fully connected layers → Binary (real/fake)

### Features
- Alternating training of generator and discriminator
- Sample image grids saved at **Epoch 0, 10, 20**
- Final plot showing **loss curves** of both networks

### How to Run (Google Colab)
1. Open the Colab notebook
2. Run all cells sequentially
3. Generated images are saved under `gan_images/`

---

## Question 4: Data Poisoning Simulation

### Overview
This project simulates a **label flipping attack** on a text sentiment classifier. The classifier is trained on a small review dataset with positive and negative labels.

### What It Does
- Trains a **Logistic Regression** model on clean data
- Poisons the data by **flipping labels** for samples mentioning `"UC Berkeley"`
- Re-evaluates the model and compares **accuracy** and **confusion matrix** before vs. after the attack

### Deliverables
- Accuracy before and after poisoning
- Confusion matrix plots
- Clean and poisoned dataset comparison

### How to Run (Google Colab)
1. Open the Colab notebook
2. Run all cells
3. See side-by-side confusion matrices and accuracy drop due to poisoning

   Video Link : https://drive.google.com/file/d/1wIMGxr4uO-vHTXW0xeKQRG40GXXUclva/view?usp=share_link
