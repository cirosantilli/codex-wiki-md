# Integer determinant and sublattice index

↑ **Parent:** [Unimodular matrix](unimodular-matrix.md)

For a square [integer matrix](integer-matrix.md) $A$ with nonzero [determinant](determinant.md), the image $A\mathbb Z^n$ is a [subgroup](subgroup.md) of the [integer lattice](integer-lattice.md). Its [index of a subgroup](index-of-a-subgroup.md) is

$$
[\mathbb Z^n:A\mathbb Z^n]=|\det A|.
$$

In particular, $A=\operatorname{diag}(2,1)$ gives all points with even first coordinate. The quotient has two [cosets](coset.md), represented by $(0,0)$ and $(1,0)$, and the fundamental cell has area two. A [determinant](determinant.md) of two therefore counts how much integer information is missing from the image.

<a id="image-an-integer-determinant-counts-missing-cosets-area-alone-cannot-preserve-integer-coordinates"></a>
![](integer-determinant-sublattice-and-rational-counterexample.png)

**[Figure 10](#image-an-integer-determinant-counts-missing-cosets-area-alone-cannot-preserve-integer-coordinates). An integer determinant counts missing cosets; area alone cannot preserve integer coordinates**. Left: $\operatorname{diag}(2,1)\mathbb Z^2$ misses odd first coordinates and has index two. Right: $\operatorname{diag}(2,1/2)$ has determinant one but maps $(0,1)$ to $(0,1/2)$, so it does not preserve the original integer lattice. Empty gray circles show reference integer points; blue filled points show the image.

The integrality hypothesis is essential. The rational [matrix](matrix.md) $R=\operatorname{diag}(2,1/2)$ has [determinant](determinant.md) one but sends $(0,1)$ to $(0,1/2)$. Its generated [Euclidean lattice](euclidean-lattice.md) has the same [covolume](covolume.md) as $\mathbb Z^2$ without being the same [integer lattice](integer-lattice.md). The [unimodular matrix](unimodular-matrix.md) criterion combines an arithmetic condition with a geometric one.

A short proof of the index formula uses [Smith normal form](smith-normal-form.md). Write $PAQ=\operatorname{diag}(d_1,\ldots,d_n)$, with $P,Q$ [unimodular matrices](unimodular-matrix.md) and positive [integers](integer-split.md) $d_i$. They preserve the relevant integer structure, so the quotient has the same size as $\prod_i\mathbb Z/d_i\mathbb Z$, namely $\prod_i d_i=|\det A|$. No assumption that the [matrix](matrix.md) is orthogonal or its basis vectors are short is needed.

## ↑ Ancestors (6)

1. [Unimodular matrix](unimodular-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
