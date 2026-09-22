<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The definition of $a$ and (c)(i) give $a\leq M$. Nonnegativity of the [variance](../../../../../variance-split.md) strengthens the lower bound to

$$
\boxed{\frac{\theta^2}{1+\theta^2}\leq a\leq M.}
$$

In fact the [variance](../../../../../variance-split.md) of one weighted observation is exactly

$$
v_{\mathrm{IS}}:=\operatorname{Var}_q(w(Y)\phi(Y))
=a(1+\theta^2)-\theta^2.
$$

It is finite by the envelope. For $v_{\mathrm{IS}}>0$, the [central limit theorem](../../../../../central-limit-theorem.md) gives approximate two-sided coverage $2\Phi(0.01\sqrt{n/v_{\mathrm{IS}}})-1$, so the paper's rounded [quantile](../../../../../quantile-function.md) yields

$$
\boxed{n_{\mathrm{IS}}=\left\lceil66{,}564\,[a(1+\theta^2)-\theta^2]\right\rceil.}
$$

If $v_{\mathrm{IS}}=0$, the weighted observation equals $\theta$ [almost surely](../../../../../almost-sure-convergence.md), and one draw is sufficient. These are theoretical budgets: $a$ and $\theta$ may themselves be unknown and need preliminary estimation in an implementation.

Compare with the average [rejection sampling](../../../../../rejection-sampling.md) cost $66{,}564M$. Ignoring integer rounding, [importance sampling](../../../../../importance-sampling.md) uses fewer proposal draws at the same approximate precision precisely when

$$
a(1+\theta^2)-\theta^2<M,
\qquad
\boxed{a<\frac{M+\theta^2}{1+\theta^2}.}
$$

For literal integer budgets, the comparison is $\lceil66{,}564v_{\mathrm{IS}}\rceil<66{,}564M$. The simpler strict inequality is the intended leading-order condition. The bound $a\leq M$ alone does not ensure an improvement when $\theta\ne0$; this is a [proposal-budget variance comparison of importance and rejection sampling](../../../../../proposal-budget-variance-comparison-of-importance-and-rejection-sampling.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
