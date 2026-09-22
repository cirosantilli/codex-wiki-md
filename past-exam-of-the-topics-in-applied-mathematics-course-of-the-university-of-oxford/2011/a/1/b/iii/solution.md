<h1 id="a/1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The positive quadrant is invariant. The non-axis [nullclines](../../../../../../nullcline.md) are $u+v=1$ and $u=1/\beta$. Below $u+v=1$, $u$ increases; above it, $u$ decreases. To the left of $u=1/\beta$, $v$ increases; to the right, it decreases.

For $\beta>1$, the [stable manifold](../../../../../../stable-manifold.md) of the interior saddle separates trajectories tending to $(1,0)$ from those for which $u\to0$ and $v\to\infty$. Exactly on that manifold, the trajectory tends to the saddle. For the illustrated $r=1,\beta=2$, the separating manifold is exactly $v=u$, since the vector field preserves that diagonal.

For $\beta<1$, every strictly positive initial state ultimately has $u\to0$ and $v\to\infty$. Indeed $\dot u\leq ru(1-u)$ implies $\limsup u\leq1$, so eventually $1-\beta u$ is bounded below by a positive constant. Then $v$ grows exponentially, forcing $u$ down. At $\beta=1$, a positive $v$ eventually drives $u$ below one; thereafter $v$ increases. A finite positive limit for $v$ would force $u\to1$, inconsistent with $\dot u\to-rv<0$, so the same exclusion outcome holds.

There are no interior [periodic orbits](../../../../../../periodic-orbit.md): the [Bendixson-Dulac criterion](../../../../../../bendixson-dulac-theorem.md) with multiplier $1/(uv)$ gives

$$
\frac\partial{\partial u}\frac{r(1-u-v)}v+\frac\partial{\partial v}\frac{1-\beta u}u=-\frac rv<0.
$$

The [phase portraits](../../../../../../phase-portrait.md) in the preceding figure show the threshold geometry and the absence of a bounded attracting coexistence state. Initial states on the axes retain the corresponding one-species dynamics.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
