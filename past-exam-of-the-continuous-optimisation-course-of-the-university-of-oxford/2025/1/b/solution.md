<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\phi(\alpha)=f(x+\alpha s)$ and $h(\alpha)=\phi(\alpha)-\phi(0)-\beta_1\alpha d$. Part (a) gives $h(\alpha)<0$ just to the right of zero. If $L$ is a lower bound for $f$, then

$$
h(\alpha)\geq L-\phi(0)-\beta_1\alpha d\longrightarrow+\infty,
$$

because $d<0$. By [continuity](../../../../continuous-function.md), there is a first positive zero $A$ of $h$, and $h(\alpha)\leq0$ on $[0,A]$. Apply the [mean value theorem](../../../../mean-value-theorem.md) to $\phi$ on this interval: for some $t\in(0,A)$,

$$
\nabla f(x+ts)^Ts=\phi'(t)=\frac{\phi(A)-\phi(0)}A=\beta_1d>\beta_2d.
$$

At this same $t$, $h(t)\leq0$ supplies the [Armijo condition](../../../../armijo-condition.md). Thus $\alpha=t>0$ satisfies both weak [Wolfe conditions](../../../../wolfe-conditions.md). The boundedness assumption prevents the [objective function](../../../../objective-function.md) from following its initial negative slope forever; this is the mechanism behind [Existence of a Wolfe step](../../../../existence-of-a-wolfe-step.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
