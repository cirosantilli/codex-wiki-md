<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\beta=1/(k_BT)$ and use the two [spin](../../../../spin.md) values $+1,-1$ as row and column labels. Define the [spin-chain transfer matrix](../../../../transfer-matrix-for-a-classical-spin-chain.md)

$$
W_{st}=e^{-\beta E_0(s,t)},\qquad s,t\in\{+1,-1\}.
$$

It is a real [symmetric matrix](../../../../symmetric-matrix.md) because $E_0(s,t)=E_0(t,s)$; every entry is strictly positive for finite bond [energies](../../../../energy-split.md) at $T>0$. The [Boltzmann factor](../../../../boltzmann-factor.md) of a [spin](../../../../spin.md) configuration factorizes into the product $W_{\sigma_1\sigma_2}\cdots W_{\sigma_L\sigma_1}$. Summing the intermediate [spin](../../../../spin.md) labels is exactly [matrix multiplication](../../../../matrix-multiplication.md), and the final closure imposes [periodic boundary conditions](../../../../periodic-boundary-conditions.md). Thus

$$
\boxed{Z_L=\sum_{\sigma_1,\ldots,\sigma_L}\prod_{j=1}^LW_{\sigma_j\sigma_{j+1}}=\operatorname{Tr}W^L.}
$$

Writing $W=\left(\begin{smallmatrix}a&b\\b&d\end{smallmatrix}\right)$, its [eigenvalues](../../../../eigenvalue.md) are

$$
\lambda_\pm=\frac{a+d\pm\sqrt{(a-d)^2+4b^2}}2,
\qquad \boxed{Z_L=\lambda_+^L+\lambda_-^L.}
$$

A positive-entry [matrix](../../../../matrix.md) need not have two positive [eigenvalues](../../../../eigenvalue.md); $\lambda_-$ can be negative. The [Perron–Frobenius theorem](../../../../perron-frobenius-theorem.md) ensures $\lambda_+>|\lambda_-|$ here. Therefore the [Helmholtz free energy](../../../../helmholtz-free-energy.md) is $F_L=-k_BT\ln Z_L$, and its value per [spin](../../../../spin.md) in the [thermodynamic limit](../../../../thermodynamic-limit.md) is $-k_BT\ln\lambda_+$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
