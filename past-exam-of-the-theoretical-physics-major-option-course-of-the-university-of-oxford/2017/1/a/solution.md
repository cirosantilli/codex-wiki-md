<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\beta=(k_BT)^{-1}$ and label the two [spin values](../../../../spin.md) in the order $+1,-1$. Assign each bond its [Boltzmann weight](../../../../boltzmann-factor.md),

$$
V_{st}=e^{-\beta E_0(s,t)},\qquad
V=\begin{pmatrix}a&b\\b&d\end{pmatrix},\qquad s,t\in\{+1,-1\}.
$$

The [symmetry](../../../../symmetry-physics.md) of the [bond energy](../../../../energy-split.md) makes $V$ a [real symmetric matrix](../../../../symmetric-matrix.md). For a fixed configuration the product of successive [matrix](../../../../matrix.md) entries is its [Boltzmann weight](../../../../boltzmann-factor.md). Summing over all [spins](../../../../spin.md) and identifying the last index with the first therefore gives

$$
\boxed{Z_L=\sum_{\sigma_1,\ldots,\sigma_L}V_{\sigma_1\sigma_2}\cdots V_{\sigma_L\sigma_1}=\operatorname{tr}V^L=\lambda_+^L+\lambda_-^L,}
$$

where

$$
\lambda_\pm=\frac{a+d\pm\sqrt{(a-d)^2+4b^2}}2.
$$

This replaces a sum over $2^L$ configurations by the powers of a two-by-two [matrix](../../../../matrix.md). For finite bond [energies](../../../../energy-split.md) at $T>0$, every [matrix](../../../../matrix.md) entry is positive, so the [Perron–Frobenius theorem](../../../../perron-frobenius-theorem.md) gives $\lambda_+>0$ and $|\lambda_-|<\lambda_+$. Hence the [Helmholtz free energy](../../../../helmholtz-free-energy.md) per [spin](../../../../spin.md) tends to $-k_BT\log\lambda_+$. A diagonal local [observable](../../../../observable.md) $O$ can be inserted at one site: $\langle O_1\rangle=\operatorname{tr}(OV^L)/Z_L$. Its limiting average is the [expectation](../../../../expected-value-split.md) in the [normalized](../../../../normalization.md) [eigenvector](../../../../eigenvector.md) of $\lambda_+$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
