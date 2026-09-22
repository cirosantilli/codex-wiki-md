<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [word](../../../../../../string.md) $abb$ has these two [leftmost derivations](../../../../../../leftmost-derivation.md):

$$
\begin{aligned}
S&\Rightarrow UST\Rightarrow aTST\Rightarrow abST
\Rightarrow abT\Rightarrow abb,\\
S&\Rightarrow UST\Rightarrow aST\Rightarrow aSTT
\Rightarrow aTT\Rightarrow abT\Rightarrow abb.
\end{aligned}
$$

In the first [grammar derivation](../../../../../../grammar-derivation.md), $U\to aT$ supplies an extra $b$; the remaining $S$ goes directly to the [empty word](../../../../../../empty-word.md). In the second [grammar derivation](../../../../../../grammar-derivation.md), $U\to a$ is used, and the remaining $S$ uses $S\to ST$ before disappearing. Every step expands the leftmost [nonterminal symbol](../../../../../../nonterminal-symbol.md), so these are genuinely different [leftmost derivations](../../../../../../leftmost-derivation.md), with different [parse trees](../../../../../../parse-tree.md) already distinguished by the [production rule](../../../../../../production-rule.md) at the $U$ node.

**Therefore $G$ is an [ambiguous grammar](../../../../../../ambiguous-grammar.md), witnessed by $abb$.**

$$
\boxed{abb\text{ has two distinct leftmost derivations in }G.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
