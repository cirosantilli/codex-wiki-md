<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Convert to minimization with $f=-F$ and retain $g\geq0$. A continuously differentiable inequality [augmented Lagrangian method](../../../../augmented-lagrangian-method.md) uses the [merit function](../../../../merit-function.md)

$$
\boxed{\Phi(x,\lambda,\mu)=f(x)+\frac1{2\mu}\sum_{i=1}^3
\left(\min\{g_i(x)-\mu\lambda_i,0\}^2-\mu^2\lambda_i^2\right),
\quad\mu>0,\quad\lambda\geq0.}
$$

For $g_i\leq\mu\lambda_i$ its contribution is $-\lambda_i g_i+g_i^2/(2\mu)$; otherwise it is the constant $-\mu\lambda_i^2/2$. This shifted truncation permits multipliers to decrease as well as increase while remaining nonnegative.

A useful initial estimate comes from the preceding pure [quadratic penalty method](../../../../quadratic-penalty-method.md) at $\mu_{-1}$:

$$
\lambda_i^{[0]}=\max\{0,-g_i(x^{[0]})/\mu_{-1}\}.
$$

Here $g(-1,-1)=(3,18,-2)$, so with $\mu_{-1}=2$ choose

$$
\boxed{\lambda^{[0]}=(0,0,1).}
$$

Then use this estimate and $\mu_0=1$ in the first augmented subproblem. Initial estimates are a choice, rather than uniquely specified data; zero multipliers would also define an initialization.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
