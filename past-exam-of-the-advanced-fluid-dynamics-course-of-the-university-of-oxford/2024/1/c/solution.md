<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take outward radial [force](../../../../force-split.md) as positive and keep the displaced element's angular rate fixed at $\Omega_0=\Omega(R_0)$. Its imbalance is

$$
\Delta f_R=\rho\left[(R_0+\xi_R)\Omega_0^2-\Phi'(R_0+\xi_R)\right].
$$

Use the equilibrium relation from part [b](../b.md), $\Phi'(R)=R\Omega(R)^2$, and a first-order [Taylor expansion](../../../../taylor-expansion.md):

$$
\boxed{\Delta f_R=-\rho R_0\left.\frac{d\Omega^2}{dR}\right|_{R_0}\xi_R+O(\xi_R^2),\qquad
|\Delta f_R|\simeq\rho\left|R_0\frac{d\Omega^2}{dR}\xi_R\right|.}
$$

The absolute values are needed for a magnitude. As printed, the proposed magnitude has a signed right side; it would be negative for outward displacement in a [Keplerian disk](../../../../keplerian-disk.md). For decreasing $\Omega^2$, the signed imbalance above points outward and therefore amplifies that fixed-angular-rate displacement. This calculation fixes the angular rate, rather than the [specific angular momentum](../../../../specific-angular-momentum.md); the latter is the conserved quantity for an uncoupled inviscid radial displacement and leads to the [Rayleigh centrifugal stability criterion](../../../../rayleigh-centrifugal-stability-criterion.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
