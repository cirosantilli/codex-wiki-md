<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The [Poincare ball model](../../../../../poincare-ball-model.md) has ideal boundary the [Riemann sphere](../../../../../riemann-sphere.md). To construct the [hyperbolic extension of a Möbius transformation](../../../../../hyperbolic-extension-of-a-mobius-transformation.md), conjugate the ball to the upper half-space model with coordinates $(z,t)\in\mathbb C\times(0,\infty)$ and metric $(|dz|^2+dt^2)/t^2$. The generators of the [Möbius group](../../../../../mobius-group.md) extend as

$$
z\mapsto z+b:\ (z,t)\mapsto(z+b,t),\qquad
z\mapsto\lambda z:\ (z,t)\mapsto(\lambda z,|\lambda|t),
$$

and

$$
z\mapsto-1/z:\ (z,t)\mapsto
\frac{(-\overline z,t)}{|z|^2+t^2}.
$$

Translations and similarities plainly preserve the metric; Euclidean inversion rescales both the squared Euclidean line element and $t^2$ by the same factor, proving the last case. Composition gives the unique orientation-preserving hyperbolic extension. Equivalently, for a determinant-one matrix its upper half-space formula is

$$
z'=\frac{(az+b)\overline{(cz+d)}+a\overline c\,t^2}
{|cz+d|^2+|c|^2t^2},\qquad
t'=\frac{t}{|cz+d|^2+|c|^2t^2}.
$$

An [isometry](../../../../../isometry.md) fixing the ball origin acts on its tangent space by an orientation-preserving orthogonal transformation; radial [geodesics](../../../../../geodesic.md) then show that the whole map is that ordinary rotation. Conversely every rotation preserves the ball metric. On the sphere these are exactly the projective special-unitary maps

$$
\boxed{z\mapsto\frac{az+b}{-\overline b\,z+\overline a},
\qquad |a|^2+|b|^2=1,}
$$

the image of $SU(2)$ modulo its central signs.

A hyperbolic line is determined by its unordered pair of ideal endpoints. It is invariant precisely when that pair is preserved as a set. A nonidentity parabolic map has one fixed point, and its square also has one, so it cannot fix or interchange two distinct endpoints. Every nonparabolic nonidentity map has two fixed points, and their joining line is invariant.

More precisely, normalize the latter map to $z\mapsto\lambda z$. Unless $\lambda=-1$, any invariant pair must consist of zero and infinity: a swapped pair would be fixed pointwise by the square, whose only fixed points remain zero and infinity when $\lambda^2\ne1$. This proves uniqueness for every nonidentity map except an elliptic half-turn. For $\lambda=-1$, every pair $\{z,-z\}$ is also invariant, giving infinitely many additional lines, besides the fixed-point axis. The identity preserves every line. Thus

$$
\boxed{\begin{gathered}
\text{An invariant line exists exactly for nonparabolic maps, including the identity;}\\
\text{it is unique except for the identity and elliptic half-turns.}
\end{gathered}}
$$

Here the uniqueness statement includes hyperbolic translations, genuine loxodromic maps and elliptic rotations through angles other than a half-turn.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
