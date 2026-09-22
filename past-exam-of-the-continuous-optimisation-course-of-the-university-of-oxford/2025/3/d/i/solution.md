<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a strictly [feasible point](../../../../../feasible-point.md), an initial barrier parameter $\mu_0>0$, and $0<\theta<1$. At outer iteration $k$, approximately minimize the [logarithmic barrier](../../../../../logarithmic-barrier.md) objective $f_{\mu_k}$ over its strictly feasible [domain of a function](../../../../../domain-of-a-function.md). For example, use damped [Newton methods](../../../../../newton-s-method-in-optimization.md), choosing an inner [step size](../../../../../step-size.md) by [backtracking line search](../../../../../backtracking-line-search.md) so that every $c_i$ stays positive and the barrier [objective function](../../../../../objective-function.md) decreases. Solve to a tolerance $\|\nabla f_{\mu_k}(x^k)\|\leq\varepsilon_k$, where $\varepsilon_k\to0$. Set $\mu_{k+1}=\theta\mu_k$ and use $x^k$ as the next starting point.

The associated [Lagrange multiplier](../../../../../lagrange-multiplier.md) estimates are

$$
\lambda_i^k=\frac{\mu_k}{c_i(x^k)}>0,\qquad\lambda_i^kc_i(x^k)=\mu_k.
$$

Reducing $\mu_k$ makes these perturbed [complementary slackness](../../../../../complementary-slackness.md) equations approach the [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md). This describes the generic [interior-point method](../../../../../interior-point-method.md); existence of a solution to every inner minimization needs appropriate additional attainment assumptions and does not follow from strict feasibility alone.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
