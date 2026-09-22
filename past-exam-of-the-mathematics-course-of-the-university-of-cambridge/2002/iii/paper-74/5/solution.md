<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Poisson manifold](../../../../../poisson-manifold.md) has a skew bilinear bracket on smooth functions which is a derivation in each argument and satisfies the [Jacobi identity](../../../../../jacobi-identity.md). Locally a [Poisson bivector](../../../../../poisson-bivector.md) $\Pi$ represents it by

$$
\{f,g\}=\Pi^{ij}\partial_i f\,\partial_jg,\qquad \Pi^{ij}=-\Pi^{ji}.
$$

The derivation property is automatic for this expression. On applying the Jacobi identity to coordinate functions, and then using the derivation property for arbitrary functions, the necessary and sufficient condition is

$$
\boxed{\Pi^{i\ell}\partial_\ell\Pi^{jk}
+\Pi^{j\ell}\partial_\ell\Pi^{ki}
+\Pi^{k\ell}\partial_\ell\Pi^{ij}=0.}
$$

Equivalently its [Schouten-Nijenhuis bracket](../../../../../schouten-nijenhuis-bracket.md) $[\Pi,\Pi]$ vanishes.

A [symplectic manifold](../../../../../symplectic-manifold.md) has a closed nondegenerate two-form $\omega$. Write its coefficient matrix as $\Omega_{ij}$ and set $\Pi^{ij}=(\Omega^{-1})^{ij}$. It is skew and defines the bracket above. Differentiating $\Pi\Omega=I$ gives $\partial_\ell\Pi=-\Pi(\partial_\ell\Omega)\Pi$. Substitution into the Jacobi condition gives

$$
\Pi^{i\ell}\partial_\ell\Pi^{jk}+\text{cyclic}
=\Pi^{ia}\Pi^{jb}\Pi^{kc}
\bigl(\partial_a\Omega_{bc}+\partial_b\Omega_{ca}+\partial_c\Omega_{ab}\bigr)=0,
$$

where the last equality is $d\omega=0$. Thus **every symplectic manifold is Poisson**. In this convention the [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) satisfies $\iota_{X_f}\omega=-df$, and $\{f,g\}=X_gf$; this will also be the convention below.

The converse fails because a Poisson bivector need not be invertible. On $\mathbb R^2$, take $\Pi=0$. Its bracket is identically zero and satisfies every Poisson axiom, but it cannot be the inverse of any nondegenerate two-form. This is an even-dimensional counterexample, so odd dimension is not the only obstruction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
