<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Jacobian matrix](../../../../jacobian-matrix.md) at the origin and its [characteristic polynomial](../../../../characteristic-polynomial.md) are

$$
M_0=\begin{pmatrix}0&\mu\\-\mu&1+\mu\end{pmatrix},\qquad
p(\lambda)=\lambda^2-(1+\mu)\lambda+\mu^2.
$$

The [fixed-point multipliers](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are

$$
\lambda_\pm=\frac{1+\mu\pm\sqrt{(1-\mu)(1+3\mu)}}{2}.
$$

By the [Jury stability criterion](../../../../jury-stability-criterion.md), both lie strictly inside the [unit circle](../../../../complex-unit-circle.md) exactly when

$$
|\mu^2|<1,\qquad p(1)=\mu(\mu-1)>0,\qquad p(-1)=\mu^2+\mu+2>0.
$$

The last condition always holds, since $\mu^2+\mu+2=(\mu+1/2)^2+7/4$. Therefore **the origin is [asymptotically stable](../../../../asymptotic-stability.md) exactly for $-1<\mu<0$ among the hyperbolic parameter values**.

For completeness, its [linear stability](../../../../linear-stability.md) throughout the parameter line is as follows. When $\mu<-1$, the complex-conjugate [Floquet multipliers](../../../../floquet-multiplier.md) have [modulus](../../../../modulus.md) $|\mu|>1$, so the origin repels. When $-1<\mu<-1/3$, their [modulus](../../../../modulus.md) is $|\mu|<1$, so it attracts with oscillation. At $\mu=-1/3$ the repeated [Floquet multiplier](../../../../floquet-multiplier.md) is $1/3$, still attracting. For $-1/3<\mu<0$, both [Floquet multipliers](../../../../floquet-multiplier.md) are real and in $(0,1)$. For $0<\mu<1$, $p(1)<0$ and $p(0)>0$, so one [Floquet multiplier](../../../../floquet-multiplier.md) lies in $(0,1)$ and the other exceeds one: the origin is a [saddle fixed point of a map](../../../../saddle-fixed-point-of-a-map.md). For $\mu>1$, the complex-conjugate [Floquet multipliers](../../../../floquet-multiplier.md) have [modulus](../../../../modulus.md) $\mu>1$, so it repels.

Possible changes at the [unit circle](../../../../complex-unit-circle.md) are exhausted by $p(1)=0$, $p(-1)=0$, or a nonreal pair with product one. They give

$$
\boxed{\mu=-1,\quad0,\quad1.}
$$

At $\mu=0$ the [Floquet multipliers](../../../../floquet-multiplier.md) are $0,1$; the nonzero [fixed point](../../../../fixed-point.md) branches in part (a) meet the origin, and part (c) identifies a [subcritical pitchfork bifurcation](../../../../subcritical-pitchfork-bifurcation.md). Indeed at $\mu=0$ the exact restricted map is $y\mapsto y+y^3$, which makes the origin unstable despite its neutral linear direction.

At $\mu=-1$ the [Floquet multipliers](../../../../floquet-multiplier.md) are $i,-i$: this is a 1:4 [strong resonance of a planar map](../../../../strong-resonance-of-a-planar-map.md), coinciding with the change from repelling to attracting as $\mu$ increases. A generic nonresonant [Neimark–Sacker bifurcation](../../../../neimark-sacker-bifurcation.md) conclusion would be unjustified. At $\mu=1$ there is a double [Floquet multiplier](../../../../floquet-multiplier.md) $+1$; the matrix has a nontrivial [Jordan block](../../../../jordan-block.md), and the two further nonzero [fixed point](../../../../fixed-point.md) branches meet the origin. [Linear stability](../../../../linear-stability.md) alone is inconclusive at these unit-modulus boundary values. The repeated [Floquet multiplier](../../../../floquet-multiplier.md) at $\mu=-1/3$ is strictly inside the [unit circle](../../../../complex-unit-circle.md) and gives no [bifurcation](../../../../bifurcation.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the nonlinear systems course of the University of Oxford](../../../split.md)
5. [Nonlinear systems course of the University of Oxford](../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
