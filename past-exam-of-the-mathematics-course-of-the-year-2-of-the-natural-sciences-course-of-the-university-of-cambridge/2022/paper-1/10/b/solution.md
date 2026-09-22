<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the normalized [eigenfunctions](../../../../../eigenfunction.md) and their [weighted inner product](../../../../../weighted-inner-product.md) $\int_a^bw\overline{\psi_m}\psi_n dx=\delta_{mn}$. [Orthogonality](../../../../../orthogonal-vectors.md) gives

$$
G[\widetilde\psi]=\sum_{n\geq0}|a_n|^2,\qquad F[\widetilde\psi]=\int_a^b\overline{\widetilde\psi}\,\mathcal L\widetilde\psi\,dx=\sum_{n\geq0}\lambda_n|a_n|^2.
$$

For complex trials, $F$ means the corresponding Hermitian [quadratic form](../../../../../quadratic-form-split.md) with $|\psi'|^2,|\psi|^2$; it agrees with the displayed functional on real trials. If $a_0\ne0$, division by $|a_0|^2$ yields

$$
\boxed{\Lambda[\widetilde\psi]=\frac{\lambda_0+\sum_{n\geq1}|b_n|^2\lambda_n}{1+\sum_{n\geq1}|b_n|^2},\qquad b_n=\frac{a_n}{a_0}.}
$$

Since $\lambda_n\geq\lambda_0$, this is at least $\lambda_0$. The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) therefore gives an upper bound from any admissible trial, improved by minimizing over trial parameters or enlarging the trial space. Equality holds when the trial is entirely in the lowest [eigenspace](../../../../../eigenspace.md).

The displayed ratio using $b_n$ presupposes $a_0\ne0$. If $a_0=0$, use the undivided quotient $\sum\lambda_n|a_n|^2/\sum|a_n|^2$ instead; the same upper-bound argument still applies. No ground-state coefficient can be divided out in that case.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
