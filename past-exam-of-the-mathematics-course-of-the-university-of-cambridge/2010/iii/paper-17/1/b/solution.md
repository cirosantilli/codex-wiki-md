<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write a point of the larger [sphere](../../../../../../sphere.md) as $(u,v)\in\mathbb R^{m+1}\times\mathbb R^{n-m}$. In the complement, $v\ne0$. There is a [homeomorphism](../../../../../../homeomorphism.md)

$$
X\longrightarrow B^{m+1}_{\mathrm{open}}\times S^{n-m-1},
\qquad (u,v)\longmapsto\left(u,\frac{v}{\lVert v\rVert}\right),
$$

whose inverse sends $(u,w)$ to $(u,\sqrt{1-\lVert u\rVert^2}\,w)$. In particular the complement has a [deformation retraction](../../../../../../deformation-retraction.md) onto its transverse [sphere](../../../../../../sphere.md). Explicitly,

$$
R_t(u,v)=\frac{((1-t)u,v)}{\sqrt{(1-t)^2\lVert u\rVert^2+\lVert v\rVert^2}},
\qquad 0\le t\le1.
$$

The denominator stays positive, the homotopy stays in the complement, and points with $u=0$ remain fixed. This establishes the [homology of an equatorial sphere complement](../../../../../../homology-of-an-equatorial-sphere-complement.md). By [homotopy invariance of homology](../../../../../../homotopy-invariance-of-homology.md), its [homology](../../../../../../homology-split.md) is therefore the [homology of a sphere](../../../../../../homology-of-a-sphere.md) of dimension $d=n-m-1$:

$$
\boxed{H_j(X;\mathbb Z)=
\begin{cases}
\mathbb Z,&d\ge1\text{ and }j=0,d,\\
\mathbb Z^2,&d=0\text{ and }j=0,\\
0,&\text{otherwise}.
\end{cases}}
$$

In the codimension-one case, the complement has two contractible components; this is why degree-zero [homology](../../../../../../homology-split.md) has rank two. Equivalently, in every case its only nonzero [reduced homology](../../../../../../reduced-homology.md) is $\widetilde H_d(X;\mathbb Z)=\mathbb Z$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
