<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathfrak m$ be the maximal ideal of the [local ring](../../../../../../local-ring.md) $A$. Every open subset of $\operatorname{Spec}A$ containing the [closed point](../../../../../../closed-point.md) $\mathfrak m$ is the whole [spectrum of a commutative ring](../../../../../../spectrum-of-a-commutative-ring.md): it contains a [principal open subscheme](../../../../../../principal-open-subscheme.md) $D(a)$ with $a\notin\mathfrak m$, and that $a$ is a [unit](../../../../../../unit-in-a-ring.md), so $D(a)=\operatorname{Spec}A$.

Given $f:\operatorname{Spec}A\to\mathbb P^n_{\mathbb Z}$, choose a standard [affine open subscheme](../../../../../../affine-open-subscheme.md) $D_+(x_i)$ containing $f(\mathfrak m)$. Its preimage is consequently all of $\operatorname{Spec}A$. The [affine-target adjunction for schemes](../../../../../../affine-target-adjunction-for-schemes.md) expresses $f$ in this chart by elements $b_j\in A$ for $j\ne i$, the images of $x_j/x_i$. It is represented by [homogeneous coordinates](../../../../../../homogeneous-coordinate.md) with $a_i=1$ and $a_j=b_j$.

Conversely, a tuple $(a_0,\ldots,a_n)$ with some $a_i\in A^\times$ defines a [morphism of schemes](../../../../../../morphism-of-schemes.md) into $D_+(x_i)$ by $x_j/x_i\mapsto a_j/a_i$. Choosing another unit entry gives the same [morphism of schemes](../../../../../../morphism-of-schemes.md), since the usual [projective space](../../../../../../projective-space-split.md) transition functions identify the ratios. Multiplying all entries by one [unit](../../../../../../unit-in-a-ring.md) does not change any ratio. If two such tuples define the same [morphism of schemes](../../../../../../morphism-of-schemes.md), choose a unit entry $a_i$ in the first and a unit entry $a_j'$ in the second. In the second chart, the function $x_i/x_j$ pulls back to $a_i'/a_j'$. Because the whole map lies in $D_+(x_i)$, this ratio is a [unit](../../../../../../unit-in-a-ring.md), so $a_i'$ is a unit too. Equality in this chart gives $a_j/a_i=a_j'/a_i'$ for every $j$, hence $a_j'=(a_i'/a_i)a_j$.

**Thus the correspondence is exactly**

$$
\boxed{\operatorname{Hom}(\operatorname{Spec}A,\mathbb P^n_{\mathbb Z})
=\{(a_i):\text{some }a_i\in A^\times\}/A^\times.}
$$

This is the [projective coordinates over a local ring](../../../../../../projective-coordinates-over-a-local-ring.md) description.

For a general [ring](../../../../../../ring.md), the key open-neighbourhood argument fails. Even a tuple generating the unit ideal need not have any unit entry. For example, over $A=k\times k$ the pair $((1,0),(0,1))$ defines a map to $\mathbb P^1$ whose two points have images $[1:0]$ and $[0:1]$. Neither coordinate is a unit, and no common unit multiple changes that fact. The map lies in no single standard chart. More generally, maps into [projective space](../../../../../../projective-space-split.md) correspond to [invertible sheaf](../../../../../../line-bundle.md) quotients of $A^{n+1}$; the quotient need not be a free rank-one module outside the [local ring](../../../../../../local-ring.md) case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
