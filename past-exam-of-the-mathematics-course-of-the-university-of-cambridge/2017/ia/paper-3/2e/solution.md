<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

A [subgroup](../../../../../subgroup.md) $H$ of a [group](../../../../../group-split.md) $G$ is a [normal subgroup](../../../../../normal-subgroup.md) when $gHg^{-1}=H$ for every $g\in G$, equivalently $gH=Hg$. The [quotient group](../../../../../quotient-group.md) $G/H$ has the left [cosets](../../../../../coset.md) as elements, with $(gH)(kH)=gkH$, identity $H$ and inverse $(gH)^{-1}=g^{-1}H$. Normality makes this multiplication independent of representatives.

The [first isomorphism theorem for groups](../../../../../first-isomorphism-theorem.md) says that for a [group homomorphism](../../../../../group-homomorphism.md) $\varphi:G\to K$, its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is normal and

$$
G/\ker\varphi\cong\operatorname{im}\varphi,
\qquad g\ker\varphi\longmapsto\varphi(g).
$$

The image is taken with the induced [group operation](../../../../../group-operation.md); surjectivity onto all of $K$ is not required.

For the given [upper triangular matrices](../../../../../upper-triangular-matrix.md), take diagonal entries:

$$
\varphi\!\begin{pmatrix}a&b\\0&d\end{pmatrix}=(a,d)
\quad\text{in}\quad\mathbb R^\times\times\mathbb R^\times.
$$

The target is a [direct product of groups](../../../../../direct-product-of-groups.md), with multiplication of nonzero [real numbers](../../../../../real-number.md) in each coordinate. Indeed the product of two such [matrices](../../../../../matrix.md) has diagonal $(aa',dd')$, proving the [group homomorphism](../../../../../group-homomorphism.md) property. Any pair of nonzero diagonal entries is attained by a [diagonal matrix](../../../../../diagonal-matrix.md), so $\varphi$ is surjective. Its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) consists precisely of the [matrices](../../../../../matrix.md) with $a=d=1$, namely $H$. Hence

$$
\boxed{H\trianglelefteq G,\qquad G/H\cong(\mathbb R^\times)^2}
$$

with coordinatewise multiplication, not addition on $\mathbb R^2$.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
