# Unimodular matrix

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unimodular_matrix)

A unimodular matrix is a square [integer matrix](integer-matrix.md) whose [determinant](determinant.md) is $1$ or $-1$. The decisive property is that its [inverse matrix](matrix-inverse-split.md) also has integer entries: multiplication by $U$ gives a [bijection](bijection.md) of the [integer lattice](integer-lattice.md) $\mathbb Z^n$ onto itself. Thus an [invertible linear map](invertible-linear-map.md) can preserve not only real coordinates but the requirement that every coordinate is an [integer](integer-split.md). These [matrices](matrix.md) form the [integral general linear group](integral-general-linear-group.md).[§7, Definition 11 and Lemma 12, printed p. 9: determinant and integer-inverse characterization](intro-to-lattice-algs-and-crypto-mastermath-spring-2018/lecture-1-introduction.md)

For an original two-dimensional example, take

$$
U=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
U^{-1}=\begin{pmatrix}1&-1\\0&1\end{pmatrix}.
$$

Its [determinant](determinant.md) is one, and it maps $(a,b)$ to $(a+b,b)$. Conversely, the integer point $(x,y)$ comes from $(x-y,y)$. For instance, $(3,2)$ has new coordinates $(1,2)$ relative to the columns $(1,0)$ and $(1,1)$. No integer point disappears, although the basis vectors and their fundamental cell change shape.

<a id="image-two-lattice-bases-generate-exactly-the-same-integer-points"></a>
![](unimodular-shear-lattice-bases.png)

**[Figure 9](#image-two-lattice-bases-generate-exactly-the-same-integer-points). Two lattice bases generate exactly the same integer points**. Original drawings of the standard basis and the columns of $U=\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$. Both displayed cells have area one. The point $(3,2)$ has coordinates $(3,2)$ in the standard basis and $(1,2)$ in the sheared basis.

This is useful whenever coordinates must remain integral. A [unimodular change of lattice basis](unimodular-change-of-lattice-basis.md) can give a shorter or more convenient description without changing the objects represented. [Smith normal form](smith-normal-form.md) and [Hermite normal form](hermite-normal-form.md) use controlled integer operations to simplify [integer matrices](integer-matrix.md); ordinary [Gaussian elimination](gaussian-elimination.md) may divide by numbers that destroy integrality. The geometric freedom is substantial: a sheared basis may look completely different while describing exactly the same infinite [set](set-split.md) of integer points.

A [determinant](determinant.md) of $-1$ is allowed too. Swapping two basis columns reverses [orientation](orientation-of-a-simplex.md) while preserving the [integer lattice](integer-lattice.md). The condition is therefore preservation of the complete integer structure, rather than a requirement to preserve orientation.

**Table of contents**

- [Integer inverse criterion for a unimodular matrix](integer-inverse-criterion-for-a-unimodular-matrix.md)
- [Unimodular change of lattice basis](unimodular-change-of-lattice-basis.md)
- [Integer determinant and sublattice index](integer-determinant-and-sublattice-index.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Automorphism of a one-dimensional complex torus](automorphism-of-a-one-dimensional-complex-torus.md)
- [Homology of an integer torus endomorphism](homology-of-an-integer-torus-endomorphism.md)
- [Integer determinant and sublattice index](integer-determinant-and-sublattice-index.md)
- [Integer matrix](integer-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/9g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/23f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/1g/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-151/4/solution.md)
- [Relator exponent-sum matrix](relator-exponent-sum-matrix.md)
- [Unimodular basis test for an integer direct summand](unimodular-basis-test-for-an-integer-direct-summand.md)
