<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At time zero, $\Upsilon_0(z)=\operatorname{Im}z$. Compactness of $K\subset\mathbb H$ gives

$$
\epsilon_0=\min_{z\in K}\operatorname{Im}z>0.
$$

Also $M_0(z)$ is uniformly bounded above on $K$. On

$$
E_\epsilon=\{\tau_\epsilon<\infty, S_{\tau_\epsilon}\geq1/2\},
$$

one has $M_{\tau_\epsilon}\geq\epsilon^{-p}2^{-q}$. Optional stopping, [Fatou lemma](../../../../../../../fatou-s-lemma.md), and the assumed conditional angular estimate give

$$
\sup_{z\in K}M_0(z)
\geq\mathbb E[M_{\tau_\epsilon};E_\epsilon]
\geq\epsilon^{-p}2^{-q}c_1
\mathbb P(\tau_\epsilon<\infty).
$$

Thus

$$
\boxed{\mathbb P_z(\tau_\epsilon<\infty)
\leq C_K\epsilon^{(8-\kappa)/8}.}
$$

The exponent $(8-\kappa)/\kappa$ requested in the question does not follow and is false as written. The [SLE Green-function estimate](../../../../../../../sle-green-function-estimate.md) gives probability comparable to $\epsilon^{1-\kappa/8}$, confirming that the denominator in the requested exponent should be $8$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
