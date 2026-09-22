<h1 id="34d/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For noninteracting [fermions](../../../../../../../fermion.md), each single-particle level has occupation $n_i\in\{0,1\}$ by the [Pauli exclusion principle](../../../../../../../pauli-exclusion-principle.md). A microstate has $E=\sum_i\epsilon_in_i$, $N=\sum_in_i$, so its grand-canonical weight is the product of its [independent](../../../../../../../independent-random-variables.md) level weights. The [grand potential](../../../../../../../grand-potential.md) is $\Omega=-kT\log\mathcal Z$; the particle number, [entropy](../../../../../../../entropy.md) and [pressure](../../../../../../../pressure.md) follow from $N=-\partial_\mu\Omega$, $S=-\partial_T\Omega$ and $P=-\partial_V\Omega$. This occupation description is the basis for the product, continuum and adiabatic calculations.

Summing separately over the two allowed occupations of every level gives

$$
\mathcal Z=\prod_i\sum_{n_i=0}^1e^{-n_i(\epsilon_i-\mu)/(kT)}
=\prod_i\left(1+e^{-(\epsilon_i-\mu)/(kT)}\right).
$$

Thus

$$
\boxed{\log\mathcal Z=\sum_i\log\left(1+e^{-(\epsilon_i-\mu)/(kT)}\right).}
$$

The factorization uses the absence of interactions; each level, including any degeneracy labels, is counted separately.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [34D](../../../34d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
