<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [Frobenius solution](../../../../../frobenius-solution.md) $y=x^\sigma\sum_{n\geq0}a_nx^n$, with $a_0\ne0$. The lowest power $x^{\sigma-1}$ has coefficient $2\sigma(2\sigma-1)a_0$, giving the [indicial equation](../../../../../indicial-equation.md)

$$
\boxed{2\sigma(2\sigma-1)=0,\qquad\sigma=0,\frac12.}
$$

For $n\geq1$, matching the coefficient of $x^{n+\sigma-1}$ gives

$$
2(n+\sigma)(2n+2\sigma-1)a_n-(2n+2\sigma-1)a_{n-1}=0.
$$

For both candidate exponents the cancelled factor is nonzero in this range, so the recurrence is

$$
\boxed{a_n=\frac{a_{n-1}}{2(n+\sigma)}.}
$$

With $a_0=1$, the exponent-zero solution is

$$
\boxed{y_1(x)=\sum_{n=0}^\infty\frac{x^n}{2^nn!}=e^{x/2}.}
$$

For $\sigma=1/2$, the coefficients are $a_n=1/(2n+1)!!=2^nn!/(2n+1)!$, giving

$$
\boxed{y_2(x)=\sqrt{x}\sum_{n=0}^\infty\frac{x^n}{(2n+1)!!}=\sqrt{x}\left(1+\frac x3+\frac{x^2}{15}+\frac{x^3}{105}+\cdots\right).}
$$

The [ratio test](../../../../../ratio-test.md) gives infinite [radius of convergence](../../../../../radius-of-convergence.md) for both series factors, since the successive ratios in magnitude are $|x|/(2n+2)$ and $|x|/(2n+3)$. The second full solution still needs a square-root branch in the complex plane; on $x>0$ it is a real solution. The distinct leading behaviors $1$ and $\sqrt{x}$ prove [linear independence](../../../../../linear-independence.md).

For an independent closed-form check on the structure, put $z=x/2$. The equation becomes $zY''+(1/2-z)Y'-(1/2)Y=0$, a [Kummer differential equation](../../../../../kummer-differential-equation.md) with equal parameters. Its [exponential reduction of a confluent hypergeometric equation with equal parameters](../../../../../exponential-reduction-of-a-confluent-hypergeometric-equation-with-equal-parameters.md) explains the elementary first solution and the branched companion.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
