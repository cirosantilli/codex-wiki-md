<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this [radially layered coaxial cable](../../../../../radially-layered-coaxial-cable.md), define

$$
L_1=\ln(c/a),\qquad L_2=\ln(b/c),\qquad
\Delta=\epsilon'L_1+\epsilon L_2,\qquad
C=\frac{V\epsilon\epsilon'}{\Delta}.
$$

Use the solution regular at the axis with bounded exterior [electric potential](../../../../../electric-potential.md), so that the empty interior and exterior have the constant [electric potentials](../../../../../electric-potential.md) fixed by their adjacent conducting cylinders.

There is no [free charge](../../../../../free-charge.md) in either [electrical insulator](../../../../../electrical-insulator.md) or on their interface. [Gauss's law](../../../../../gauss-s-law.md) and continuity of normal [electric displacement field](../../../../../electric-displacement-field.md) give $D_\rho=C/\rho$ in both layers. The [electric potential difference](../../../../../electric-potential-difference.md) fixes the constant because

$$
V=\int_a^bE_\rho\,d\rho=C\left(\frac{L_1}{\epsilon}+\frac{L_2}{\epsilon'}\right).
$$

The [electric potential](../../../../../electric-potential.md), including the empty regions bounded by the conducting cylinders, is therefore

$$
\boxed{\phi(\rho)=\begin{cases}
V,&0\leq\rho\leq a,\\[2pt]
\displaystyle\frac V\Delta\left[\epsilon'\ln(c/\rho)+\epsilon\ln(b/c)\right],&a<\rho<c,\\[2pt]
\displaystyle\frac{V\epsilon}{\Delta}\ln(b/\rho),&c\leq\rho<b,\\[2pt]
0,&\rho\geq b.
\end{cases}}
$$

Both inner and outer [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) hold, and the [electric potential](../../../../../electric-potential.md) is continuous at the material interface, where

$$
\boxed{\phi(c)=\frac{V\epsilon\ln(b/c)}{\epsilon'\ln(c/a)+\epsilon\ln(b/c)}.}
$$

Taking the negative [gradient](../../../../../gradient.md) of the [electric potential](../../../../../electric-potential.md) yields

$$
\boxed{\mathbf E(\rho)=\begin{cases}
0,&\rho<a\ \text{or}\ \rho>b,\\[2pt]
\displaystyle\frac{V\epsilon'}{\Delta\rho}\mathbf e_\rho,&a<\rho<c,\\[2pt]
\displaystyle\frac{V\epsilon}{\Delta\rho}\mathbf e_\rho,&c<\rho<b.
\end{cases}}
$$

The radial [electric field](../../../../../electric-field-split.md) generally jumps at $\rho=c$, but $\epsilon E_\rho(c^-)=\epsilon'E_\rho(c^+)$, as required by the absence of free [surface charge density](../../../../../surface-charge-density.md) there. The conducting cylinders carry opposite [linear charge densities](../../../../../linear-charge-density.md) $\lambda=2\pi C$ and $-\lambda$.

For an [Amperian loop](../../../../../amperian-loop.md) of radius $\rho$, the enclosed [electric current](../../../../../electric-current.md) is zero, $I$, or zero according as $\rho<a$, $a<\rho<b$, or $\rho>b$. The [magnetostatic Ampère law](../../../../../magnetostatic-ampere-law.md) therefore gives $H_\varphi=I/(2\pi\rho)$ in the gap, and zero outside. Using the two [magnetic permeabilities](../../../../../permeability-electromagnetism.md),

$$
\boxed{\mathbf B(\rho)=\begin{cases}
0,&\rho<a\ \text{or}\ \rho>b,\\[2pt]
\displaystyle\frac{\mu I}{2\pi\rho}\mathbf e_\varphi,&a<\rho<c,\\[2pt]
\displaystyle\frac{\mu'I}{2\pi\rho}\mathbf e_\varphi,&c<\rho<b.
\end{cases}}
$$

The tangential [magnetic field strength](../../../../../magnetic-field-strength.md) is continuous at the material interface, while the tangential [magnetic field](../../../../../magnetic-field-split.md) need not be. At each ideal conducting surface and at the material interface, the displayed [electric field](../../../../../electric-field-split.md) and [magnetic field](../../../../../magnetic-field-split.md) formulas specify one-sided limits; a single interface value is unnecessary when the limiting values differ.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
