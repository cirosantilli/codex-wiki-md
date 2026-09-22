<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [filtration on a group](../../../../../filtration-on-a-group.md) is a function $\omega:G\to\mathbb R\cup\{\infty\}$ satisfying

$$
\omega(xy^{-1})\geq\min\{\omega(x),\omega(y)\},
\qquad
\omega([x,y])\geq\omega(x)+\omega(y).
$$

It is a [p-valuation](../../../../../p-valuation.md) when it is separated and, for $x\ne1$,

$$
\omega(x)>\frac1{p-1},
\qquad
\omega(x^p)=\omega(x)+1.
$$

Let $p$ be odd and let

$$
G=\ker\bigl(\operatorname{GL}_2(\mathbb Z_p)\to\operatorname{GL}_2(\mathbb F_p)\bigr)
=1+pM_2(\mathbb Z_p).
$$

For $g=1+A\ne1$, define $\omega(g)=\min_{i,j}v_p(A_{ij})$. Matrix multiplication and the identity

$$
[1+A,1+B]-1=(1+A)^{-1}(1+B)^{-1}(AB-BA)
$$

give the two filtration inequalities. Since $\omega(g)\geq1>1/(p-1)$, only the p-power condition remains. The [binomial theorem](../../../../../binomial-theorem.md) gives

$$
(1+A)^p-1=pA+\sum_{i=2}^{p-1}\binom piA^i+A^p.
$$

The first term has valuation $1+\omega(g)$, while every other term has strictly larger valuation because $p$ is odd and $\omega(g)\geq1$. Hence $\omega(g^p)=\omega(g)+1$, so this is a p-valuation.

Finally, if $\omega_1,\omega_2$ are p-valuations, put $\omega=\min(\omega_1,\omega_2)$. Taking minima preserves both filtration inequalities and the strict lower bound, while

$$
\omega(g^p)=\min_i\bigl(\omega_i(g)+1\bigr)=\omega(g)+1.
$$

If $\omega(g)=\infty$, both original valuations force $g=1$. Therefore **the pointwise minimum of two p-valuations is again a p-valuation**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 145](../../paper-145-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
