<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the new integrand, $\theta=\mathbb E_p[e^{-X_1}]=e^{1/2}$ and $\operatorname{Var}_p(e^{-X_1})=e^2-e$, independently of dimension. [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) therefore yields

$$
\mathbb P\!\left(|\widehat\theta_n^{\mathrm{RS}}-\theta|\geq\varepsilon\right)
\leq\frac{e^2-e}{n\varepsilon^2}.
$$

A sufficient positive integer sample count is

$$
\boxed{n=\left\lceil\frac{e^2-e}{\delta\varepsilon^2}\right\rceil.}
$$

The [ceiling function](../../../../../ceiling-function.md) ensures that the bound is at most $\delta$, so the strict-error event in the question has [probability](../../../../../probability.md) at least $1-\delta$. The required number of accepted draws is independent of $d$; their expected proposal count is $n\sigma^d$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
