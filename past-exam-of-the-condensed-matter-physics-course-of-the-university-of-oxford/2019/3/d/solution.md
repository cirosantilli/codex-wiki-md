<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the screened [Coulomb potential](../../../../coulomb-potential-energy.md) of a singly ionized donor as $V(r)=-\kappa/r$, with $\kappa=e^2/(4\pi\epsilon_0\epsilon_r)$ and $r=|\mathbf r-\mathbf r_0|$. The electron's motion is two-dimensional, but its electrostatic interaction is the ordinary three-dimensional $1/r$ interaction restricted to the layer; it is not a logarithmic two-dimensional electrostatic potential.

For the rotationally symmetric bound state, the two-dimensional radial [Schrödinger equation](../../../../schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m_e^*}\left(\frac{d^2\psi}{dr^2}+\frac1r\frac{d\psi}{dr}\right)-\frac\kappa r\psi=E\psi.
$$

For $\psi=Ae^{-br}$, the radial Laplacian is $(b^2-b/r)\psi$. Cancel the $1/r$ term to obtain

$$
\boxed{b=\frac{2m_e^*\kappa}{\hbar^2}=\frac2{a_B^*},\qquad E=-\frac{\hbar^2b^2}{2m_e^*}=-\frac{2m_e^*\kappa^2}{\hbar^2}.}
$$

Thus the positive [two-dimensional hydrogenic donor](../../../../two-dimensional-hydrogenic-donor.md) binding energy is four times the three-dimensional effective Rydberg:

$$
\boxed{E_B=4(13.6057\,\mathrm{eV})\frac{0.026}{15^2}\simeq6.29\,\mathrm{meV},\qquad b\simeq6.55\times10^7\,\mathrm m^{-1}.}
$$

The decay length is $1/b=a_B^*/2\simeq15.3\,\mathrm{nm}$. Normalization, if desired, follows from $1=2\pi|A|^2\int_0^\infty re^{-2br}dr=\pi|A|^2/(2b^2)$, giving $A=b\sqrt{2/\pi}$ up to a constant phase. This ideal result neglects finite well thickness, dielectric mismatch at the interfaces and short-range impurity corrections.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
