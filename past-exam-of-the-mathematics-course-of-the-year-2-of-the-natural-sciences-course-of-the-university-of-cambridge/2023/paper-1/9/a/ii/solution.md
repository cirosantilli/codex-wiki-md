<h1 id="9/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the fixed source and receiver to be $A=(a,h_A)$ and $B=(b,h_B)$ on the same side of the mirror, with $h_A,h_B>0$. In the uniform medium, the [Fermat principle](../../../../../../fermat-principle.md) minimizes the length through a reflection point $P=(s,0)$:

$$
L(s)=\sqrt{(s-a)^2+h_A^2}+\sqrt{(s-b)^2+h_B^2}.
$$

Its stationary equation is

$$
L'(s)=\frac{s-a}{\sqrt{(s-a)^2+h_A^2}}+\frac{s-b}{\sqrt{(s-b)^2+h_B^2}}=0.
$$

The two fractions are the signed tangential components of the ray directions. Equality of their magnitudes gives $\sin\theta_i=\sin\theta_r$, where both angles are measured from the [normal vector](../../../../../../normal-vector.md) to the mirror and lie in $[0,\pi/2)$. Hence the [law of reflection](../../../../../../law-of-reflection.md) is

$$
\boxed{\theta_i=\theta_r.}
$$

For uniqueness, differentiate once more:

$$
L''(s)=\frac{h_A^2}{[(s-a)^2+h_A^2]^{3/2}}+\frac{h_B^2}{[(s-b)^2+h_B^2]^{3/2}}>0.
$$

Thus $L$ is a [strictly convex function](../../../../../../strictly-convex-function.md), its [derivative](../../../../../../derivative.md) increases from $-2$ to $2$, and it has exactly one stationary point, its [global minimum](../../../../../../global-minimum.md). Explicitly,

$$
\boxed{s_* =\frac{h_Ba+h_Ab}{h_A+h_B}.}
$$

Substitution gives $(s_*-a)/h_A=(b-s_*)/h_B$, verifying the reflection angles and the existence of that unique solution. Equivalently it is the point where the line from $A$ to the mirror image $(b,-h_B)$ crosses the mirror.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
