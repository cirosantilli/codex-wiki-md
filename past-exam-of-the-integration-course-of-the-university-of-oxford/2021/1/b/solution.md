<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On $(0,1)$, the integrand is bounded by one. For $x\to\infty$, $\alpha x^\beta-2\log x\to\infty$, since every positive power grows faster than the [natural logarithm](../../../../natural-logarithm.md). Thus $e^{-\alpha x^\beta}\leq x^{-2}$ eventually. The [comparison test for integrals](../../../../comparison-test-for-integrals.md) proves [Lebesgue integrability](../../../../integrability.md).

To prove joint [continuity](../../../../continuous-function.md), fix $(\alpha_0,\beta_0)$ with both coordinates positive. In a sufficiently small parameter rectangle, $\alpha\geq a:=\alpha_0/2>0$ and $\beta\geq b:=\beta_0/2>0$. For every parameter pair in this rectangle,

$$
0\leq e^{-\alpha x^\beta}\leq H(x):=\begin{cases}1,&0<x<1,\\e^{-a x^b},&x\geq1.\end{cases}
$$

The first argument shows that $H$ is [integrable](../../../../integrability.md). Along any parameter [sequence](../../../../sequence.md) tending to $(\alpha_0,\beta_0)$, the integrands converge [pointwise](../../../../pointwise-convergence.md), and the same $H$ dominates their eventual tail. The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) gives $g(\alpha,\beta)\to g(\alpha_0,\beta_0)$. The [sequential criterion for continuity](../../../../sequential-characterization-of-continuity-in-metric-spaces.md) proves the required joint [continuity](../../../../continuous-function.md) throughout the positive quadrant.

For comparison, the [change of variables](../../../../change-of-variables-formula.md) $u=\alpha x^\beta$ identifies the value with a [gamma function](../../../../gamma-function.md):

$$
\boxed{g(\alpha,\beta)=\frac{\Gamma(1/\beta)}{\beta\alpha^{1/\beta}}.}
$$

The domination argument establishes [continuity](../../../../continuous-function.md) directly, without needing a separate theorem about parameter dependence of the [gamma function](../../../../gamma-function.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
