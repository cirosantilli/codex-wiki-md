<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [orbit-stabilizer theorem](../../../../../../../orbit-stabilizer-theorem.md) identifies the [orbit of a group action](../../../../../../../orbit-group-theory.md) of $s$ with the [set](../../../../../../../set-split.md) of [left cosets](../../../../../../../left-coset.md) of $G_s$. Explicitly, there is a [bijection](../../../../../../../bijection.md)

$$
\boxed{G/G_s\longrightarrow G\cdot s,\qquad gG_s\longmapsto g\cdot s.}
$$

Here $G/G_s$ denotes a [set](../../../../../../../set-split.md) of [cosets](../../../../../../../coset.md); it is not asserted to be a [quotient group](../../../../../../../quotient-group.md). To prove the identification, observe that

$$
gG_s=hG_s\iff h^{-1}g\in G_s
\iff(h^{-1}g)\cdot s=s
\iff g\cdot s=h\cdot s.
$$

This equivalence proves both well-definedness and [injectivity](../../../../../../../injective-function.md). Every element of the [orbit of a group action](../../../../../../../orbit-group-theory.md) has the form $g\cdot s$, proving [surjectivity](../../../../../../../surjective-function.md).

In particular, for a [finite group](../../../../../../../finite-group.md), the [cardinalities](../../../../../../../cardinality.md) satisfy

$$
\boxed{|G\cdot s|=[G:G_s]=\frac{|G|}{|G_s|},\qquad|G|=|G\cdot s|\,|G_s|.}
$$

The last equality follows from [Lagrange's theorem](../../../../../../../lagrange-s-theorem.md) applied to the [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
