<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the same real [elastic stiffness tensor](../../../../../../elastic-stiffness-tensor.md) for both fields, including its minor and major symmetries, and let $t_i^a=\widehat\sigma_{ij}^a n_j$, with outward unit boundary normal $n_j$. No [complex conjugation](../../../../../../complex-conjugation.md) is needed for the initial bilinear identity. Define

$$
F_j=\widehat\sigma_{ij}^a\widehat u_i^b-\widehat u_i^a\widehat\sigma_{ij}^b.
$$

The [divergence](../../../../../../divergence.md) has two force-balance terms and two cross-gradient terms. The latter cancel because

$$
\widehat\sigma_{ij}^a\partial_j\widehat u_i^b=\widehat\sigma_{ij}^b\partial_j\widehat u_i^a;
$$

this follows by exchanging the two strain-gradient factors using major symmetry and the minor pair symmetries. The frequency-domain equations then give

$$
\partial_jF_j=-(\rho\omega_a^2\widehat u_i^a+\widehat f_i^a)\widehat u_i^b+\widehat u_i^a(\rho\omega_b^2\widehat u_i^b+\widehat f_i^b).
$$

Integrating and applying the [divergence theorem](../../../../../../divergence-theorem.md) proves

$$
\boxed{\int_{\mathcal D}\left[-(\rho\omega_a^2\widehat u_i^a+\widehat f_i^a)\widehat u_i^b+\widehat u_i^a(\rho\omega_b^2\widehat u_i^b+\widehat f_i^b)\right]dV=\int_{\partial\mathcal D}(t_i^a\widehat u_i^b-\widehat u_i^at_i^b)dS.}
$$

This is the [Betti identity for elastodynamic fields](../../../../../../betti-identity-for-elastodynamic-fields.md). Spatially varying stiffness is allowed because its [derivatives](../../../../../../derivative.md) remain inside the [divergence](../../../../../../divergence.md). The original PDF's constitutive contraction is $c_{ijpq}\partial_p\widehat u_q$; the TeX's repeated [displacement field](../../../../../../displacement-field-mechanics.md) index is erroneous.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
