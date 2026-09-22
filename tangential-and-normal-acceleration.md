# Tangential and normal acceleration

↑ **Parent:** [Normal and tangential components](normal-and-tangential-components.md)

For a twice continuously differentiable [regular curve](regular-curve.md) describing motion, let $v=\|r'(t)\|>0$, $T=r'/v$, and let $N$ be the [principal normal vector](principal-normal-vector.md) where the [curvature](curvature.md) $\kappa$ is positive. Differentiating the [velocity vector](velocity-vector.md) $r'=vT$ gives

$$
\boxed{a=r''=\dot v\,T+\kappa v^2N.}
$$

The [tangential component](tangential-component.md) changes the [speed](speed.md); the [normal component](normal-component.md) changes the direction of the [velocity vector](velocity-vector.md). A particle can therefore have nonzero [acceleration](acceleration.md) at constant [speed](speed.md), as in [circular motion](circular-motion.md) with constant [speed](speed.md). The formula follows from $dT/dt=(dT/ds)(ds/dt)=\kappa vN$ and the [product rule](product-rule.md). When $\kappa=0$, the normal contribution vanishes even though the [principal normal vector](principal-normal-vector.md) is undefined there. [Widnall and Peraire, MIT 16.07 Lecture 6: intrinsic coordinates, pp. 1–4](https://ocw.mit.edu/courses/16-07-dynamics-fall-2009/84852a46fa77de9a750245ceb761255a_MIT16_07F09_Lec06.pdf)

In dimensionless coordinates, take $r(t)=(t,t^2)$. At $t=1$,

$$
v=\sqrt5,\qquad
\dot v=\frac4{\sqrt5},\qquad
\kappa=\frac{2}{5\sqrt5},\qquad
T=\frac{(1,2)^T}{\sqrt5},\qquad
N=\frac{(-2,1)^T}{\sqrt5}.
$$

The resulting [vector](vector.md) components are

$$
a_T=\left(\frac45,\frac85\right)^T,\qquad
a_N=\left(-\frac45,\frac25\right)^T,\qquad
\boxed{a_T+a_N=(0,2)^T=r''(1).}
$$

Both increasing [speed](speed.md) and turning contribute to the same [acceleration](acceleration.md).

<a id="image-acceleration-on-a-parabola-has-both-tangential-and-normal-parts"></a>
![](tangent-normal-acceleration-on-parabola.png)

**[Figure 6](#image-acceleration-on-a-parabola-has-both-tangential-and-normal-parts). Acceleration on a parabola has both tangential and normal parts**. At $t=1$, the [acceleration](acceleration.md) $(0,2)^T$ is the sum of $(4/5,8/5)^T$ tangent to the path and $(-4/5,2/5)^T$ normal to it. This is a dimensionless mathematical trajectory.

## ↑ Ancestors (8)

1. [Normal and tangential components](normal-and-tangential-components.md)
2. [Unit normal](unit-normal.md)
3. [Normal vector](normal-vector.md)
4. [Differential geometry](differential-geometry-split.md)
5. [Geometry and topology](geometry-and-topology-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
