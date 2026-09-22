<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p:U(H)\to PU(H)$ for the scalar quotient. Local strongly continuous sections exist: near a fixed projective unitary, fix its phase by requiring one nonzero [matrix](../../../../../../matrix.md) coefficient, taken relative to a fixed representative, to be positive real. Thus the pullback $E=\{(z,V):p(V)=\rho(z)\}$ is a locally trivial central extension of the [circle](../../../../../../circle.md) by the [circle](../../../../../../circle.md). It is compact, since finitely many closed arcs inside such trivializing neighbourhoods cover the compact base and each pullback is a product with the compact fibre.

Any two lifts commute up to a scalar. Their [commutator](../../../../../../commutator.md) defines a continuous alternating bicharacter $c(z,w)$ on the base: the scalar [commutator](../../../../../../commutator.md) is independent of phase choices and multiplicative in each argument. If $z$ is an irrational rotation, its powers are dense and $c(z,z^m)=1$ for every integer $m$. Continuity makes $c(z,w)=1$ for every $w$. Such $z$ are themselves dense, so **all the lifts commute**, and $E$ is abelian.

The tautological representation $R(z,V)=V$ is strongly continuous. Choose a unit [vector](../../../../../../vector.md) $\xi$ and average its [rank-one orthogonal projection](../../../../../../rank-one-orthogonal-projection.md) over [Haar measure](../../../../../../haar-measure.md) on $E$:

$$
K=\int_E R(e)|\xi\rangle\langle\xi|R(e)^*\,de.
$$

The integrand is trace-norm continuous, so $K$ is positive compact with [trace](../../../../../../matrix-trace.md) one, and commutes with $R(E)$. A positive [eigenvalue](../../../../../../eigenvalue.md) has a nonzero finite-dimensional [eigenspace](../../../../../../eigenspace.md) invariant under $E$. Commuting unitary [matrices](../../../../../../matrix.md) on that space have a common unit [eigenvector](../../../../../../eigenvector.md) $\eta$. Therefore $R(e)\eta=\chi(e)\eta$ for a continuous character $\chi$ of $E$.

On the central fibre, $R(1,\lambda I)=\lambda I$, so $\chi(1,\lambda I)=\lambda$. Consequently

$$
\boxed{U_z=\chi(z,V)^{-1}V\quad\text{for any lift }V\text{ of }\rho(z)}
$$

is independent of that lift. It is a [homomorphism](../../../../../../homomorphism.md) and strongly continuous, because the continuous map on $E$ descends through its quotient to the base. It satisfies $p(U_z)=\rho(z)$. This proves [circle projective representations lift to unitary representations](../../../../../../circle-projective-representations-lift-to-unitary-representations.md) using an actual central character, rather than assuming a global choice of phases.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
