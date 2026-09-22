<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Partition the lattice into blocks of side $b$ sites, with $b>1$, and retain one coarse spin $\sigma'_R$ per block. A [blocking kernel](../../../../../../blocking-kernel.md) is a nonnegative conditional weight $K_b(\sigma',\sigma)$ normalized by $\sum_{\sigma'}K_b(\sigma',\sigma)=1$ for every microscopic configuration. A deterministic majority rule, with fair resolution of ties, is one example.

Define the blocked [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) and its field-independent constant by

$$
e^{-\beta_{\rm th}[H(u',\sigma')+N'C']}=
\sum_\sigma K_b(\sigma',\sigma)e^{-\beta_{\rm th}[H(u,\sigma)+NC]},\qquad N'=N/b^D.
$$

Summing over $\sigma'$ proves exact equality of the old and new [partition functions](../../../../../../canonical-partition-function.md). The lattice spacing becomes $ba$; expressing lengths again in the original units completes the [real-space renormalization group](../../../../../../real-space-renormalization-group.md) step. Blocking generally generates many-body and longer-range interactions, so exactness requires retaining the full operator space and the additive constant. A finite-coupling truncation is a calculational approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
