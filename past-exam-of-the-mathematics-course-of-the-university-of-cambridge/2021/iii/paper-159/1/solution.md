<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Picard group](../../../../../picard-group.md) $\operatorname{Pic}(X)$ is the set of isomorphism classes of [line bundles](../../../../../line-bundle.md) on $X$, with tensor product as addition, the trivial bundle as zero and the dual bundle as inverse. On a smooth projective surface, line bundles can be represented by divisors. The [intersection pairing on the Picard group of a surface](../../../../../intersection-pairing-on-the-picard-group-of-a-surface.md) is the symmetric bilinear map

$$
\operatorname{Pic}(X)\times\operatorname{Pic}(X)\longrightarrow\mathbb Z,
\qquad ([D],[E])\longmapsto D\cdot E,
$$

obtained by moving the divisors into proper position and counting their intersections with multiplicity.

The surface

$$
\mathbb P_{\mathbb P^1}(\mathcal O\oplus\mathcal O(1))
$$

is the first [Hirzebruch surface](../../../../../hirzebruch-surface.md) $\mathbb F_1$. If $S$ is its [negative section](../../../../../negative-section-of-a-hirzebruch-surface.md) and $F$ a fiber of the ruling, its [Picard lattice of a Hirzebruch surface](../../../../../picard-lattice-of-a-hirzebruch-surface.md) is

$$
\operatorname{Pic}(\mathbb F_1)=\mathbb ZS\oplus\mathbb ZF,
\qquad
S^2=-1,quad S\cdot F=1,quad F^2=0.
$$

Now let $\pi:X\to\mathbb P^2$ be the given nonisomorphic [birational](../../../../../birational-variety.md) morphism. A birational morphism between smooth projective surfaces factors as a nonempty sequence of point blowups. Let $H=\pi^*[\text{line}]$, and take the total transform $E$ on $X$ of the exceptional curve of the first blowup. The [intersection formula for blowing up a surface](../../../../../intersection-formula-for-blowing-up-a-surface.md) gives

$$
H^2=1,qquad E^2=-1,qquad H\cdot E=0.
$$

Therefore the nonzero [Picard group](../../../../../picard-group.md) element $H+E$ satisfies

$$
(H+E)^2=1-1=0.
$$

This is the [isotropic divisor from a nontrivial birational morphism to the projective plane](../../../../../isotropic-divisor-from-a-nontrivial-birational-morphism-to-the-projective-plane.md).

For a morphism $\phi:\mathbb P^2\to\mathbb P^n$, the pullback of the hyperplane bundle has the form

$$
\phi^*\mathcal O_{\mathbb P^n}(1)\cong\mathcal O_{\mathbb P^2}(d)
$$

for an integer $d\geq0$. If a line $\ell$ is contracted to a point, this bundle restricts trivially to $\ell$, whereas

$$
\mathcal O_{\mathbb P^2}(d)|_\ell\cong\mathcal O_{\mathbb P^1}(d).
$$

Its [degree](../../../../../degree-of-a-divisor.md) is therefore zero, so $d=0$. The homogeneous sections defining $\phi$ are then constants, and $\phi$ is constant. This proves the [morphism from the projective plane contracting a line](../../../../../morphism-from-the-projective-plane-contracting-a-line.md) criterion.

Finally choose an integer $r>C^2$ and blow up $r$ distinct points of the smooth curve $C$. For the resulting morphism $\pi:X'\to X$, let $E_1,\ldots,E_r$ be the [exceptional curves](../../../../../exceptional-divisor.md). The [strict transform](../../../../../strict-transform.md) is

$$
C'=\pi^*C-\sum_{i=1}^rE_i,
$$

and the [self-intersection after blowing up points on a smooth curve](../../../../../self-intersection-after-blowing-up-points-on-a-smooth-curve.md) formula gives

$$
(C')^2=C^2-r<0.
$$

Blowing up a smooth point of a smooth curve does not change that curve itself, so $\pi|_{C'}:C'\to C$ is an isomorphism.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 159](../../paper-159-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
