<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

For a lattice-periodic potential, [Bloch's theorem](../../../../bloch-s-theorem-split.md) permits energy eigenfunctions $\psi_{\mathbf k}(\mathbf r)=e^{i\mathbf k\cdot\mathbf r}u_{\mathbf k}(\mathbf r)$, where $u_{\mathbf k}(\mathbf r+\mathbf R)=u_{\mathbf k}(\mathbf r)$ for every lattice translation $\mathbf R$. The [crystal momentum](../../../../crystal-momentum.md) is $\hbar\mathbf k$, defined modulo a [reciprocal lattice](../../../../reciprocal-lattice.md) vector. A reciprocal vector $\mathbf G$ satisfies $\mathbf G\cdot\mathbf R\in2\pi\mathbb Z$, so $e^{i\mathbf G\cdot\mathbf r}$ is lattice-periodic.

Expand the [Bloch wave](../../../../bloch-state.md) as plane waves in one momentum class, $\psi=\sum_{\mathbf q}c_{\mathbf q}e^{i\mathbf q\cdot\mathbf r}$ with $\mathbf q=\mathbf k+\mathbf G'$. Substitution into the [Schrödinger equation](../../../../schrodinger-equation.md), using $U=\sum_{\mathbf G}U_{\mathbf G}e^{i\mathbf G\cdot\mathbf r}$, gives a kinetic coefficient $\hbar^2q^2c_{\mathbf q}/(2m)$ and potential coefficient $\sum_{\mathbf G}U_{\mathbf G}c_{\mathbf q-\mathbf G}$. Independence of the plane waves therefore gives

$$
\boxed{\left(\frac{\hbar^2q^2}{2m}-E\right)c_{\mathbf q}+\sum_{\mathbf G}U_{\mathbf G}c_{\mathbf q-\mathbf G}=0.}
$$

This uses $\mathbf q$ for the paper's running plane-wave index, to distinguish it from the fixed reduced Bloch wavevector.

For $G=2\pi/a$, the sine potential has coefficients $U_G=-iV$, $U_{-G}=iV$. At the [Brillouin zone](../../../../brillouin-zone.md) boundary, the free states $e^{i\pi x/a}$ and $e^{-i\pi x/a}$ are degenerate. Keeping these two resonant waves in the [nearly-free electron model](../../../../nearly-free-electron-model.md) gives

$$
\begin{pmatrix}\beta-E&-iV\\iV&\beta-E\end{pmatrix}\begin{pmatrix}c_+\\c_-\end{pmatrix}=0,\qquad\boxed{\beta=\frac{\hbar^2\pi^2}{2ma^2}.}
$$

The determinant is $(\beta-E)^2-V^2$, so **the two energies are $E_\pm=\beta\pm|V|$**, separated by $2|V|$. With $V>0$, the lower combination has coefficients $(1,-i)/\sqrt2$ and density proportional to $1-\sin Gx$; the upper has $(1,i)/\sqrt2$ and density $1+\sin Gx$. The lower wave places less weight where the potential is positive. Coupling to nonresonant plane waves gives higher-order corrections beyond this two-wave approximation.

The first [Brillouin zone](../../../../brillouin-zone.md) of a [primitive cubic lattice](../../../../primitive-cubic-lattice.md) is the cube $|k_i|\leq\pi/a$. Its boundary along $(100)$ is the face center $(\pi/a,0,0)$, while along $(111)$ it is the corner $(\pi/a,\pi/a,\pi/a)$. Therefore

$$
\boxed{E_{100}^{(0)}=\beta,\qquad E_{111}^{(0)}=3\beta.}
$$

A spin-degenerate band accommodates two electrons per cell. To be a [band insulator](../../../../band-insulator.md), the filled first band must be separated from the second at every wavevector; a direct local splitting alone is insufficient. Under the paper's uniform-boundary-gap estimate, take the lower edge as $E^{(0)}-V$ and the upper edge as $E^{(0)}+V$. The highest lower edge is $3\beta-V$ and the lowest upper edge is $\beta+V$. Thus the [indirect gap in a uniformly split zone-boundary model](../../../../indirect-gap-in-a-uniformly-split-zone-boundary-model.md) is

$$
E_g^{\rm ind}=(\beta+V)-(3\beta-V)=2(V-\beta),\qquad\boxed{V>\frac{\hbar^2\pi^2}{2ma^2}.}
$$

Equality gives touching rather than a positive gap; for smaller $V$, [overlapping energy bands prevent a band insulator](../../../../overlapping-energy-bands-prevent-a-band-insulator.md). This final threshold is the stated uniform-splitting band-edge estimate. A quantitative three-dimensional potential mixes several plane waves at corners and requires its full band structure rather than assuming the two-wave sine calculation remains exact there.

## ↑ Ancestors (13)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
