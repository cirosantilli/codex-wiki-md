<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Von Neumann hierarchy](../../../../../../von-neumann-hierarchy.md) and the [constructible hierarchy](../../../../../../constructible-hierarchy.md) are defined by [transfinite recursion](../../../../../../transfinite-recursion.md):

$$
\boxed{V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad
V_\lambda=\bigcup_{\alpha<\lambda}V_\alpha},
$$



$$
\boxed{L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\qquad
L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha}.
$$

The union clauses apply to nonzero [limit ordinals](../../../../../../limit-ordinal.md). The [definable power set](../../../../../../definable-power-set-split.md) $\operatorname{Def}(L_\alpha)$ consists of subsets definable over $(L_\alpha,\in)$ by a [first-order formula](../../../../../../first-order-formula.md) with finitely many parameters from $L_\alpha$. Definability over that structure is essential; it is not unrestricted definability in the ambient universe. The full [constructible universe](../../../../../../constructible-universe.md) is $L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha$.

For an infinite [cardinal number](../../../../../../cardinal-number.md) $\kappa$, the [hereditarily small set](../../../../../../hereditarily-small-set.md) collection is

$$
\boxed{H_\kappa=\{x:|\operatorname{tc}(\{x\})|<\kappa\}},
$$

where $\operatorname{tc}$ is [transitive closure](../../../../../../transitive-closure.md). Using $\operatorname{tc}(x)$ instead gives the same size criterion for infinite $\kappa$. This bounds the whole membership ancestry, not just $|x|$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
