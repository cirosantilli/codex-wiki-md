<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) means fixed position relative to the rotating wire: $r=a$ and $z=f(a)$ are constant, while $\theta=\omega t$ continues to change. Substituting $\dot r=\ddot r=0$ into the equation gives

$$
\boxed{f'(a)=\frac{a\omega^2}{g}.}
$$

For the [linear stability](../../../../../../linear-stability.md) calculation, set $r=a+\epsilon$ and retain terms of first order in $\epsilon$ and $\dot\epsilon$. The term $\dot r^2$ contributes only at second order, and variation of the factor multiplying $\ddot\epsilon$ also contributes only at second order. Thus

$$
\boxed{\left(1+f'(a)^2\right)\ddot\epsilon
=\left(\omega^2-gf''(a)\right)\epsilon.}
$$

The two strict sign cases are treated in the following parts. If $gf''(a)=\omega^2$, this [linearization](../../../../../../linearization.md) has no restoring term and higher orders are needed to classify the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md).

For the specified wire,

$$
f'(r)=\frac{\omega^2r}{g}-\sin(r/b),\qquad
f''(r)=\frac{\omega^2}{g}-\frac1b\cos(r/b).
$$

Hence the complete set of positive [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) radii is

$$
\boxed{a_n=n\pi b,\qquad n=1,2,3,\ldots.}
$$

At $a_n$,

$$
\left[1+\left(\frac{n\pi b\omega^2}{g}\right)^2\right]\ddot\epsilon
=\frac gb(-1)^n\epsilon.
$$

Therefore **odd $n$ give a [stable equilibrium](../../../../../../stable-equilibrium.md), and even $n$ give an [unstable equilibrium](../../../../../../unstable-equilibrium.md)**. There is no degenerate sign case in this example. The corresponding heights are $f(a_n)=\omega^2n^2\pi^2b^2/(2g)+b(-1)^n$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
