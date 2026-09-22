<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

Assume $A>0$ and $\alpha>0$, so the excitation energy increases with momentum and vanishes in the ground state. With one internal state, the number of states in a spherical momentum shell is $V4\pi k^2dk/(2\pi)^3$. Since $k=(\epsilon/A)^{1/\alpha}/\hbar$,

$$
\boxed{g(\epsilon)\,d\epsilon=\frac{V}{2\pi^2\alpha\hbar^3A^{3/\alpha}}\epsilon^{3/\alpha-1}\,d\epsilon.}
$$

An internal degeneracy multiplies this [density of states](../../../../../density-of-states.md) by its degeneracy factor.

The [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md) is $\bar n(\epsilon)=[e^{(\epsilon-\mu)/(k_BT)}-1]^{-1}$. For a finite nonnegative occupation of the zero-energy state, its denominator must be positive, requiring $\mu<0$. At [Bose-Einstein condensation](../../../../../bose-einstein-condensation.md) the thermodynamic-limit chemical potential approaches $0$ from below, and the ground state must be counted separately; therefore “$\mu<0$” is a finite-system condition, while the condensed limit has $\mu=0$.

In a box whose shape is fixed, each momentum quantum number scales as $V^{-1/3}$, so each energy level scales as $V^{-\alpha/3}$. Differentiating the [grand potential](../../../../../grand-potential.md) $\Omega=k_BT\sum_j\log(1-e^{-(\epsilon_j-\mu)/(k_BT)})$ at fixed $T,\mu$ gives

$$
p=-\left(\frac{\partial\Omega}{\partial V}\right)_{T,\mu}=\sum_j\bar n_j\frac{\alpha\epsilon_j}{3V},\qquad\boxed{pV=\frac\alpha3E_{\rm total}.}
$$

The zero-energy condensate contributes neither pressure nor kinetic energy.

The number outside the ground state is

$$
\boxed{N_{\rm ex}=\frac{V}{2\pi^2\alpha\hbar^3A^{3/\alpha}}\int_0^\infty\frac{\epsilon^{3/\alpha-1}}{e^{(\epsilon-\mu)/(k_BT)}-1}\,d\epsilon.}
$$

At $\mu\uparrow0$, its low-energy integrand is proportional to $\epsilon^{3/\alpha-2}$. The integral is finite precisely when $3/\alpha>1$, so

$$
\boxed{\text{a finite-density condensate is possible for }0<\alpha<3.}
$$

For these exponents, the maximum excited population is

$$
N_{\rm ex}^{\max}=\frac{V\,\Gamma(3/\alpha)\zeta(3/\alpha)}{2\pi^2\alpha\hbar^3A^{3/\alpha}}(k_BT)^{3/\alpha}.
$$

This follows by expanding the Bose denominator in positive exponentials and integrating each term. It tends to zero as $T\downarrow0$, forcing excess particles into the ground state at fixed nonzero total number. At $\alpha=3$ the divergence is logarithmic; for $\alpha>3$ it is stronger, so there is no positive-temperature thermodynamic-limit condensation of this homogeneous gas.

Photons have $\alpha=1$ and two polarizations, but in ordinary blackbody equilibrium their number is not conserved and $\mu=0$ at every temperature. Cooling reduces their number rather than forcing an excess into a ground state, so an ordinary equilibrium photon gas does not condense. Systems imposing an effective photon-number constraint and an appropriate confined spectrum are different from the unconstrained photon gas considered here.

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
