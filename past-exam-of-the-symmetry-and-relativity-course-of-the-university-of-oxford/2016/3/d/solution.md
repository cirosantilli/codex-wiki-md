<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a forward wave, the [Faraday's law of induction](../../../../faraday-s-law-of-induction.md) fixes the relative amplitudes and signs:

$$
\mathbf B_0=\frac1\omega\mathbf k\times\mathbf E_0,
\qquad B_0=-\frac{k}{\omega}E_0=-\frac ncE_0.
$$

Thus the two scalar amplitudes in the source cannot both be positive when the stated propagation direction and axes are used. The supplied product magnitude fixes only an overall amplitude in the chosen field units.

One convenient potential representative is

$$
\boxed{\varphi=0,\qquad
\mathbf A=-\hat{\mathbf y}\frac{E_0}{\omega}\sin(\omega t-kz),\qquad
K^\mu=(\omega/c,0,0,n\omega/c).}
$$

Indeed $-\partial_t\mathbf A$ gives the electric field and $\nabla\times\mathbf A$ gives the signed magnetic field above. Moreover $\nabla\cdot\mathbf A+c^{-2}\partial_t\varphi=0$, the [Lorenz gauge condition](../../../../lorenz-gauge-condition.md). The potentials are not unique because residual [gauge transformations](../../../../gauge-transformation.md) may preserve this condition.

Since $n>1$, the electromagnetic [electromagnetic field invariants](../../../../electromagnetic-field-invariants.md) satisfy $\mathbf E\cdot\mathbf B=0$ and $B^2-E^2/c^2=(n^2-1)E^2/c^2>0$ away from field nodes. A boost along positive $z$ with speed $u=c/n$ gives

$$
E'_y=\gamma_u(E_y+uB_x)=0,\qquad
B'_x=-\frac{E_0}{c}\sqrt{n^2-1}\cos(\omega't'-k'z').
$$

Here $\omega'=\gamma_u(\omega-uk)=0$ and $k'=(\omega/c)\sqrt{n^2-1}$. The wave becomes a static spatially varying magnetic pattern in this frame. This is possible because its medium wave four-vector is spacelike, $K^2=(1-n^2)\omega^2/c^2<0$; it is not a vacuum-photon rest frame. The medium moves in the new frame, so its original rest-frame constitutive relation must not be reused there unchanged.

No inertial frame makes the magnetic field vanish throughout a nontrivial wave: that would turn the positive invariant $B^2-E^2/c^2$ into a nonpositive one. Both fields vanish at isolated nodes already, which is distinct from removing a field everywhere.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
