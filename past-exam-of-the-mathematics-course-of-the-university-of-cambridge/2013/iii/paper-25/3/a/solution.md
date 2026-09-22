<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $t_j=j2^{-n}$ and $\Delta_j=X_{t_{j+1}}-X_{t_j}$. Telescoping $X_{t_{j+1}}^2-X_{t_j}^2=2X_{t_j}\Delta_j+\Delta_j^2$ gives

$$
M_1^{(n)}=\sum_{j=0}^{2^n-1}X_{t_j}\Delta_j.
$$

The [martingale transform](../../../../../../martingale-transform.md) summands are orthogonal in $L^2$: for an earlier summand, conditioning on the sigma-algebra at the start of the later increment makes the cross expectation zero. Hence

$$
\mathbb E(M_1^{(n)})^2=\sum_j\mathbb E[X_{t_j}^2\Delta_j^2]\le C^2\sum_j\mathbb E\Delta_j^2.
$$

The [martingale](../../../../../../martingale-split.md) increments themselves are also orthogonal. Since $X_0=0$, their variance sum equals $\mathbb E X_1^2\le C^2$. Therefore

$$
\boxed{\mathbb E(M_1^{(n)})^2\le C^4.}
$$

Only discrete martingale orthogonality is used here; no pre-existing [quadratic variation](../../../../../../quadratic-variation.md) calculation is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
