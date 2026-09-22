<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first term is the [bending energy](../../../../../bending-energy.md) of rod 1, whose preferred [bending strain of a rod](../../../../../bending-strain-of-a-rod.md) is zero. The second is the [bending energy](../../../../../bending-energy.md) of rod 2 relative to its preferred [intrinsic curvature of an elastic filament](../../../../../intrinsic-curvature-of-an-elastic-filament.md) $\hat u$. The third is its [stretching energy](../../../../../stretching-energy.md), with stretching stiffness $kB_2$ and stress-free [stretch ratio](../../../../../stretch-ratio.md) $\alpha^+=1$. Each term is an energy per unit reference [arc length](../../../../../arc-length.md) before [integration](../../../../../integral-split.md).

Substitute $u^+=u$ and $\alpha^+-1=-au$. The resulting [quadratic function](../../../../../quadratic-function.md) of $u$ has density

$$
q(u)=\frac12(B_1+B_2+ka^2B_2)u^2-B_2\hat u\,u+\frac12B_2\hat u^2.
$$

There are no derivatives of $u$ or imposed end constraints in this [minimum potential energy principle in elasticity](../../../../../minimum-potential-energy-principle-in-elasticity.md). Since

$$
q'(u)=(B_1+B_2+ka^2B_2)u-B_2\hat u,\qquad
q''(u)=B_1+B_2+ka^2B_2>0,
$$

the unique pointwise minimizer is also the constant global minimizer:

$$
\boxed{u_* =\frac{B_2\hat u}{B_1+B_2+ka^2B_2}
=\frac{\hat u}{B_1/B_2+1+ka^2}.}
$$

For example, [completing the square](../../../../../completing-the-square.md) gives

$$
\mathcal E[u]-\mathcal E[u_*]
=\frac{B_1+B_2+ka^2B_2}{2}\int_0^L(u-u_*)^2\,dS\ge0,
$$

which also proves uniqueness, up to equality [almost everywhere](../../../../../almost-everywhere.md), without merely assuming a uniform [curvature](../../../../../curvature.md).

With $k$, $a$ and $\hat u$ fixed, the two limits are

$$
\boxed{\begin{aligned}
B_1/B_2\to\infty &: \quad u_*\to0,\\
B_1/B_2\to0 &: \quad u_*\to\frac{\hat u}{1+ka^2}.
\end{aligned}}
$$

In the first limit, rod 1 dominates the [bending energy](../../../../../bending-energy.md) and suppresses the bend. In the second, rod 1 offers negligible bending resistance, but following rod 2's preferred [bending strain of a rod](../../../../../bending-strain-of-a-rod.md) still shortens rod 2 through the bonded geometry. The competition between its [bending energy](../../../../../bending-energy.md) and [stretching energy](../../../../../stretching-energy.md) leaves $u_*<\hat u$ when $\hat u>0$ and $ka^2>0$. Only when that stretching penalty also vanishes does $u_*\to\hat u$.

These formulae describe an admissible bonded [elastic rod](../../../../../elastic-rod.md) provided $1-au_*>0$. If parameters instead force $au_*\ge1$, the unconstrained quadratic minimizer is outside the kinematic regime of the model; the given energy does not itself enforce positive [stretch ratio](../../../../../stretch-ratio.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical mechanical biology course of the University of Oxford](../../../../split.md)
6. [Mathematical mechanical biology course of the University of Oxford](../../../../../mathematical-mechanical-biology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
