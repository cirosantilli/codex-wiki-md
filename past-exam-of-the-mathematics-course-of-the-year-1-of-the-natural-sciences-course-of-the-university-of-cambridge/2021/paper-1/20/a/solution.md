<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $a=\pi/3$, $b=2\pi/3$ and take $n$ equal subintervals of width $h=(b-a)/n=\pi/(3n)$. Since [sine](../../../../../sine.md) is continuous, its integral is the limit of the left-endpoint [Riemann sums](../../../../../riemann-sum.md)

$$
J=\lim_{n\to\infty}h\sum_{j=0}^{n-1}\sin(a+jh).
$$

Using [Euler's formula](../../../../../euler-s-formula.md), the corresponding complex sum is a finite [geometric series](../../../../../geometric-series.md):

$$
S_n=h\sum_{j=0}^{n-1}e^{i(a+jh)}=he^{ia}\frac{1-e^{inh}}{1-e^{ih}},\qquad nh=b-a=\frac\pi3.
$$

Since $(e^{ih}-1)/h\to i$,

$$
\lim S_n=\frac{e^{ib}-e^{ia}}i=\frac{(-1/2+i\sqrt3/2)-(1/2+i\sqrt3/2)}i=i.
$$

Taking [imaginary parts](../../../../../imaginary-part.md) gives

$$
\boxed{J=1.}
$$

One can see the same limit entirely within the real sums: the finite trigonometric-sum identity obtained from this geometric sum gives

$$
h\sum_{j=0}^{n-1}\sin(a+jh)=h\frac{\sin(nh/2)}{\sin(h/2)}\sin\left(a+\frac{n-1}{2}h\right)=\frac h2\cot\frac h2\longrightarrow1.
$$

Thus the evaluation is explicitly by a [Riemann sum](../../../../../riemann-sum.md), as required.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
