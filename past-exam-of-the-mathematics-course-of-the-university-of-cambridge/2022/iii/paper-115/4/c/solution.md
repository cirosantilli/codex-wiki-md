<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The vertical tangent space of the trivial principal $\mathbb R$-bundle is spanned by $\partial_z$. Since

$$
D=\operatorname{span}\{\partial_\theta+f\partial_z,\ \partial_t+g\partial_z\}
$$

projects isomorphically onto the tangent space of $S^1\times\mathbb R$, it is always complementary to the vertical direction. It is the [horizontal distribution of a principal connection](../../../../../../horizontal-distribution-of-a-principal-connection.md) precisely when it is invariant under the principal translations $z\mapsto z+a$. The horizontal lifts of $\partial_\theta$ and $\partial_t$ are unique, so this invariance is equivalent to

$$
\partial_zf=\partial_zg=0.
$$

The functions must also be smooth and [periodic](../../../../../../periodic-function.md) in $\theta$, as is already required for them to be functions on the cylinder.

Under these conditions the connection form is

$$
\mathcal A=dz-f\,d\theta-g\,dt.
$$

It sends $\partial_z$ to $1$, is translation-invariant, and has kernel $D$, proving sufficiency as well. Since the structure group $\mathbb R$ is [abelian](../../../../../../abelian-group.md), the bracket term vanishes and

$$
\boxed{\mathcal F=d\mathcal A=(\partial_tf-\partial_\theta g)\,d\theta\wedge dt.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
