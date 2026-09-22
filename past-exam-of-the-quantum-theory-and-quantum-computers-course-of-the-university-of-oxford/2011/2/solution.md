<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use an expansion for the [eigenstate](../../../eigenstate.md) continuing the nondegenerate level, with intermediate [normalization](../../../normalization.md) $\langle\psi_0,\psi(\epsilon)\rangle=1$:

$$
E(\epsilon)=E_0+\epsilon E^{(1)}+\epsilon^2E^{(2)}+O(\epsilon^3),\qquad
\psi(\epsilon)=\psi_0+\epsilon\chi+\epsilon^2\eta+\cdots,\qquad\langle\psi_0,\chi\rangle=0.
$$

Insert these expressions into the [eigenvalue](../../../eigenvalue.md) equation. At first order,

$$
(H_0-E_0)\chi=-(H'-E^{(1)})\psi_0.
$$

Taking the [inner product](../../../inner-product-split.md) with $\psi_0$ eliminates the left side by self-adjointness. Thus

$$
\boxed{E^{(1)}=\langle\psi_0,H'\psi_0\rangle,\qquad
E(\epsilon)=\langle\psi_0,H\psi_0\rangle+O(\epsilon^2).}
$$

For $j\ne0$, projection onto $\psi_j$ instead gives

$$
\langle\psi_j,\chi\rangle=\frac{\langle\psi_j,H'\psi_0\rangle}{E_0-E_j}.
$$

At second order, projecting the [eigenvalue](../../../eigenvalue.md) equation onto $\psi_0$ gives $E^{(2)}=\langle\psi_0,H'\chi\rangle$. Expand $\chi$ in the orthonormal energy [basis](../../../basis.md) and use self-adjointness of $H'$:

$$
\boxed{\epsilon^2E^{(2)}=\epsilon^2\sum_{j\ne0}\frac{|\langle\psi_j,H'\psi_0\rangle|^2}{E_0-E_j}.}
$$

Nondegeneracy ensures the denominators for this level do not vanish; convergence and validity of the expansion are among the assumed perturbation-theory hypotheses.

For the [cosine perturbation of the ground level in a one-dimensional box](../../../cosine-perturbation-of-the-ground-level-in-a-one-dimensional-box.md), write $u=\pi x/a$. The product-to-sum identity gives

$$
\cos(2u)\sin u=\tfrac12\bigl(\sin(3u)-\sin u\bigr),
$$

so, with the given common [normalization](../../../normalization.md) of the sine eigenfunctions,

$$
\boxed{V\phi_1=\frac\epsilon2(\phi_3-\phi_1).}
$$

The diagonal [matrix](../../../matrix.md) element is $-\epsilon/2$, and the only nonzero off-diagonal [matrix](../../../matrix.md) element out of the [ground state](../../../ground-state.md) is $\langle\phi_3,V\phi_1\rangle=\epsilon/2$. Let $E_{\mathrm{box}}=\pi^2\hbar^2/(2ma^2)$. Since $\mathcal E_3=9E_{\mathrm{box}}$, the ground energy is

$$
E_{\mathrm{ground}}=E_{\mathrm{box}}-\frac\epsilon2+\frac{\epsilon^2/4}{E_{\mathrm{box}}-9E_{\mathrm{box}}}+O(\epsilon^3)
=\boxed{\frac{\pi^2\hbar^2}{2ma^2}-\frac\epsilon2-\frac{ma^2\epsilon^2}{16\pi^2\hbar^2}+O(\epsilon^3).}
$$

The second-order term is negative, as expected for a nondegenerate ground level: every excited-[quantum state](../../../quantum-state.md) denominator is negative. The first-order shift is also negative for positive $\epsilon$, because the ground-[quantum state](../../../quantum-state.md) density is largest near the center, where this perturbing potential is negative.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2011](../../2011-split.md)
3. [Past exam of the quantum theory and quantum computers course of the University of Oxford](../../split.md)
4. [Quantum theory and quantum computers course of the University of Oxford](../../../quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
