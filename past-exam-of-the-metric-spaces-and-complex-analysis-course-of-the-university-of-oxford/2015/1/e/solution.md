<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

We can arrange that **neither the [supremum](../../../../supremum.md) nor the [infimum](../../../../infimum.md) is attained**. By part (d), choose a [continuous function](../../../../continuous-function.md) $f$ on $X$ with [unbounded](../../../../unbounded.md) range, and put $u=|f|$. Choose $x_n\in X$ so that $t_n=u(x_n)$ increases strictly to infinity. Construct a [continuous function](../../../../continuous-function.md) $h:[0,\infty)\to\mathbb R$ with

$$
h(t_n)=(-1)^n n:
$$

keep it constant up to $t_1$ and interpolate linearly on each $[t_n,t_{n+1}]$. Since $t_n\to\infty$, the joining points have no finite accumulation, so this defines a [continuous function](../../../../continuous-function.md) everywhere on its domain.

Now set

$$
\boxed{g(x)=\frac{h(u(x))}{\sqrt{1+h(u(x))^2}}.}
$$

By [function composition](../../../../function-composition.md), $g$ is [continuous](../../../../continuous-function.md), and $-1<g(x)<1$ for every $x$. Along the even and odd chosen points,

$$
g(x_{2n})\longrightarrow1,\qquad g(x_{2n+1})\longrightarrow-1.
$$

Thus $\sup_Xg=1$ and $\inf_Xg=-1$, and neither is a value of $g$. This proves the [bounded continuous witness with neither extremum attained](../../../../bounded-continuous-witness-with-neither-extremum-attained.md) construction, including for [subsets](../../../../subset.md) that are [bounded](../../../../boundedness.md) but not [closed](../../../../closed-set.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
