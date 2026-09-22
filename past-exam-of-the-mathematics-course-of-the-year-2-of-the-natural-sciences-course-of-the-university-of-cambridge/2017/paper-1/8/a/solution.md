<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The origin is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md) of the [Hermite differential equation](../../../../../hermite-differential-equation.md), so put $y=\sum_{n=0}^{\infty}a_nx^n$. Substitution and matching powers gives

$$
\sum_{n=0}^{\infty}\left[(n+2)(n+1)a_{n+2}+(\lambda-2n)a_n\right]x^n=0.
$$

Thus the [linear recurrence relation](../../../../../linear-recurrence-relation.md) is

$$
\boxed{a_{n+2}=\frac{2n-\lambda}{(n+2)(n+1)}a_n,\qquad n\geq0.}
$$

Even and odd coefficients evolve independently from arbitrary $a_0,a_1$. The general [power series](../../../../../power-series.md) solution is

$$
\boxed{y(x)=a_0\sum_{j=0}^{\infty}\frac{\prod_{r=0}^{j-1}(4r-\lambda)}{(2j)!}x^{2j}
+a_1\sum_{j=0}^{\infty}\frac{\prod_{r=0}^{j-1}(4r+2-\lambda)}{(2j+1)!}x^{2j+1},}
$$

with an empty product equal to one. Its first terms are

$$
y=a_0\left[1-\frac\lambda2x^2+\frac{\lambda(\lambda-4)}{24}x^4+\cdots\right]
+a_1\left[x+\frac{2-\lambda}{6}x^3+\frac{(2-\lambda)(6-\lambda)}{120}x^5+\cdots\right].
$$

Both series converge at every finite $x$, since the ratio of successive terms in each parity subsequence tends to zero. For a nonzero [polynomial](../../../../../polynomial-split.md) of degree $N$, the highest coefficient in the [differential equation](../../../../../differential-equation-split.md) requires $\lambda=2N$. Conversely, at such a value the appropriate parity series terminates, while its opposite-parity initial coefficient can be set to zero. Hence

$$
\boxed{\lambda=2N,\qquad N=0,1,2,\ldots,\qquad y\propto H_N(x).}
$$

Here $H_N$ is a physicists' [Hermite polynomial](../../../../../hermite-polynomial.md). Two explicit choices are

$$
\boxed{\lambda=4:\ y=4x^2-2,\qquad \lambda=6:\ y=8x^3-12x.}
$$

Direct differentiation verifies both. These are [polynomial](../../../../../polynomial-split.md) solutions up to an arbitrary overall factor. Without a [polynomial](../../../../../polynomial-split.md) requirement or additional [boundary conditions](../../../../../boundary-condition.md), the equation also has nonpolynomial solutions for other real $\lambda$; discreteness here comes from termination.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
