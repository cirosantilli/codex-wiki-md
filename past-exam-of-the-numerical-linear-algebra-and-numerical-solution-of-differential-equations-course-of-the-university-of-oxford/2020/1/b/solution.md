<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the [chain rule](../../../../chain-rule.md), $y''=f_x+f_yf$ along the exact solution. Applying [Taylor's theorem](../../../../taylor-s-theorem.md) to the exact increment and the two arguments of $f$ gives

$$
\frac{y(x+h)-y(x)}h=f(x,y(x))+\frac h2y''(x)+O(h^2),\qquad
\Phi(x,y(x),h)=f(x,y(x))+\beta h(f_x+f_yf)(x,y(x))+O(h^2).
$$

The assumed differentiability makes the remainders uniform on $0\leq x\leq1-h$. Subtracting gives the [consistency error](../../../../normalized-local-truncation-error.md)

$$
\boxed{T_n=h\left(\frac12-\beta\right)y''(x_n)+O(h^2).}
$$

Here $O$ denotes [Big O notation](../../../../big-o-notation.md). The general [order of a numerical method](../../../../order-of-a-numerical-method.md) is therefore one for $\beta\ne1/2$ and at least two for $\beta=1/2$. For example, on $y'=y$ with unit initial value, $y_N=(1+h+\beta h^2)^{1/h}$. Expanding its [logarithm](../../../../logarithm.md) gives $y_N=e[1+(\beta-1/2)h+O(h^2)]$, so the first-order term is actually nonzero when $\beta\ne1/2$.

To control accumulation, the [mean value theorem](../../../../mean-value-theorem.md) and the bound on $f_y$ give

$$
|\Phi(x,u,h)-\Phi(x,v,h)|\leq L(1+\beta hL)|u-v|.
$$

Put $K_h=L(1+\beta hL)$, $q_h=1+hK_h$ and $e_n=y(x_n)-y_n$. The exact and numerical updates yield $|e_{n+1}|\leq q_h|e_n|+h|T_n|$, with $e_0=0$. Iterating this recurrence, as in the [Lipschitz one-step error bound](../../../../lipschitz-one-step-error-bound.md), gives

$$
|e_n|\leq\frac{q_h^n-1}{K_h}\max_{j<n}|T_j|
\leq\frac{e^{K_hx_n}-1}{K_h}\max_{j<n}|T_j|.
$$

Because $K_h\leq L(1+L)$ for $h\leq1$, the prefactor is bounded independently of the mesh. When $\beta=1/2$, the [consistency error](../../../../normalized-local-truncation-error.md) is $O(h^2)$, hence the maximum [global error](../../../../global-discretization-error.md) is $O(h^2)$. This proves at least second-order [numerical convergence](../../../../convergence-of-a-numerical-method.md) of the [explicit midpoint method](../../../../explicit-midpoint-method.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
