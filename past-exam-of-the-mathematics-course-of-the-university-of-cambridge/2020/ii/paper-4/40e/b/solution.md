<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand $a,u,f$ in the two-dimensional [Fourier basis](../../../../../../fourier-basis.md). Applying the derivative and product rules from part (a), the $(m,n)$ coefficient of the equation is

$$
-\pi^2\sum_{p,q\in\mathbb Z}
(mp+nq)\widehat a_{m-p,n-q}\widehat u_{p,q}
=\widehat f_{m,n}.
$$

The normalization and compatibility conditions are

$$
\boxed{\widehat u_{0,0}=0,
\qquad \widehat f_{0,0}=0}.
$$

Thus, on $\mathbb Z^2\setminus\{(0,0)\}$, the infinite [Fourier spectral method](../../../../../../fourier-spectral-method.md) system is

$$
\boxed{\sum_{p,q}A_{(m,n),(p,q)}\widehat u_{p,q}=-\widehat f_{m,n}},
\qquad
\boxed{A_{(m,n),(p,q)}=\pi^2(mp+nq)\widehat a_{m-p,n-q}}.
$$

For a square [spectral truncation](../../../../../../spectral-truncation.md), choose

$$
\Lambda_N=\{(m,n):|m|,|n|\leq N\}\setminus\{(0,0)\},
$$

retain equations and unknowns indexed by $\Lambda_N$, and set omitted coefficients to zero. This is the [Fourier–Galerkin method](../../../../../../fourier-galerkin-method.md): it projects the residual onto the retained [Fourier modes](../../../../../../fourier-mode.md). Other finite mode sets may be used in the same way.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
