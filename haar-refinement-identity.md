# Haar refinement identity

↑ **Parent:** [Haar wavelet](haar-wavelet.md)

The normalized [Haar scaling functions](haar-scaling-function.md) and wavelets obey

$$
\varphi_{j,k}=2^{-1/2}(\varphi_{j+1,2k}+\varphi_{j+1,2k+1}),\qquad
\psi_{j,k}=2^{-1/2}(\varphi_{j+1,2k}-\varphi_{j+1,2k+1}).
$$

This orthogonal two-by-two transformation gives the [multiresolution analysis](multiresolution-analysis.md) decomposition $V_{j+1}=V_j\oplus W_j$. Iterating it expresses a [Haar approximation](haar-projection.md) either through level-$j$ cell averages or through coarse averages and all wavelet details at lower levels. The identities remain valid locally for coefficient integrals of [locally integrable functions](locally-integrable-function.md), without a global $L^2$ assumption.

## ↑ Ancestors (8)

1. [Haar wavelet](haar-wavelet.md)
2. [Orthonormal wavelet](orthonormal-wavelet.md)
3. [Wavelet](wavelet.md)
4. [Fourier analysis](fourier-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-7/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-33/3/solution.md)
