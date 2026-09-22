# Fourier-Galerkin matrix for a drift-diffusion equation

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

For $u_t=u_{xx}-w'u_x$ and Fourier truncation $|n|\leq D$,

$$
\dot{\widehat u}_n=\sum_{|m|\leq D}B_{nm}\widehat u_m,
$$

where

$$
B_{nm}=-\pi^2n^2\delta_{nm}
+\pi^2(n-m)m\,\widehat w_{n-m}.
$$

For $w(x)=\cos\pi x$, the nonconstant block has Gershgorin discs in the closed left half-plane, while the constant mode lies in the kernel. Hence every eigenvalue has nonpositive real part and the matrix is singular.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/41a/b/solution.md)
