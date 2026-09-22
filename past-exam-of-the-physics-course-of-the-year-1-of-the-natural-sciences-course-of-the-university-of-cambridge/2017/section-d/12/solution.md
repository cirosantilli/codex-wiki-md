<h1 id="section-d/12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

Here $V(x,y)$ is the [potential energy](../../../../potential-energy.md) and $E$ is the stationary [energy](../../../../energy-split.md) [eigenvalue](../../../../eigenvalue.md). The [Schrödinger equation](../../../../schrodinger-equation.md) is the [eigenvalue](../../../../eigenvalue.md) equation for kinetic plus [potential energy](../../../../potential-energy.md). Its boundary conditions select the allowed energies. For a normalized [wavefunction](../../../../wave-function-split.md), the [Born rule](../../../../born-rule.md) assigns probability $|\psi(x,y)|^2dx\,dy$ to a small area, and $\int|\psi|^2dx\,dy=1$. A stationary state's full time dependence is $\psi(x,y)e^{-iEt/\hbar}$; its [probability density](../../../../probability-density.md) is time-independent.

The infinite walls impose $\psi=0$ on all four boundaries. For a separated solution $\psi=X(x)Y(y)$ in the zero-potential interior,

$$
\frac{X''}{X}+\frac{Y''}{Y}=-\frac{2mE}{\hbar^2}.
$$

The first term depends only on $x$ and the second only on $y$, so each is constant, $-k_x^2$ and $-k_y^2$. Vanishing at $x=0$ and $y=0$ removes the cosine terms. Vanishing at the other boundaries gives

$$
\boxed{k_x=\frac{n_x\pi}{a},\qquad k_y=\frac{n_y\pi}{b},\qquad n_x,n_y=1,2,\ldots.}
$$

The normalized [two-dimensional infinite square well](../../../../two-dimensional-infinite-square-well.md) [eigenbasis](../../../../eigenbasis.md) and energies are

$$
\boxed{\psi_{n_xn_y}(x,y)=\frac2{\sqrt{ab}}\sin\frac{n_x\pi x}{a}\sin\frac{n_y\pi y}{b},\qquad E_{n_xn_y}=\frac{\pi^2\hbar^2}{2m}\left(\frac{n_x^2}{a^2}+\frac{n_y^2}{b^2}\right).}
$$

Normalization follows from the two sine-squared integrals $a/2$ and $b/2$. Zero quantum numbers would give an identically zero function. These separated products form a basis, not every possible [wavefunction](../../../../wave-function-split.md): a general state is their [superposition](../../../../superposition-principle.md), and a degenerate [energy](../../../../energy-split.md) eigenspace can have nonseparable stationary combinations of products with that same [energy](../../../../energy-split.md).

For $a=1\,\mathrm{nm}$ and $b=2\,\mathrm{nm}$, the ground state is $(1,1)$ and the nearest excitation is $(1,2)$, along the longer side. The next quantum along the shorter side costs more [energy](../../../../energy-split.md). Thus

$$
\boxed{\epsilon_{\min}=E_{12}-E_{11}=\frac{3\pi^2\hbar^2}{2m_eb^2}=4.52\times10^{-20}\,\mathrm J=0.282\,\mathrm{eV}.}
$$

This transition has nonzero dipole matrix element for an electric-field component along $y$. Light polarized strictly along $x$ would not drive it, so the minimum assumes an allowed [polarization](../../../../polarization-waves.md) rather than an arbitrary fixed one.

For the requested degeneracy, keep $b>a$. The first two states are necessarily $(1,1)$ and $(1,2)$, since $E_{21}-E_{12}=3\pi^2\hbar^2(a^{-2}-b^{-2})/(2m)>0$. The third level is the smaller of $E_{21}$ and $E_{13}$: states with both indices at least two lie above $E_{21}$, and higher states on the $n_x=1$ sequence lie above $E_{13}$. Make these two candidates equal:

$$
\frac4{a^2}+\frac1{b^2}=\frac1{a^2}+\frac9{b^2},\qquad \boxed{b=\sqrt{\frac83}\,a=1.633\,\mathrm{nm}.}
$$

The [third-level degeneracy in a rectangular quantum box](../../../../third-level-degeneracy-in-a-rectangular-quantum-box.md) then has lowest distinct energies $11/8$, $5/2$ and $35/8$ in units $\pi^2\hbar^2/(2m_ea^2)$, with multiplicities one, one and two. The third-level pair is exactly $(2,1)$ and $(1,3)$.

## ↑ Ancestors (12)

1. [12](../12.md)
2. [Section D](../../section-d.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
