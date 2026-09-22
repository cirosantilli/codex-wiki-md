<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

A nonidentity [Möbius transformation](../../../../../mobius-transformation.md) has either two distinct fixed points on the Riemann sphere or one double fixed point. With two fixed points, conjugate them to zero and infinity. A Möbius map fixing both is $z\mapsto kz$ with $k\ne0$. With one fixed point, conjugate it to infinity; the resulting map is affine, $z\mapsto az+b$. If $a\ne1$ it would have another fixed point, so $a=1$ and $b\ne0$. Scaling the coordinate makes it $z\mapsto z+1$. The identity is already the case $k=1$.

Define $\operatorname{tr}^2(g)$ using a determinant-one representing [matrix](../../../../../matrix.md); the two possible lifts differ by sign, so its square is well defined and invariant under conjugation. For $z\mapsto kz$ it is $k+2+k^{-1}$, while for a nontrivial translation it is four. If two nonidentity dilations have equal trace-square, their multipliers satisfy the same quadratic and are either equal or reciprocal. Inversion $z\mapsto1/z$ conjugates one reciprocal multiplier to the other. Trace-square four forces the dilation multiplier to be one, which is the excluded identity; thus every nonidentity map with that invariant is in the translation class. This proves $\boxed{g\sim h\iff\operatorname{tr}^2(g)=\operatorname{tr}^2(h)}$ for the stated nonidentity maps.

**Not every such map fixes an interior point of hyperbolic three-space.** In its upper-half-space extension, $z\mapsto z+1$ translates the horizontal coordinate and has no fixed point at positive height. A dilation extends as $(z,t)\mapsto(kz,|k|t)$, so it fixes the vertical axis only when $|k|=1$; if $|k|\ne1$, the height changes. Boundary fixed points therefore do not imply an interior fixed point.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
