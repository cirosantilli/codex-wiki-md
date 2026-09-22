<h1 id="section-b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $q$ be the [coordination number of a lattice](../../../../../coordination-number-of-a-lattice.md), the number of nearest neighbours of each cell away from boundaries. Define an effective [chemical potential](../../../../../chemical-potential-split.md) incorporating the cell's translational [entropy](../../../../../entropy-split.md):

$$
\widetilde\mu=\mu+k_BT\ln\frac b{\lambda^3},\qquad
\left(\frac{e^{\beta\mu}b}{\lambda^3}\right)^{\sum n_\alpha}=e^{\beta\widetilde\mu\sum n_\alpha}.
$$

Use $\langle\alpha\alpha'\rangle$ for an unordered nearest-neighbour bond, counted once. The occupation [Hamiltonian](../../../../../hamiltonian.md) including the chemical-potential term is

$$
\mathcal H_{\rm occ}=-4J\sum_{\langle\alpha\alpha'\rangle}n_\alpha n_{\alpha'}-\widetilde\mu\sum_\alpha n_\alpha.
$$

Under $n_\alpha=(1+\sigma_\alpha)/2$, one bond contributes

$$
-4Jn_\alpha n_{\alpha'}=-J\left(1+\sigma_\alpha+\sigma_{\alpha'}+\sigma_\alpha\sigma_{\alpha'}\right).
$$

In a regular lattice with periodic [boundary conditions](../../../../../boundary-condition.md), the number of bonds is $Mq/2$, and each spin occurs in $q$ linear bond terms. Therefore

$$
\mathcal H_{\rm eff}=-J\sum_{\langle\alpha\alpha'\rangle}\sigma_\alpha\sigma_{\alpha'}
-\left(qJ+\frac{\widetilde\mu}{2}\right)\sum_\alpha\sigma_\alpha
-\frac{MqJ}{2}-\frac{M\widetilde\mu}{2}.
$$

The pair sum equals one half of the ordered sum used in the paper. Consequently the effective field is

$$
\boxed{h(T,\mu)=qJ+\frac\mu2+\frac{k_BT}{2}\ln\frac b{\lambda^3}.}
$$

Thus $\Xi=\sum_{\{\sigma\}}e^{-\beta\mathcal H_{\rm eff}}$ is the [Ising model](../../../../../ising-model.md) partition sum, including the displayed spin-independent constant if its absolute normalization is required. Dropping that constant changes $\Xi$ by a multiplicative factor but leaves spin [probabilities](../../../../../probability.md) and the phase-transition argument unchanged. For simple cubic cells in three dimensions, $q=6$ and the first term in $h$ is $6J$. Open boundaries replace $q$ by the local coordination near the surface; the stated uniform field is the bulk or periodic-lattice result.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
