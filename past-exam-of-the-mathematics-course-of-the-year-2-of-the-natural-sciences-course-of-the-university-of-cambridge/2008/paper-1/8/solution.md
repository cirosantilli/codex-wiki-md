<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Termwise differentiation of the convergent [Frobenius series](../../../../frobenius-solution.md) and collection of powers in the [Bessel differential equation](../../../../bessel-differential-equation.md) gives the lowest coefficient $(\sigma^2-\nu^2)a_0$, the next coefficient $[(\sigma+1)^2-\nu^2]a_1$, and, for $n\geq2$, the coefficient $[(\sigma+n)^2-\nu^2]a_n+a_{n-2}$. Since $a_0\ne0$, the stated choices $\sigma=\pm\nu$, $a_1=0$ and the recurrence make all coefficients vanish.

For $\nu=1/2$, the two resulting even-coefficient series are

$$
\sigma=\tfrac12:\quad a_0x^{1/2}\left(1-\frac{x^2}{3!}+\frac{x^4}{5!}-\cdots\right)=a_0\frac{\sin x}{\sqrt x},
$$

and

$$
\sigma=-\tfrac12:\quad a_0x^{-1/2}\left(1-\frac{x^2}{2!}+\frac{x^4}{4!}-\cdots\right)=a_0\frac{\cos x}{\sqrt x}.
$$

These are linearly independent on $x>0$ and give the [Bessel functions of order one half](../../../../bessel-functions-of-order-one-half.md), up to normalization. The specified condition $a_1=0$ is sufficient; in the negative-exponent branch at this particular order the next coefficient equation alone would allow $a_1$ to be free, adding a multiple of the positive-exponent solution.

For the [Legendre differential equation](../../../../legendre-differential-equation.md), substitution gives the full conditions

$$
\boxed{\sigma(\sigma-1)=0,\qquad \sigma(\sigma+1)a_1=0,\qquad
a_{n+2}=\frac{(\sigma+n)(\sigma+n+1)-\lambda(\lambda+1)}{(\sigma+n+2)(\sigma+n+1)}a_n\quad(n\geq0).}
$$

Thus $\sigma=0$ permits arbitrary $a_1$, while $\sigma=1$ requires $a_1=0$. This [Frobenius recurrence for the Legendre equation](../../../../frobenius-recurrence-for-the-legendre-equation.md) separates the even and odd series. The nearest singular points of the differential equation are $\pm1$, so the series about zero has radius at least one, and the generic nonterminating solutions have radius exactly one. Particular cancellations can give a larger radius.

Termination occurs when the degree reaches a nonnegative integer $N$ with $\lambda(\lambda+1)=N(N+1)$. For $\lambda\geq0$ this gives

$$
\boxed{\lambda=N\in\{0,1,2,\ldots\}.}
$$

Choose the even branch for even $N$ or the odd branch for odd $N$ to obtain a [Legendre polynomial](../../../../legendre-polynomial.md). The recurrence then terminates and gives a solution for all real $x$, with infinite radius of convergence. A nonzero entire solution at other $\lambda\geq0$ is impossible: each nonterminating parity has coefficient ratio tending to one in the variable $x^2$, and so radius one.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
