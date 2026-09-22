<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $M=\max\{b,y_1,\ldots,y_n\}$. The [continuous uniform distribution](../../../../continuous-uniform-distribution.md) likelihood contributes $\phi^{-n}\mathbf1_{\{\phi\geq\max_i y_i\}}$, while the [Pareto distribution](../../../../pareto-distribution.md) prior contributes $\phi^{-a-1}\mathbf1_{\{\phi\geq b\}}$. Their product proves [Uniform-Pareto conjugacy](../../../../uniform-pareto-conjugacy.md):

$$
\boxed{p(\phi\mid\boldsymbol y)=(a+n)M^{a+n}\phi^{-(a+n+1)}\mathbf1_{\{\phi\geq M\}}}.
$$

Thus the [posterior distribution](../../../../bayesian-posterior.md) is Pareto with shape $a+n$ and lower bound $M$. Its density is strictly decreasing on its support, so the [highest posterior density interval](../../../../highest-posterior-density-interval.md) begins at $M$. Since the upper-tail probability is $(M/u)^{a+n}$, the required upper endpoint satisfies $(M/u)^{a+n}=0.05$. The [Pareto highest density interval](../../../../pareto-highest-density-interval.md) is therefore

$$
\boxed{[M,\ M\,20^{1/(a+n)}]}.
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
