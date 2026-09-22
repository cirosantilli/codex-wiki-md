<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The homogeneous equation is a [Cauchy-Euler equation](../../../../cauchy-euler-equation.md). Trying $y=x^m$ gives the repeated [indicial root](../../../../indicial-root.md)

$$
m(m-1)+3m+1=(m+1)^2=0.
$$

Hence, for $x>0$,

$$
\boxed{y_h=\frac{C_1+C_2\log x}{x}.}
$$

Both independent solutions diverge at the origin, so no nonzero homogeneous combination satisfies the zero-origin conditions by continuous extension.

For a source point $\xi>0$, finiteness on $0<x<\xi$ forces the [Green function](../../../../green-s-function-split.md) to vanish on that side. On $x>\xi$, continuity and the unit first-derivative jump require

$$
G(\xi^+,\xi)=0,\qquad G_x(\xi^+,\xi)=1.
$$

Using the homogeneous solutions gives the [causal Green function for a repeated-root Euler operator](../../../../causal-green-function-for-a-repeated-root-euler-operator.md)

$$
\boxed{G(x,\xi)=\begin{cases}0,&0\leq x<\xi,\\\displaystyle\frac{\xi^2}{x}\log\frac{x}{\xi},&x\geq\xi>0.\end{cases}}
$$

Indeed, the [Wronskian](../../../../wronskian.md) of $x^{-1}$ and $x^{-1}\log x$ is $x^{-3}$, and direct [differentiation](../../../../differentiation.md) gives $G_x(\xi^+,\xi)=1$. Since $G$ is continuous, its second derivative produces precisely a unit [Dirac delta](../../../../dirac-delta-function.md), with no derivative of a delta. For each positive source it is identically zero near the origin, so both required origin values vanish. The differential operator itself is interpreted on $x>0$; no value of its singular coefficients at zero is needed.

Integrating against the forcing yields

$$
y(x)=\int_0^\infty G(x,\xi)\xi\,d\xi=\frac1x\int_0^x\xi^3\log\frac{x}{\xi}\,d\xi=x^3\int_0^1s^3\log\frac1s\,ds.
$$

The last [integral](../../../../integral-split.md) equals $1/16$, by [integration by parts](../../../../integration-by-parts.md) or differentiating $\int_0^1s^pds=1/(p+1)$. Consequently

$$
\boxed{y(x)=\frac{x^3}{16}.}
$$

Substitution gives $y''+3y'/x+y/x^2=(6+9+1)x/16=x$, while $y(0)=y'(0)=0$. The divergent homogeneous solutions prove uniqueness in the regular class. No boundary condition at infinity was imposed or required.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
