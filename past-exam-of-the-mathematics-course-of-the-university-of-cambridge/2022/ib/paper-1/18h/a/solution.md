<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
d_t=\#\{i:X_i=t\},
\qquad
r_t=\#\{i:X_i\geq t\}
=n-\sum_{s<t}d_s.
$$

Thus $d_t$ patients recover during month $t$, while $r_t-d_t$ survive that month without recovery. The [likelihood function](../../../../../../likelihood-function.md) is

$$
\boxed{
L(q_1,\ldots,q_T)
=\prod_{t=1}^T
q_t^{d_t}(1-q_t)^{r_t-d_t}}.
$$

The independent $\operatorname{Beta}(T,1)$ prior densities are proportional to $q_t^{T-1}$. [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md) therefore leaves the coordinates posteriorly independent, with

$$
\boxed{
q_t\mid X
\sim\operatorname{Beta}
\bigl(T+d_t,\ 1+r_t-d_t\bigr)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
