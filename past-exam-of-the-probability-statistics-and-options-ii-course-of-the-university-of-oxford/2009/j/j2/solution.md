<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

In SI units [Maxwell's equations](../../../../maxwell-equations-split.md) are

$$
\nabla\cdot E=\rho_e/\epsilon_0,\quad\nabla\cdot B=0,\quad\nabla\times E=-\partial_tB,\quad\nabla\times B=\mu_0J+\mu_0\epsilon_0\partial_tE.
$$

The given vector [identity](../../../../identity-element.md) yields

$$
\nabla\cdot(E\times B)=B\cdot(\nabla\times E)-E\cdot(\nabla\times B)=-B\cdot\partial_tB-\mu_0E\cdot J-\mu_0\epsilon_0E\cdot\partial_tE.
$$

Divide by $\mu_0$ and collect the two energy [derivatives](../../../../derivative.md) to obtain the local [identity](../../../../identity-element.md) $\partial_t\mathcal U+\nabla\cdot P+E\cdot J=0$. Integration over the fixed region and the [divergence theorem](../../../../divergence-theorem.md) give the required integral conservation law. Its terms are, respectively, the rate of change of stored [electromagnetic energy](../../../../electromagnetic-energy.md), the outward [electromagnetic energy](../../../../electromagnetic-energy.md) flux through the boundary, and work per unit time done by the [field](../../../../field.md) on charges. The last term transfers energy from the [field](../../../../field.md) to matter when positive.

In vacuum put $\rho_e=0$, $J=0$ and write $\phi=kz-\omega t$. [Faraday's law](../../../../faraday-s-law-of-induction.md) gives the plane-wave [magnetic field](../../../../magnetic-field-split.md)

$$
\boxed{B=(0,\alpha k\cos\phi/\omega,0).}
$$

Both divergence equations are satisfied, and the remaining curl equation gives $k^2=\mu_0\epsilon_0\omega^2$. Hence $\boxed{\omega=ck,\quad c=(\mu_0\epsilon_0)^{-1/2}}$, with $B_y=E_x/c$. Here the corresponding [field](../../../../field.md) is the pure wave, with no added static background.

Its electric and magnetic energy densities are equal. Explicitly,

$$
\boxed{\mathcal U=\epsilon_0\alpha^2\cos^2\phi,\qquad P=\epsilon_0c\alpha^2\cos^2\phi\,\hat z,\qquad|P|=c\mathcal U.}
$$

The energy flux points in the propagation direction, toward increasing $z$.

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
