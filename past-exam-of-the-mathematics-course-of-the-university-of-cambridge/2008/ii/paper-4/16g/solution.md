<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

For [Hartogs theorem](../../../../../hartogs-theorem.md), collect all well-order relations on all subsets of a set $x$. They form a set, since the relations belong to the power set of $x\times x$. Replacement collects their [ordinal](../../../../../ordinal.md) order types in a set $T$. Define

$$
\alpha=\sup\{\beta+1:\beta\in T\}.
$$

If there were an injection $\alpha\to x$, transfer the well-order of $\alpha$ to its image. Its type would put $\alpha$ in $T$, giving $\alpha+1\leq\alpha$, impossible. Thus **some [ordinal](../../../../../ordinal.md) does not inject into $x$**, without using choice.

Assume the [axiom of choice](../../../../../axiom-of-choice.md) and let a nonempty [partially ordered set](../../../../../partially-ordered-set.md) $P$ have an upper bound for every chain. Suppose it has no maximal element. Choose, from every subset of $P$ with a nonempty set of strict upper bounds, one such strict upper bound. Every chain has a strict upper bound: first take an upper bound and then a strictly larger element, using the absence of maximal elements. Take a Hartogs [ordinal](../../../../../ordinal.md) $\alpha$ for $P$. [Transfinite recursion](../../../../../transfinite-recursion.md) chooses $p_\beta$, for each $\beta<\alpha$, strictly above all previously chosen elements. Their predecessors form a chain at every stage, so this recursion is defined and strictly increasing. It gives an injection $\alpha\to P$, contradicting the choice of $\alpha$. Hence $P$ has a maximal element, proving [Zorn's lemma](../../../../../zorn-s-lemma.md).

For the [well-ordering theorem](../../../../../well-ordering-theorem.md), take a choice function on the nonempty subsets of $x$ and recursively choose an element of $x$ not previously selected. If this process had not exhausted $x$ at any stage below its Hartogs [ordinal](../../../../../ordinal.md) $\alpha$, it would define an injection $\alpha\to x$, again impossible. Therefore it exhausts $x$ at some [ordinal](../../../../../ordinal.md) stage $\beta<\alpha$. Order each element by its unique selection index; this transfers the [ordinal](../../../../../ordinal.md) well-order to all of $x$. The empty set is already well-ordered. These proofs use [transfinite recursion](../../../../../transfinite-recursion.md), not an unstated fixed-point theorem.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
