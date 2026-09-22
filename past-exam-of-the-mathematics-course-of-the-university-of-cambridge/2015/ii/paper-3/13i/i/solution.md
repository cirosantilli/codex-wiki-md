<h1 id="13i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Zorn lemma](../../../../../../zorn-s-lemma.md) states that a nonempty [partially ordered set](../../../../../../partially-ordered-set.md) in which every [chain in a partial order](../../../../../../chain-in-a-partial-order.md) has an upper bound has a maximal element. Here is a proof from the [axiom of choice](../../../../../../axiom-of-choice.md) and [Hartogs theorem](../../../../../../hartogs-theorem.md).

Suppose there is no maximal element. Every chain $C$ has a strict upper bound: choose an upper bound $b$ and then an element strictly greater than $b$. The family of sets of strict upper bounds is a set of nonempty subsets of the underlying set $P$. **The axiom of choice is used here** to choose, simultaneously for every chain $C$, one strict upper bound $b(C)$.

By [Hartogs theorem](../../../../../../hartogs-theorem.md) there is an [ordinal](../../../../../../ordinal.md) $\kappa$ admitting no injection into $P$. [Transfinite recursion](../../../../../../transfinite-recursion.md) defines $x_\alpha$ for $\alpha<\kappa$ by

$$
x_\alpha=b(\{x_\beta:\beta<\alpha\}).
$$

At each stage the previous elements form a chain, and $x_\alpha$ is strictly above every one of them. Hence $\alpha\mapsto x_\alpha$ is an injection $\kappa\to P$, a contradiction. Therefore **a maximal element exists**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [13I](../../13i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
