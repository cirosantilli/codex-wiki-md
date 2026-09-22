<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work from time one; a finite initial prefix does not affect convergence. Fix a positive integer $a$, and use the [stopping time](../../../../../../stopping-time.md) $\tau_a$ and budget $A_n$ from part (b). Define

$$
Z_n^{(a)}=X_{n\wedge\tau_a}+a-U_{n\wedge\tau_a}.
$$

It is nonnegative. For each finite $n$, the stopped variable $X_{n\wedge\tau_a}$ is [integrable](../../../../../../integrability.md): it is bounded by the finite sum $X_1+\cdots+X_n$, and the budget is bounded by $a$.

The stopped increment of $X$ is

$$
X_{(n+1)\wedge\tau_a}-X_{n\wedge\tau_a}
=\mathbf1_{\{\tau_a>n\}}(X_{n+1}-X_n).
$$

Taking [conditional expectations](../../../../../../conditional-expectation.md), the assumed drift bound gives

$$
\mathbb E[X_{(n+1)\wedge\tau_a}\mid\mathcal F_n]
\leq X_{n\wedge\tau_a}+Y_n\mathbf1_{\{\tau_a>n\}}.
$$

The last term is bounded by $a$; no integrability assumption on the unlocalized $Y_n$ has been used. Its contribution is exactly cancelled by the budget decrement from part (b), giving

$$
\mathbb E[Z_{n+1}^{(a)}\mid\mathcal F_n]\leq Z_n^{(a)}.
$$

Thus $Z^{(a)}$ is an [integrable](../../../../../../integrability.md) nonnegative [supermartingale](../../../../../../supermartingale.md). By the [almost sure supermartingale convergence theorem](../../../../../../almost-sure-supermartingale-convergence-theorem.md) it has a finite almost-sure limit. The bounded decreasing budget $A_n$ has a finite pathwise limit as well, so $X_{n\wedge\tau_a}=Z_n^{(a)}-A_n$ converges to a finite limit [almost surely](../../../../../../almost-sure-convergence.md).

Take the intersection of these probability-one convergence events over all positive integers $a$. On the further probability-one event $\sum_{j\geq1}Y_j<\infty$, choose an integer $a$ strictly larger than that total. Then $\tau_a=\infty$, so the stopped sequence is the original one. Consequently

$$
\boxed{X_n\text{ converges almost surely to a finite limit}.}
$$

This proves [supermartingale convergence with summable adapted drift](../../../../../../supermartingale-convergence-with-summable-adapted-drift.md) under almost-sure summability alone; it does not require $\mathbb E\sum_jY_j<\infty$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
