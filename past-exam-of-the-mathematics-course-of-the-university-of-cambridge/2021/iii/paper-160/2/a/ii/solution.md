<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The restriction form of the [restriction branching rule for a symmetric group](../../../../../../../restriction-branching-rule-for-a-symmetric-group.md) is

$$
\boxed{\operatorname{Res}^{S_n}_{S_{n-1}}S^\lambda
\cong\bigoplus_{\mu\in\lambda^-}S^\mu},
$$

where $\lambda^-$ contains the distinct partitions obtained by deleting one [Removable node of a Young diagram](../../../../../../../removable-node-of-a-young-diagram.md). In particular, the restriction is multiplicity-free.

Restrict the alternating expression

$$
\psi^\lambda=\sum_{\pi\in S_N}\operatorname{sgn}(\pi)\xi^{\lambda-\mathrm{id}+\pi}.
$$

The supplied restriction formula for a Young permutation character, with $k=1$, says that each term restricts by subtracting one from each possible component. After collecting the alternating sums, this gives

$$
\operatorname{Res}^{S_n}_{S_{n-1}}\psi^\lambda
=\sum_i\psi^{\lambda-\epsilon_i}.
$$

If row $i$ has no removable node, part i straightens $\psi^{\lambda-\epsilon_i}$ against the adjacent term with the opposite sign, or makes it zero when two shifted entries coincide. The surviving terms are exactly $\psi^\mu$ for $\mu\in\lambda^-$. Since $\lambda$ and each surviving $\mu$ are partitions, $\psi^\lambda=\chi^\lambda$ and $\psi^\mu=\chi^\mu$. We obtain

$$
\operatorname{Res}^{S_n}_{S_{n-1}}\chi^\lambda
=\sum_{\mu\in\lambda^-}\chi^\mu.
$$

Complex representations of a [finite group](../../../../../../../finite-group.md) are semisimple, so equality of characters proves the asserted module decomposition.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 160](../../../../paper-160-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
