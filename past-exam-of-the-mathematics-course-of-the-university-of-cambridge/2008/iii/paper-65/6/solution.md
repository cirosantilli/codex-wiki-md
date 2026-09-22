<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Poisson manifold](../../../../../poisson-manifold.md) is a [smooth manifold](../../../../../smooth-manifold.md) with a smooth antisymmetric [bivector](../../../../../bivector.md) $\pi=\frac12\pi^{ij}\partial_i\wedge\partial_j$ whose function bracket $\{f,g\}=\pi^{ij}(\partial_if)(\partial_jg)$ satisfies the [Jacobi identity](../../../../../jacobi-identity.md). The bracket is automatically a derivation in each argument. A [symplectic manifold](../../../../../symplectic-manifold.md) has a nondegenerate [differential two-form](../../../../../2-form.md) $\omega$ satisfying $d\omega=0$, that is, a [closed differential form](../../../../../closed-differential-form.md); nondegeneracy forces its dimension to be even. It determines a nondegenerate [Poisson structure](../../../../../poisson-structure.md). We use matrix convention $\pi=-\omega^{-1}$, so that $\iota_{X_H}\omega=dH$ corresponds to $X_H(f)=\{f,H\}$.

Examples of genuinely nonsymplectic Poisson geometries include the zero bracket on $\mathbb R^3$ and the [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) $\{x_i,x_j\}=\epsilon_{ijk}x_k$ on $\mathbb R^3$. Their three-dimensional underlying manifold cannot carry a nondegenerate two-form. In the latter case the Poisson rank is two away from the origin and zero at the origin, with spheres and the origin as [symplectic leaves](../../../../../symplectic-leaf.md). Even in even dimension a given Poisson structure need not come from a symplectic form: $\pi=x\partial_x\wedge\partial_y$ on $\mathbb R^2$ satisfies Jacobi but vanishes along $x=0$. The statement concerns this degenerate structure, not a claim that $\mathbb R^2$ admits no other symplectic structure.

For any candidate bivector, applying the [Jacobi identity](../../../../../jacobi-identity.md) to coordinate functions gives the necessary condition

$$
\boxed{J^{ijk}:=\pi^{i\ell}\partial_\ell\pi^{jk}
+\pi^{j\ell}\partial_\ell\pi^{ki}
+\pi^{k\ell}\partial_\ell\pi^{ij}=0.}
$$

It is sufficient as well: expanding $\{f,\{g,h\}\}$ and its cyclic companions cancels all terms with second derivatives by antisymmetry of $\pi$. What remains is $J^{ijk}(\partial_if)(\partial_jg)(\partial_kh)$. This is the [coordinate Jacobi condition for a Poisson bivector](../../../../../coordinate-jacobi-condition-for-a-poisson-bivector.md).

For a symplectic form, differentiate $\omega\pi=-I$ to obtain $\partial_\ell\pi=\pi(\partial_\ell\omega)\pi$. Substituting this into the cyclic expression gives

$$
J^{ijk}=-\pi^{ia}\pi^{jb}\pi^{kc}
\bigl(\partial_a\omega_{bc}+\partial_b\omega_{ca}+\partial_c\omega_{ab}\bigr)=0,
$$

because $d\omega=0$. Thus **the inverse symplectic structure always satisfies the Jacobi identity**. Conversely, for a nondegenerate Poisson structure, multiplying by three inverse matrices proves closure of its associated two-form.

In momentum space, choose Hamiltonian $H(\mathbf p)=E(\mathbf p)$ and the constant [Poisson bivector](../../../../../poisson-bivector.md)

$$
\boxed{\pi^{ij}=e\epsilon_{ijk}B_k,\qquad
\pi=e\left(B_1\partial_{p_2}\wedge\partial_{p_3}
+B_2\partial_{p_3}\wedge\partial_{p_1}
+B_3\partial_{p_1}\wedge\partial_{p_2}\right).}
$$

Its [Poisson bracket](../../../../../poisson-bracket.md) is $\{f,g\}=e\mathbf B\cdot(\nabla f\times\nabla g)$. The [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) therefore gives

$$
\dot p_i=\{p_i,E\}=e\epsilon_{ijk}B_k\partial_{p_j}E
=e(\mathbf v\times\mathbf B)_i,\qquad \mathbf v=\nabla_{\mathbf p}E,
$$

exactly the prescribed motion. The sign here uses the signed charge $e$ as printed; an electron's physical charge may be negative. Since the [magnetic field](../../../../../magnetic-field.md) is uniform, every derivative of $\pi^{ij}$ vanishes, so every term in $J^{ijk}$ is zero. **Jacobi holds independently of the dispersion function $E$.** This is the [momentum-space Poisson structure for a uniform magnetic field](../../../../../momentum-space-poisson-structure-for-a-uniform-magnetic-field.md).

For $e\mathbf B\ne0$ this bivector has rank two and $C(\mathbf p)=\mathbf B\cdot\mathbf p$ is a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md): $\{C,f\}=0$ for every $f$. Its [symplectic leaves](../../../../../symplectic-leaf.md) are the planes $C=c$. For axes with $\mathbf B=B_0\mathbf e_3$, the leaf form is $\omega=(eB_0)^{-1}dp_1\wedge dp_2$ in our inverse-sign convention. Also $\dot E=\{E,E\}=0$, so trajectories on a [Fermi surface](../../../../../fermi-surface.md) lie on its intersections with these planes, typically curves. The energy surface is invariant for this Hamiltonian, but need not be a Poisson submanifold; the bracket has been defined on the whole momentum space. If $e\mathbf B=0$, the Poisson structure and motion vanish.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
