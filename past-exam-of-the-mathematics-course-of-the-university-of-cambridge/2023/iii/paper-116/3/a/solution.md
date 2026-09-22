<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since the [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) $\lambda$ is inaccessible, $(V_\lambda,\in)$ is a [model](../../../../../../model-of-a-first-order-theory.md) of ZFC. The [Downward Lowenheim-Skolem theorem](../../../../../../downward-lowenheim-skolem-theorem.md) gives an [elementary substructure](../../../../../../elementary-substructure.md)

$$
X\prec V_\lambda
$$

of [cardinality](../../../../../../cardinal-number.md) $\kappa$ such that

$$
V_\kappa\cup\{\kappa,U\}\subseteq X.
$$

One may obtain $X$ concretely as the [Skolem hull](../../../../../../skolem-hull.md) of this set; its cardinality remains $\kappa$ because the language of set theory is countable and $|V_\kappa|=\kappa$.

Apply the [Mostowski collapse theorem](../../../../../../mostowski-collapse-theorem.md) to $X$ and write $\pi:X\to M$ for the collapse. Then $M$ is a [transitive set](../../../../../../transitive-set.md), $|M|=\kappa$, and $\pi$ fixes $V_\kappa$ pointwise. It also fixes $\kappa$, because it fixes every ordinal below $\kappa$. By [elementarity](../../../../../../elementary-substructure.md), $X$ satisfies ZFC and regards $U$ as a [kappa-complete filter](../../../../../../kappa-complete-filter.md) that is a [nonprincipal ultrafilter](../../../../../../nonprincipal-ultrafilter.md) on $\kappa$. Therefore, with $\bar U=\pi(U)$,

$$
(M,\in)\models\mathrm{ZFC}+\text{“$\kappa$ is a measurable cardinal, witnessed by $\bar U$.”}
$$

The internal ultrafilter $\bar U$ need not equal the original $U$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
