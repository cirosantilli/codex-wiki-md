# Implicit midpoint consistency bound

↑ **Parent:** [Implicit midpoint rule](implicit-midpoint-rule.md)

For an exact solution $y'=f(t,y)$, define the [normalized local truncation error](normalized-local-truncation-error.md) of the [implicit midpoint rule](implicit-midpoint-rule.md) by

$$
\tau_n=\frac{y(t_n+h)-y(t_n)}h-
f\left(t_n+\frac h2,\frac{y(t_n+h)+y(t_n)}2\right).
$$

If $\|y''\|\leq M_2$, $\|y'''\|\leq M_3$ and the state [Jacobian matrix](jacobian-matrix.md) of $f$ has [operator norm](operator-norm.md) at most $L$ on the intervening state segments, then the displayed bound holds uniformly on a fixed finite interval. To prove it, put $t=t_n+h/2$. Symmetric [Taylor expansions](taylor-expansion.md) give

$$
\left\|\frac{y(t+h/2)-y(t-h/2)}h-y'(t)\right\|
\leq\frac{M_3h^2}{24},\qquad
\left\|\frac{y(t+h/2)+y(t-h/2)}2-y(t)\right\|
\leq\frac{M_2h^2}{8}.
$$

For the first bound, integrate the second-order remainder of $y'(t+s)$ over the symmetric step; for the second, average the second-order remainders of $y$ at the endpoints. The odd terms cancel. The [Lipschitz condition](lipschitz-continuity.md) for $f$ and $y'(t)=f(t,y(t))$ finish the proof by the [triangle inequality](triangle-inequality.md). The unnormalized step residual is $h\tau_n=O(h^3)$.

## ↑ Ancestors (9)

1. [Implicit midpoint rule](implicit-midpoint-rule.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method-split.md)
4. [One-step method](one-step-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Implicit midpoint Lipschitz estimate](implicit-midpoint-lipschitz-estimate.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2023/3/b/solution.md)
