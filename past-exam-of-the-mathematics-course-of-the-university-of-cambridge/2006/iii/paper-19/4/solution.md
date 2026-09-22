<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $V=\mathbb C^n$. We use [complete reducibility of compact-group representations](../../../../../complete-reducibility-of-compact-group-representations.md), and the highest-weight classification: the multiplicity of $V_\lambda$ in a completely [reducible representation](../../../../../reducible-representation.md) is the [dimension](../../../../../dimension-vector-space.md) of its weight-$\lambda$ subspace killed by all [positive root](../../../../../positive-root.md) vectors. Each [irreducible](../../../../../irreducible-representation.md) summand contributes just its one-dimensional highest-weight line to that subspace.

Symmetrizing and antisymmetrizing the three tensor factors give [invariant subspaces](../../../../../invariant-subspace.md) $\operatorname{Sym}^3V$ and $\Lambda^3V$ of $V^{\otimes3}$. The vectors $e_1^{\otimes3}$ and $e_1\wedge e_2\wedge e_3$ are [highest-weight vectors](../../../../../highest-weight-vector.md) of [weights](../../../../../weight-representation-theory.md) $(3,0,\ldots,0)$ and $(1,1,1,0,\ldots,0)$ respectively. The unitary version of the [Weyl dimension formula](../../../../../weyl-dimension-formula.md) is

$$
\dim V_\lambda=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}.
$$

It gives

$$
\dim V_{(3)}=\prod_{j=2}^n\frac{j+2}{j-1}=\binom{n+2}3,
\qquad
\dim V_{(1,1,1)}=\prod_{i=1}^3\frac{n-i+1}{4-i}=\binom n3.
$$

These are exactly the [dimensions](../../../../../dimension-vector-space.md) of the third [symmetric power](../../../../../symmetric-power.md) and [exterior power](../../../../../exterior-power.md), so each is [irreducible](../../../../../irreducible-representation.md) and occurs once in those subspaces.

The [weight](../../../../../weight-representation-theory.md) $(2,1,0,\ldots,0)$ in $V^{\otimes3}$ has basis

$$
a=e_1\otimes e_1\otimes e_2,\quad
b=e_1\otimes e_2\otimes e_1,\quad
c=e_2\otimes e_1\otimes e_1.
$$

The only [positive root](../../../../../positive-root.md) vector that acts nontrivially on this [weight space](../../../../../weight-space.md) is $E_{12}$. Acting on the [tensor product](../../../../../tensor-product.md) as the sum of its actions on the three factors, it sends each of $a,b,c$ to $e_1^{\otimes3}$. Consequently the [highest-weight vectors](../../../../../highest-weight-vector.md) in this space are precisely

$$
Aa+Bb+Cc\quad\text{with}\quad A+B+C=0.
$$

This is a two-dimensional space, so $V_{(2,1)}$ occurs exactly twice. Its [dimension](../../../../../dimension-vector-space.md) is

$$
\dim V_{(2,1)}=2\prod_{j=3}^n\frac{j+1}{j-2}
=\frac{n(n^2-1)}3.
$$

The [dimensions](../../../../../dimension-vector-space.md) of the summands already found add to

$$
\binom{n+2}3+\binom n3+2\frac{n(n^2-1)}3=n^3.
$$

Thus no other [irreducible](../../../../../irreducible-representation.md) summand can remain. We have proved the full decomposition

$$
\boxed{V^{\otimes3}\cong V_{(3,0,\ldots)}\oplus V_{(1,1,1,0,\ldots)}\oplus V_{(2,1,0,\ldots)}^{\oplus2}.}
$$

There are four summands counted with multiplicity and three distinct [isomorphism](../../../../../isomorphism.md) types.

For $n=2$, the exterior cube vanishes. The third [symmetric power](../../../../../symmetric-power.md) still has [highest weight](../../../../../highest-weight-of-a-representation.md) $(3,0)$ and [dimension](../../../../../dimension-vector-space.md) $4$, while the same two-dimensional highest-vector calculation gives two copies of the [representation](../../../../../group-representation.md) of [weight](../../../../../weight-representation-theory.md) $(2,1)$ and [dimension](../../../../../dimension-vector-space.md) $2$. It is $\det\otimes V$, since a [determinant twist](../../../../../determinant-twist.md) shifts the standard [highest weight](../../../../../highest-weight-of-a-representation.md) $(1,0)$ to $(2,1)$. Hence

$$
\boxed{(\mathbb C^2)^{\otimes3}\cong\operatorname{Sym}^3\mathbb C^2\oplus(\det\otimes\mathbb C^2)^{\oplus2},\qquad8=4+2+2.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
