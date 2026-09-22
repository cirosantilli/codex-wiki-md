<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a sufficiently regular [Itô diffusion](../../../../../../ito-diffusion.md) with $D=\sigma\sigma^T/2$, a density $\pi$ is stationary if and only if it solves the stationary [Fokker-Planck equation](../../../../../../fokker-planck-equation.md)

$$
\nabla\mathbin\cdot\left(b\pi-\nabla\mathbin\cdot(D\pi)\right)=0,
$$

with integrable [Fokker-Planck probability current](../../../../../../fokker-planck-probability-current.md) and boundary conditions that make its outward flux vanish. Here $(\nabla\mathbin\cdot(D\pi))_i=\sum_j\partial_j(D_{ij}\pi)$.

For the displayed parametrization, assume

$$
\pi(x)=Z^{-1}e^{-H(x)},
$$

where $Z<\infty$, that $D(x)$ is symmetric positive semidefinite, and that $Q(x)$ is antisymmetric. Substituting $\nabla\pi=-\pi\nabla H$ and the stated $\Gamma$ into the probability current cancels all $D$ terms. The remaining divergence is

$$
-\sum_{i,j}\partial_i\partial_j(Q_{ij}\pi)=0,
$$

because the second derivatives are symmetric in $i,j$ whereas $Q_{ij}=-Q_{ji}$. Thus these conditions, together with the boundary and regularity assumptions, imply stationarity. More generally, the divergence equation above is the exact necessary and sufficient condition; within this construction, $\pi\propto e^{-H}$ and antisymmetric $Q$ are the standard way to satisfy it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
