<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $R^+$ be the [positive roots](../../../../../../positive-root.md), $W$ the [Weyl group](../../../../../../weyl-group.md), $\ell(w)$ its [Coxeter length](../../../../../../coxeter-length.md), $\rho$ the [half-sum of positive roots](../../../../../../half-sum-of-positive-roots.md), and $\alpha^\vee$ a [coroot](../../../../../../coroot.md). For a dominant integral highest weight $\lambda$, the [Weyl character formula](../../../../../../weyl-character-formula.md) is

$$
\operatorname{ch}L_\lambda
=\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}}
=\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{e^\rho\prod_{\alpha\in R^+}(1-e^{-\alpha})}.
$$

Taking the value at the identity gives the [Weyl dimension formula](../../../../../../weyl-dimension-formula.md)

$$
\dim L_\lambda
=\prod_{\alpha\in R^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}
{\langle\rho,\alpha^\vee\rangle}.
$$

For the q-character convention relevant to the [Principal sl2 subalgebra](../../../../../../principal-sl2-subalgebra.md), set $h_{\mathrm{pr}}=2\rho^\vee$, so $\alpha_i(h_{\mathrm{pr}})=2$ for every simple root, and define

$$
\operatorname{ch}_qL_\lambda
=\sum_\mu(\dim L_\lambda[\mu])q^{\mu(h_{\mathrm{pr}})}.
$$

The q-character formula is the principal specialization of the [Weyl character formula](../../../../../../weyl-character-formula.md):

$$
\boxed{\operatorname{ch}_qL_\lambda
=\frac{\sum_{w\in W}(-1)^{\ell(w)}q^{\langle w(\lambda+\rho),2\rho^\vee\rangle}}
{\sum_{w\in W}(-1)^{\ell(w)}q^{\langle w\rho,2\rho^\vee\rangle}}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
