<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Represent a [Möbius transformation](../../../../../mobius-transformation.md) by a matrix, with nonzero scalar multiples representing the same map. Matrix multiplication reproduces composition, so $\theta$ is a [group homomorphism](../../../../../group-homomorphism.md). Every Möbius map has a representing matrix $A\in GL_2(\mathbb C)$; multiplying $A$ by either square root of $(\det A)^{-1}$ gives a matrix in $SL_2(\mathbb C)$ representing the same map. Thus $\theta$ is surjective. A matrix in its kernel represents the identity and is therefore scalar; determinant one leaves

$$
\boxed{\ker\theta=\{I,-I\}}.
$$

If a nonidentity Möbius map $T$ has two distinct fixed points, conjugate those points to $0$ and $\infty$. The conjugated map fixes both and hence has the form $S(z)=\mu z$ with $\mu\ne0,1$. If $T$ has one fixed point, conjugate it to $\infty$. The resulting affine map has the form $az+b$; having no finite fixed point forces $a=1$ and $b\ne0$, and conjugating by a scaling makes it $S(z)=z+1$.

Directly, the finite fixed points satisfy

$$
cz^2+(d-a)z-b=0.
$$

Including $\infty$ when appropriate, a nonidentity Möbius map consequently has one or two distinct fixed points.

Finally suppose $T$ has the unique fixed point $z_0$. With the conjugacy $R$ above,

$$
RTR^{-1}(z)=z+1,
\qquad
(RTR^{-1})^n(z)=z+n.
$$

Every finite point tends to $\infty$ on the [Riemann sphere](../../../../../riemann-sphere.md), while $\infty$ itself is fixed. Applying the continuous map $R^{-1}$ shows that

$$
\boxed{T^n(z)\longrightarrow z_0}
$$

for every $z\in\mathbb C\cup\{\infty\}$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
