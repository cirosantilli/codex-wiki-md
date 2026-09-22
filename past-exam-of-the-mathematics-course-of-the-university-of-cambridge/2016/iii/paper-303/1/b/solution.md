<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the scalar [order parameter](../../../../../../order-parameter.md) can take either sign. The cubic term breaks $m\mapsto-m$ symmetry, and a positive quartic coefficient bounds the [Landau free energy](../../../../../../landau-free-energy.md) below. Stationary points satisfy

$$
A'(m)=m(A_2+A_3m+A_4m^2)=0,
$$

so, besides the disordered point $m=0$, the possible ordered points are

$$
m_\pm=\frac{-A_3\pm\sqrt{A_3^2-4A_2A_4}}{2A_4}.
$$

The disordered point has curvature $A''(0)=A_2$ and is locally stable when $A_2>0$. Nonzero [stationary points](../../../../../../stationary-point.md) first appear when

$$
A_2\le\frac{A_3^2}{4A_4}.
$$

That condition alone does not make them the equilibrium phase: one must compare their [free energies](../../../../../../thermodynamic-free-energy.md).

At a nonzero [stationary point](../../../../../../stationary-point.md), substitute $A_2=-A_3m-A_4m^2$ to obtain

$$
A(m)=-\frac{A_3m^3}{6}-\frac{A_4m^4}{4}
=-\frac{m^3}{12}(2A_3+3A_4m).
$$

For an ordered state to coexist with $A(0)=0$, this requires

$$
\boxed{m_{\mathrm{coex}}=-\frac{2A_3}{3A_4},\qquad
A_{2,\mathrm{coex}}=\frac{2A_3^2}{9A_4}.}
$$

Both curvatures at [phase coexistence](../../../../../../phase-coexistence.md) are positive and equal to $2A_3^2/(9A_4)$. The barrier is at $m=-A_3/(3A_4)$. In fact the potential at [phase coexistence](../../../../../../phase-coexistence.md) factorizes:

$$
A(m)=\frac{A_4}{4}m^2\left(m+\frac{2A_3}{3A_4}\right)^2.
$$

The two distinct minima are therefore explicit, with a finite jump in the [order parameter](../../../../../../order-parameter.md) whenever $A_3\ne0$.

To state the equilibrium inequalities for either sign of $A_3$, put $m=-\operatorname{sgn}(A_3)\rho$ with $\rho\ge0$. This sign always has lower energy than the opposite sign of equal magnitude. Then

$$
A(m)=\rho^2\left[\frac{A_2}{2}-\frac{|A_3|}{3}\rho+\frac{A_4}{4}\rho^2\right].
$$

The bracket's minimum is $A_2/2-A_3^2/(9A_4)$. It follows that

$$
\boxed{\begin{aligned}
A_2>\frac{2A_3^2}{9A_4}&:\quad m=0\text{ is the unique global minimum},\\
A_2=\frac{2A_3^2}{9A_4}&:\quad m=0\text{ and }m_{\mathrm{coex}}\text{ coexist},\\
A_2<\frac{2A_3^2}{9A_4}&:\quad\text{the global minimum is ordered}.
\end{aligned}}
$$

The favored ordered minimum, when it exists, is

$$
m_{\mathrm{ord}}=-\operatorname{sgn}(A_3)
\frac{|A_3|+\sqrt{A_3^2-4A_2A_4}}{2A_4}.
$$

Thus **a [first-order phase transition](../../../../../../first-order-phase-transition.md) is possible and occurs when the coefficients cross the coexistence relation**. There is **no continuous transition between $m=0$ and the equilibrium ordered state while $A_3$ remains nonzero and $A_4$ remains finite and positive**. The ordered state becomes globally favorable while $A_2$ is still positive, before the disordered curvature can vanish. Although a stationary solution tends to zero at $A_2=0$, it is not the global transition branch. A continuous transition would require eliminating the cubic term, outside the stated $A_3\ne0$ condition.

The [spinodal points](../../../../../../spinodal-point.md) clarify the metastable region: for $2A_3^2/(9A_4)<A_2<A_3^2/(4A_4)$ the ordered minimum is metastable; for $0<A_2<2A_3^2/(9A_4)$ the disordered minimum is metastable. At $A_2=0$ the disordered state loses local stability. These local-stability limits should not be mistaken for the [first-order transition in a cubic-quartic Landau potential](../../../../../../first-order-transition-in-a-cubic-quartic-landau-potential.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
