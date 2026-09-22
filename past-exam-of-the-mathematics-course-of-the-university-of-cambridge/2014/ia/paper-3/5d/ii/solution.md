<h1 id="5d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Place the [cube](../../../../../../cube.md) at the origin with face normals $\pm e_1,\pm e_2,\pm e_3$, and label opposite faces by $(1,2),(3,4),(5,6)$. Every cube symmetry is a [signed permutation matrix](../../../../../../signed-permutation-matrix.md): there are $2^3\,3!=48$ choices. Its [group action](../../../../../../group-action.md) on faces is faithful because fixing all faces fixes all their normal directions. Central inversion $-I$ exchanges every opposite pair and therefore acts as $h$. Since $-I$ commutes with every linear cube symmetry, the face-action image lies in $C_{S_6}(h)$. The preceding count gives $|C_{S_6}(h)|=48$, so the faithful face action is onto this [centraliser](../../../../../../centralizer.md):

$$
\boxed{G\cong C_{S_6}(h).}
$$

For the remaining isomorphism, let $R$ be the [rotational symmetry group of a cube](../../../../../../rotational-symmetry-group-of-a-cube.md). Half the signed permutation [matrices](../../../../../../matrix.md) have [determinant](../../../../../../determinant.md) $1$, so $|R|=24$. Central inversion has [determinant](../../../../../../determinant.md) $-1$, and every orientation-reversing symmetry is $(-I)r$ for a unique $r\in R$. Since $-I$ is central and $R\cap\{I,-I\}=\{I\}$, multiplication gives a [direct product of groups](../../../../../../direct-product-of-groups.md):

$$
G\cong C_2\times R.
$$

The [group action](../../../../../../group-action.md) of $R$ on the four body diagonals is faithful. To prove this, choose direction [vectors](../../../../../../vector.md) $(1,1,1),(1,-1,-1),(-1,1,-1),(-1,-1,1)$. They span $\mathbb R^3$, and their only linear relation is that their sum is zero. A rotation fixing all four diagonal lines sends each listed [vector](../../../../../../vector.md) to itself or its negative. Applying the relation forces all four signs to agree. The all-negative choice is $-I$, which is not in $R$, so the rotation is the identity. Thus $R$ embeds in $S_4$; both have order $24$, giving $R\cong S_4$. Finally $C_{S_6}(g)\cong C_2\times S_4$ from part (i). Consequently

$$
\boxed{G\cong C_2\times S_4\cong C_{S_6}(g).}
$$

The [direct-product decomposition of the cube symmetry group](../../../../../../direct-product-decomposition-of-the-cube-symmetry-group.md) supplies the second isomorphism, while the first comes from the specified face action.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
