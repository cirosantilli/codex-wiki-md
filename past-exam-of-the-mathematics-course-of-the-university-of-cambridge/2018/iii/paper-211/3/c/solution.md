<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Iterating the [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md) gives

$$
X_j=a^jx+b\sum_{\ell=0}^{j-1}a^\ell+\sum_{r=1}^ja^{j-r}\xi_r.
$$

For $q_r=\sum_{j=r}^t\theta_ja^{j-r}$, regrouping the sum of the exponents gives

$$
\sum_{j=1}^t\theta_jX_j=x\sum_{j=1}^t\theta_ja^j+b\sum_{r=1}^tq_r+\sum_{r=1}^tq_r\xi_r.
$$

The [independent](../../../../../../independent-random-variables.md) innovations factorize the [moment-generating function](../../../../../../moment-generating-function.md). Consequently

$$
\boxed{A_t=\sum_{j=1}^t\theta_ja^j,\qquad B_t=\sum_{r=1}^t\bigl(bq_r+\psi(q_r)\bigr),\qquad q_r=\sum_{j=r}^t\theta_ja^{j-r}.}
$$

Finite sums avoid a division by $a-1$, so these formulas include $a=0$ and $a=1$; zeroth powers in these sums are $1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
