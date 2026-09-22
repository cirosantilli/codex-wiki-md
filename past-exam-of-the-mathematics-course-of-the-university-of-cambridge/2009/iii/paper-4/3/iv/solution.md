<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [permutation character](../../../../../../permutation-character.md) $\xi^\mu(g)$ is the number of $\mu$-[tabloids](../../../../../../tabloid.md) fixed by $g$, since the trace of a permutation matrix counts fixed basis elements. It is therefore an integer. Arrange the partitions in decreasing lexicographic order. If $\lambda$ strictly dominates $\mu$, the first part at which they differ is larger for $\lambda$, so this ordering places $\lambda$ before $\mu$.

For the first partition $(n)$, there is just one [tabloid](../../../../../../tabloid.md), and $\chi^{(n)}=\xi^{(n)}=1_{S_n}$ is integer-valued. At a general partition $\mu$, the decomposition in (iii) can be rearranged as

$$
\chi^\mu=\xi^\mu-\sum_{\substack{\lambda\unrhd\mu\\\lambda\ne\mu}}a_{\lambda\mu}\chi^\lambda,\qquad a_{\lambda\mu}\in\mathbb Z_{\geq0}.
$$

By induction, all characters in the sum are already integer-valued; the [permutation character](../../../../../../permutation-character.md) and all coefficients are also integral. Thus $\chi^\mu$ is integer-valued. Finite induction proves that [symmetric-group characters are integer-valued](../../../../../../symmetric-group-characters-are-integer-valued.md):

$$
\boxed{\chi^\lambda(g)\in\mathbb Z\qquad(g\in S_n,\ \lambda\vdash n).}
$$

The diagonal coefficient one is essential: it lets us solve for $\chi^\mu$ without division, preserving integrality.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
