<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [normalized velocity-reset collision operator](../../../../../../normalized-velocity-reset-collision-operator.md),

$$
\langle Lf,g\rangle=\rho(f)\overline{\rho(g)}-\langle f,g\rangle=\langle f,Lg\rangle.
$$

This bounded everywhere-defined operator is [self-adjoint](../../../../../../self-adjoint-operator.md). Put $h=f/M$. Expanding the square with the [probability measure](../../../../../../probability-measure.md) $M(v)\,dv$ gives

$$
\int\!\!\int|h(v_*)-h(v)|^2M(v)M(v_*)\,dv\,dv_*
=2\|f\|_H^2-2|\rho(f)|^2.
$$

It follows that

$$
\boxed{\langle Lf,f\rangle=-\frac12\int\!\!\int|h(v_*)-h(v)|^2M(v)M(v_*)\,dv\,dv_*\leq0}.
$$

Replacing the difference by $(f(v_*)M(v)-f(v)M(v_*))/(M(v)M(v_*))$ gives the other printed [integral](../../../../../../integral.md) expression. For real functions the modulus squares are ordinary squares; the modulus version also proves the complex-space statement.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
