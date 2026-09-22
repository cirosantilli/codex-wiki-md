<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Recognize that $z^2=(x^2-y^2)+2ixy$ and $e^{-z}=e^{-x}(\cos y-i\sin y)$. Their product has exactly the specified real part. Its imaginary part is

$$
v_0=e^{-x}[2xy\cos y-(x^2-y^2)\sin y].
$$

One can also recover it directly from the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). Differentiating the specified real part gives

$$
u_x=e^{-x}[(2x-x^2+y^2)\cos y+2y(1-x)\sin y].
$$

Integration of $v_y=u_x$ gives $v=v_0+h(x)$; the other equation $v_x=-u_y$ then forces $h'(x)=0$. Thus the most general answer on a connected domain is

$$
\boxed{f(z)=z^2e^{-z}+iC,\qquad C\in\mathbb R.}
$$

Indeed the difference of any two [analytic functions](../../../../../holomorphic-function-split.md) with the same real part has zero real part; its two [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) force its imaginary part to be constant. This proves that no further analytic freedom is missing.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
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
