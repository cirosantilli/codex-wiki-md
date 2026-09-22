<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Seek a [power series](../../../../../power-series.md) $y=\sum_{j\ge0}a_jx^j$. The initial values give $a_0=0$ and $a_1=1$. Matching the coefficient of $x^j$ for $j\ge1$ gives $j(j+1)a_{j+1}+a_j=0$. Induction yields $a_j=(-1)^{j-1}/[(j-1)!j!]$, hence

$$
\boxed{y(x)=\sum_{k=0}^\infty\frac{(-1)^kx^{k+1}}{k!(k+1)!}
=x-\frac{x^2}2+\frac{x^3}{12}-\frac{x^4}{144}+\cdots.}
$$

The ratio of successive absolute terms is $|x|/[(k+1)(k+2)]$, so the series and its derivatives converge on every compact interval and satisfy the equation and initial values.

The first recursive approximations are $y_1=x-x^2/2$, $y_2=x-x^2/2+x^3/12$ and $y_3=x-x^2/2+x^3/12-x^4/144$. The general formula is

$$
\boxed{y_n(x)=\sum_{k=0}^n\frac{(-1)^kx^{k+1}}{k!(k+1)!}.}
$$

It holds for $n=0$. Assuming it for $n-1$, twice integrating $y_n''=-y_{n-1}/x$ with the required initial values gives the [Volterra integral equation](../../../../../volterra-integral-equation.md) iteration

$$
y_n=x-\int_0^x(x-s)\frac{y_{n-1}(s)}s\,ds.
$$

Each monomial integrates by $\int_0^x(x-s)s^k\,ds=x^{k+2}/[(k+1)(k+2)]$, producing precisely the next truncated series and proving the induction. The integrand is continuous at zero by its limiting value, since each previous iterate has zero constant term. Thus the [Volterra iteration for a singular power-series problem](../../../../../volterra-iteration-for-a-singular-power-series-problem.md) produces successive partial sums, converging with derivatives on compact sets to the analytic solution already found.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
