<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Share each on-site field energy equally between its two neighboring bonds. In the ordered basis $\sigma=+1,-1$, the symmetric [transfer matrix for a classical spin chain](../../../../transfer-matrix-for-a-classical-spin-chain.md) is

$$
\boxed{T_{ss'}=e^{-\beta Jss'+\frac12\beta B(s+s')},\qquad
T=\begin{pmatrix}e^{-K+h}&e^K\\e^K&e^{-K-h}\end{pmatrix},\quad K=\beta J,\ h=\beta B.}
$$

The product $\prod_jT_{\sigma_j\sigma_{j+1}}$ recovers each bond and each field term once. Summing the periodic indices closes a [trace](../../../../matrix-trace.md), giving $Z_N=\operatorname{Tr}T^N$. The two [eigenvalues](../../../../eigenvalue.md) are

$$
\boxed{\lambda_\pm=e^{-K}\cosh h
\pm\sqrt{e^{-2K}\sinh^2h+e^{2K}},\qquad Z_N=\lambda_+^N+\lambda_-^N.}
$$

The square-root argument is positive. Moreover $\det T=e^{-2K}-e^{2K}<0$, so $\lambda_-<0$ even at nonzero field. Its sign must not be discarded merely because all matrix entries are positive. The [Perron–Frobenius theorem](../../../../perron-frobenius-theorem.md) ensures that the positive [eigenvalue](../../../../eigenvalue.md) $\lambda_+$ has the larger modulus, and the infinite-chain [free energy](../../../../thermodynamic-free-energy.md) is $f_\infty=-\beta^{-1}\log\lambda_+$. For even $N$, both terms in the finite-size [partition function](../../../../canonical-partition-function.md) are positive.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
