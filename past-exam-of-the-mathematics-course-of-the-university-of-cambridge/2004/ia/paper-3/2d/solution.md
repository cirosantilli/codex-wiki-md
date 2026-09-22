<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

The [Möbius group](../../../../../mobius-group.md) consists of maps $z\mapsto(az+b)/(cz+d)$ with $ad-bc\ne0$, acting on the [Riemann sphere](../../../../../riemann-sphere.md) $\widehat{\mathbb C}=\mathbb C\cup\{\infty\}$. Proportional matrices represent the same map. Thus it is $\mathrm{PGL}_2(\mathbb C)$, equivalently $\mathrm{PSL}_2(\mathbb C)$ after normalizing the determinant. A zero denominator gives the image $\infty$, while $\infty$ maps to $a/c$ when $c\ne0$ and stays at infinity when $c=0$.

Fixing both zero and infinity forces $b=c=0$, leaving $z\mapsto\lambda z$ with $\lambda\ne0$. Composition multiplies the parameters, giving a bijective [group homomorphism](../../../../../group-homomorphism.md) from the [multiplicative group of nonzero complex numbers](../../../../../complex-multiplicative-group.md) to this [pointwise stabilizer](../../../../../pointwise-stabilizer.md).

For the other pair, take $T(z)=z/(1-z)$, which sends zero to zero and one to infinity. Conjugate the scaling subgroup by this [Möbius transformation](../../../../../mobius-transformation.md):

$$
\boxed{T^{-1}(\lambda T(z))=\frac{\lambda z}{1+(\lambda-1)z},\qquad \lambda\in\mathbb C^*.}
$$

Every map fixing zero and one arises this way. Composition again multiplies $\lambda$, proving **both subgroups are isomorphic to $\mathbb C^*$**. This is the [Möbius pointwise stabilizer of two points](../../../../../mobius-pointwise-stabilizer-of-two-points.md); conjugation changes the selected fixed points without changing its group structure.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
