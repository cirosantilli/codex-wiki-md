# Spherical law of sines

↑ **Parent:** [Spherical trigonometry](spherical-trigonometry.md)

For a nondegenerate convex minor [spherical triangle](spherical-triangle.md), with angular sides $a,b,c$ opposite interior [angles](angle.md) $A,B,C$, the [spherical law of sines](spherical-law-of-sines.md) states

$$
\frac{\sin A}{\sin a}=\frac{\sin B}{\sin b}=\frac{\sin C}{\sin c}.
$$

The [sines](sine.md) of sides refer to central [angles](angle.md), so a physical side [length](length.md) $\ell_a$ on a [sphere](sphere.md) of [radius](radius.md) $R$ must enter as $\sin(\ell_a/R)$. All six [angles](angle.md) lie in $(0,\pi)$, and the denominators are positive. The reciprocal form, $\sin a/\sin A=\sin b/\sin B=\sin c/\sin C$, is equivalent. This is Tatum's sine formula, equation 3.5.1, in [Celestial Mechanics, section 3.5: spherical sine and cosine formulas](https://www.astro.uvic.ca/~tatum/celmechs/celm3.pdf).

A short proof explains the [symmetry](symmetry-physics.md) of the [spherical law of sines](spherical-law-of-sines.md). Let $u,v,w$ be the vertex [unit vectors](unit-vector.md) at $A,B,C$. At $u$, the outgoing unit [tangent vectors](tangent-vector.md) towards $v,w$ are $t_B=(v-\cos c\,u)/\sin c$ and $t_C=(w-\cos b\,u)/\sin b$. Their [angle](angle.md) is $A$, so the magnitude of their [cross product](cross-product.md) is $\sin A$. Since both [tangent vectors](tangent-vector.md) are [orthogonal](orthogonal-vectors.md) to $u$, the [scalar triple product](scalar-triple-product.md) obeys

$$
|u\cdot(v\times w)|=\sin b\sin c\sin A=\sin c\sin a\sin B=\sin a\sin b\sin C.
$$

Dividing by $\sin a\sin b\sin c$ proves the [spherical law of sines](spherical-law-of-sines.md). Its beauty is that the same three-dimensional [scalar triple product](scalar-triple-product.md) can be calculated at any vertex, producing all three ratios at once.

For the [spherical triangle](spherical-triangle.md) worked out under the [spherical law of cosines](spherical-law-of-cosines.md), $A=90^\circ$, $b=c=60^\circ$ and $\cos a=1/4$. Hence $\sin a=\sqrt{15}/4$, and the [spherical law of sines](spherical-law-of-sines.md) gives

$$
\sin B=\frac{\sin b\sin A}{\sin a}=\frac{\sqrt3/2}{\sqrt{15}/4}=\frac2{\sqrt5}.
$$

The [inverse sine](inverse-sine.md) gives $B\approx63.434949^\circ$, but the supplementary [angle](angle.md) $116.565051^\circ$ has the same [sine](sine.md). The [spherical law of sines](spherical-law-of-sines.md) alone therefore leaves two candidates for this [angle](angle.md). The [spherical law of cosines](spherical-law-of-cosines.md), using the known three sides, gives $\cos B=1/\sqrt5>0$ and selects $63.434949^\circ$; likewise $C=B$. When only two sides and an opposite [angle](angle.md) are given, two distinct valid [spherical triangles](spherical-triangle.md) can remain. A [cosine](cosine.md) relation resolves an [inverse sine](inverse-sine.md) branch only when enough additional data are known; it does not make every ambiguous data set unique.

## ↑ Ancestors (6)

1. [Spherical trigonometry](spherical-trigonometry.md)
2. [Spherical geometry](spherical-geometry.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/5c/solution.md)
- [Spherical law of cosines](spherical-law-of-cosines.md)
- [Spherical law of sines](spherical-law-of-sines.md)
- [Spherical triangle](spherical-triangle.md)
- [Spherical trigonometry](spherical-trigonometry.md)
