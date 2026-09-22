<h1 id="20/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the two travelling profiles, the [initial conditions](../../../../../../initial-condition.md) imply

$$
f(x)+g(x)=\cos^2(x/2),\qquad -vf'(x)+vg'(x)=0.
$$

Since $v\ne0$, $g-f$ is constant. One may therefore choose

$$
f(x)=\tfrac12\cos^2(x/2)+C,\qquad
g(x)=\tfrac12\cos^2(x/2)-C,
$$

where the constants cancel in the sum. The [D'Alembert formula](../../../../../../d-alembert-s-formula.md) then gives

$$
\begin{aligned}
\psi(x,t)&=\frac12\cos^2\left(\frac{x-vt}{2}\right)
+\frac12\cos^2\left(\frac{x+vt}{2}\right)\\
&=\boxed{\frac12+\frac12\cos x\cos(vt)}.
\end{aligned}
$$

This agrees exactly with the restricted-domain solution from part (b). The whole-line cosine profile already has zero spatial [derivative](../../../../../../derivative.md) at both $x=0$ and $x=\pi$ for every time, so its restriction satisfies the [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) without further modification.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [20](../../../20.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
