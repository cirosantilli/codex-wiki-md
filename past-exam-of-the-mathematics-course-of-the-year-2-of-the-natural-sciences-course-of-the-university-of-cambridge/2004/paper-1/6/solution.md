<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Wronskian](../../../../wronskian.md) is $W=y_1y_2'-y_1'y_2$. If constants $A,B$ obey $Ay_1+By_2=0$, differentiating gives $Ay_1'+By_2'=0$. At any point where $W\ne0$, these form an invertible two-by-two system, forcing $A=B=0$. Thus the two solutions are linearly independent.

For the given equation, the normalized coefficients are $p=(1-x)/(2x)$ and $q=-1/(4x)$, so zero is a [regular singular point](../../../../regular-singular-point.md). Substitute a [Frobenius series](../../../../frobenius-solution.md) $y=x^r\sum_{n=0}^\infty a_nx^n$, $a_0\ne0$. The lowest power gives the [indicial equation](../../../../indicial-equation.md)

$$
\boxed{2r(2r-1)=0,\qquad r=0,\ \tfrac12.}
$$

The coefficient of $x^{n+r}$ gives

$$
2(n+r+1)(2n+2r+1)a_{n+1}=(2n+2r+1)a_n.
$$

For either root the common factor is nonzero for $n\geq0$, so

$$
\boxed{a_{n+1}=\frac{a_n}{2(n+r+1)}.}
$$

With leading coefficient one, the two independent solutions are

$$
\boxed{y_1=\sum_{n=0}^\infty\frac{x^n}{2^nn!}=e^{x/2},\qquad y_2=x^{1/2}\sum_{n=0}^\infty\frac{x^n}{(2n+1)!!}=\sqrt{x}\left(1+\frac x3+\frac{x^2}{15}+\frac{x^3}{105}+\cdots\right).}
$$

Their analytic series factors both have **infinite radius of convergence**, because the ratio of consecutive terms tends to zero for every fixed $x$. The factor $x^{1/2}$ still gives the second solution a branch point at zero; it is not an entire function or an ordinary Taylor series there. On $x>0$, the general real solution is $C_1y_1+C_2y_2$. This is the $b=1/2$, $z=x/2$ case of the [exponential reduction of a confluent hypergeometric equation with equal parameters](../../../../exponential-reduction-of-a-confluent-hypergeometric-equation-with-equal-parameters.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
