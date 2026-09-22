<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Write $\mu=\mu_0\mu_r$ and $\epsilon=\epsilon_0\epsilon_r$ for homogeneous scalar material constants, and use $\mathbf J=\sigma\mathbf E$. Taking the [curl](../../../curl.md) of [Faraday's law of induction](../../../faraday-s-law-of-induction.md) and substituting the [Ampere-Maxwell law](../../../ampere-s-circuital-law.md) gives

$$
\nabla\times(\nabla\times\mathbf E)=-\mu\partial_t(\sigma\mathbf E+\epsilon\partial_t\mathbf E).
$$

The [vector calculus identity](../../../vector-calculus-identity.md) for a double [curl](../../../curl.md) therefore yields

$$
\boxed{\nabla^2\mathbf E-\nabla(\nabla\cdot\mathbf E)=\mu\epsilon\,\partial_t^2\mathbf E+\mu\sigma\,\partial_t\mathbf E.}
$$

The second term represents [electric current](../../../electric-current.md) response, rather than [displacement current](../../../displacement-current.md). A dispersive $\sigma(\omega)$ is used in the [frequency domain](../../../frequency-domain.md); its general time-domain counterpart is a temporal response convolution.

For the convention $e^{i(\mathbf k\cdot\mathbf r-\omega t)}$, the [plane wave](../../../plane-wave.md) equation is

$$
\left[\mathbf k\mathbf k^T+\left(\mu\epsilon\omega^2+i\mu\sigma\omega-k^2\right)\mathsf I\right]\mathbf E_0=0.
$$

Decompose the [electric field](../../../electric-field-split.md) into components parallel and perpendicular to $\mathbf k$. With $S=\mu\epsilon\omega^2+i\mu\sigma\omega$, the longitudinal eigenvalue is $S$ and each transverse eigenvalue is $S-k^2$; thus the determinant is $S(S-k^2)^2$. For a transverse [electromagnetic wave](../../../electromagnetic-wave-split.md), $\mathbf k\cdot\mathbf E_0=0$ and

$$
\boxed{k^2=\frac{\omega^2}{c^2}+i\mu_0\sigma\omega}
$$

when $\mu_r=1$ and the background $\epsilon_r\simeq1$. A real dissipative [electrical conductivity](../../../electrical-conductivity.md) generally makes $k$ complex, with the decaying branch chosen for a passive medium.

For a cold, collisionless, unmagnetized [plasma](../../../plasma-physics.md), treat ions as stationary and write $e>0$ for the magnitude of the [elementary charge](../../../elementary-charge.md). The electron equation of motion is $-i\omega m_e\mathbf v=-e\mathbf E$, so

$$
\mathbf v=-\frac{ie}{m_e\omega}\mathbf E,\qquad
\mathbf J=-N_e e\mathbf v=\sigma(\omega)\mathbf E,\qquad
\boxed{\sigma(\omega)=\frac{iN_e e^2}{m_e\omega}.}
$$

This reactive response includes no collision-induced [Joule heating](../../../joule-heating.md). Substitution into the transverse [dispersion relation](../../../dispersion-relation-split.md) gives

$$
\boxed{k^2c^2=\omega^2-\omega_p^2,\qquad \omega_p=\sqrt{\frac{N_ee^2}{m_e\epsilon_0}},\qquad n=\frac{ck}{\omega}=\sqrt{1-\frac{\omega_p^2}{\omega^2}}.}
$$

The quantity $\omega_p$ is the electron [plasma frequency](../../../plasma-frequency.md). The [refractive index](../../../refractive-index.md) is real above this cutoff; below it, the [wave](../../../wave-split.md) is evanescent. The electron response is represented here by $\sigma(\omega)$, so it must not also be counted a second time in the background [permittivity](../../../permittivity-split.md).

For a nonzero longitudinal component, taking the [dot product](../../../dot-product.md) of the matrix equation with $\mathbf k$ instead gives $S(\mathbf k\cdot\mathbf E_0)=0$. The same cold [plasma](../../../plasma-physics.md) response makes $S=(\omega^2-\omega_p^2)/c^2$, hence

$$
\boxed{\omega^2=\omega_p^2,\qquad \omega=\omega_p\quad\hbox{for positive frequency}.}
$$

At nonzero $k$, the remaining equation forces $\mathbf E_0$ to be parallel to $\mathbf k$, and [Faraday's law of induction](../../../faraday-s-law-of-induction.md) gives $\mathbf B_0=0$. These are electrostatic [Langmuir waves](../../../langmuir-wave.md), with no $k$ dependence of [angular frequency](../../../angular-frequency.md) in the zero-temperature model. Equilibrium neutrality does not forbid their perturbed [charge density](../../../charge-density.md); [Gauss's law](../../../gauss-s-law.md) requires such a density when $\mathbf k\cdot\mathbf E_0\ne0$.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2016](../../2016-split.md)
3. [Past exam of the electromagnetism and optics course of the University of Oxford](../../split.md)
4. [Electromagnetism and optics course of the University of Oxford](../../../electromagnetism-and-optics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
