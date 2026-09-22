<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The original PDF shows the chain $A\to C\to B$, not a collider. Its [Bayesian network](../../../../../../../bayesian-network.md) factorization is $p(a,b,c)=p(a)p(c\mid a)p(b\mid c)$. For any $c$ with positive marginal [probability](../../../../../../../probability.md),

$$
p(a,b\mid c)=\frac{p(a)p(c\mid a)p(b\mid c)}{p(c)}=p(a\mid c)p(b\mid c).
$$

Integrating or summing over $a$ also gives the same conditional marginal $p(b\mid c)$. Thus

$$
\boxed{A\mathrel{\perp\!\!\!\perp}B\mid C.}
$$

This is [conditional independence](../../../../../../../conditional-independence.md); the graph does not generally imply marginal [independence](../../../../../../../independent-random-variables.md), since summing $p(a)p(c\mid a)p(b\mid c)$ over $c$ can transmit dependence from $A$ to $B$. Special [statistical parameter](../../../../../../../statistical-parameter.md) choices can make marginal [independence](../../../../../../../independent-random-variables.md) hold as well, so the claim is that only the conditional statement is guaranteed by the graph. [Conditional distributions](../../../../../../../conditional-distribution.md) on null values of $C$ are immaterial to this assertion.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
