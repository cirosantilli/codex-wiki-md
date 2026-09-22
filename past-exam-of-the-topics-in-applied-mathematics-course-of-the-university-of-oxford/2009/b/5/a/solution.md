<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [fixed point](../../../../../fixed-point.md) $z_*$ of a map $F:\mathbb R^2\to\mathbb R^2$ satisfies $F(z_*)=z_*$. Its linear perturbations evolve by the [Jacobian matrix](../../../../../jacobian-matrix.md) $DF(z_*)$: both [eigenvalues](../../../../../eigenvalue.md) must lie strictly inside the [unit disk](../../../../../unit-disk.md) for linear [asymptotic stability](../../../../../asymptotic-stability.md). One inside and one outside gives a saddle; both outside give a repeller. Unit-modulus [eigenvalues](../../../../../eigenvalue.md) require nonlinear analysis, unlike the continuous-time test using signs of real parts.

Here a [fixed point](../../../../../fixed-point.md) has $x=y=p$ and $2p=a(p-p^3/3)$. Therefore

$$
\boxed{p=0\text{ for all }a>0,\qquad p=\pm\sqrt{3-6/a}\text{ for }a>2.}
$$

At zero the characteristic equation is $\lambda^2+\lambda-a=0$. Its negative root is less than $-1$ for every $a>0$, while its positive root crosses $+1$ at $a=2$. Thus zero is a saddle for $0<a<2$ and a real repeller for $a>2$, with a pitchfork of fixed-point branches at $a=2$.

At either nonzero point the characteristic equation is $\lambda^2+\lambda+2a-6=0$, whose [discriminant](../../../../../discriminant.md) is $25-8a$. For $2<a<3$ the [fixed points](../../../../../fixed-point.md) are saddles. At $a=3$ their [periodic-orbit multipliers](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are $0,-1$, giving a flip threshold. For $3<a<25/8$ they are attracting real nodes; at $25/8$ repeated-eigenvalue [degenerate nodes](../../../../../degenerate-node.md); and for $25/8<a<7/2$ attracting foci. The [Jury stability criterion](../../../../../jury-stability-criterion.md) conditions reduce to $a>3$ and $a<7/2$, confirming the full stable interval.

At $a=7/2$ the [periodic-orbit multipliers](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are $e^{\pm2\pi i/3}$. For larger $a$ they form a repelling [focus equilibrium](../../../../../focus-dynamical-systems.md). This is a unit-circle crossing at a [strong resonance of a planar map](../../../../../strong-resonance-of-a-planar-map.md) with ratio $1:3$; [linearization](../../../../../linearization.md) alone does not justify asserting a generic nonresonant Neimark-Sacker bifurcation. The period-two branch at the flip threshold is derived next, including an additional family absent from the source's proposed quadratic.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
