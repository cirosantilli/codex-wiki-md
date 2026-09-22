<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\mathcal V=\langle V_\kappa,\in,R\rangle$. Because $\kappa$ is inaccessible, $|V_\xi|<\kappa$ for every $\xi<\kappa$, and $\kappa$ is regular. Choose one witness in $V_\kappa$ for every existential formula of this expanded language and every finite parameter tuple for which a witness exists. These are [Skolem functions](../../../../../../../skolem-function.md); they can be chosen in the ambient universe even when $R$ is not definable inside $V_\kappa$.

For each $\xi<\kappa$, the ranks of all chosen witnesses with parameters from $V_\xi$ have [supremum](../../../../../../../supremum.md) below $\kappa$: there are fewer than $\kappa$ such parameters and only countably many formulas. Choose $F(\xi)<\kappa$ strictly above those ranks. The limit closure points

$$
C=\{\alpha<\kappa:\alpha\text{ is limit and }\forall\xi<\alpha\ F(\xi)<\alpha\}
$$

form a [club set](../../../../../../../club-set.md). At $\alpha\in C$, every existential assertion in $\mathcal V$ with parameters in $V_\alpha$ has a witness in $V_\alpha$. The [Tarski-Vaught test](../../../../../../../tarski-vaught-test.md) yields

$$
\langle V_\alpha,\in,R\cap V_\alpha\rangle\prec\mathcal V.
$$

Thus the set $E$ of all such elementary levels is unbounded. It is also closed: the union at a limit of increasing elementary levels is an [elementary substructure](../../../../../../../elementary-substructure.md) by the [elementary chain theorem](../../../../../../../elementary-chain-theorem.md), and the union of their ranks is $V_\alpha$ with predicate $R\cap V_\alpha$. Therefore

$$
\boxed{E\text{ is closed and unbounded in }\kappa.}
$$

This is [club reflection below an inaccessible cardinal](../../../../../../../club-reflection-below-an-inaccessible-cardinal.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
