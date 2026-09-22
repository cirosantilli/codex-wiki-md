<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the rotationally invariant free-space [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md), put $s=\sqrt{(x-x')^2+(y-y')^2}$. Away from the source, the [radial Laplacian](../../../../../radial-laplacian.md) gives $(sG')'=0$, hence $G=A\log s^2+C$. Integrate its [Poisson equation](../../../../../poisson-s-equation.md) over a disk of radius $r$ about the source. The [divergence theorem](../../../../../divergence-theorem.md) gives $2\pi r(2A/r)=-1/\epsilon_0$, so

$$
\boxed{G=-\frac{1}{4\pi\epsilon_0}\log\big((x-x')^2+(y-y')^2\big)+C.}
$$

A fixed reference length can be inserted inside the [logarithm](../../../../../logarithm.md) and absorbed into $C$. The resulting [electric field](../../../../../electric-field-split.md) decays like $1/s$.

Strictly, the stated pointwise decay as $y\to\pm\infty$ alone does not justify “most general”: one can also add the [harmonic function](../../../../../harmonic-function.md) $\operatorname{Re}e^{(x+iy)^2}$, whose [gradient](../../../../../gradient.md) has that decay for every fixed $x$. This is the same growth issue as a [zero-boundary harmonic function with pointwise vertical decay](../../../../../zero-boundary-harmonic-function-with-pointwise-vertical-decay.md). The displayed answer is the usual isotropic free-space choice; requiring the field to vanish uniformly in every direction at spatial infinity removes these extra harmonic additions. An additive constant remains undetermined.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
