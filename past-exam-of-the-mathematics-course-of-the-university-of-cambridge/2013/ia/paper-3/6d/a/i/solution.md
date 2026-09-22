<h1 id="6d/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $M=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ in the [special linear group over a finite field](../../../../../../../special-linear-group-over-a-finite-field.md), define the [Möbius transformation](../../../../../../../mobius-transformation.md) $M\cdot x=(ax+b)/(cx+d)$ when the denominator is nonzero, and set $M\cdot x=\infty$ when it is zero. At the extra point, $M\cdot\infty=a/c$ for $c\ne0$, and $M\cdot\infty=\infty$ for $c=0$. [Determinant](../../../../../../../determinant.md) one prevents simultaneous zero numerator and denominator.

The [orbit-stabiliser theorem](../../../../../../../orbit-stabilizer-theorem.md) states $|G\cdot x|=[G:G_x]$, and for a [finite group](../../../../../../../finite-group.md) $|G|=|G\cdot x||G_x|$. The matrix $\begin{pmatrix}t&-1\\1&0\end{pmatrix}$ sends infinity to any chosen $t\in\mathbb F_p$, so **the orbit of infinity is the whole [projective line](../../../../../../../projective-line.md)**, of size $p+1$. Its [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md) is

$$
\boxed{G_\infty=\left\{\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}:a\in\mathbb F_p^*,\ b\in\mathbb F_p\right\},}
$$

which has $p(p-1)$ elements. Consequently

$$
\boxed{|\mathrm{SL}_2(p)|=(p+1)p(p-1)=p(p^2-1).}
$$

The [SL2 action on a finite projective line](../../../../../../../sl2-action-on-a-finite-projective-line.md) need not be faithful: scalar matrices can fix every projective point. Faithfulness is not needed for this orbit calculation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [6D](../../../6d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
