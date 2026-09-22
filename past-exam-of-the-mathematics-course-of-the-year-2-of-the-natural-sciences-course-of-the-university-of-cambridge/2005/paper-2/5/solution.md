<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The one-sided [Laplace transform](../../../../laplace-transform.md) is $\bar u(p)=\int_0^\infty e^{-pt}u(t)dt$ for sufficiently large $\operatorname{Re}p$. [Integration by parts](../../../../integration-by-parts.md), with the exponential suppressing the upper boundary, gives

$$
\overline{u'}=p\bar u-u(0),\qquad\overline{u''}=p^2\bar u-pu(0)-u'(0),\qquad\overline{u'''}=p^3\bar u-p^2u(0)-pu'(0)-u''(0).
$$

Differentiation under the integral gives $d\bar u/dp=-\int_0^\infty te^{-pt}u(t)dt$, proving $\overline{tu}=-d\bar u/dp$. Start with $\overline{e^{-t}}=1/(p+1)$ and apply this rule repeatedly:

$$
\boxed{\bar v_0=\frac1{p+1},\quad\bar v_1=\frac1{(p+1)^2},\quad\bar v_2=\frac2{(p+1)^3},\quad\bar v_3=\frac6{(p+1)^4}.}
$$

With all three initial data zero, transforming the forced equation gives $(p+1)^3\bar y=1/(p+1)$. Thus $\bar y=(p+1)^{-4}$ and the listed inverse transform gives

$$
\boxed{y(t)=\frac{t^3e^{-t}}6,\qquad t\geq0.}
$$

The cubic factor is also the [resonant exponential particular solution](../../../../resonant-exponential-particular-solution.md) associated with the triple characteristic root $-1$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
