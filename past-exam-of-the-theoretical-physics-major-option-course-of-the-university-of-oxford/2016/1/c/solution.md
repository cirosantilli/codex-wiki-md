<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [sawtooth Ising chain](../../../../sawtooth-ising-chain.md), each apex [spin](../../../../spin.md) occurs in only one triangle. Put $K=\beta J$. Summing that [spin](../../../../spin.md) first gives the effective [transfer matrix](../../../../transfer-matrix.md)

$$
T_{ss'}=\sum_{t=\pm1}\exp\{K[ss'+t(s+s')]\}
=2e^{Kss'}\cosh[K(s+s')].
$$

In the ordered basis $s=+1,-1$ this is

$$
T=\begin{pmatrix}2e^K\cosh2K&2e^{-K}\\2e^{-K}&2e^K\cosh2K\end{pmatrix}.
$$

Its symmetric and antisymmetric [eigenvectors](../../../../eigenvector.md) are $(1,1)/\sqrt2$ and $(1,-1)/\sqrt2$, with [eigenvalues](../../../../eigenvalue.md)

$$
\lambda_+=e^{3K}+3e^{-K},\qquad\lambda_-=e^{3K}-e^{-K}.
$$

Consequently

$$
\boxed{Z_L=(e^{3K}+3e^{-K})^L+(e^{3K}-e^{-K})^L,\qquad
f_\infty=-\frac{k_BT}{2}\log(e^{3K}+3e^{-K}).}
$$

At $J=0$, the result is $Z_L=4^L$, correctly counting $2L$ independent [Ising spins](../../../../ising-spin-variable.md). As $T\to0$, $f_\infty\to-3J/2$, the energy of three satisfied ferromagnetic bonds per two sites.

The printed summand lacks grouping brackets. The result above uses the translation-invariant common-$J$ interpretation. If base and apex bonds instead have independent couplings $J_b,J_a$, the same derivation gives $\lambda_\pm=2e^{\beta J_b}\cosh(2\beta J_a)\pm2e^{-\beta J_b}$; specifying those couplings is essential before giving a different answer.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
