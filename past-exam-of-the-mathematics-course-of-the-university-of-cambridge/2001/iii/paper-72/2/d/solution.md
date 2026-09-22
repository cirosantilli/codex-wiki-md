<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First interpret the displayed critical [correlation function](../../../../../../correlation-function.md) as the [connected correlation function](../../../../../../connected-correlation-function.md)

$$
G_c(x)=\langle m(x)m(0)\rangle-\langle m\rangle^2.
$$

Above the transition at zero field the subtraction is zero; in an ordered phase it is essential. For a dimensionless source coupled to the total [magnetization](../../../../../../magnetization.md) $M=\int d^dx\,m(x)$, differentiating $Z$ twice gives $\chi=V^{-1}(\langle M^2\rangle-\langle M\rangle^2)$. Translation invariance then proves the [correlation-function susceptibility sum rule](../../../../../../correlation-function-susceptibility-sum-rule.md)

$$
\chi=\int d^dx\,G_c(x).
$$

Insert the scaling form, use spherical coordinates and set $s=r/\xi$:

$$
\chi_s=S_d\int_a^\infty dr\,r^{1-\eta}g(r/\xi)
=S_d\xi^{2-\eta}\int_{a/\xi}^\infty ds\,s^{1-\eta}g(s).
$$

For $\eta<2$, finite nonzero $g(0)$ and an integrable large-$s$ tail, the last integral tends to a finite nonzero constant. Microscopic separations add an analytic response background. Thus the singular [magnetic susceptibility](../../../../../../magnetic-susceptibility.md) obeys $\chi_s\asymp\xi^{2-\eta}$, and at zero field $\xi\asymp|t|^{-\nu}$ gives the [Fisher scaling relation](../../../../../../fisher-scaling-relation.md)

$$
\boxed{\gamma=(2-\eta)\nu.}
$$

A dimensional magnetic field would add a nonsingular inverse-temperature prefactor. Integrating the full unsubtracted ordered-phase [correlation function](../../../../../../correlation-function.md) instead would yield a volume-divergent term $V\langle m\rangle^2$, which is not the intrinsic susceptibility appearing in this exponent identity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
