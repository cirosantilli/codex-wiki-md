<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

An [inversion in a circle](../../../../../inversion-in-a-circle.md) on the [Riemann sphere](../../../../../riemann-sphere.md) is the anti-Möbius involution fixing that generalized circle pointwise. For a Euclidean circle with centre $a$ and radius $R>0$, it is

$$
\boxed{J_\Gamma(z)=a+\frac{R^2}{\overline z-\overline a},\qquad J_\Gamma(a)=\infty,\quad J_\Gamma(\infty)=a.}
$$

It reverses the argument relative to the centre and sends radius $r$ to $R^2/r$, so exactly the points of the circle are fixed. For a straight line, regarded as a circle through infinity, inversion is the ordinary reflection in that line. These formulas prove existence. For uniqueness, the composition of two anti-Möbius transformations fixing the same circle pointwise is a [Möbius transformation](../../../../../mobius-transformation.md) fixing at least three distinct points, hence the identity. Therefore the two inversions agree.

Every inversion has the form $(a\overline z+b)/(c\overline z+d)$ with $ad-bc\ne0$. Composing two conjugate-linear fractional expressions cancels the [complex conjugations](../../../../../complex-conjugation.md) and gives $(Az+B)/(Cz+D)$ with nonzero [determinant](../../../../../determinant.md). Induction proves that **an even number of inversions gives a [Möbius transformation](../../../../../mobius-transformation.md)**.

Conversely translations are compositions of reflections in parallel lines, rotations are compositions of reflections in two lines through their centre, and positive dilations are compositions of two concentric circle inversions: $J_RJ_1(z)=R^2z$. Thus every nonconstant affine map $z\mapsto az+b$ is an even composition. The map $z\mapsto1/z$ is $J_{|z|=1}$ composed with reflection in the real axis, also an even composition. If $c\ne0$, factor a general [Möbius transformation](../../../../../mobius-transformation.md) as

$$
\frac{az+b}{cz+d}=\frac ac+\frac{bc-ad}{c^2}\frac1{z+d/c}.
$$

This is a composition of affine maps and $1/z$. If $c=0$, it is already affine. **Every [Möbius transformation](../../../../../mobius-transformation.md) is therefore a composition of an even number of inversions**, with the identity represented by zero inversions or by any inversion repeated twice.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
