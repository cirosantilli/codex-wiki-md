<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

A [vector space](../../../../../vector-space-split.md) over the [real numbers](../../../../../real-number.md) is a [set](../../../../../set-split.md) $V$ with an [addition](../../../../../addition.md) making it an [abelian group](../../../../../abelian-group.md) and a [scalar multiplication](../../../../../scalar-multiplication.md) by $\mathbb R$ satisfying, for [scalars](../../../../../scalar.md) $a,b$ and [vectors](../../../../../vector.md) $u,v$, the identities $a(u+v)=au+av$, $(a+b)v=av+bv$, $a(bv)=(ab)v$ and $1v=v$. A [vector subspace](../../../../../vector-subspace.md) is a nonempty subset closed under [addition](../../../../../addition.md) and [scalar multiplication](../../../../../scalar-multiplication.md); a [proper vector subspace](../../../../../proper-vector-subspace.md) is one unequal to $V$. A [spanning set](../../../../../spanning-set.md) is a [set](../../../../../set-split.md) whose finite [linear combinations](../../../../../linear-combination.md) give every [vector](../../../../../vector.md) of $V$. A [basis](../../../../../basis.md) is a [linearly independent](../../../../../linear-independence.md) [spanning set](../../../../../spanning-set.md). The [dimension](../../../../../dimension-vector-space.md) is the number of [vectors](../../../../../vector.md) in a [basis](../../../../../basis.md), or its cardinality when the [basis](../../../../../basis.md) is infinite.

The [sum of vector subspaces](../../../../../sum-of-vector-subspaces.md) and their [intersection of vector subspaces](../../../../../intersection-of-vector-subspaces.md) are

$$
U+W=\{u+w:u\in U,\ w\in W\},\qquad
U\cap W=\{v\in V:v\in U\text{ and }v\in W\}.
$$

Both are [vector subspaces](../../../../../vector-subspace.md): [addition](../../../../../addition.md) and [scalar multiplication](../../../../../scalar-multiplication.md) preserve the displayed forms or simultaneous membership. The [intersection of vector subspaces](../../../../../intersection-of-vector-subspaces.md) is never empty because **$0\in U\cap W$**.

For the two given [hyperplanes](../../../../../hyperplane.md), adding and subtracting their defining equations gives $x_1=x_2$ and $x_3=x_4$. Hence

$$
U\cap W=\{(a,a,b,b):a,b\in\mathbb R\}
=\operatorname{span}\{b_1,b_2\},\quad b_1=(1,1,0,0),\quad b_2=(0,0,1,1).
$$

These two nonzero [vectors](../../../../../vector.md) are [orthogonal](../../../../../orthogonal-vectors.md), and consequently form an [orthogonal basis](../../../../../orthogonal-basis.md) of the [intersection of vector subspaces](../../../../../intersection-of-vector-subspaces.md). Put $u=(1,-1,-1,1)$ and $w=(1,-1,1,-1)$. Direct substitution gives $u\in U$, $w\in W$. Their [dot products](../../../../../dot-product.md) with $b_1,b_2$ vanish, and $u\cdot w=0$. Each defining equation of $U$ or $W$ is one nonzero linear constraint in four variables, so each [vector subspace](../../../../../vector-subspace.md) has [dimension](../../../../../dimension-vector-space.md) three. Thus each space has the indicated [orthogonal basis](../../../../../orthogonal-basis.md):

$$
\boxed{U:\ (b_1,b_2,u),\qquad W:\ (b_1,b_2,w),\qquad U+W:\ (b_1,b_2,u,w).}
$$

The last four [vectors](../../../../../vector.md) are nonzero and mutually [orthogonal](../../../../../orthogonal-vectors.md), so they are a [basis](../../../../../basis.md) of $\mathbb R^4$. They lie in $U+W$, proving $U+W=V$. The [dimension](../../../../../dimension-vector-space.md) identity is therefore verified numerically:

$$
\boxed{\dim U+\dim W=3+3=4+2=\dim(U+W)+\dim(U\cap W).}
$$

## ↑ Ancestors (11)

1. [8D](../8d.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
