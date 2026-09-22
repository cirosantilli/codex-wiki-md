<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For $N$ data values, define the [discrete Fourier transform](../../../../../discrete-fourier-transform.md) by

$$
\widehat v_k=\sum_{j=0}^{N-1}v_j\omega_N^{jk},\qquad\omega_N=e^{-2\pi i/N},\qquad
v_j=\frac1N\sum_{k=0}^{N-1}\widehat v_k\omega_N^{-jk}.
$$

Direct evaluation costs $O(N^2)$ operations. For even $N$, split the sum into even and odd indices. If $E_k$ and $O_k$ are the length-$N/2$ transforms of $v_{2j}$ and $v_{2j+1}$, then

$$
\widehat v_k=E_k+\omega_N^k O_k,\qquad
\widehat v_{k+N/2}=E_k-\omega_N^k O_k,\qquad0\le k<N/2.
$$

The fact that $\omega_N^2=\omega_{N/2}$ makes the two smaller transforms reusable; $\omega_N^{k+N/2}=-\omega_N^k$ gives the second output. This is the [FFT butterfly](../../../../../fft-butterfly.md). For $N=2^p$ recursively splitting until length one gives

$$
T(N)=2T(N/2)+O(N)=O(N\log N).
$$

An iterative [Cooley-Tukey FFT algorithm](../../../../../cooley-tukey-fft-algorithm.md) can arrange the input in bit-reversed order and apply butterflies of lengths $2,4,\ldots,N$. The factors $\omega_N^k$ are the twiddle factors. Each level uses $O(N)$ work, and in-place organization uses $O(N)$ storage. The inverse uses the conjugate roots with the final normalization $1/N$. Mixed-radix factorizations extend the same idea beyond powers of two. For a two-dimensional array, transforming rows and then columns implements the two-dimensional transform, again exploiting separability.

For a concrete Poisson application, choose $-\Delta u=f$ in the unit square with zero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). Let $h=1/N$ and use interior indices $i,j=1,\ldots,N-1$. The five-point [finite difference](../../../../../finite-difference-split.md) equation is

$$
\frac{4u_{ij}-u_{i-1,j}-u_{i+1,j}-u_{i,j-1}-u_{i,j+1}}{h^2}=f_{ij}.
$$

The product sine vectors diagonalize this matrix. Their eigenvalues are

$$
\lambda_{k\ell}=\frac4{h^2}\left[\sin^2\frac{\pi k}{2N}+\sin^2\frac{\pi\ell}{2N}\right],\qquad1\le k,\ell<N.
$$

Define the two-dimensional [discrete sine transform](../../../../../discrete-sine-transform.md) coefficients by

$$
\widehat f_{k\ell}=\frac4{N^2}\sum_{i,j=1}^{N-1}f_{ij}\sin\frac{\pi ki}{N}\sin\frac{\pi\ell j}{N}.
$$

The sine orthogonality identity $\sum_{i=1}^{N-1}\sin(\pi ki/N)\sin(\pi ri/N)=N\delta_{kr}/2$ gives the inverse reconstruction. The [discrete sine transform Poisson solver](../../../../../discrete-sine-transform-poisson-solver.md) is therefore

$$
\boxed{\widehat u_{k\ell}=\widehat f_{k\ell}/\lambda_{k\ell},\qquad
u_{ij}=\sum_{k,\ell=1}^{N-1}\widehat u_{k\ell}\sin\frac{\pi ki}{N}\sin\frac{\pi\ell j}{N}.}
$$

All eigenvalues are positive, so there is no division by a zero mode for Dirichlet data. Nonzero prescribed boundary values are moved to the right side at neighboring interior points before transforming.

To compute the sine transform with a [Fast Fourier transform](../../../../../cooley-tukey-fft-algorithm.md), extend a one-dimensional interior vector oddly to length $2N$: set $v_0=v_N=0$ and $v_{2N-j}=-v_j$. Its length-$2N$ Fourier coefficient is $-2i\sum_{j=1}^{N-1}v_j\sin(\pi kj/N)$. Thus ordinary FFTs compute each sine transform. Apply this along all rows and columns, divide the coefficients, and apply inverse transforms. The total cost is **$O(N^2\log N)$ operations and $O(N^2)$ storage** for $O(N^2)$ unknowns. The method solves the finite-difference linear system directly to rounding accuracy; discretization error is separate and is second order for sufficiently smooth data and solution.

Boundary conditions determine the appropriate transform. Periodic data use the ordinary two-dimensional [discrete Fourier transform](../../../../../discrete-fourier-transform.md) and eigenvalues $4h^{-2}[\sin^2(\pi k/N)+\sin^2(\pi\ell/N)]$. The constant mode then requires zero-mean forcing, and the solution mean is fixed separately. Neumann conditions similarly use an appropriate [discrete cosine transform](../../../../../discrete-cosine-transform.md), with a compatibility condition and an undetermined additive constant. A Fourier spectral discretization would use continuous spectral eigenvalues instead of the finite-difference eigenvalues above. The speed comes from a constant-coefficient separable operator on a regular rectangle; a general irregular domain or variable-coefficient equation is not diagonalized by this simple FFT construction.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
