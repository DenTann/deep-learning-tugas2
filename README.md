# Studi Komparatif Empiris Model Generatif (AE, Sparse AE, VAE, GAN, DCGAN, DDPM) & Pembuktian Batasan MLP Classifier

Repositori ini berisi implementasi PyTorch untuk tugas mandiri mata kuliah **Deep Learning**.

## Penulis
* **Nama:** Demetrius Denzell Tan
* **NIM:** 2802393030

## Struktur Repositori
* `src/01_mlp_classifier_proof.ipynb`: Eksperimen pembuktian batasan matematis dan empiris bobot ($W^T$) serta ruang laten $Z_{MLP}$ pada MLP Classifier.
* `src/02_autoencoders_vae.ipynb`: Pelatihan dan evaluasi Vanilla Autoencoder, Sparse Autoencoder ($L_1$), dan Variational Autoencoder (VAE).
* `src/03_gan_dcgan_ddpm.ipynb`: Pelatihan dan evaluasi Vanilla GAN, DCGAN, dan Denoising Diffusion Probabilistic Models (DDPM), serta pembuatan grafik komparatif.
* `results/`: Kompilasi lima figur visualisasi resolusi tinggi (300 DPI).

## Cara Menjalankan Kode
1. Instal seluruh dependensi:
   ```bash
   pip install -r requirements.txt
   ```

2. Jalankan notebook eksperimen secara berurutan di Google Colab atau Jupyter Notebook (dengan GPU dan seed=42):
*  Buka dan jalankan src/01_mlp_classifier_proof.ipynb untuk menghasilkan results/figur_3_mlp_proof.png.
*  Buka dan jalankan src/02_autoencoders_vae.ipynb untuk menghasilkan results/figur_1_rekonstruksi.png.
*  Buka dan jalankan src/03_gan_dcgan_ddpm.ipynb untuk menghasilkan results/figur_2_sampling.png, results/figur_4_interpolasi.png, dan results/figur_5_loss_ddpm.png.