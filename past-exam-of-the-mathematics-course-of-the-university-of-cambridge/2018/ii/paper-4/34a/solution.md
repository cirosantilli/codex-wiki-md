<h1 id="34a/solution">Solution</h1>

↑ **Parent:** [34A](../34a.md)

A three-dimensional [Bravais lattice](../../../../../bravais-lattice.md) is the set of all integer combinations of three linearly independent primitive vectors. Its [reciprocal lattice](../../../../../reciprocal-lattice.md) is

$$
\Lambda^*=\{G:G\mathbin{\cdot}R\in2\pi\mathbb Z
\text{ for every }R\in\Lambda\},
$$

and the first [Brillouin zone](../../../../../brillouin-zone.md) is the [Wigner-Seitz cell](../../../../../wigner-seitz-cell.md) of the origin in reciprocal space.

For the stated [FCC lattice](../../../../../face-centered-cubic-lattice.md), the primitive-cell volume is

$$
\Omega=a_1\mathbin{\cdot}(a_2\times a_3)=\frac{a^3}{4}.
$$

The reciprocal-basis formula gives

$$
\boxed{
 b_1=\frac{2\pi}{a}(-e_1+e_2+e_3),\quad
 b_2=\frac{2\pi}{a}(e_1-e_2+e_3),\quad
 b_3=\frac{2\pi}{a}(e_1+e_2-e_3)}.
$$

A reciprocal primitive cell, and hence the [Brillouin zone](../../../../../brillouin-zone.md), has volume

$$
\boxed{\frac{(2\pi)^3}{\Omega}=\frac{32\pi^3}{a^3}}.
$$

In the first [Born approximation](../../../../../born-approximation.md), with momentum transfer $q=k-k'$, the [scattering amplitude](../../../../../scattering-amplitude.md) is

$$
f_V(k;k')=-\frac{m}{2\pi\hbar^2}
\int_{\mathbb R^3}e^{iq\cdot r}V(r)\,d^3r.
$$

For the spherical shell, align the polar axis with $q$ and use its radial [Dirac delta function](../../../../../dirac-delta-function.md):

$$
\int e^{iq\cdot r}V_0\delta(r-d)\,d^3r
=4\pi V_0d^2\frac{\sin(qd)}{qd}.
$$

Therefore

$$
\boxed{\widetilde f_V(k;k')
=-\frac{2mV_0d^2}{\hbar^2}\frac{\sin(qd)}{qd}}.
$$

Translation of each atomic potential multiplies its transform by a phase, so the [crystal lattice structure factor](../../../../../crystal-lattice-structure-factor.md) gives

$$
f_{V_\Lambda}(k;k')
=\widetilde f_V(k;k')\sum_{R\in\Lambda}e^{iq\cdot R}.
$$

For an infinite lattice, the lattice [Poisson summation formula](../../../../../poisson-summation-formula.md) turns the sum into

$$
\sum_{R\in\Lambda}e^{iq\cdot R}
=\frac{(2\pi)^3}{\Omega}
\sum_{G\in\Lambda^*}\delta^{(3)}(q-G).
$$

Thus the amplitude vanishes away from reciprocal-lattice momentum transfers.

In [elastic scattering](../../../../../elastic-scattering.md), $|k|=|k'|$ and hence

$$
|q|=2k\sin\frac\theta2.
$$

The two shortest relevant reciprocal-vector lengths of this [FCC lattice](../../../../../face-centered-cubic-lattice.md) are

$$
|G_2|=\frac{2\pi\sqrt3}{a},
\qquad |G_1|=\frac{4\pi}{a}.
$$

Both are kinematically available when $k>2\pi/a$. Assigning their scattering angles $\theta_2$ and $\theta_1$, respectively, gives

$$
\boxed{\frac{\sin(\theta_1/2)}{\sin(\theta_2/2)}
=\frac{|G_1|}{|G_2|}=\frac2{\sqrt3}}.
$$

## ↑ Ancestors (10)

1. [34A](../34a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
