<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix the convention $\iota_{X_f}\omega=-df$ for a [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md). Nondegeneracy of the [symplectic form](../../../../../symplectic-form.md) gives one unique smooth $X_f$ for each smooth real-valued function $f$. Define the [Poisson bracket](../../../../../poisson-bracket.md) by

$$
\{f,g\}=\omega(X_f,X_g)=X_f(g).
$$

In coordinates with $\omega=\sum dq^i\wedge dp_i$, this is $\sum(f_{q^i}g_{p_i}-f_{p_i}g_{q^i})$. Thus the sign convention is explicit and agrees with the usual coordinate [Poisson bracket](../../../../../poisson-bracket.md). By [Cartan's magic formula](../../../../../cartan-s-magic-formula.md), $\mathcal L_{X_f}\omega=d\iota_{X_f}\omega+\iota_{X_f}d\omega=0$. The contraction–[Lie derivative](../../../../../lie-derivative-of-a-differential-form.md) commutator identity now gives

$$
\iota_{[X_f,X_g]}\omega=\mathcal L_{X_f}(\iota_{X_g}\omega)-\iota_{X_g}(\mathcal L_{X_f}\omega)=-d(X_f g)=-d\{f,g\}.
$$

Hence **the [Hamiltonian Lie algebra homomorphism](../../../../../hamiltonian-lie-algebra-homomorphism.md) is $\boxed{\Phi(f)=X_f,\quad[X_f,X_g]=X_{\{f,g\}}}$**. It is linear and onto the space of [Hamiltonian vector fields](../../../../../hamiltonian-vector-field.md) by definition. For completeness, the [Jacobi identity](../../../../../jacobi-identity.md) for the bracket on functions follows from closure of $\omega$: evaluating $d\omega=0$ on $X_f,X_g,X_h$ and using the displayed commutator relation gives the cyclic Jacobi sum zero. Thus this really is a map of [Lie algebras](../../../../../lie-algebra-split.md), not just a bracket-preserving notation.

Its kernel is determined by nondegeneracy:

$$
\boxed{\ker\Phi=\{f:df=0\}=\{\text{locally constant smooth functions}\}.}
$$

On a connected manifold these are precisely the real constants; on a disconnected manifold the constant may differ on each component. Therefore the quotient by these functions is isomorphic to the [Lie algebra](../../../../../lie-algebra-split.md) of [Hamiltonian vector fields](../../../../../hamiltonian-vector-field.md). The printed “homeomorphis” is interpreted as homomorphism: the map before taking this quotient is not an isomorphism because of its nontrivial kernel. The alternative convention $\iota_{X_f}\omega=df$ requires a corresponding bracket sign change to retain this homomorphism.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
