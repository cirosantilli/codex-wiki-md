<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $s=\sigma_Y\sigma_Z$ and $W=YZ-\mathbb E(YZ)$. The variables $Y$ and $Z$ need not be [independent random variables](../../../../../../independent-random-variables.md). Part (d) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) imply, for every integer $q\geq2$,

$$
\mathbb E|YZ|^q
\leq\bigl(\mathbb E|Y|^{2q}\mathbb E|Z|^{2q}\bigr)^{1/2}
\leq2^{q+1}q!s^q.
$$

Also $|\mathbb E(YZ)|\leq s$ by Cauchy-Schwarz, because $\mathbb EY^2\leq\sigma_Y^2$ and $\mathbb EZ^2\leq\sigma_Z^2$. Thus $\mathbb EW^2=\operatorname{Var}(YZ)\leq16s^2$, and, for $q\geq3$,

$$
\mathbb EW_+^q
\leq2^{q-1}\left(\mathbb E|YZ|^q+|\mathbb E(YZ)|^q\right)
\leq2^{2q+1}q!s^q
=\frac{q!}{2}(64s^2)(4s)^{q-2}.
$$

Part (c) shows that $W$ is [sub-Gamma in the right tail](../../../../../../sub-gamma-random-variable-in-the-right-tail.md) with variance parameter $64s^2$ and scale parameter $4s$.

If $\mathbb E(YZ)\geq0$, then $W_+\leq(YZ)_+\leq|YZ|$. Consequently

$$
\mathbb EW_+^q\leq2^{q+1}q!s^q
=\frac{q!}{2}(16s^2)(2s)^{q-2},
$$

while $\mathbb EW^2\leq16s^2$. Another application of part (c) gives the improved variance parameter $16\sigma_Y^2\sigma_Z^2$ and scale parameter $2\sigma_Y\sigma_Z$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
