<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Taking $x=y=a$ in (c) and using that $B_t$ has no atom at $a$ gives

$$
\mathbb P(T_a\leq t)=\mathbb P(S_t\geq a)=2\mathbb P(B_t\geq a)
=2\left(1-\Phi\left(\frac a{\sqrt t}\right)\right),\qquad t>0.
$$

This is the [distribution function](../../../../../../cumulative-distribution-function.md) of the [Brownian first-passage time](../../../../../../brownian-first-passage-time.md); (b) ensures that it is a proper [probability distribution](../../../../../../probability-distribution.md). Comparing these [distribution functions](../../../../../../cumulative-distribution-function.md) gives the [Brownian scaling](../../../../../../brownian-scaling.md) identity $T_{ca}\overset d=c^2T_a$ for $c>0$.

For an integer $n\geq1$, set $T_0=0$ and successively hit the levels $a,2a,\ldots,na$. The [Strong Markov property](../../../../../../strong-markov-property.md) at these finite [stopping times](../../../../../../stopping-time.md) and spatial translation imply that

$$
T_a-T_0,\ T_{2a}-T_a,\ldots,T_{na}-T_{(n-1)a}
$$

are [independent random variables](../../../../../../independent-random-variables.md), each with the [probability distribution](../../../../../../probability-distribution.md) of $T_a$. Thus, for [independent](../../../../../../independent-random-variables.md) copies $T_a^{(j)}$,

$$
T_a^{(1)}+\cdots+T_a^{(n)}\overset d=T_{na}\overset d=n^2T_a.
$$

Therefore

$$
\boxed{\frac{T_a^{(1)}+\cdots+T_a^{(n)}}{n^2}\overset d=T_a,\qquad \alpha=\frac12.}
$$

The paper's definition is the [strictly stable distribution](../../../../../../strictly-stable-distribution.md) convention, with no centering term, a special case of a [stable distribution](../../../../../../stable-distribution.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
