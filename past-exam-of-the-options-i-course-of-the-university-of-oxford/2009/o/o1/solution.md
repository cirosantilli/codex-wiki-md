<h1 id="o/o1/solution">Solution</h1>

↑ **Parent:** [O1](../o1.md)

By [continuity](../../../../continuous-function.md) of the [cumulative distribution function](../../../../cumulative-distribution-function.md) and nonnegativity, $F(0)=0$; strict increase and $F(x)\to1$ allow inversion for every $0<t<1$. The [probability integral transform](../../../../probability-integral-transform.md) follows from

$$
\mathbb P(F(X)\leq t)=\mathbb P(X\leq F^{-1}(t))=t.
$$

Thus $F(X)$ is [uniformly distributed](../../../../continuous-uniform-distribution.md) on $(0,1)$.

The [order statistics](../../../../order-statistic.md) arrange the sample increasingly: $X_{(1)}\leq\cdots\leq X_{(n)}$. Strict monotonicity means $F(X_{(i)})$ is the $i$th [order statistic](../../../../order-statistic.md) of $n$ independent uniform variables. Its [density](../../../../density.md) is

$$
\frac{n!}{(i-1)!(n-i)!}\,t^{i-1}(1-t)^{n-i},\qquad0<t<1,
$$

obtained by choosing the $i-1$ observations below $t$ and the $n-i$ above it. This is the [beta distribution](../../../../beta-distribution.md) with parameters $i,n+1-i$, so

$$
\boxed{\mathbb E F(X_{(i)})=\frac i{n+1}}.
$$

For the given [log-logistic distribution](../../../../log-logistic-distribution.md), rearrangement gives

$$
\log\frac{F(x)}{1-F(x)}=(\beta-1)\log x-(\beta-1)\log\alpha.
$$

Consequently plot $y_i=\log(i/(n+1-i))$ vertically against $x_i^*=\log X_{(i)}$ horizontally. Under a good fit, replacing $F(X_{(i)})$ by its plotting position $i/(n+1)$ gives an approximate straight line with

$$
\boxed{\text{slope}=\beta-1,\qquad\text{intercept}=-(\beta-1)\log\alpha}.
$$

This is a diagnostic [probability plot](../../../../probability-plot.md), rather than an assertion that the [expectation](../../../../expected-value-split.md) of the nonlinear transformed [order statistic](../../../../order-statistic.md) equals that transformed plotting position. Positive observations occur almost surely under the model.

## ↑ Ancestors (12)

1. [O1](../o1.md)
2. [O](../../o.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
