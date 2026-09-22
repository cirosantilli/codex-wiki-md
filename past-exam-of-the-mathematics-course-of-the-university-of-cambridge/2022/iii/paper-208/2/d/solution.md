<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\ell^*$ be a maximizing index for the original sample. Since $Z_i'$ is at least the value of its $\ell^*$th linear form,

$$
(Z-Z_i')_+
\leq\{(X_i-X_i')A_{i,\ell^*}\}_+,
$$

and hence

$$
(Z-Z_i')_+^2
\leq(X_i-X_i')^2A_{i,\ell^*}^2.
$$

The one-sided replacement form of the [Efron–Stein inequality](../../../../../../efron-stein-inequality.md) is

$$
\operatorname{Var}(Z)
\leq\sum_i\mathbb E(Z-Z_i')_+^2.
$$

For independent uniform signs, $\mathbb E[(X_i-X_i')^2\mid X]=2$. It follows that

$$
\operatorname{Var}(Z)
\leq2\mathbb E\sum_iA_{i,\ell^*}^2
\leq2\max_{1\leq\ell\leq m}\sum_iA_{i,\ell}^2.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
