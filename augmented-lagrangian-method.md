# Augmented Lagrangian method

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)

For smooth constraints $g_i\geq0$, minimize

$$
\Phi(x,\lambda,\mu)=f(x)+\frac1{2\mu}\sum_i
\bigl(\min(g_i(x)-\mu\lambda_i,0)^2-\mu^2\lambda_i^2\bigr)
$$

approximately in $x$, then update the nonnegative [Lagrange multipliers](lagrange-multiplier.md) by the displayed projected rule. Equality constraints instead contribute $-\nu_jh_j+h_j^2/(2\mu)$ and use the unprojected update $\nu_j^+=\nu_j-h_j/\mu$. The construction combines [Lagrangian duality](lagrangian-duality.md) with a [quadratic penalty method](quadratic-penalty-method.md).

For an inequality, the exact identity is $\min(g_i,\mu\lambda_i)=\mu(\lambda_i-\lambda_i^+)$. Its unshifted negative part satisfies $\min(g_i,0)=\mu\min(\lambda_i-\lambda_i^+,0)$. On a violated constraint, accurate new multipliers therefore give violation of the order of $\mu$ times the multiplier error. This can achieve high feasibility accuracy without a vanishingly small $\mu$, reducing [condition number](condition-number.md) difficulties. The negative-part qualification is essential if an iterate approaches a binding constraint from the feasible side.

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Merit function](merit-function.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/1/iv/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/5/iii/solution.md)
