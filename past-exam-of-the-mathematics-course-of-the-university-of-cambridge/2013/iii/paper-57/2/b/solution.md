<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a hidden variable in the [deterministic local hidden-variable model](../../../../../../deterministic-local-hidden-variable-model.md), so that every $A_j,B_j$ is an integer. Let $[x]_d$ be the representative of $x$ modulo $d$ in $\{0,\ldots,d-1\}$. The terms in the [chained modular Bell inequality](../../../../../../chained-modular-bell-inequality.md) alternate between the two parties. Before reduction their sum telescopes:

$$
(A_1-B_1)+(B_1-A_2)+(A_2-B_2)+\cdots+(A_N-B_N)+(B_N-A_1-1)=-1.
$$

After reduction, the sum $T$ is a nonnegative integer congruent to $-1$ modulo $d$. For $d\geq2$, the smallest possible such integer is $d-1$. Thus $T\geq d-1$ for each hidden variable separately. Averaging over the setting-independent distribution gives

$$
\boxed{\sum_{j=1}^N\mathbb E\big([A_j-B_j]_d\big)+\sum_{j=1}^{N-1}\mathbb E\big([B_j-A_{j+1}]_d\big)+\mathbb E\big([B_N-A_1-1]_d\big)\geq d-1}.
$$

Here each expectation is the [expectation value](../../../../../../expectation-value.md) of the reduced random variable, not the residue of its expectation. Each term can be measured using one setting at each site. The proof uses their common deterministic assignments rather than any joint quantum measurement of incompatible local settings. Stochastic [local hidden-variable theories](../../../../../../local-hidden-variable-theory.md) satisfy the same bound: include their local random seeds in $\lambda$ and average the resulting deterministic assignments.

The printed final coefficient in the definition of the average is typographically incomplete. The expectation used here is the usual $\mathbb E X=\sum_{x=0}^{d-1}xP(X=x)$, with final coefficient $d-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
