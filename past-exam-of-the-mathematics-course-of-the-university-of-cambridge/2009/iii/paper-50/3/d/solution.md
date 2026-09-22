<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the rank-one [orthogonal projections](../../../../../../orthogonal-projection.md) $P_i=|\phi_i\rangle\langle\phi_i|$. Their [pinching map](../../../../../../pinching-map.md) gives

$$
\mathcal P(\rho)=\sum_iP_i\rho P_i
=\sum_i\langle\phi_i|\rho|\phi_i\rangle\,|\phi_i\rangle\langle\phi_i|=\rho_d.
$$

This has exactly the specified diagonal entries and no off-diagonal entries. Applying the [entropy increase under nonselective projective measurement](../../../../../../entropy-increase-under-nonselective-projective-measurement.md) proved in part (c) therefore gives

$$
\boxed{S(\rho)\leq S(\rho_d).}
$$

Writing $q_i=\langle\phi_i|\rho|\phi_i\rangle$, the output [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is the [Shannon entropy](../../../../../../information-entropy.md) $S(\rho_d)=-\sum_iq_i\log q_i$. Equality holds precisely when $\rho$ was already diagonal in this basis.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
