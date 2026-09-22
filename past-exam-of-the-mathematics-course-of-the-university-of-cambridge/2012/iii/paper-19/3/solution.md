<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [CW complex](../../../../../cw-complex.md) $X$, let $X^k$ be its $k$-skeleton. The [cellular chain complex](../../../../../cellular-chain-complex.md) is

$$
C_k^{\mathrm{cell}}(X)=H_k(X^k,X^{k-1};\mathbb Z)\cong\bigoplus_{\text{$k$-cells }e}\mathbb Z[e].
$$

The [isomorphism](../../../../../isomorphism.md) uses [excision](../../../../../excision-theorem.md) and $H_k(D^k,S^{k-1})\cong\mathbb Z$, after choosing an [orientation](../../../../../orientation-of-a-simplex.md) for each cell. In degree zero, take $X^{-1}=\varnothing$ and the free group on the vertices. The differential is the composite

$$
H_k(X^k,X^{k-1})\xrightarrow{\partial}H_{k-1}(X^{k-1})
\longrightarrow H_{k-1}(X^{k-1},X^{k-2}).
$$

The [long exact sequences](../../../../../long-exact-sequence.md) of skeleton pairs imply $d_{k-1}d_k=0$. The [cellular boundary formula](../../../../../cellular-boundary-formula.md) describes its coefficient at a $(k-1)$-cell as the [mapping degree](../../../../../degree-of-a-continuous-mapping.md) of the attaching [sphere](../../../../../sphere.md) after all other $(k-1)$-cells are collapsed. In degree one this is the signed difference of the two endpoints. The [cellular homology theorem](../../../../../cellular-homology-theorem.md) identifies the [homology](../../../../../homology-split.md) of this complex with [singular homology](../../../../../singular-homology.md): relative [homology](../../../../../homology-split.md) of successive skeletons is concentrated in their cell dimension, and the exact skeleton sequences leave precisely these kernels modulo images. This is the construction, rather than merely a count of cells.

The filtration $\mathbb{CP}^0\subset\mathbb{CP}^1\subset\mathbb{CP}^2$ gives one cell in each of dimensions zero, two and four, since $\mathbb{CP}^k\setminus\mathbb{CP}^{k-1}\cong\mathbb C^k$. There are no odd-dimensional cells, so every cellular differential vanishes. Thus

$$
H_k(\mathbb{CP}^2;\mathbb Z)\cong\begin{cases}\mathbb Z,&k=0,2,4,\\0,&\text{otherwise}.\end{cases}
$$

The [complex projective line](../../../../../complex-projective-line.md) has one zero-cell and one two-cell. Its product with itself has one zero-cell, two two-cells and one four-cell. Its [cellular chain complex](../../../../../cellular-chain-complex.md) again has zero differentials, giving

$$
H_k(\mathbb{CP}^1\times\mathbb{CP}^1;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0,4,\\\mathbb Z^2,&k=2,\\0,&\text{otherwise}.
\end{cases}
$$

A [homeomorphism](../../../../../homeomorphism.md) induces [isomorphisms](../../../../../isomorphism.md) on [homology groups](../../../../../homology-group.md). The second groups have different ranks, and therefore

$$
\boxed{\mathbb{CP}^2\not\cong\mathbb{CP}^1\times\mathbb{CP}^1.}
$$

Now orient the [Complex projective plane](../../../../../complex-projective-plane.md) by its complex coordinates. The inclusion of its two-skeleton $\mathbb{CP}^1$ identifies the [fundamental class](../../../../../fundamental-class.md) of a projective line with a generator $h$ of $H_2(\mathbb{CP}^2;\mathbb Z)\cong\mathbb Z$: the cellular generator has no incoming three-cell boundary and no outgoing boundary.

Take the projective lines $L_0=\{z_2=0\}$ and $L_1=\{z_1=0\}$. A path of unitary coordinate transformations takes one to the other, so their oriented [homology classes](../../../../../homology-class.md) are both $h$. They meet in the single point $[1:0:0]$. In its affine chart, let $w=z_1/z_0$ and $v=z_2/z_0$. Their [tangent spaces](../../../../../tangent-space.md) are the complex $w$-axis and complex $v$-axis, so the intersection is a [transverse intersection](../../../../../transverse-intersection.md). The ordered real bases

$$
(\partial_{\operatorname{Re}w},\partial_{\operatorname{Im}w}),
\qquad(\partial_{\operatorname{Re}v},\partial_{\operatorname{Im}v})
$$

concatenate to the complex [orientation](../../../../../orientation-of-a-simplex.md) of the ambient four-manifold. Thus the local sign is $+1$, and

$$
\boxed{h\cdot h=[L_0]\cdot[L_1]=1.}
$$

This computes the [intersection form](../../../../../intersection-form.md) using distinct representatives of the same class, avoiding an ill-defined attempt to count a line intersecting itself as a set. Bilinearity now gives

$$
\lambda(ah,bh)=ab,\qquad [\lambda]_{h}=(1),\qquad\det[\lambda]=1.
$$

Equivalently, the map $H_2\to\operatorname{Hom}(H_2,\mathbb Z)$ sending $a$ to $\lambda(a,-)$ is an [isomorphism](../../../../../isomorphism.md). This is exactly a [unimodular intersection pairing](../../../../../unimodular-intersection-pairing.md), and proves [projective lines generate a unimodular intersection form](../../../../../projective-lines-generate-a-unimodular-intersection-form.md). Reversing the ambient [orientation](../../../../../orientation-of-a-simplex.md) would change the matrix to $(-1)$ and would still be unimodular.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
