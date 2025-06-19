# Compressed_Sensing_PGD


Compressed sensing is a powerful signal processing framework that enables accurate reconstruction of sparse signals from far fewer measurements than traditionally required by the Nyquist-Shannon sampling theorem. In this project, we explore sparse signal reconstruction using the Proximal Gradient Descent (PGD) method, with a specific focus on the Iterative Shrinkage-Thresholding Algorithm (ISTA). We formulate the recovery task as an $\ell_1$-regularized least squares optimization problem, commonly known as the LASSO formulation, to promote sparsity in the solution.

Our implementation targets 2 two-dimensional grayscale images, simulating undersampling through random masks and applying transformations in the Discrete Cosine Transform (DCT) domain to exploit sparsity. GPU acceleration via CuPy significantly boosts performance for large-scale images. Reconstruction quality is evaluated using Peak Signal-to-Noise Ratio (PSNR) across varying sampling ratios. The results demonstrate that PGD can successfully reconstruct visually and quantitatively accurate images—even when as little as 1\% of the pixel data is retained—highlighting its potential for practical applications such as accelerated MRI. This study confirms that PGD is a simple, effective, and scalable method for sparse recovery problems.

