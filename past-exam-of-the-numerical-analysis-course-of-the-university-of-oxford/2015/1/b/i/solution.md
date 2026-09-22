<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

It suffices to assume $f\in C^2[a,b]$. The [polynomial interpolation error](../../../../../polynomial-interpolation-error.md) for the endpoint [linear interpolant](../../../../../linear-interpolant.md) gives, for every interior $x$, some $\xi_x\in(a,b)$ with

$$
f(x)-\ell(x)=\frac{f''(\xi_x)}2(x-a)(x-b).
$$

Let $M=\max_{[a,b]}|f''|$, which exists by [continuity](../../../../../continuous-function.md) of the [second derivative](../../../../../second-derivative.md) and the [extreme value theorem](../../../../../extreme-value-theorem.md). Since $(x-a)(b-x)\geq0$,

$$
|f(x)-\ell(x)|\leq\frac M2(x-a)(b-x).
$$

Integrating this pointwise inequality and using the [triangle inequality for an integral](../../../../../integral-triangle-inequality.md) yields

$$
\begin{aligned}
\left|\int_a^bf(x)\,dx-T(f)\right|
&\leq\frac M2\int_a^b(x-a)(b-x)\,dx\\
&=\frac M2\int_0^{b-a}t\bigl((b-a)-t\bigr)\,dt
=\frac{M(b-a)^3}{12}.
\end{aligned}
$$

Thus

$$
\boxed{|I(f)-T(f)|\leq\frac{(b-a)^3}{12}\max_{[a,b]}|f''|.}
$$

This derivation does not require choosing $\xi_x$ as a continuous [function](../../../../../function-split.md) of $x$; the pointwise upper bound is sufficient.

The constant is sharp. Take the [quadratic polynomial](../../../../../quadratic-polynomial.md) $f(x)=(x-a)^2$ and write $L=b-a$. Its exact [integral](../../../../../integral-split.md) is $L^3/3$, its [trapezoidal rule](../../../../../trapezoidal-rule.md) value is $L^3/2$, and $\max|f''|=2$. Consequently

$$
|I(f)-T(f)|=\frac{L^3}{6}=\frac{L^3}{12}\max|f''|.
$$

Equality holds, so **no smaller universal constant than $1/12$ works** under these assumptions. This is the [sharp one-panel trapezoidal error bound](../../../../../sharp-one-panel-trapezoidal-error-bound.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
