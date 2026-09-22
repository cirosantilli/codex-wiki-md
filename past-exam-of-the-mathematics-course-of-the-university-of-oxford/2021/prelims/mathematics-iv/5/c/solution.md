<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Initially $\dot r=0$ also gives $\dot z=H'(b)\dot r=0$. Thus the initial [velocity](../../../../../../velocity.md) is azimuthal, with $|h|=bv$. By [conservation of energy](../../../../../../conservation-of-energy.md), the supplied [mechanical energy](../../../../../../mechanical-energy.md) divided by $m/2$ gives

$$
[1+(H'(r))^2]\dot r^2+\frac{b^2v^2}{r^2}+2gH(r)=v^2+2gH(b).
$$

The first term is nonnegative. Consequently

$$
\boxed{2gH(r)+\frac{b^2v^2}{r^2}\leq2gH(b)+v^2.}
$$

For a positive launch [speed](../../../../../../speed.md) $v>0$, introduce twice the [radial effective potential on a surface of revolution](../../../../../../radial-effective-potential-on-a-surface-of-revolution.md) per unit [mass](../../../../../../mass.md),

$$
S(r)=2gH(r)+\frac{b^2v^2}{r^2},\qquad B=S(b)=2gH(b)+v^2.
$$

It satisfies

$$
S''(r)=2gH''(r)+\frac{6b^2v^2}{r^4}>0,
$$

so it is a [strictly convex function](../../../../../../strictly-convex-function.md). Also $S(r)\to\infty$ as $r\to\infty$. To justify the other endpoint carefully, [convexity](../../../../../../convex-function.md) gives $H(r)\geq H(b)+H'(b)(r-b)$ for $0<r<b$. This supplies a finite lower bound near $0$, and the positive $r^{-2}$ term consequently forces $S(r)\to\infty$ there.

Thus $S$ has a unique [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md) at some $r_m>0$. Its [derivative](../../../../../../derivative.md) is strictly increasing and zero there, so $S$ decreases to $r_m$ and increases afterwards. Its [sublevel set](../../../../../../sublevel-set.md) $S(r)\leq B$ is a single interval $[b_1,b_2]$, with $0<b_1\leq b\leq b_2<\infty$. If $B>S(r_m)$, the two boundary [equations](../../../../../../equation.md) $S(b_i)=B$ have distinct solutions; if $B=S(r_m)$, both boundaries are $r_m$. The [conservation of energy](../../../../../../conservation-of-energy.md) identity therefore proves

$$
\boxed{b_1\leq r(t)\leq b_2.}
$$

The two [radii](../../../../../../radius.md) coincide exactly when $b=r_m$, equivalently $S'(b)=0$. This gives

$$
\boxed{b_1=b_2=b\quad\Longleftrightarrow\quad v^2=gbH'(b).}
$$

The [equation](../../../../../../equation.md) in [b](../b.md) then has the constant solution $r=b$, with $\dot\theta=\pm v/b$: this is a [circular orbit](../../../../../../circular-orbit.md).

**A positive inner bound requires $v>0$.** If zero launch [speed](../../../../../../speed.md) is allowed, $h=0$ and the displayed [inequality](../../../../../../inequality-mathematics.md) only gives $r\leq b$ because $H$ is strictly increasing; one may take the limiting inner bound $b_1=0$. For example, $H(r)=r^2$ satisfies all the stated hypotheses but permits inward motion from rest all the way towards the excluded axis. The two-positive-turning-radii argument therefore uses the natural interpretation of “launched with [speed](../../../../../../speed.md) $v$” as $v>0$.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [5](../../5.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
