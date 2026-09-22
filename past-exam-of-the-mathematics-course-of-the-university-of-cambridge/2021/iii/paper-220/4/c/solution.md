<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the notation supplied in the question, $\widetilde U_t=\psi_t(U_t)$ and $dU_t=\sqrt\kappa\,dB_t$. The [Itô formula](../../../../../../ito-s-lemma.md) and $\partial_t\psi_t(U_t)=-3\psi_t''(U_t)$ give

$$
d\widetilde U_t
=\sqrt\kappa\,\psi_t'(U_t)dB_t
+\left(\frac\kappa2-3\right)\psi_t''(U_t)dt.
$$

For $\kappa=6$, the [drift](../../../../../../drift-coefficient.md) vanishes. The resulting [continuous local martingale](../../../../../../continuous-local-martingale.md) has [quadratic variation](../../../../../../quadratic-variation.md)

$$
d\langle\widetilde U\rangle_t
=6\psi_t'(U_t)^2dt
=3\,d\widetilde a(t).
$$

If $s=\widetilde a(t)/2$ is the usual half-plane-capacity time, then $\langle\widetilde U\rangle=6s$. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) therefore gives

$$
\widetilde U_s=\sqrt6\,\widetilde B_s
$$

for a standard [Brownian motion](../../../../../../brownian-motion-split.md) $\widetilde B$. The mapped hulls are consequently an $\operatorname{SLE}_6$, which proves locality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 220](../../../paper-220-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
