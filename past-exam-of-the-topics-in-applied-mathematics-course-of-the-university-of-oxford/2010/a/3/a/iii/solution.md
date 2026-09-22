<h1 id="a/3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $a=f_u$, $b=f_v$, $c=g_u$, $d=g_v$, $\Delta=ad-bc$. Stability without [diffusion](../../../../../../diffusion.md) requires $a+d<0$ and $\Delta>0$. For a mode with $q=k^2$, the characteristic equation is

$$
\lambda^2-[a+d-(D_u+D_v)q]\lambda+h(q)=0,\quad h(q)=D_uD_vq^2-(D_va+D_ud)q+\Delta.
$$

For positive diffusivities the [trace](../../../../../../matrix-trace.md) stays negative for every $q\geq0$, so growth can occur only if $h(q)<0$. Put $S=D_va+D_ud$. This upward-opening quadratic has a negative interval at positive $q$ exactly when $S>0$ and $S^2>4D_uD_v\Delta$, or

$$
\boxed{a+d<0,\quad\Delta>0,\quad0<2\sqrt{D_uD_v\Delta}<D_ud+D_va.}
$$

If $D_u=D_v=D_0$, the right side is $D_0(a+d)<0$, impossible. Equivalently [diffusion](../../../../../../diffusion.md) would merely subtract $D_0q$ from both reaction [eigenvalues](../../../../../../eigenvalue.md). Thus **unequal diffusivities are necessary**.

The potentially unstable band has endpoints

$$
q_\pm=\frac{S\pm\sqrt{S^2-4D_uD_v\Delta}}{2D_uD_v},\qquad0<q_-<q_+.
$$

These are necessary continuous-wave-number conditions. Actual instability on the specified bounded domain additionally requires an allowed $q$ strictly between them. The strict inequalities exclude neutral onset and presume both diffusivities are positive, as in an ordinary two-chemical [diffusion](../../../../../../diffusion.md) model.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
