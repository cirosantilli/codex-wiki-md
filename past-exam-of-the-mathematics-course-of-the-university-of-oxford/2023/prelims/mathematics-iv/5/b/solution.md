<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $a>0$ and the intended horizontal launch around a parallel of the [surface of revolution](../../../../../../surface-of-revolution.md): $\dot r(0)=\dot z(0)=0$, $a\dot\theta(0)=v$. Then $h=av$ and $E=v^2/2+gf(a)$. Since $\dot z=f'(r)\dot r$, the conserved [energy](../../../../../../energy-split.md) becomes

$$
\frac12[1+f'(r)^2]\dot r^2+U(r)=E,\qquad
U(r)=\frac{a^2v^2}{2r^2}+gf(r).
$$

Here $U$ is the [radial effective potential on a surface of revolution](../../../../../../radial-effective-potential-on-a-surface-of-revolution.md). Rearrangement gives

$$
\boxed{D(r):=\frac{v^2}{2g}(r^2-a^2)+r^2[f(a)-f(r)]
=\frac{r^2}{2g}[1+f'(r)^2]\dot r^2\geq0.}
$$

For a nonconstant bounded radial motion with $v>0$, there must be another finite radial bound $b\ne a$ satisfying $D(b)=0$, equivalently

$$
\boxed{\frac{v^2}{g}=\frac{2b^2[f(b)-f(a)]}{b^2-a^2}.}
$$

The interval between the radial bounds must be dynamically accessible: $D\geq0$ inside, and a simple endpoint must have a forbidden region $D<0$ beyond it. Equivalently the motion must lie in a bounded part of $\{r>0:U(r)\leq E\}$ separated from escape by a potential barrier. When $f$ stays finite near zero and $v>0$, the [centrifugal barrier](../../../../../../centrifugal-barrier.md) already excludes $r=0$; an outer barrier is the additional requirement. An arbitrary second algebraic root on a disconnected allowed branch would not establish boundedness.

The initial radial [acceleration](../../../../../../acceleration.md), obtained by projecting [Newton's second law](../../../../../../newton-s-second-law.md) along $\mathbf e_r+f'(a)\mathbf e_z$, is

$$
\ddot r(0)=\frac{v^2/a-gf'(a)}{1+f'(a)^2}.
$$

Thus $v^2/g>af'(a)$ starts the particle outward, and $v^2/g<af'(a)$ starts it inward. Equality gives the exact [circular orbit](../../../../../../circular-orbit.md) $r=a$ and needs no second distinct radial bound. A double root at a different radius can instead be approached asymptotically: this [separatrix](../../../../../../separatrix.md) is bounded, although the radial motion is not periodic. If $v=0$, the [centrifugal barrier](../../../../../../centrifugal-barrier.md) disappears and the particle may pass through the axis, still with bounded $r$.

The source leaves a direction ambiguity at points where $f'(a)=0$: every horizontal tangent direction is then possible, so “projected horizontally” alone does not imply $h=av$. The displayed inequality uses the azimuthal launch specified above; at $f'(a)\ne0$ that direction is forced by horizontality and tangency.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
