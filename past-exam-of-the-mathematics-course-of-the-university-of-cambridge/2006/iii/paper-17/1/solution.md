<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in the classical setting of [varieties](../../../../../algebraic-variety.md) over an algebraically closed [field](../../../../../field.md) $k$. A prevariety is separated when its [diagonal morphism](../../../../../diagonal-morphism.md) $\Delta_X:X\to X\times_kX$ is a [closed immersion](../../../../../closed-immersion.md); for prevarieties the diagonal is already an immersion, so this is equivalent to its image being closed. A [complete variety](../../../../../complete-variety.md) has the following closed-projection property: for every [variety](../../../../../algebraic-variety.md) $Y$, projection $X\times_kY\to Y$ maps closed subsets to closed subsets. This is [universal closedness](../../../../../universally-closed-morphism.md); since a [variety](../../../../../algebraic-variety.md) is separated and of finite type, it is equivalent to the structural map being [proper](../../../../../proper-morphism.md).

First consider [projective space](../../../../../projective-space-split.md). In two sets of homogeneous coordinates its diagonal is defined by

$$
X_iY_j-X_jY_i=0\qquad(0\le i,j\le n).
$$

These equations hold exactly when the two nonzero coordinate [vectors](../../../../../vector.md) are proportional. They are homogeneous in each coordinate set, so they define a closed subset of $\mathbb P^n\times\mathbb P^n$. On a common [affine chart](../../../../../affine-chart-of-a-variety.md), the diagonal map is the usual [closed immersion](../../../../../closed-immersion.md) defined by equality of the affine coordinates. Thus [projective space](../../../../../projective-space-split.md) is separated. If $X\hookrightarrow\mathbb P^n$ is a [projective embedding](../../../../../projective-embedding.md), its diagonal is the intersection of that closed diagonal with $X\times X$. Consequently **every [projective variety](../../../../../projective-variety.md) is separated**.

Here is an algebraic proof of completeness, rather than an appeal to projective compactness in an analytic topology. It suffices to prove [closedness of projection from projective space](../../../../../closedness-of-projection-from-projective-space.md) over an [affine chart](../../../../../affine-chart-of-a-variety.md) $Y$, with [coordinate ring](../../../../../coordinate-ring.md) $A=k[Y]$. A closed subset $Z\subseteq\mathbb P^n\times Y$ is cut out by a [homogeneous ideal](../../../../../homogeneous-ideal.md) $I\subseteq A[T_0,\ldots,T_n]$. Put $B=A[T_0,\ldots,T_n]/I$ and write $B_d$ for its degree-$d$ part. Each $B_d$ is a finitely generated $A$-module, because it is a quotient of the free [module](../../../../../module-mathematics.md) on the degree-$d$ monomials.

Suppose the fibre over $y\in Y$ is empty. The specialized homogeneous equations then have no nonzero common zero. By the [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md), some power of each $T_i$ belongs to the specialized ideal. If those powers are $T_i^{r_i}$, then every monomial of degree $d=1+\sum_i(r_i-1)$ belongs to that ideal. Hence

$$
B_d\otimes_A k(y)=0.
$$

The [Nakayama lemma](../../../../../nakayama-lemma.md) gives $(B_d)_{\mathfrak m_y}=0$. Since $B_d$ is finitely generated, there is $a\in A\setminus\mathfrak m_y$ with $(B_d)_a=0$: choose generators and multiply finitely many elements annihilating their [localizations](../../../../../localization-of-a-ring.md). On the [principal open subset](../../../../../principal-open-subscheme.md) $D(a)$, all graded pieces of degree at least $d$ vanish too, since the quotient is generated in degree one. Every fibre over $D(a)$ is therefore empty: a projective point would have a nonzero coordinate whose degree-$d$ power could not vanish. Thus the complement of the projection of $Z$ is open, proving the required closed-projection property.

An [affine open cover](../../../../../affine-open-cover.md) of an arbitrary $Y$ establishes the same result there. Finally, a closed subset of $X\times Y$ is closed in $\mathbb P^n\times Y$ when $X$ is a [projective variety](../../../../../projective-variety.md), so its image is closed by the preceding argument. Therefore

$$
\boxed{\text{Every projective variety is separated and complete.}}
$$

Over a non-algebraically-closed [field](../../../../../field.md), the corresponding statement concerns schemes or geometric points. Projection of rational points alone need not be closed, so it must not replace the completeness definition.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
