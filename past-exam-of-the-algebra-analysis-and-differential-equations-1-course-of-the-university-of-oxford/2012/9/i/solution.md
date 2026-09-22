<h1 id="9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [Laplace transform of a derivative](../../../../laplace-transform-of-a-derivative.md), first apply [integration by parts](../../../../integration-by-parts.md) on a finite interval:

$$
\int_0^T e^{-pt}\dot x(t)\,dt
=e^{-pT}x(T)-x(0)+p\int_0^T e^{-pt}x(t)\,dt.
$$

Under the usual transform hypotheses, including sufficient regularity for [integration by parts](../../../../integration-by-parts.md), existence of the derivative's [Laplace transform](../../../../laplace-transform.md), and $e^{-pT}x(T)\to0$, passing to the [limit](../../../../limit-of-a-function.md) gives

$$
\boxed{\mathcal L\{\dot x\}(p)=p\bar x(p)-x(0).}
$$

These conditions hold, for example, for a continuously differentiable $x$ with $x$ and $\dot x$ of [exponential order](../../../../exponential-order.md), in a sufficiently far right half-plane. Existence of $\bar x(p)$ alone does not establish all of these derivative-transform hypotheses; the finite-interval identity displays exactly which boundary term must disappear. The polynomial solution in the last part satisfies them for every $\operatorname{Re}p>0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [9](../../9.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
