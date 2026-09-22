<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Assume $T$ is a [group homomorphism](../../../../../../../group-homomorphism.md). For any $a,b\in G$, expanding $(ab)^3=a^3b^3$ and cancelling the initial $a$ and final $b$ gives the useful identity

$$
\boxed{(ba)^2=a^2b^2.}\qquad\text{(1)}
$$

We also need a consequence of compatibility with [conjugation](../../../../../../../conjugation.md). Calculate the cube of $gzg^{-1}$ in two ways:

$$
gz^3g^{-1}=(gzg^{-1})^3
=T(g)T(z)T(g)^{-1}=g^3z^3g^{-3}.
$$

Cancelling shows $g^2z^3=z^3g^2$. Thus the square of every element of $G$ commutes with every element of the [image of a group homomorphism](../../../../../../../image-of-a-group-homomorphism.md) $J=T(G)$.

Now take any $x,y\in J$. In particular $x^2y=yx^2$. Applying (1) to $x,y$ and then using this commutation gives

$$
yxyx=x^2y^2,
\qquad
xyx=y^{-1}x^2y^2=x^2y,
\qquad
yx=xy.
$$

This proves the [abelian image of a cubing homomorphism](../../../../../../../abelian-image-of-a-cubing-homomorphism.md) property. Since the [image of a group homomorphism](../../../../../../../image-of-a-group-homomorphism.md) is a [subgroup](../../../../../../../subgroup.md), $\boxed{T(G)\text{ is an abelian group}}$.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [b](../../b.md)
3. [5](../../../5.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
