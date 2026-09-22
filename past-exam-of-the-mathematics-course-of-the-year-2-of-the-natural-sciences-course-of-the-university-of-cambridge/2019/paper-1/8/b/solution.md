<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After normalization, $p=-6x^2/(1-x^3)$ and $q=-6x/(1-x^3)$. Both are analytic at zero, so $\boxed{x=0\text{ is ordinary}}$. At one,

$$
(x-1)p=\frac{6x^2}{1+x+x^2},\qquad (x-1)^2q=\frac{6x(x-1)}{1+x+x^2}
$$

are analytic, whereas $p,q$ themselves have [poles](../../../../../pole.md). Hence $\boxed{x=1\text{ is a regular singular point}}$.

Insert $y=\sum_{n\geq0}a_nx^n$. The coefficient of $x^0$ gives $a_2=0$; for $k\geq1$ the coefficient of $x^k$ gives

$$
(k+2)(k+1)a_{k+2}=(k+2)(k+1)a_{k-1}.
$$

Thus $a_n=a_{n-3}$ for $n\geq3$. The initial data give $a_0=1$, $a_1=0$, so

$$
\boxed{y(x)=1+x^3+x^6+\cdots=\frac1{1-x^3},\qquad |x|<1.}
$$

The radius is one because the three cube roots of unity are [poles](../../../../../pole.md) of this solution. A direct structural check observes that the differential equation is exactly $[(1-x^3)y]''=0$. Thus $(1-x^3)y=A+Bx$, and the initial data select $A=1,B=0$. This is the [product-derivative reduction of a second-order differential equation](../../../../../product-derivative-reduction-of-a-second-order-differential-equation.md).

## ↑ Ancestors (13)

1. [B](../b.md)
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
