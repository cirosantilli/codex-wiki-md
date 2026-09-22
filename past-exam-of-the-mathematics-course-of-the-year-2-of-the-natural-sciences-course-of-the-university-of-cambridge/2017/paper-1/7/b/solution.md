<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the prescribed imaginary part with respect to $y$:

$$
v_y=e^x[(1+x)\cos y-y\sin y].
$$

The [Cauchy-Riemann equation](../../../../../cauchy-riemann-equations.md) $u_x=v_y$ integrates to

$$
u=e^x(x\cos y-y\sin y)+F(y).
$$

Its $y$ derivative is $u_y=-e^x[(x+1)\sin y+y\cos y]+F'(y)$. On the other hand, $-v_x=-e^x[(x+1)\sin y+y\cos y]$. The second [Cauchy-Riemann equation](../../../../../cauchy-riemann-equations.md) therefore requires $F'(y)=0$. Combining the real and imaginary parts,

$$
e^x[(x\cos y-y\sin y)+i(y\cos y+x\sin y)]=(x+iy)e^{x+iy}.
$$

Thus the most general answer on a connected domain is

$$
\boxed{f(z)=ze^z+C,\qquad C\in\mathbb R.}
$$

A real constant preserves the given imaginary part. Conversely, the difference of any two such [analytic functions](../../../../../holomorphic-function-split.md) has zero imaginary part, and its Cauchy-Riemann derivatives force it to be constant. This proves completeness, rather than only exhibiting one possible [harmonic conjugate](../../../../../harmonic-conjugate.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
