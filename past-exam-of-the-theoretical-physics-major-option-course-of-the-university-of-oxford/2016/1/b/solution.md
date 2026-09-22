<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each pair of adjacent [spins](../../../../spin.md), define the [transfer matrix for a classical spin chain](../../../../transfer-matrix-for-a-classical-spin-chain.md) by $T_{ss'}=e^{-\beta E_0(s,s')}$. Multiplying its entries gives the [Boltzmann factor](../../../../boltzmann-factor.md) of a whole configuration. The [periodic boundary condition](../../../../periodic-boundary-conditions.md) identifies the last index with the first, so

$$
Z_L=\sum_{\sigma_1,\ldots,\sigma_L}T_{\sigma_1\sigma_2}\cdots T_{\sigma_L\sigma_1}
=\boxed{\operatorname{Tr}T^L=\sum_\alpha\lambda_\alpha^L.}
$$

The assumed interchange symmetry of $E_0$ makes $T$ a real [symmetric matrix](../../../../symmetric-matrix.md), hence it has an orthonormal [eigenbasis](../../../../eigenbasis.md). At finite positive [temperature](../../../../temperature-split.md), every matrix entry is strictly positive, so the [Perron–Frobenius theorem](../../../../perron-frobenius-theorem.md) supplies a unique positive largest [eigenvalue](../../../../eigenvalue.md) $\lambda_+$, larger in modulus than every other one. Therefore $L^{-1}\log Z_L\to\log\lambda_+$.

Local observables become matrix insertions. For example, with $S_{ss'}=s\delta_{ss'}$,

$$
\langle\sigma_1\rangle=\frac{\operatorname{Tr}(ST^L)}{\operatorname{Tr}T^L},
\qquad
\langle\sigma_1\sigma_{1+r}\rangle=\frac{\operatorname{Tr}(ST^rST^{L-r})}{Z_L}.
$$

Thus [partition functions](../../../../canonical-partition-function.md) and [correlation functions](../../../../correlation-function.md) reduce to a fixed-dimensional [eigenvalue](../../../../eigenvalue.md) problem, rather than a sum over exponentially many [microstates](../../../../microstate.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
