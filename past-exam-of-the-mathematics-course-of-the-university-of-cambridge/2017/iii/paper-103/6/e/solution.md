<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Fix $\lambda\vdash n$ and $\rho\vdash n-1$. Write $\rho\nearrow\mu$ when a single [addable node of a Young diagram](../../../../../../addable-node-of-a-young-diagram.md) turns $\rho$ into $\mu$. For each positive part $\lambda_i$, let $\lambda^{\downarrow i}$ be the [partition of an integer](../../../../../../partition-of-an-integer.md) obtained by decreasing that part by one, sorting, and omitting zeros. The [Vershik linear relations](../../../../../../vershik-linear-relations.md) are

$$
\boxed{\sum_{\mu:\rho\nearrow\mu}M(\mu,\lambda)
=\sum_{i:\lambda_i>0}M(\rho,\lambda^{\downarrow i}).}
$$

Equal row lengths must be counted separately on the right. Equivalently, if $c(\lambda,\gamma)$ is the number of rows whose decrement produces $\gamma$, the right side is $\sum_{\gamma\nearrow\lambda}c(\lambda,\gamma)M(\rho,\gamma)$. There is no multiplicity coefficient on the left because irreducible [restriction branching rule for a symmetric group](../../../../../../restriction-branching-rule-for-a-symmetric-group.md) is simple.

To prove the relations, restrict the [Young permutation module](../../../../../../young-permutation-module.md) $M^\lambda$ to the subgroup $S_{n-1}$ fixing $n$. The [tabloids](../../../../../../tabloid.md) split into [orbits of a group action](../../../../../../orbit-of-a-group-action.md) according to which labeled row contains $n$. Removing that entry gives, for row $i$, the [Young permutation module](../../../../../../young-permutation-module.md) with composition $\lambda-e_i$, which is isomorphic to the one for its sorted partition. Hence

$$
\operatorname{Res}^{S_n}_{S_{n-1}}M^\lambda\cong\bigoplus_{i:\lambda_i>0}M^{\lambda^{\downarrow i}}.
$$

Its $V^\rho$ multiplicity is the right side. On the other hand decompose $M^\lambda$ into [irreducible representations](../../../../../../irreducible-representation.md) first and apply the [restriction branching rule for a symmetric group](../../../../../../restriction-branching-rule-for-a-symmetric-group.md) to each summand. Its $V^\rho$ multiplicity is then the left side. Equality proves the relation.

For example $\lambda=(2,2)$ restricts to $2M^{(2,1)}$, so the coefficient is two rather than one. For $\lambda=(1^n)$, the [regular representation](../../../../../../regular-representation.md), the relation reduces to $\sum_{\mu:\rho\nearrow\mu}\dim V^\mu=n\dim V^\rho$. These checks emphasize why counting distinct resulting partitions without their row multiplicities would give a false recurrence.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
