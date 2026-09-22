<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $P=(\omega^{ab})$ be a smooth [antisymmetric matrix](../../../../../skew-symmetric-matrix.md) field. It defines a [Poisson bivector](../../../../../poisson-bivector.md) through

$$
\{f,g\}=\omega^{ab}(x)\,\partial_af\,\partial_bg,\qquad f,g\in C^\infty(U).
$$

This [Poisson bracket](../../../../../poisson-bracket.md) is bilinear, antisymmetric and a [derivation](../../../../../derivation-of-an-algebra.md) in each argument. It defines a [Poisson manifold](../../../../../poisson-manifold.md) when it also satisfies the [Jacobi identity](../../../../../jacobi-identity.md). Apply that identity in the form $\{\{f,g\},h\}+\{\{g,h\},f\}+\{\{h,f\},g\}=0$ to the coordinate functions. Since $\{x^a,x^b\}=\omega^{ab}$, it gives

$$
\boxed{J^{abc}:=\omega^{dc}\partial_d\omega^{ab}
+\omega^{db}\partial_d\omega^{ca}
+\omega^{da}\partial_d\omega^{bc}=0.}
$$

This is the [coordinate Jacobi condition for a Poisson bivector](../../../../../coordinate-jacobi-condition-for-a-poisson-bivector.md). It is also sufficient: in the [Jacobi identity](../../../../../jacobi-identity.md) for arbitrary functions the terms containing second derivatives cancel by antisymmetry, leaving $J^{abc}(\partial_af)(\partial_bg)(\partial_ch)$. Thus the coordinate condition captures the whole obstruction.

Now suppose the [Poisson bivector](../../../../../poisson-bivector.md) is nondegenerate. Write $S=P^{-1}$, so $S_{ab}\omega^{bc}=\delta_a^c$, and define the [2-form](../../../../../2-form.md)

$$
\Omega=\frac12 S_{ab}\,dx^a\wedge dx^b.
$$

An overall minus sign in identifying the [symplectic form](../../../../../symplectic-form.md) depends on the convention for [Hamiltonian vector fields](../../../../../hamiltonian-vector-field.md); it does not affect the closure argument. Differentiating the inverse matrix gives

$$
\partial_dS_{ij}=-S_{ia}(\partial_d\omega^{ab})S_{bj}
=S_{ia}S_{jb}\partial_d\omega^{ab}.
$$

Contract the coordinate [Jacobi identity](../../../../../jacobi-identity.md) with $S_{ia}S_{jb}S_{kc}$. Antisymmetry gives $\omega^{dc}S_{kc}=-\delta_k^d$, and similarly for the other terms, hence

$$
S_{ia}S_{jb}S_{kc}J^{abc}
=-\{\partial_kS_{ij}+\partial_jS_{ki}+\partial_iS_{jk}\}=0.
$$

The cyclic expression is precisely the coefficient of the [exterior derivative](../../../../../exterior-derivative.md) $d\Omega$. Therefore

$$
\boxed{d\Omega=0.}
$$

Since $S$ is antisymmetric and nondegenerate, $\Omega$ is a [symplectic form](../../../../../symplectic-form.md). This proves the [closure of the inverse of a nondegenerate Poisson bivector](../../../../../closure-of-the-inverse-of-a-nondegenerate-poisson-bivector.md). The matrix entries $\omega^{ab}$ are scalar functions; the codomain in the source's matrix description should be read as the space of antisymmetric matrices, rather than a vector-valued individual entry.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
