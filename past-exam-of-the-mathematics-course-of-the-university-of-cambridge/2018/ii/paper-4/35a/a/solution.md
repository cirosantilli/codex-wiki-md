<h1 id="35a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expanding the trace in the spin basis gives

$$
\operatorname{Tr}(M^N)
=\sum_{s_1,\ldots,s_N}M_{s_1s_2}M_{s_2s_3}\cdots M_{s_Ns_1}
=\sum_{\{s_i\}}e^{-\beta H}=Z,
$$

so the [transfer matrix for the one-dimensional Ising model](../../../../../../transfer-matrix-for-the-one-dimensional-ising-model.md) reproduces the [partition function](../../../../../../canonical-partition-function.md).

In the ordered basis $s=+1,-1$,

$$
M=\begin{pmatrix}
e^{\beta(J+B)}&e^{-\beta J}\\
e^{-\beta J}&e^{\beta(J-B)}
\end{pmatrix}.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are

$$
\boxed{\lambda_\pm=e^{\beta J}\cosh(\beta B)
\pm\sqrt{e^{2\beta J}\sinh^2(\beta B)+e^{-2\beta J}}}.
$$

Since $\lambda_+>|\lambda_-|$ at every positive [temperature](../../../../../../temperature.md), the [thermodynamic limit](../../../../../../thermodynamic-limit.md) gives the [Helmholtz free energy](../../../../../../helmholtz-free-energy.md) per spin

$$
\boxed{f=-kT\log\lambda_+}.
$$

This is an [analytic function](../../../../../../space-of-holomorphic-functions.md) of $T$ and $B$ for $T>0$, so the one-dimensional short-range [Ising model](../../../../../../ising-model.md) has no finite-temperature [phase transition](../../../../../../phase-transition.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [35A](../../35a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
