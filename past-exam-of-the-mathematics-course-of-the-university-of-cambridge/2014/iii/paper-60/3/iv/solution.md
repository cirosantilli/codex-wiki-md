<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use [Klein's inequality](../../../../../../klein-s-inequality.md), or equivalently [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md). First check the support needed for the logarithm. If $q_y=0$, positivity gives $|\rho_{yz}|^2\leq\rho_{yy}\rho_{zz}=0$ for every $z$; the corresponding row and column vanish. Thus [support inclusion under rank-one dephasing](../../../../../../support-inclusion-under-rank-one-dephasing.md) gives $\operatorname{supp}\rho\subseteq\operatorname{supp}\sigma$, and the logarithms may be evaluated on this support.

Since $\log\sigma$ is diagonal in the dephasing basis,

$$
\operatorname{Tr}\rho\log_2\sigma=\sum_{y:q_y>0}q_y\log_2q_y=\operatorname{Tr}\sigma\log_2\sigma.
$$

The [relative-entropy identity for rank-one dephasing](../../../../../../relative-entropy-identity-for-rank-one-dephasing.md) follows:

$$
D(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)=S(\sigma)-S(\rho).
$$

[Klein's inequality](../../../../../../klein-s-inequality.md) gives $D(\rho\|\sigma)\geq(\operatorname{Tr}\rho-\operatorname{Tr}\sigma)/\ln2=0$. Therefore

$$
\boxed{S(\Lambda(\rho))\geq S(\rho).}
$$

Equality holds precisely when $\rho=\sigma$, meaning that the input was already diagonal in the chosen basis. This quantifies why [rank-one dephasing](../../../../../../rank-one-dephasing.md) removes coherence without reducing the entropy.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
