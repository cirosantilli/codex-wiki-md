<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $W^-_t=B_{h-t}-B_h$ and $W^+_t=B_{h+t}-B_h$, $0\leq t\leq h$, with $h=1/2$. Both start at zero and are continuous. Increments of $W^-$ over consecutive disjoint time intervals are negatives of Brownian increments over corresponding disjoint past intervals, read in reverse order. They are independent centered [normal random variables](../../../../../../gaussian-random-variable.md) with covariance equal to the interval length times the identity. The same properties hold for $W^+$ using future increments. Every past increment is independent of all the future increments after deterministic time $h$, so the two whole processes are independent, by finite-dimensional [independence](../../../../../../independent-random-variables.md) and generation by rational-time evaluations. They are the [independent Brownian arms at a deterministic time](../../../../../../independent-brownian-arms-at-a-deterministic-time.md).

Let $R^-$ and $R^+$ be their ranges. Pathwise,

$$
R^-=A_1-B_h,\qquad R^+=A_2-B_h,\qquad
\lambda(R^-\cap R^+)=\lambda(A_1\cap A_2).
$$

Although $W^-$ need not be independent of $B_h$, this last equality uses only translation invariance of [Lebesgue measure](../../../../../../lebesgue-measure.md). Put $p(y)=\mathbb P(T_y\leq h)$ for a standard [Brownian motion](../../../../../../brownian-motion-split.md) started at zero. [Independence](../../../../../../independent-random-variables.md) of the centered processes and [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
0=\mathbb E\lambda(R^-\cap R^+)=\int_{\mathbb R^2}\mathbb P(y\in R^-)\mathbb P(y\in R^+)\,dy
=\boxed{\int_{\mathbb R^2}p(y)^2\,dy}.
$$

Since $p\geq0$, it follows that $p(y)=0$ for Lebesgue-almost every $y$. Therefore

$$
\mathbb E\lambda(A_1)=\int_{\mathbb R^2}p(y)\,dy=0.
$$

The scaling relation in part (a) gives $\mathbb E\lambda(R)=2\mathbb E\lambda(A_1)=0$. A nonnegative random variable of [expectation](../../../../../../expected-value.md) zero vanishes almost surely, proving the [area of a planar Brownian path](../../../../../../area-of-a-planar-brownian-path.md) result

$$
\boxed{\lambda(\{B_t:0\leq t\leq1\})=0\quad\text{almost surely}.}
$$

The integral argument establishes the needed almost-everywhere spatial assertion; it does not require a prior theorem that individual points are polar.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
