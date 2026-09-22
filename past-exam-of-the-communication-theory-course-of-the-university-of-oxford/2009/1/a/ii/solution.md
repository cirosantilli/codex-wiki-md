<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [Gibbs inequality](../../../../../gibbs-inequality.md) to the [joint distribution](../../../../../joint-probability-distribution.md) and the product of its marginals. Restrict to the Cartesian product of their positive supports, so the reference probabilities are strictly positive as the supplied inequality requires. Expanding gives

$$
0\leq\sum_{x,y}p(x,y)\log_2\frac{p(x,y)}{p_X(x)p_Y(y)}
=H(X)-H(X\mid Y).
$$

This proves the second inequality. For the first, apply the same argument to the conditional [joint distribution](../../../../../joint-probability-distribution.md) of $(X,Z)$ for each $y$ with $p_Y(y)>0$, and average with those probabilities:

$$
0\leq\sum_y p_Y(y)I(X;Z\mid Y=y)
=H(X\mid Y)-H(X\mid Y,Z).
$$

Here the conditional support restriction again removes zero marginal probabilities. Thus

$$
\boxed{H(X\mid Y,Z)\leq H(X\mid Y)\leq H(X)}.
$$

The nonnegative differences are [conditional mutual information](../../../../../conditional-mutual-information.md) and [mutual information](../../../../../mutual-information.md), respectively.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
