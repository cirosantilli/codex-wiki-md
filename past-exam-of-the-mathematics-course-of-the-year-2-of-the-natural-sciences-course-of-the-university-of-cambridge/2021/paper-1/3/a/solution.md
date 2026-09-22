<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed source point $\xi\in(a,b)$, the [Green function](../../../../../green-s-function-split.md) is defined by

$$
\boxed{L_xG(x;\xi)=\delta(x-\xi),\qquad G(a;\xi)=G(b;\xi)=0,}
$$

where $\delta$ is the [Dirac delta distribution](../../../../../dirac-delta-function.md) and the operator acts on $x$. The corresponding solution is

$$
\boxed{y(x)=\int_a^bG(x;\xi)f(\xi)\,d\xi.}
$$

Applying $L_x$ under the integral gives $f(x)$ by the defining delta identity, while the endpoint values vanish. With the stated continuous coefficients, one may define the normalized distributional equation $G_{xx}+(\beta/\alpha)G_x+(\gamma/\alpha)G=\delta(x-\xi)/\alpha(\xi)$; this avoids multiplying a general distributional second [derivative](../../../../../derivative.md) by a merely continuous coefficient.

Existence of this inverse [Green function](../../../../../green-s-function-split.md) additionally requires that the homogeneous two-point [boundary value problem](../../../../../boundary-value-problem-split.md) have only the zero solution. The assumptions printed in the question alone do not ensure this: $y''+y$ on $[0,\pi]$ has the nonzero zero-endpoint solution $\sin x$. At such resonance there are [solvability conditions](../../../../../solvability-condition.md) and no ordinary inverse kernel for arbitrary $f$. The construction below is nonresonant.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
