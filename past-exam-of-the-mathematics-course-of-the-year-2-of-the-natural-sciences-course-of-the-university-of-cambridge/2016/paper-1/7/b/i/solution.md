<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the branch of $\sqrt{(\zeta+1)(\zeta-1)}$ [holomorphic](../../../../../../holomorphic-function-split.md) in the [upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) whose boundary value at zero is $+i$. Then

$$
f'(\zeta)=\frac1{\sqrt{1-\zeta^2}},\qquad f(0)=0,
$$

and [integration](../../../../../../integral-split.md) gives $\boxed{z=\arcsin\zeta,\quad\zeta=\sin z}$ on this branch. The normalization and intended upper-half-plane image fix the otherwise ambiguous square-root sign.

To see the image, put $z=x+iy$. For $-\pi/2<x<\pi/2$ and $y>0$,

$$
\operatorname{Im}\sin z=\cos x\sinh y>0.
$$

The bottom edge maps monotonically onto $[-1,1]$. The right wall maps by $\sin(\pi/2+iy)=\cosh y$ onto $[1,\infty)$, and the left by $\sin(-\pi/2+iy)=-\cosh y$ onto $(-\infty,-1]$. These boundaries describe the [conformal map of a vertical half-strip by sine](../../../../../../conformal-map-of-a-vertical-half-strip-by-sine.md).

For completeness, the map is one-to-one in the interior: equality of two sine values forces arguments differing by $2\pi m$ or summing to $(2m+1)\pi$, and neither alternative yields two distinct points in this half-strip. It is onto the [upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) as well. Setting $w=e^{iz}$ gives $w^2-2i\zeta w-1=0$; the root product is $-1$, and no root lies on $|w|=1$ because that would make $\zeta$ real. Thus exactly one root has $|w|<1$. The identity $\operatorname{Im}\zeta=(\operatorname{Re}w)(|w|^{-2}-1)/2$ then gives $\operatorname{Re}w>0$, so $z=-i\log w$ belongs to the half-strip. The closure gives the stated boundary-inclusive region; [holomorphy](../../../../../../holomorphic-function-split.md) is understood in its open interior.

In this region the transformed function is $G(z)=\log(2+\sin z)$. Its only finite intrinsic [branch point](../../../../../../branch-point.md) in the closure occurs where $2+\sin z=0$:

$$
\boxed{z_*=-\frac\pi2+i\operatorname{arcosh}2=-\frac\pi2+i\log(2+\sqrt3),\qquad\zeta_*=-2.}
$$

It lies on the left boundary. There are no singularities in the open half-strip. The points $\zeta=\pm1$, where $f'$ diverges, map to the bottom corners; $G$ is [holomorphic](../../../../../../holomorphic-function-split.md) through those corners since $2+\sin z\neq0$ there.

For the principal logarithm, the boundary segment $z=-\pi/2+iy$, $y\geq\operatorname{arcosh}2$, is the preimage of its cut $\zeta\leq-2$. Points on that cut above $z_*$ admit local [analytic continuation](../../../../../../analytic-continuation.md) after changing branch; $z_*$ itself is the genuine logarithmic [branch point](../../../../../../branch-point.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
