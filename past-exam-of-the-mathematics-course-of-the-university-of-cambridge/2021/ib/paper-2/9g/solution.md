<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

A subset $S\subseteq M$ freely generates $M$ when every $m\in M$ has a unique expression

$$
m=\sum_{s\in S}r_ss
$$

with $r_s\in R$ and only finitely many nonzero coefficients. Equivalently, $S$ is a [basis of a module](../../../../../basis-of-a-module.md) and $M$ is the [free module](../../../../../free-module.md) on $S$.

If $S$ freely generates $M$ and $f:S\to N$ is any function, define

$$
\phi\left(\sum_sr_ss\right)=\sum_sr_sf(s).
$$

Unique coordinates make $\phi$ well defined; it is an $R$-module homomorphism and is the only extension of $f$. Conversely, apply the proposed universal property to the free module $F=R^{(S)}$ and the inclusion of $S$ into $M$. It gives maps $F\to M$ and $M\to F$ extending the corresponding functions on $S$. Uniqueness makes both composites identity maps, so $M\cong F$ and $S$ freely generates $M$. This is the [universal property of a free module](../../../../../universal-property-of-a-free-module.md).

Now let $T$ generate the free module $M$ and $|T|=m$. Choose a [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak m$ of the nontrivial ring $R$. Then $k=R/\mathfrak m$ is a field, and

$$
M/\mathfrak mM
$$

is a $k$-vector space. The images of a basis $S$ of $M$ form a vector-space basis, while the images of $T$ span it. Therefore

$$
|S|=\dim_k(M/\mathfrak mM)\leq m.
$$

In particular $S$ is finite. Applying this result in both directions to two finite bases shows that they have equal cardinality, the [rank of a free module](../../../../../rank-of-a-free-module.md) $\operatorname{rk}M$.

A Euclidean domain is a [principal ideal domain](../../../../../principal-ideal-domain.md). By the [submodule theorem for free modules over a principal ideal domain](../../../../../submodule-theorem-for-free-modules-over-a-principal-ideal-domain.md), every submodule $N$ of the finite-rank free module $M$ is free. Since a basis of $M$ generates it, the preceding inequality applied in the standard proof gives

$$
\boxed{\operatorname{rk}N\leq\operatorname{rk}M}.
$$

The [primary decomposition theorem for finitely generated modules over a principal ideal domain](../../../../../primary-decomposition-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) states that

$$
M\cong R^r\oplus
\bigoplus_{p}\bigoplus_j R/(p^{\,e_{p,j}}),
$$

where $p$ ranges over finitely many nonassociate irreducibles and the positive exponents are uniquely determined up to order. Equivalently, the torsion part decomposes into its primary cyclic summands.

Let $H$ be a finite subgroup of the multiplicative group of a field. It is a finite abelian group, hence the theorem over $\mathbb Z$ gives an invariant-factor decomposition

$$
H\cong C_{d_1}\times\cdots\times C_{d_r},
\qquad d_1\mid\cdots\mid d_r.
$$

Its exponent is $d_r$, so every element of $H$ is a root of $X^{d_r}-1$. A degree-$d_r$ polynomial over a field has at most $d_r$ roots, whence

$$
|H|\leq d_r.
$$

But $d_r\leq|H|$, and equality forces all earlier factors to be trivial. Thus

$$
\boxed{H\text{ is cyclic}}.
$$

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
