<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The equation $(A^*A+\alpha_*I)u_*=A^*f$ is the [Tikhonov normal equation](../../../../../../../tikhonov-normal-equation.md). For $u=u_*+h$, expand the [Tikhonov regularization](../../../../../../../tikhonov-regularization.md) functional:

$$
\begin{aligned}
\phi_{\alpha_*}(u)
&=\phi_{\alpha_*}(u_*)
+2\operatorname{Re}\langle A^*(Au_*-f)+\alpha_*u_*,h\rangle_X\\
&\quad+\|Ah\|_Y^2+\alpha_*\|h\|_X^2.
\end{aligned}
$$

The normal equation makes the linear term zero. The final two terms are nonnegative and are strictly positive for $h\ne0$ because $\alpha_*>0$. Thus $u_*$ is the unique global minimizer.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
