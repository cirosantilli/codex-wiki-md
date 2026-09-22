<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Seek a [Frobenius solution](../../../../../frobenius-solution.md) $y=z^r\sum_{n\geq0}a_nz^n$ with $a_0\ne0$. Since $(z+z^3)^2=z^2+2z^4+z^6$, its lowest coefficient gives the [indicial equation](../../../../../indicial-equation.md)

$$
[r(r-1)+3r+1]a_0=(r+1)^2a_0=0.
$$

Thus the repeated [indicial root](../../../../../indicial-root.md) is $\boxed{r=-1}$. Equating the coefficient of $z^{n+r}$ before setting $r=-1$ gives

$$
(n+r+1)^2a_n+2(n+r-2)(n+r-3)a_{n-2}+(n+r-4)(n+r-5)a_{n-4}=0.
$$

For $n\geq1$ this becomes the [linear recurrence relation](../../../../../linear-recurrence-relation.md)

$$
\boxed{a_n=-\frac{2(n-3)(n-4)a_{n-2}+(n-5)(n-6)a_{n-4}}{n^2},\qquad a_j=0\text{ for }j<0.}
$$

Every coefficient is fixed by $a_0$, since the denominator never vanishes for $n\geq1$. In particular $a_1=0$ and then every odd coefficient is zero. Therefore there is $\boxed{\text{exactly one independent pure Frobenius series}}$, not two merely because the indicial root repeats. If "power series" means an ordinary [Taylor series](../../../../../taylor-series.md) with nonnegative integer powers, the only such solution is zero: its coefficient equation starts with $a_0=0$ and inductively forces all coefficients to vanish.

A second independent local solution is a [logarithmic solution from a repeated Frobenius exponent](../../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md). Indeed, [Abel's identity](../../../../../abel-s-identity.md) gives $W=Cz^{-3}[1+O(z^2)]$. For the normalized first solution $y_1=z^{-1}[1+O(z^2)]$, [reduction of order](../../../../../reduction-of-order.md) gives

$$
y_2=y_1\int^z\frac{\exp[-\int^sP(v)dv]}{y_1(s)^2}\,ds.
$$

After choosing the harmless multiplicative constant in the numerator, its integrand is $1/s+O(s)$, so $y_2=y_1\log z+z^{-1}\times\text{an analytic series}$. The nonzero logarithmic coefficient proves that this second solution is not another pure [Frobenius solution](../../../../../frobenius-solution.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
