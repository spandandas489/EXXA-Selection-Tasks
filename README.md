# EXXA-Selection-Tasks
Repository for submissions to EXXA selection tasks under ML4SCI

---

## Tasks Overview

### General Task — Protoplanetary Disk Clustering
Unsupervised clustering of protoplanetary disk images using a convolutional autoencoder. Latent representations are reduced via PCA → UMAP and clustered with k-means and HDBSCAN. 


---

### Image Task — Image Reconstruction
Benchmarks two autoencoder variants (MSE-only vs. combined MSE+MS-SSIM) on protoplanetary disk image reconstruction. 




---

### Sequential Task — Exoplanet Transit Detection
Binary classification of Kepler light curves (planet vs. non-planet) using raw multi-transit segments. A 1D CNN+BiLSTM architecture captures both local transit features and global temporal structure.


---

## Pre-trained Weights

All model weights are available in the `Pre-trained Models and Weights/` directory. Each notebook has a `LOAD_PRETRAINED` flag at the top of the configuration cell — set it to `True` to skip training and load the saved weights directly.

| Weight File | Task | Description |
|---|---|---|
| `autoencoder_weights` | General | CNN autoencoder for disk clustering |
| `mse_only_autoencoder` | Image | Autoencoder trained with MSE loss only |
| `combined_loss_autoencoder` | Image | Autoencoder trained with MSE + MS-SSIM loss |
| `transit_classifier` | Sequential | 1D CNN+BiLSTM for transit classification |

---

## Author

**Spandan Das**





