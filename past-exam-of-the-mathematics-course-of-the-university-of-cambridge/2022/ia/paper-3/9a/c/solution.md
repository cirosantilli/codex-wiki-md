<h1 id="9a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each field has only an azimuthal component and is independent of $r$ and $\phi$. The [curl in spherical coordinates](../../../../../../curl-in-spherical-coordinates.md) therefore reduces to

$$
(\nabla\times\mathbf A)_r
=\frac1{r\sin\theta}
\frac{\partial}{\partial\theta}
\bigl(\sin\theta A_\phi\bigr),
\qquad
(\nabla\times\mathbf A)_\theta
=-\frac1r\frac{\partial}{\partial r}(rA_\phi),
$$

and its $\phi$ component vanishes. The [half-angle identities](../../../../../../half-angle-identities.md)

$$
\sin\theta\tan\frac\theta2=1-\cos\theta,
\qquad
\sin\theta\left(-\cot\frac\theta2\right)=-(1+\cos\theta)
$$

show in both cases that

$$
\boxed{\nabla\times\mathbf A_+
=\nabla\times\mathbf A_-
=\frac{\mathbf e_r}{r^2}
=\frac{\mathbf x}{r^3}}.
$$

Apply part (a) with $g(r)=r^{-3}$. Then

$$
\nabla\cdot\frac{\mathbf x}{r^3}
=r(-3r^{-4})+3r^{-3}=0
$$

away from the origin, explicitly confirming that each resulting [curl](../../../../../../curl.md) has zero [divergence](../../../../../../divergence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9A](../../9a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
