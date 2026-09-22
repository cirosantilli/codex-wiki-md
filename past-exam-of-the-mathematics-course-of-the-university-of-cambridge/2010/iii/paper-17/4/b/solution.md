<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the standard [orientations](../../../../../../orientation-of-a-simplex.md) on the three [spheres](../../../../../../sphere.md) and the complex [orientation](../../../../../../orientation-of-a-simplex.md) on [Complex projective space](../../../../../../complex-projective-space.md). Let $h\in H^2(\mathbb{CP}^3;\mathbb Z)$ satisfy $\langle h^3,[\mathbb{CP}^3]\rangle=1$. The [cohomology ring of complex projective space](../../../../../../cohomology-ring-of-complex-projective-space.md) is $\mathbb Z[h]/(h^4)$. The [Künneth theorem](../../../../../../kunneth-theorem.md) gives

$$
H^*((S^2)^3;\mathbb Z)=\mathbb Z[a,b,c]/(a^2,b^2,c^2),
\qquad |a|=|b|=|c|=2,
\qquad \langle abc,[(S^2)^3]\rangle=1.
$$

Write the [induced map on cohomology](../../../../../../induced-map-on-cohomology.md) as $f^*h=pa+qb+rc$ with integers $p,q,r$. Naturality and [graded commutativity of the cup product](../../../../../../graded-commutativity-of-the-cup-product.md) give

$$
f^*(h^3)=(pa+qb+rc)^3=6pqr\,abc.
$$

The [mapping degree](../../../../../../degree-of-a-continuous-mapping.md) is therefore $d=6pqr$. This is the [factorial degree obstruction for products of two-spheres](../../../../../../factorial-degree-obstruction-for-products-of-two-spheres.md). Every positive value is a positive multiple of six, so **the least possible positive degree is at least $6$**.

To attain it, identify each oriented [sphere](../../../../../../sphere.md) with $\mathbb{CP}^1$. Send three projective linear forms to the coefficients of their product:

$$
F:(\mathbb{CP}^1)^3\longrightarrow\mathbb{CP}^3,
\qquad ([a_1:b_1],[a_2:b_2],[a_3:b_3])\longmapsto[c_0:c_1:c_2:c_3],
$$

where

$$
\prod_{i=1}^3(a_i z+b_i w)=c_0z^3+c_1z^2w+c_2zw^2+c_3w^3.
$$

No product of nonzero linear forms is the zero polynomial. Rescaling any factor rescales all coefficients by the same nonzero scalar. The map is therefore well-defined and is a [holomorphic map](../../../../../../holomorphic-map.md) on the products of projective charts.

Choose a homogeneous cubic with three distinct roots, all in an affine chart. Its preimages are exactly the $3!=6$ orderings of its three projective linear factors. In root coordinates, the derivative of the elementary-symmetric coefficient map has [determinant](../../../../../../determinant.md) equal, up to sign, to the [Vandermonde determinant](../../../../../../vandermonde-determinant.md), the product of the three pairwise root differences. This is nonzero for distinct roots, so all six preimages are regular. A nonsingular complex-linear derivative preserves the underlying real [orientation](../../../../../../orientation-of-a-simplex.md), since its real [determinant](../../../../../../determinant.md) is the squared absolute value of its complex [determinant](../../../../../../determinant.md). Each preimage consequently contributes $+1$ to the [mapping degree](../../../../../../degree-of-a-continuous-mapping.md). Hence

$$
\boxed{\deg F=6,\qquad d_{\min}=6.}
$$

This [polynomial multiplication map to complex projective space](../../../../../../polynomial-multiplication-map-to-complex-projective-space.md) provides the requested example without assuming that a prescribed [cohomology](../../../../../../cohomology-split.md) homomorphism is realizable by a continuous map.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
