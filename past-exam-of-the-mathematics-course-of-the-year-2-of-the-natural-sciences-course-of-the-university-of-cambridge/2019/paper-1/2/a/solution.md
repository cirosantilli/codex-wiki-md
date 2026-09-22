<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write a nonzero separated solution as $T=X(x)Y(y)S(t)$. Division of the [heat equation](../../../../../heat-equation.md) by this product gives

$$
\frac{S'}{\lambda S}=\frac{X''}{X}+\frac{Y''}{Y}.
$$

The two spatial factors solve independent constant-coefficient [eigenvalue](../../../../../eigenvalue.md) problems. Zero endpoint values in $x$ require

$$
X_n(x)=\sin(n\pi x/a),\qquad X_n''=-(n\pi/a)^2X_n,\quad n=1,2,\ldots.
$$

The insulating conditions require

$$
Y_m(y)=\cos(m\pi y/b),\qquad Y_m''=-(m\pi/b)^2Y_m,\quad m=0,1,2,\ldots.
$$

The zero cosine mode is the nonzero constant function and must be retained; there is no nonzero zero-index sine mode. The temporal equation is $S'=-\lambda\pi^2(n^2/a^2+m^2/b^2)S$. Superposing the complete sine-cosine basis yields

$$
\boxed{T(x,y,t)=\sum_{n=1}^\infty\sum_{m=0}^\infty A_{nm}\sin\frac{n\pi x}{a}\cos\frac{m\pi y}{b}\exp\left[-\lambda\pi^2\left(\frac{n^2}{a^2}+\frac{m^2}{b^2}\right)t\right].}
$$

The constants are fixed by expansion of the initial profile. [Orthogonality](../../../../../orthogonal-vectors.md) gives sine norm $a/2$; the cosine norm is $b$ at $m=0$ and $b/2$ otherwise. This is the [heat equation on a rectangle with two insulated sides](../../../../../heat-equation-on-a-rectangle-with-two-insulated-sides.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
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
