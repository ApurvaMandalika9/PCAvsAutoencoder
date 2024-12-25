# PCAvsAutoencoder

Applied the PCA and the autoencoder (AE) to a collection of handwritten digit images from the USPS dataset. The whole dataset is loaded and stored in the matrix A with shape 3000 × 256. Each row of matrix A represents a 16 × 16 handwritten digit image (between 0 and 9), which is flattened to a 256-dimensional vector. 
- PCA : Evaluated the code by testing different numbers of the principal component that p = 32, 64, 128.
- AE : Evaluated the code by testing three different dimensions for the hidden representation d that d = 32, 64, 128.

- Compared both PCA and AE with p=d: Observed that when p is low(32, 64), AE has marginally lower reconstruction error than PCA. When p is high, PCA error is marginally low. So, if we ignore the minor differences in the errors, overall in conclusion, when the weights are shared between encoder and decoder, AE is equivalent to PCA.   
