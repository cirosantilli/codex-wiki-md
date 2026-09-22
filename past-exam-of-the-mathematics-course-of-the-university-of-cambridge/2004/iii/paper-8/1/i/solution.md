<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Poisson structure](../../../../../../poisson-structure.md) is a real bilinear operation on [smooth functions](../../../../../../smooth-function.md) on $M$,

$$
\{\cdot,\cdot\}:C^\infty(M)\times C^\infty(M)\longrightarrow C^\infty(M),
$$

which is antisymmetric, obeys the [Jacobi identity](../../../../../../jacobi-identity.md), and is a [derivation](../../../../../../derivation-of-an-algebra.md) in each argument. Explicitly,

$$
\{f,g\}=-\{g,f\},\qquad
\{f,\{g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0,\qquad
\{f,gh\}=\{f,g\}h+g\{f,h\}.
$$

Antisymmetry supplies the corresponding [Leibniz rule](../../../../../../leibniz-rule.md) in the first argument. Equivalently it is a smooth [Poisson bivector](../../../../../../poisson-bivector.md) $\Pi$ with $\{f,g\}=\Pi(df,dg)$ and $[\Pi,\Pi]=0$ for the [Schouten-Nijenhuis bracket](../../../../../../schouten-nijenhuis-bracket.md). In local coordinates,

$$
\{f,g\}=\sum_{i,j}\Pi^{ij}(x)\partial_i f\partial_j g,\qquad
\Pi^{ij}=-\Pi^{ji},\qquad
\sum_l\left(\Pi^{il}\partial_l\Pi^{jk}+\Pi^{jl}\partial_l\Pi^{ki}+\Pi^{kl}\partial_l\Pi^{ij}\right)=0.
$$

The last equation is the coordinate [Jacobi identity](../../../../../../jacobi-identity.md). Nondegeneracy is not part of the definition: a [Poisson structure](../../../../../../poisson-structure.md) may have [Casimir functions](../../../../../../casimir-function-of-a-poisson-manifold.md) and [symplectic leaves](../../../../../../symplectic-leaf.md) of different dimensions.

A [Hamiltonian system](../../../../../../hamiltonian-system.md) consists of such a [Poisson manifold](../../../../../../poisson-manifold.md), a [Hamiltonian](../../../../../../hamiltonian.md) $H\in C^\infty(M)$, and the flow of its [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md). Choose the convention

$$
\boxed{X_H(f)=\{f,H\},\qquad \dot x^i=\sum_j\Pi^{ij}\partial_jH.}
$$

For an observable with no explicit time dependence, $df/dt=\{f,H\}$. In particular $H$ is conserved because $\{H,H\}=0$. For the canonical [Poisson bracket](../../../../../../poisson-bracket.md), this convention gives $\dot q_i=\partial H/\partial p_i$ and $\dot p_i=-\partial H/\partial q_i$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
