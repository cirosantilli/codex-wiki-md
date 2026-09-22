<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take [metric signature](../../../../metric-signature.md) $(+,-,-,-)$ and the supplied covariant [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md), so $F_{0i}=E_i$ and $F_{ij}=-\epsilon_{ijk}B_k$. Raising both indices reverses the time-space components but leaves the spatial components unchanged. Its complete contraction is therefore

$$
F_{\mu\nu}F^{\mu\nu}=2(B^2-E^2).
$$

Define the [dual electromagnetic field tensor](../../../../dual-electromagnetic-field-tensor.md) by $\widetilde F^{\mu\nu}=\tfrac12\varepsilon^{\mu\nu\rho\sigma}F_{\rho\sigma}$, with $\varepsilon^{0123}=+1$. Direct contraction gives

$$
\boxed{E^2-B^2=-\frac12F_{\mu\nu}F^{\mu\nu},\qquad
\mathbf E\cdot\mathbf B=-\frac14F_{\mu\nu}\widetilde F^{\mu\nu}.}
$$

These [electromagnetic field invariants](../../../../electromagnetic-field-invariants.md) are complete tensor contractions. The second is a [pseudoscalar](../../../../pseudoscalar.md): it is invariant under proper [Lorentz transformations](../../../../lorentz-transformation.md) and changes sign under spatial inversion.

For $T^{0i}$ the metric trace term vanishes. Since $F^0{}_j=E_j$,

$$
F^0{}_{\rho}F^{i\rho}=\sum_jE_j(-\epsilon_{ijk}B_k)=-(\mathbf E\times\mathbf B)_i.
$$

Consequently the [Poynting vector](../../../../poynting-vector.md) is exactly the time-space row in the stated $c=1$ units:

$$
\boxed{(T^{01}_{\rm em},T^{02}_{\rm em},T^{03}_{\rm em})
=\frac1{\mu_0}\mathbf E\times\mathbf B.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
