<h1 id="11e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
J(z)=\frac1{\overline z}
$$

be reflection in the unit circle, and represent a [Möbius transformation](../../../../../../mobius-transformation.md) $g$ by

$$
M=\begin{pmatrix}\alpha&\beta\\ \gamma&\delta\end{pmatrix}.
$$

A direct calculation shows that $JgJ$ is represented by

$$
\tau(M)=\begin{pmatrix}\overline\delta&\overline\gamma\\
\overline\beta&\overline\alpha\end{pmatrix}.
$$

Thus $gJ=Jg$ exactly when $M$ and $\tau(M)$ differ by a nonzero scalar. Applying the conjugate-linear involution $\tau$ twice shows that this scalar has [modulus](../../../../../../modulus.md) one. Rescaling $M$ by a suitable complex scalar then makes $M=\tau(M)$. Consequently all commuting maps, and only those maps, have the form

$$
\boxed{g(z)=\frac{az+b}{\overline b z+\overline a}},
\qquad |a|^2-|b|^2\ne0.
$$

This is the [Möbius maps commuting with reflection in the unit circle](../../../../../../mobius-maps-commuting-with-reflection-in-the-unit-circle.md) classification.

For such a map,

$$
|az+b|^2-|\overline b z+\overline a|^2
=(|a|^2-|b|^2)(|z|^2-1).
$$

It follows that $|g(z)|<1$ whenever $|z|<1$ precisely when

$$
\boxed{|a|>|b|}.
$$

The inverse has the same property, so these and only these maps preserve the unit disc.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
