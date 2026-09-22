<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work on a fixed finite interval $[a,a+T]$. Write $Y_n=y(x_n)$, $t=x_n+h/2$, and use the paper's [normalized local truncation error](../../../../normalized-local-truncation-error.md)

$$
\tau_n=\frac{Y_{n+1}-Y_n}{h}
-f\left(t,\frac{Y_{n+1}+Y_n}2\right).
$$

Assume $y$ has bounded continuous [derivatives](../../../../derivative.md) through order three on this interval, with $\|y''\|\leq M_2$ and $\|y'''\|\leq M_3$. Assume also that the [Jacobian matrix](../../../../jacobian-matrix.md) $f_y$ has [operator norm](../../../../operator-norm.md) at most $L$ on the segments joining $y(t)$ to the endpoint averages. For a scalar equation this last hypothesis is simply $|\partial f/\partial y|\leq L$ there.

Two symmetric estimates separate the errors. By [Taylor's theorem](../../../../taylor-s-theorem.md) applied to $y'$ about $t$, the linear term integrates to zero on $[-h/2,h/2]$, giving

$$
\begin{aligned}
\left\|\frac{Y_{n+1}-Y_n}{h}-y'(t)\right\|
&=\left\|\frac1h\int_{-h/2}^{h/2}\bigl(y'(t+s)-y'(t)\bigr)\,ds\right\|\\
&\leq\frac{M_3}{2h}\int_{-h/2}^{h/2}s^2\,ds
=\frac{M_3h^2}{24}.
\end{aligned}
$$

Likewise the two linear terms in the endpoint expansions cancel, and their second-order remainders give

$$
\left\|\frac{Y_{n+1}+Y_n}2-y(t)\right\|\leq\frac{M_2h^2}{8}.
$$

The derivative bound on $f$ gives a [Lipschitz condition](../../../../lipschitz-continuity.md) in its second variable. Since $y'(t)=f(t,y(t))$, the [triangle inequality](../../../../triangle-inequality.md) now yields

$$
\boxed{\|\tau_n\|\leq
\left(\frac{M_3}{24}+\frac{LM_2}{8}\right)h^2
=Kh^2.}
$$

The constant is independent of $n$ and $h$ as long as the steps remain in the fixed interval. This [implicit midpoint consistency bound](../../../../implicit-midpoint-consistency-bound.md) proves [numerical consistency](../../../../consistency-of-a-numerical-method.md) of order two. The corresponding unnormalized residual is $h\tau_n=O(h^3)$; the two powers conventionally called [local truncation error](../../../../local-truncation-error.md) differ because the paper divides by the step size. If local error instead means the error of an exactly solved numerical step started at $Y_n$, the small-step [Lipschitz condition](../../../../lipschitz-continuity.md) gives the bound $h\|\tau_n\|/(1-hL/2)=O(h^3)$ as well.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
