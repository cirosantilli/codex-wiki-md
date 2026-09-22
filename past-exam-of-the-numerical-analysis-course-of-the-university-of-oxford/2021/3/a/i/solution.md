<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here $y'=x/(1+y^2)$ and $y(0)=1$. Since $x\geq0$, the solution is nondecreasing, so $y(x)\geq1$. In fact $0\leq y'\leq1/2$ on $[0,1]$, which also bounds the solution and ensures it extends across this entire interval. The smooth right-hand side makes $y$ twice continuously differentiable, with [second derivative](../../../../../second-derivative.md)

$$
y''=\frac1{1+y^2}-\frac{2x^2y}{(1+y^2)^3}
=\frac{(1+y^2)^2-2x^2y}{(1+y^2)^3}.
$$

For $y\geq1$ and $0\leq x\leq1$,

$$
(1+y^2)^2\geq4y^2\geq2y\geq2x^2y,
$$

so $y''\geq0$. The subtracted term in the first expression is nonnegative, giving the useful bound

$$
\boxed{0\leq y''(x)\leq\frac1{1+y(x)^2}\leq\frac12\qquad(0\leq x\leq1).}
$$

The integral form of the [Taylor remainder](../../../../../taylor-remainder.md) now gives

$$
\begin{aligned}
\tau_n
&=\frac{y(x_{n+1})-y(x_n)}h-f(x_n,y(x_n))\\
&=\frac1h\int_{x_n}^{x_{n+1}}(x_{n+1}-t)y''(t)\,dt.
\end{aligned}
$$

Therefore the [normalized local truncation error](../../../../../normalized-local-truncation-error.md) satisfies the stronger estimate

$$
\boxed{0\leq\tau_n\leq\frac h4\leq\frac h2.}
$$

This proves the requested bound for $n=1,\ldots,N-1$, and also for $n=0$, which will be needed to start the [global error](../../../../../global-discretization-error.md) estimate. For $N=1$ the stated range is empty, but the estimate at $n=0$ still applies.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
