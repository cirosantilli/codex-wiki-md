<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0\leq x\leq1$ and every real $z$,

$$
|\partial_yf(x,z)|=\frac{2x|z|}{(1+z^2)^2}
\leq\frac{x}{1+z^2}\leq1,
$$

where $2|z|\leq1+z^2$ was used. The [mean value theorem](../../../../../mean-value-theorem.md) therefore proves [Lipschitz continuity](../../../../../lipschitz-continuity.md) in $y$ with constant $1$.

Let $e_n=y(x_n)-y_n$. The [explicit Euler method](../../../../../euler-method.md) and the exact-solution identity from part (i) give

$$
e_{n+1}=e_n+h\big(f(x_n,y(x_n))-f(x_n,y_n)\big)+h\tau_n.
$$

Using the requested [local truncation error](../../../../../local-truncation-error.md) bound $|\tau_n|\leq h/2$, including at $n=0$, yields

$$
|e_{n+1}|\leq(1+h)|e_n|+\frac{h^2}{2},\qquad e_0=0.
$$

Iteration and the finite [geometric series](../../../../../geometric-series.md) give

$$
|e_N|\leq\frac{h^2}{2}\sum_{j=0}^{N-1}(1+h)^j
=\frac h2\big((1+h)^N-1\big).
$$

Since $1+h\leq e^h$ and $Nh=1$,

$$
\boxed{|y(1)-y_N|\leq\frac{e-1}{2}h.}
$$

Keeping the stronger bound $|\tau_n|\leq h/4$ from part (i) improves the same proof to $(e-1)h/4$. The requested inequality follows already from the weaker bound.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
