<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [propositional type](../../../../../../propositional-type.md) is a set $\Sigma$ of [propositional formulas](../../../../../../propositional-formula.md); a [Boolean valuation](../../../../../../boolean-valuation.md) realizes it if every member is true, and omits it if at least one member is false. A consistent [propositional theory](../../../../../../propositional-theory.md) $T$ locally omits $\Sigma$ if every formula $\theta$ which implies all members of $\Sigma$ modulo $T$ is refutable modulo $T$. Equivalently, whenever $T\cup\{\theta\}$ is consistent, there is a $\sigma\in\Sigma$ for which $T\cup\{\theta,\neg\sigma\}$ is consistent. For a consistent [propositional type](../../../../../../propositional-type.md), this says that it is a [nonprincipal propositional type](../../../../../../nonprincipal-propositional-type.md).

The **[extended omitting types theorem for propositional logic](../../../../../../extended-omitting-types-theorem-for-propositional-logic.md)** says that if a consistent $T$ locally omits each of a countable family $\Sigma_0,\Sigma_1,\ldots$, there is one [Boolean valuation](../../../../../../boolean-valuation.md) satisfying $T$ and omitting them all. It also works inside any prescribed finite condition consistent with $T$.

To prove it, start with such a condition $\theta_0$, taking $\top$ when none is prescribed. At stage $i$, choose $\sigma_i\in\Sigma_i$ such that

$$
T\cup\{\theta_i,\neg\sigma_i\}\text{ is consistent},\qquad
\theta_{i+1}=\theta_i\land\neg\sigma_i.
$$

Such a choice exists by local omission. More explicitly, failure would imply $T\vdash\theta_i\to\sigma$ for every $\sigma\in\Sigma_i$, hence $T\vdash\neg\theta_i$, contradicting the stage invariant. Every finite subset of $T\cup\{\theta_0\}\cup\{\neg\sigma_i:i\in\mathbb N\}$ lies inside a consistent stage. By the [propositional compactness theorem](../../../../../../propositional-compactness-theorem.md) and the [completeness theorem for propositional logic](../../../../../../completeness-theorem-for-propositional-logic.md), it has a [Boolean valuation](../../../../../../boolean-valuation.md). That [Boolean valuation](../../../../../../boolean-valuation.md) satisfies $T$ and makes the selected member $\sigma_i$ of every type false. **All types are therefore omitted simultaneously.** No effective test for consistency is assumed, and the argument does not require the ambient propositional language to be countable. Only the family of omission requirements is countable.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
