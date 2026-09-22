<h1 id="11a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [electric field](../../../../../../electric-field.md) of this [point charge](../../../../../../point-charge.md) is a translated and scaled version of the radial field in part (ii). If $\mathbf a\notin V$ and $\mathbf a\notin\partial V$, its [divergence](../../../../../../divergence.md) vanishes throughout $V$, so the [divergence theorem](../../../../../../divergence-theorem.md) gives zero [flux integral](../../../../../../flux-integral.md).

If $\mathbf a$ lies inside $V$, remove a small ball centered at $\mathbf a$. On the remaining volume the [divergence](../../../../../../divergence.md) is zero. Its boundary is $\partial V$ together with the small [sphere](../../../../../../sphere.md), whose outward normal for the punctured volume points towards $\mathbf a$. That inner [sphere](../../../../../../sphere.md) contributes $-q/\epsilon_0$, by the $4\pi$ [sphere](../../../../../../sphere.md) flux computed in part (ii). Thus the exterior flux must be $q/\epsilon_0$:

$$
\boxed{\int_{\partial V}\mathbf E\cdot d\mathbf S
=\begin{cases}0,&\mathbf a\notin V,\\q/\epsilon_0,&\mathbf a\in V.\end{cases}}
$$

This is [Gauss's law](../../../../../../gauss-s-law.md) for a [point charge](../../../../../../point-charge.md). The assumption that the charge is not on the boundary is essential to these alternatives.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
