# Power boundedness of a two-level Fourier scheme

↑ **Parent:** [von Neumann stability analysis](von-neumann-stability-analysis.md)

For a two-level Fourier recurrence $\widehat u^{n+1}=a(\theta)\widehat u^n+b(\theta)\widehat u^{n-1}$, the amplification [matrix](matrix.md) is

$$
T(\theta)=\begin{pmatrix}a(\theta)&b(\theta)\\1&0\end{pmatrix}.
$$

[Stability](stability-of-a-numerical-method.md) requires its powers to be uniformly bounded in the time index and the mesh frequencies. If its two amplification roots have [modulus](modulus.md) at most one and their separation has a positive mesh-independent lower bound, the [eigenvectors](eigenvector.md) $(\xi_j,1)^T$ give a uniformly bounded [diagonalization of a matrix](diagonalization-of-a-matrix.md), proving stability. A repeated unit-modulus root of this companion [matrix](matrix.md) instead produces a [Jordan block](jordan-block.md) and linear growth in time. Thus checking only the [moduli](modulus.md) of the roots is insufficient.

**Table of contents**

- [Uniform stability of a shifted two-level advection scheme](uniform-stability-of-a-shifted-two-level-advection-scheme.md)

## ↑ Ancestors (8)

1. [von Neumann stability analysis](von-neumann-stability-analysis.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/4/b/solution.md)
