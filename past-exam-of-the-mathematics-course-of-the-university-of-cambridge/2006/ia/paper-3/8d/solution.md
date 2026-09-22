<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Let $T(z)=(az+b)/(cz+d)$, with $ad-bc\ne0$. If $c=0$, then $d\ne0$ and

$$
T(z)=\frac ad z+\frac bd,
$$

a composition of a nonzero scaling and a translation. If $c\ne0$, rearrange the fraction as

$$
T(z)=\frac ac+\frac{bc-ad}{c^2}\frac1{z+d/c}.
$$

Thus every [Möbius transformation](../../../../../mobius-transformation.md) is a composition, in order, of translation by $d/c$, reciprocal inversion, nonzero scaling by $(bc-ad)/c^2$, and translation by $a/c$. All formulas act on the [Riemann sphere](../../../../../riemann-sphere.md), including zero and infinity. The scaling parameter must be nonzero for that factor to be a [Möbius transformation](../../../../../mobius-transformation.md).

For three distinct finite points, define the [cross-ratio](../../../../../cross-ratio.md) normalization

$$
F_z(\zeta)=\frac{(\zeta-z_1)(z_2-z_3)}{(\zeta-z_3)(z_2-z_1)}.
$$

It sends $z_1,z_2,z_3$ to $0,1,\infty$ respectively. If $z_3=\infty$, use $(\zeta-z_1)/(z_2-z_1)$; if $z_1=\infty$, use $(z_2-z_3)/(\zeta-z_3)$; if $z_2=\infty$, use $(\zeta-z_1)/(\zeta-z_3)$. These are the corresponding limits of the same formula and cover all possible triples. Form the analogous normalization $F_w$ of the target triple. Then

$$
\boxed{T=F_w^{-1}\circ F_z}
$$

has all three specified images, proving existence. For uniqueness, the quotient of any two such maps fixes the three source points. Conjugating by $F_z$ gives a [Möbius transformation](../../../../../mobius-transformation.md) fixing $0,1,\infty$. Fixing zero and infinity forces it to be $\lambda\zeta$, and fixing one forces $\lambda=1$. The quotient is identity, so the two maps are equal.

The [Möbius transformations permuting three points](../../../../../mobius-transformations-permuting-three-points.md) are therefore in one-to-one correspondence with permutations of the triple. For the normalized set the six maps and their ordered images of $(0,1,\infty)$ are

$$
\begin{array}{c|c}
T(z)&(T(0),T(1),T(\infty))\\\hline
z&(0,1,\infty)\\
1-z&(1,0,\infty)\\
1/z&(\infty,1,0)\\
1/(1-z)&(1,\infty,0)\\
z/(z-1)&(0,\infty,1)\\
(z-1)/z&(\infty,0,1).
\end{array}
$$

They realize all six permutations. The action map to the [symmetric group](../../../../../symmetric-group.md) is a homomorphism, is injective by the three-point uniqueness proof, and is onto by this list. Hence

$$
\boxed{G\cong S_3}.
$$

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
