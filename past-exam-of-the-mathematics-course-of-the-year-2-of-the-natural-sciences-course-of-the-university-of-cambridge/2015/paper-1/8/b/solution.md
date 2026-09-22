<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because zero is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md), substitute $y=\sum_{j\geq0}a_jx^j$. Matching powers gives

$$
(j+2)(j+1)a_{j+2}+(n^2-j^2)a_j=0,\qquad\boxed{a_{j+2}=\frac{j^2-n^2}{(j+2)(j+1)}a_j.}
$$

Even and odd coefficients evolve independently. Taking $(a_0,a_1)=(1,0)$ and $(0,1)$ constructs solutions

$$
\begin{aligned}
y_{\rm e}&=1-\frac{n^2x^2}{2!}+\frac{n^2(n^2-4)x^4}{4!}-\frac{n^2(n^2-4)(n^2-16)x^6}{6!}+\cdots,\\
y_{\rm o}&=x+\frac{(1-n^2)x^3}{3!}+\frac{(1-n^2)(9-n^2)x^5}{5!}+\cdots.
\end{aligned}
$$

Their initial values and [derivatives](../../../../../derivative.md) give $W(y_{\rm e},y_{\rm o})(0)=1$, so they are [linearly independent](../../../../../linear-independence.md). These [power series of the Chebyshev differential equation](../../../../../power-series-of-the-chebyshev-differential-equation.md) span the local solution space. A useful check is $y_{\rm e}=\cos(n\arcsin x)$ and $y_{\rm o}=\sin(n\arcsin x)/n$, with $y_{\rm o}=\arcsin x$ at $n=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
