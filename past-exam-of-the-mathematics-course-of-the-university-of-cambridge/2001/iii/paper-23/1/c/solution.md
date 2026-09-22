<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Risk aversion](../../../../../../risk-aversion.md) means that a sure mean is preferred to the corresponding risky [portfolio wealth](../../../../../../portfolio-wealth.md). An increasing [concave](../../../../../../concave-function.md) [utility function](../../../../../../utility-function-split.md), with $u'>0$ and $u''\le0$, has this property by the [Jensen inequality](../../../../../../jensen-s-inequality.md); [strictly concave](../../../../../../strictly-concave-function.md) utility gives strict preference for nondegenerate risks. Differentiating the [expected utility](../../../../../../expected-utility.md) from part (a) gives

$$
U'(x)=-p(g-r)u'(w_g)+(1-p)(r-b)u'(w_b),\qquad U''(x)=p(g-r)^2u''(w_g)+(1-p)(r-b)^2u''(w_b)\le0.
$$

An interior optimum therefore satisfies

$$
\boxed{p(g-r)u'(w_g)=(1-p)(r-b)u'(w_b).}
$$

This balances the expected loss of [marginal utility](../../../../../../marginal-utility.md) in the good state against its expected gain in the bad state. The borrowing constraint also requires checking the endpoints: $x_*=0$ if $U'(0)\le0$, while $x_*=T$ would require $U'(T)\ge0$. At $x=T$ both state wealths equal $T(1+r)$, so

$$
U'(T)=[r-pg-(1-p)b]u'(T(1+r))<0.
$$

Hence an optimum never puts all wealth into deposits. If $U'(0)>0$, continuity and the displayed endpoint sign give an interior root, and [concavity](../../../../../../concave-function.md) makes every such root globally optimal. Under [strict concavity](../../../../../../strict-concavity.md) it is unique.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
