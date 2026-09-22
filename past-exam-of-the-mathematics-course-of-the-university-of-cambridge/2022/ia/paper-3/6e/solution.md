<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

A [Möbius transformation](../../../../../mobius-transformation.md) of the [Riemann sphere](../../../../../riemann-sphere.md) is a map

$$
z\longmapsto\frac{az+b}{cz+d},
\qquad ad-bc\ne0,
$$

with its natural values at the pole and at infinity.

For three distinct points $z_1,z_2,z_3$, define

$$
T_z(\zeta)=
\frac{(\zeta-z_2)(z_1-z_3)}
     {(\zeta-z_3)(z_1-z_2)}.
$$

The usual limiting conventions cover an infinite $z_i$. This Möbius transformation sends $(z_1,z_2,z_3)$ to $(1,0,\infty)$. Defining $T_w$ similarly, the map

$$
\boxed{f=T_w^{-1}\circ T_z}
$$

sends $z_i$ to $w_i$. If two Möbius transformations do so, their quotient fixes $0,1,\infty$. A Möbius transformation fixing infinity is affine, and fixing zero and one then makes it the identity. This proves uniqueness.

With this convention, the [cross-ratio](../../../../../cross-ratio.md) is

$$
[z_1,z_2,z_3,z_4]
=T_z(z_4)
=\frac{(z_4-z_2)(z_1-z_3)}
{(z_4-z_3)(z_1-z_2)}.
$$

Substitution shows that translations, nonzero scalings, and inversion preserve it; since these generate the Möbius group, every Möbius transformation preserves cross-ratios.

Conversely, suppose a [bijection](../../../../../bijection.md) $f$ of the Riemann sphere preserves every cross-ratio. Let $m$ be the unique Möbius transformation agreeing with $f$ at three chosen points $z_1,z_2,z_3$. For any other $z$, preservation by $f$ and $m$ gives

$$
[z_1,z_2,z_3,z]
=[f(z_1),f(z_2),f(z_3),f(z)]
=[f(z_1),f(z_2),f(z_3),m(z)].
$$

The last coordinate in a cross-ratio with three fixed distinct entries is injective, so $f(z)=m(z)$. The equality already holds at the three base points, hence $f=m$ everywhere and $f$ is Möbius.

Finally, the map $z\mapsto a\overline z+b$ is constant when $a=0$ and therefore is not Möbius. If $a\ne0$, it is bijective and fixes infinity. Were it Möbius, it would have the affine form $\alpha z+\beta$. Equality on real $z$ forces $\alpha=a$ and $\beta=b$, whereas equality at $z=i$ would require $ai=-ai$, contradicting $a\ne0$. Thus

$$
\boxed{\text{there are no such }a,b}.
$$

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
