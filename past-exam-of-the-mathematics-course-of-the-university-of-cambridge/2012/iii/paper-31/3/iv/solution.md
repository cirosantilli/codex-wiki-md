<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $\eta=\operatorname{Im}z>0$. For a real [eigenvalue](../../../../../../eigenvalue.md) $\lambda$,

$$
\operatorname{Im}\frac1{\lambda-z}=\frac{\eta}{(\lambda-\operatorname{Re}z)^2+\eta^2}>0.
$$

The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) therefore gives $\operatorname{Im}g>0$ and $\operatorname{Im}q_i\geq0$, since $q_i$ is a sum of $(\lambda-z)^{-1}$ with nonnegative coefficients given by squared eigenvector coordinates of $x_i$. This is the [positive imaginary part of a Stieltjes matrix resolvent](../../../../../../positive-imaginary-part-of-a-stieltjes-matrix-resolvent.md). Hence

$$
|z+g|\geq\eta,\qquad |z+q_i|\geq\eta.
$$

Apply the [triangle inequality](../../../../../../triangle-inequality.md) to the identity above, and add and subtract the minor trace:

$$
\begin{aligned}|\varepsilon_N(z)|&\leq\frac1{\eta^2N}\sum_{i=1}^N|q_i-g|\\&\leq\frac1{\eta^2N}\sum_{i=1}^N|q_i-g^{(i)}|+\frac1{\eta^2N}\sum_{i=1}^N|g^{(i)}-g|.
\end{aligned}
$$

The allowed [principal minor resolvent trace bound](../../../../../../principal-minor-resolvent-trace-bound.md), with the printed $N$ normalization, bounds the second average by $c/(\eta N)$. Thus the explicit conclusion is

$$
\boxed{|\varepsilon_N(z)|\leq\frac1{(\operatorname{Im}z)^2N}\sum_{i=1}^N\left|x_i^T(X_N^{(i)}-zI)^{-1}x_i-g_N^{(i)}(z)\right|+\frac{c}{(\operatorname{Im}z)^3N}.}
$$

In particular, the final term is $O((\operatorname{Im}z)^{-3}N^{-1})$ with a constant independent of $N$. The upper-half-plane restriction gives the displayed positive denominators; in the lower half-plane the analogous bound uses $|\operatorname{Im}z|$.

The chosen centering also has a probabilistic meaning. The column vector $x_i$ is independent of the minor, has mean zero and coordinate [variance](../../../../../../variance-split.md) $1/N$, so its [conditional expectation](../../../../../../conditional-expectation.md) satisfies

$$
\mathbb E[q_i\mid X_N^{(i)}]=\frac1N\operatorname{Tr}G^{(i)}=g_N^{(i)}.
$$

This explains why the bound isolates fluctuations of a [quadratic form](../../../../../../quadratic-form.md) around the minor trace. Mean centering alone is not a concentration estimate; no unrequested limiting assertion is being assumed.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
