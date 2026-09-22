<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The interpolated exponent is strictly between $p_0$ and $p_1$. Apply [Hölder's inequality](../../../../../../holder-s-inequality.md) to $|f|^p=|f|^{p(1-\theta)}|f|^{p\theta}$ with [conjugate exponents](../../../../../../conjugate-exponents.md) $p_0/[p(1-\theta)]$ and $p_1/(p\theta)$. Their reciprocals sum to one, so

$$
\boxed{\|f\|_p\leq\|f\|_{p_0}^{1-\theta}\|f\|_{p_1}^{\theta}.}
$$

This gives $L^{p_0}\cap L^{p_1}\subseteq L^p$.

For the other inclusion take any $a>0$ and use the [threshold decomposition between Lp spaces](../../../../../../threshold-decomposition-between-lp-spaces.md)

$$
g=f\mathbf1_{\{|f|>a\}},\qquad
h=f\mathbf1_{\{|f|\leq a\}}.
$$

Because $p_0-p<0<p_1-p$,

$$
\int|g|^{p_0}\leq a^{p_0-p}\int|f|^p,\qquad
\int|h|^{p_1}\leq a^{p_1-p}\int|f|^p.
$$

Thus $g\in L^{p_0}$, $h\in L^{p_1}$ and $f=g+h$, proving $L^p\subseteq L^{p_0}+L^{p_1}$. Raising the two [norm](../../../../../../norm.md) bounds to powers $1-\theta$ and $\theta$ gives a power of $a$ equal to

$$
(1-\theta)(1-p/p_0)+\theta(1-p/p_1)=0,
$$

and a power of $\|f\|_p$ equal to one. Hence

$$
\boxed{\|g\|_{p_0}^{1-\theta}\|h\|_{p_1}^{\theta}\leq\|f\|_p.}
$$

For later use, choose $a=\|f\|_p$ when $f\ne0$. Each endpoint [norm](../../../../../../norm.md) is then at most $\|f\|_p$, so $\|f\|_{L^{p_0}+L^{p_1}}\leq2\|f\|_p$ for the [sum of Lp spaces](../../../../../../sum-of-lp-spaces.md) [norm](../../../../../../norm.md). If $f=0$, take $g=h=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
