<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the first [Frobenius solution](../../../../frobenius-solution.md), take the larger [indicial root](../../../../indicial-root.md) $r=a$ and normalize the first coefficient to one:

$$
y_+(x)=x^a\sum_{n=0}^\infty c_nx^n,\qquad c_0=1,
\qquad c_j=0\quad(j<0).
$$

Substitution and comparison of the coefficient of $x^{n+a}$ give

$$
\big[(n+a)^2-a^2\big]c_n+bc_{n-\beta}=0,
\qquad\boxed{c_n=-\frac{b\,c_{n-\beta}}{n(n+2a)}\quad(n\geq1).}
$$

Every denominator is nonzero because $a\geq0$.

For $\beta=1$, the [recurrence relation](../../../../recurrence-relation.md) is $c_n=-bc_{n-1}/[n(n+2a)]$, so

$$
\boxed{y_+(x)=x^a\left[1-\frac{b}{1+2a}x+
\frac{b^2}{2(1+2a)(2+2a)}x^2+\cdots\right],\quad
c_n=\frac{(-b)^n}{\prod_{j=1}^n j(j+2a)}.}
$$

For $\beta=2$, $c_1=0$ and all odd coefficients vanish; the even coefficients satisfy $c_{2k}=-bc_{2k-2}/[2k(2k+2a)]$. Hence

$$
\boxed{y_+(x)=x^a\left[1-\frac{b}{4(1+a)}x^2+
\frac{b^2}{32(1+a)(2+a)}x^4+\cdots\right].}
$$

For any positive integer $\beta$, induction in the [recurrence relation](../../../../recurrence-relation.md) shows that only indices divisible by $\beta$ survive:

$$
\boxed{y_+(x)=x^a\sum_{k=0}^\infty
\frac{(-b)^k x^{k\beta}}{\prod_{j=1}^k j\beta(j\beta+2a)}.}
$$

The empty product for $k=0$ equals one. Successive terms in the [power series](../../../../power-series.md) factor have ratio of magnitudes

$$
\frac{|b|\,|x|^\beta}{(k+1)\beta((k+1)\beta+2a)}\longrightarrow0.
$$

Thus the [ratio test](../../../../ratio-test.md) gives convergence for every finite $x$; a nonintegral $a$ still requires a chosen side of zero or a complex branch for the factor $x^a$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
