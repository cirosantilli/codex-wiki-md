<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\phi:C\setminus S\to\mathbb P^n$ be the given algebraic [morphism of algebraic varieties](../../../../../../morphism-of-algebraic-varieties.md). Its value at the generic point supplies homogeneous coordinates $[h_0:\cdots:h_n]$ with $h_i\in k(C)$, not all zero. Thus it defines a [rational map of projective varieties](../../../../../../rational-map-of-projective-varieties.md) on $C$.

Fix a missing point $p\in S$. The [local ring of a smooth algebraic curve](../../../../../../local-ring-of-a-smooth-algebraic-curve.md) at $p$ is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md) $A=\mathcal O_{C,p}$, with [uniformizer](../../../../../../uniformizer.md) $t$ and [valuation](../../../../../../valuation.md) $v_p$. Put

$$
m=\min_{h_i\ne0}v_p(h_i),\qquad a_i=t^{-m}h_i.
$$

Zero coordinates remain zero. Every $a_i$ is in $A$, and some $a_j$ is a unit because its valuation is zero. Choose a neighborhood $U$ of $p$ on which all $a_i$ are regular and $a_j$ remains nonvanishing; this is possible because membership in the local ring means regularity on a neighborhood. The affine target-chart coordinates

$$
\frac{a_i}{a_j}\qquad(i\ne j)
$$

are regular on $U$, so they define a [morphism of algebraic varieties](../../../../../../morphism-of-algebraic-varieties.md) $U\to\mathbb P^n$. At $p$ its homogeneous value is $[a_0(p):\cdots:a_n(p)]$, well-defined because $a_j(p)\ne0$.

Multiplication of all homogeneous coordinates by the same nonzero [rational function](../../../../../../rational-function.md) does not change their projective point. Thus this local morphism agrees with the original one on the common dense open where their coordinates were chosen. They agree throughout the overlap: the target's diagonal is closed, being defined in homogeneous coordinate pairs by $T_iU_j-T_jU_i=0$ for all $i,j$. Thus the equalizer is closed and contains that dense open. Apply this construction at each point of the finite set $S$ and glue with the original morphism. The same closed-diagonal argument proves uniqueness. Therefore

$$
\boxed{\phi\text{ extends uniquely to a morphism }C\to\mathbb P^n.}
$$

This gives the [extension of a rational map from a smooth projective curve](../../../../../../extension-of-a-rational-map-from-a-smooth-projective-curve.md) by explicit local coordinates. The mechanism is the one-dimensional smooth local ring: it permits removal of the smallest common pole order while leaving at least one unit coordinate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
