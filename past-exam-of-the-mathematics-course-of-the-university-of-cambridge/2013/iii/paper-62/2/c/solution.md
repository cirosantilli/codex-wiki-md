<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Compute the [convex conjugate](../../../../../../convex-conjugate.md) of $f_z$ at a general pair $(v,y)$. With $w=z+u-x$, the independent variables become $(x,w)$ and $u=w+x-z$, so

$$
\begin{aligned}
f_z^*(v,y)
&=\sup_{x,w}\{\langle v+y,x\rangle+\langle y,w\rangle
-\langle y,z\rangle-k(x)-h(w)\}\\
&=k^*(v+y)+h^*(y)-\langle y,z\rangle.
\end{aligned}
$$

Therefore the [Lagrange dual function](../../../../../../lagrange-dual-function.md) is

$$
\boxed{\psi_z(y)=\langle y,z\rangle-k^*(y)-h^*(y).}
$$

Using [strong duality](../../../../../../strong-duality.md) from the preceding solution gives

$$
\boxed{F(z)=\sup_y[\langle y,z\rangle-k^*(y)-h^*(y)],
\qquad F=(k^*+h^*)^*.}
$$

Equivalently the [conjugate of an infimal convolution](../../../../../../conjugate-of-an-infimal-convolution.md) is $F^*=k^*+h^*$, and the continuous convex $F$ equals its [biconjugate](../../../../../../biconjugate.md).

For practical [subgradient](../../../../../../subgradient.md) computation, minimize the known convex dual objective

$$
k^*(y)+h^*(y)-\langle z,y\rangle.
$$

Every optimizer, and only an optimizer, belongs to $\partial F(z)$ by [Fenchel–Young inequality](../../../../../../fenchel-young-inequality.md). The full characterization is

$$
\boxed{\partial F(z)
=\arg\max_y\psi_z(y)
=\{y:z\in\partial(k^*+h^*)(y)\}.}
$$

This is [infimal-convolution dual subgradients](../../../../../../infimal-convolution-dual-subgradients.md); the set is nonempty because $F$ is finite convex everywhere. If both conjugates are differentiable at the optimizer, solve $\nabla k^*(y)+\nabla h^*(y)=z$. For nonsmooth conjugates, use the displayed aggregate [subdifferential](../../../../../../subdifferential.md) or a convex minimization algorithm. Replacing it by $\partial k^*(y)+\partial h^*(y)$ requires the usual [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) qualification; it is not automatically justified solely by knowing the two conjugates.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
