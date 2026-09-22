<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stated kernel is the [Brownian bridge covariance kernel](../../../../../../brownian-bridge-covariance-kernel.md). Its eigenvalue equation is

$$
\lambda\phi(s)=\int_0^1\{\min(s,t)-st\}\phi(t)\,dt.
$$

The right-hand side vanishes at $s=0$ and $s=1$, and differentiating it twice gives

$$
\lambda\phi''(s)=-\phi(s),
\qquad
\phi(0)=\phi(1)=0.
$$

Thus the normalized eigenfunctions and eigenvalues are

$$
\phi_k(t)=\sqrt2\sin(k\pi t),
\qquad
\lambda_k=\frac1{k^2\pi^2},
\qquad k\geq1.
$$

The [Karhunen–Loève expansion](../../../../../../karhunen-loeve-expansion.md) is consequently

$$
X(t)=\mu(t)+\sum_{k=1}^{\infty}\xi_k\sqrt2\sin(k\pi t)
=\mu(t)+\sum_{k=1}^{\infty}\frac{Z_k}{k\pi}\sqrt2\sin(k\pi t),
$$

with convergence in $L^2(\Omega;L^2[0,1])$, where $\mathbb EZ_k=0$ and $\mathbb E[Z_jZ_k]=\mathbf1_{\{j=k\}}$. Covariance alone does not imply that the $Z_k$ are independent or normal; they are independent standard normal variables when $X$ is Gaussian.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
