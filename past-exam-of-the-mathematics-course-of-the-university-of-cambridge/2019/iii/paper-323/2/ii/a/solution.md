<h1 id="2/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Memorylessness means that the ensemble's average [density operator](../../../../../../../density-matrix.md) is $\rho^{(n)}=\pi^{\otimes n}$. Its [spectral decomposition](../../../../../../../spectral-decomposition.md) is

$$
\rho^{(n)}=\sum_{i^n}q_{i_1}\cdots q_{i_n}|\phi_{i^n}\rangle\langle\phi_{i^n}|,\qquad
|\phi_{i^n}\rangle=|\phi_{i_1}\rangle\otimes\cdots\otimes|\phi_{i_n}\rangle.
$$

The product eigenvalues give

$$
S(\rho^{(n)})
=-\sum_{i^n}\left(\prod_jq_{i_j}\right)\log_2\left(\prod_jq_{i_j}\right)
=nH(q)=nS(\pi).
$$

Zero eigenvalues contribute zero to the [Von Neumann entropy](../../../../../../../von-neumann-entropy-split.md) and are excluded from logarithmic typicality tests.

The [quantum typical subspace](../../../../../../../quantum-typical-subspace.md) is the span of eigenvectors whose eigenvalues satisfy

$$
\left|-\frac1n\log_2(q_{i_1}\cdots q_{i_n})-S(\pi)\right|\leq\varepsilon.
$$

Its orthogonal projection $P_\varepsilon^{(n)}$ selects precisely the classical [typical set](../../../../../../../typical-set.md) for the eigenvalue distribution $q$. The [typical-set cardinality bounds](../../../../../../../typical-set-cardinality-bounds.md) and the [weak law of large numbers](../../../../../../../weak-law-of-large-numbers.md) therefore give

$$
\boxed{\dim\mathcal T_\varepsilon^{(n)}\leq2^{n(S(\pi)+\varepsilon)}},\qquad
\boxed{\operatorname{Tr}(\rho^{(n)}P_\varepsilon^{(n)})\geq1-\delta}
$$

for any fixed $\delta>0$ and all sufficiently large $n$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [2](../../../2.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
