<h1 id="j/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In SI units the [Maxwell's equations](../../../../maxwell-equations-split.md) in vacuum, with sources, are

$$
\nabla\cdot E=\rho/\epsilon_0,\quad \nabla\cdot B=0,\quad
\nabla\times E=-\partial_tB,\quad
\nabla\times B=\mu_0j+\mu_0\epsilon_0\partial_tE.
$$

Taking the divergence of the last equation and using [Gauss's law](../../../../gauss-s-law.md) gives $\partial_t\rho+\nabla\cdot j=0$, the local [conservation of electric charge](../../../../charge-conservation.md). Thus sources that violate [charge conservation](../../../../charge-conservation.md) cannot satisfy all the [Maxwell's equations](../../../../maxwell-equations-split.md). Equivalently, with this conservation law the curl evolution preserves the electric divergence constraint if it holds initially; [Faraday's law](../../../../faraday-s-law-of-induction.md) similarly preserves $\nabla\cdot B=0$.

With $\rho=j=0$, use $\nabla\times(\nabla\times E)=\nabla(\nabla\cdot E)-\Delta E$ and substitute the two curl equations. This gives $-\Delta E=-\mu_0\epsilon_0\partial_t^2E$. Applying the same calculation to $B$ yields

$$
\boxed{\Delta E-c^{-2}E_{tt}=0,\qquad
\Delta B-c^{-2}B_{tt}=0,\quad c=(\mu_0\epsilon_0)^{-1/2}.}
$$

A monochromatic [plane wave](../../../../plane-wave.md) has one [angular frequency](../../../../angular-frequency.md) $\omega$ and constant-phase planes $\mathbf K\cdot r=\omega t-\text{constant}$, normal to the [wavevector](../../../../wavevector.md) $\mathbf K$. Its [wavelength](../../../../wavelength.md) is $2\pi/|\mathbf K|$.

For a nontrivial traveling wave with $\omega\neq0$, substitution of the displayed [electric field](../../../../electric-field-split.md) into the divergence equation gives $\mathbf K\cdot e_1=\mathbf K\cdot e_2=0$. [Faraday's law](../../../../faraday-s-law-of-induction.md) is satisfied by

$$
\boxed{B=\frac1\omega\,\mathbf K\times E,\qquad
\omega^2=c^2|\mathbf K|^2,\qquad \mathbf K\cdot e_1=\mathbf K\cdot e_2=0.}
$$

Indeed $\partial_tB=\mathbf K\times E_\phi$ and $\nabla\times E=-\mathbf K\times E_\phi$. The magnetic divergence is zero, while [Ampère's law](../../../../ampere-s-circuital-law.md) reduces to $|\mathbf K|^2E_\phi/\omega=(\omega/c^2)E_\phi$, giving the [dispersion relation](../../../../dispersion-relation-split.md). The amplitudes may be arbitrary transverse vectors; they need not be mutually orthogonal or have equal lengths. Their combination describes the [polarization](../../../../polarization-waves.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [J](../../j.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
