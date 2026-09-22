<h1 id="15f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Constant [Gaussian curvature](../../../../../../gaussian-curvature.md) one gives $f''+f=0$, so, after a shift of the arc-length parameter, $f=C\cos u$ with $C>0$ on an interval contained in $(-\pi/2,\pi/2)$. To close the surface by adding only two points, the limiting parallels at both ends must collapse to points on the axis. If an end had limiting radius $f>0$, it would contribute a whole missing circle, which two added points cannot supply. Thus the parameter interval is the full interval between consecutive zeros, and its two ends are $u=\pm\pi/2$.

At a smooth axis point the tangent plane of a [surface of revolution](../../../../../../surface-of-revolution.md) is invariant under all rotations about the axis, so it must be horizontal. The unit meridian tangent must consequently have $g'\to0$ and $|f'|\to1$ there. But $|f'(\pm\pi/2)|=C$, so smoothness forces **$C=1$**. The arc-length identity also illustrates the alternatives: $C>1$ prevents reaching either zero with real $g'$, while $0<C<1$ gives a nonhorizontal limiting meridian and a conical singularity.

Now $g'^2=1-f'^2=\cos^2u$. On the connected interior, $g'$ has one fixed sign because $\cos u>0$. Therefore $g=g_0\pm\sin u$, and

$$
\boxed{f^2+(g-g_0)^2=\cos^2u+\sin^2u=1.}
$$

The revolved surface is the unit sphere centered at $(0,0,g_0)$, with only its two poles $(0,0,g_0\pm1)$ omitted. Those points are antipodal. This proves the claim using [smooth endpoint criterion for a surface of revolution](../../../../../../smooth-endpoint-criterion-for-a-surface-of-revolution.md), without integrating a general square root.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15F](../../15f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
