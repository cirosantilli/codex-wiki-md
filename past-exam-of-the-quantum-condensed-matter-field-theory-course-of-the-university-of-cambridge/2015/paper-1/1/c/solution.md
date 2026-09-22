<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) $\{c_n,c_m^\dagger\}=\delta_{nm}$ and $\{c_n,c_m\}=0$. In particular, $n_m=c_m^\dagger c_m$ is a [projector](../../../../../projection-linear-algebra.md), so $(1-2n_m)^2=1$. Define $K_n=\prod_{m<n}(1-2n_m)$. Then $K_n^\dagger=K_n$, $K_n^2=1$, and $K_n$ commutes with $c_n$ and $c_n^\dagger$. Taking the adjoint of the given raising operator gives $S_n^-=c_n^\dagger K_n$. Hence

$$
[S_n^+,S_n^-]
=K_nc_nc_n^\dagger K_n-c_n^\dagger K_n^2c_n
=c_nc_n^\dagger-c_n^\dagger c_n
=1-2n_n=2S_n^z.
$$

Also $[n_n,c_n]=-c_n$ and $[n_n,c_n^\dagger]=c_n^\dagger$ imply $[S_n^z,S_n^\pm]=\pm S_n^\pm$. For different sites, exchanging two [fermion](../../../../../fermion.md) operators contributes one minus sign and commuting an operator through the other site's parity string contributes another; their product is positive. Thus distinct [spin](../../../../../spin.md) algebras commute. **The string supplies precisely the signs required for the [Jordan–Wigner transformation](../../../../../jordan-wigner-transformation.md).** The [fermion](../../../../../fermion.md) vacuum corresponds to [spin](../../../../../spin.md) up, while one occupied site corresponds to [spin](../../../../../spin.md) down; this convention fixes subsequent signs.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
