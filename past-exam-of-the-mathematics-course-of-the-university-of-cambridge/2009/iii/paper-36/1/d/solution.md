<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With a uniform [Beta distribution](../../../../../../beta-distribution.md) [prior](../../../../../../prior-probability.md), the [posterior predictive distribution](../../../../../../posterior-predictive-distribution.md) for another batch of the same size is

$$
p(y\mid x)=\binom my
\frac{\mathrm B(x+y+1,2m-x-y+1)}{\mathrm B(x+1,m-x+1)}.
$$

But $\mathrm B(x+1,m-x+1)=1/[(m+1)\binom mx]$. Hence

$$
\boxed{p(y\mid x)=(m+1)\binom mx\binom my\,
\mathrm B(x+y+1,2m-x-y+1)=p(x\mid y).}
$$

The displayed expression is symmetric in $x,y$. This is the [uniform-count predictive property](../../../../../../uniform-count-predictive-property.md): the joint batch counts are exchangeable and both marginal counts are uniform. Conditional reversal is not a general property of arbitrary priors; it holds here because those marginal probabilities coincide.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
