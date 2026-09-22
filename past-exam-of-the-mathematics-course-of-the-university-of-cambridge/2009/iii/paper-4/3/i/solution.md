<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose first that $U$ is not contained in $(S^\lambda)^\perp$. Since [polytabloids](../../../../../../polytabloid.md) span $S^\lambda$, there exist $u\in U$ and a tableau $t$ with $\langle u,e_t\rangle\ne0$. The [column antisymmetrizer](../../../../../../column-antisymmetrizer-of-a-young-tableau.md) identity from the preliminaries gives

$$
\kappa_tu=\langle u,e_t\rangle e_t\in U.
$$

Therefore $e_t\in U$. Because $U$ is an $S_n$-submodule, it contains all translates $ge_t=e_{gt}$, and these span the [Specht module](../../../../../../specht-module.md). Hence $S^\lambda\subseteq U$. If the initial supposition fails, $U\subseteq(S^\lambda)^\perp$. This proves the [James submodule theorem](../../../../../../james-submodule-theorem.md)

$$
\boxed{U\supseteq S^\lambda\quad\text{or}\quad U\subseteq(S^\lambda)^\perp.}
$$

Now let $W$ be a submodule of $S^\lambda$. Apply the dichotomy to $W\subseteq M^\lambda$. Either $W=S^\lambda$, or $W\subseteq S^\lambda\cap(S^\lambda)^\perp$. Positivity of the Hermitian form gives $S^\lambda\cap(S^\lambda)^\perp=\{0\}$: a vector in this intersection has squared norm zero. The same intersection is zero for the bilinear form by the agreement of complements explained above. Since $S^\lambda\ne0$, the only submodules are $0$ and itself. Therefore

$$
\boxed{S^\lambda\text{ is simple over }\mathbb C.}
$$

This use of characteristic zero and nondegeneracy is why the conclusion does not automatically extend to every modular [Specht module](../../../../../../specht-module.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
