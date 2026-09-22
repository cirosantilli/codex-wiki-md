<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) convention $\iota_{X_t}\omega=dH_t$, which is forced by the sign of the formula in this part. This is the opposite of the default sign in the linked general article. Since $d\lambda=-\omega$, [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) gives

$$
\mathcal L_{X_t}\lambda
=d(\iota_{X_t}\lambda)+\iota_{X_t}d\lambda
=d(\iota_{X_t}\lambda-H_t).
$$

Differentiate the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) along the [smooth isotopy](../../../../../../smooth-isotopy.md) and integrate from $0$ to $t$:

$$
\begin{aligned}
\rho_t^*\lambda-\lambda
&=\int_0^t\rho_s^*\mathcal L_{X_s}\lambda\,ds\\
&=d\int_0^t(\iota_{X_s}\lambda-H_s)\circ\rho_s\,ds.
\end{aligned}
$$

Thus the required [exact differential form](../../../../../../exact-differential-form.md) has the explicit primitive

$$
\boxed{F_t=\int_0^t(\iota_{X_s}\lambda-H_s)\circ\rho_s\,ds,\qquad\rho_t^*\lambda-\lambda=dF_t.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 140](../../../paper-140-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
