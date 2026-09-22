<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $0<u<1$ define the generalized inverse, or [quantile function](../../../../../quantile-function.md), by

$$
Q(u)=\inf\{x\in\mathbb R:F(x)\geq u\}.
$$

It is finite because the [cumulative distribution function](../../../../../cumulative-distribution-function.md) tends to zero and one at the two infinities. Monotonicity and right continuity of $F$ give the key equivalence

$$
Q(u)\leq x\quad\Longleftrightarrow\quad u\leq F(x).
$$

For the forward implication, choose points in the defining set approaching its infimum from above. Right continuity gives $F(Q(u))\geq u$, and then monotonicity gives $F(x)\geq u$ whenever $Q(u)\leq x$. The reverse implication follows immediately because $x$ then belongs to the defining set. Consequently, for a continuous [uniform distribution](../../../../../continuous-uniform-distribution.md) draw $U$,

$$
\boxed{P(Q(U)\leq x)=P(U\leq F(x))=F(x).}
$$

This proves [inverse transform sampling](../../../../../inverse-transform-sampling.md) for discontinuous as well as continuous distribution functions.

There is a minor endpoint defect in the printed codomain. The true [quantile endpoint at probability one](../../../../../quantile-endpoint-at-probability-one.md) is $Q(1)=\inf\{x:F(x)=1\}$, which equals $+\infty$ for an unbounded-above [normal distribution](../../../../../normal-distribution.md). Thus it need not be real at one. Use the extended-real value there, or assign an arbitrary finite value at this single probability level. Since $P(U=1)=0$, either choice gives the same sampled distribution; the latter supplies a real-valued version on all of $(0,1]$. **The endpoint has no effect on the inverse-transform law.**

For [rejection sampling](../../../../../rejection-sampling.md), choose a proposal [probability density function](../../../../../probability-density-function.md) $g$ that can be sampled and a finite constant $M$ with $f(y)\leq Mg(y)$ wherever the target has positive mass. Generate independent pairs $(Y_j,U_j)$, with $Y_j$ of density $g$ and $U_j$ uniform. Accept $Y_j$ if $U_j\leq f(Y_j)/(Mg(Y_j))$; otherwise discard the pair and repeat with fresh independent draws. At points where both densities vanish the acceptance rule may be defined arbitrarily. For any measurable set $A$,

$$
P(Y_j\in A,\text{ acceptance})=\int_A g(y)\frac{f(y)}{Mg(y)}dy=\frac1M\int_A f(y)dy.
$$

Thus one trial accepts with probability $1/M$, and the conditional density given acceptance is $f$. More explicitly, summing over the index of the first accepted proposal gives

$$
P(\text{output}\in A)=\sum_{j\geq1}(1-1/M)^{j-1}\frac1M\int_Af(y)dy=\int_Af(y)dy.
$$

The probability of never accepting is zero, since $M<\infty$, and the expected number of proposals is $M$. **The algorithm terminates almost surely and samples the target density exactly.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
