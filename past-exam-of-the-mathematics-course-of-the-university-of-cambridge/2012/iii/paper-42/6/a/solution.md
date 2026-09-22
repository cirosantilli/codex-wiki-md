<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gibbard-Satterthwaite theorem](../../../../../../gibbard-satterthwaite-theorem.md) concerns a deterministic [social choice function](../../../../../../social-choice-function.md) on all profiles of strict preferences over a finite set of at least three alternatives. If it is onto and [strategyproof](../../../../../../strategyproofness.md), it is a [dictatorship in social choice](../../../../../../dictatorship-in-social-choice.md): one fixed voter always obtains its top alternative. Equivalently, every onto nondictatorial rule on this unrestricted domain is manipulable. Dictatorships themselves are [strategyproof](../../../../../../strategyproofness.md). We prove the implication for two voters.

First derive the [rank-raising monotonicity lemma](../../../../../../rank-raising-monotonicity-lemma.md). If changing one report changes the selected alternative from $a$ to $b$, [strategyproofness](../../../../../../strategyproofness.md) in the old profile requires $a\succ b$ in the old order, while [strategyproofness](../../../../../../strategyproofness.md) in the new profile requires $b\succ a$ in the new order. Therefore a change that never lowers the selected $a$ relative to any formerly lower alternative cannot change the outcome.

Onto-ness now implies unanimity. For every $a$, some profile selects it. Raise $a$ to first place in each voter's order; the preceding lemma keeps the outcome at $a$. Moreover the outcome cannot be $b$ when both voters rank some $a$ above $b$: starting from such an outcome, raise $b$ to second place directly below $a$ in each order. These changes never lower $b$ relative to anything, so would preserve $b$ at a profile unanimously topping $a$, a contradiction. Thus the rule respects unanimous pairwise preference.

For each pair $a,b$, promote that pair to the first two places in each report, preserving the voter's order between them. Both dominate every outsider unanimously, so the outcome is $a$ or $b$. The result depends only on the two voters' comparisons of $a,b$, not on the lower alternatives: changing a tail cannot reverse the choice between two alternatives whose relative order did not change, since one direction of that change would be a profitable report. These binary choices define a complete strict social relation satisfying pairwise unanimity and independence from other comparisons.

This relation is transitive. To see why, suppose its choices on some triple form a directed cycle. Put those three alternatives first in both reports, preserving their individual relative orders. Unanimity excludes all outsiders, so the rule chooses one of the three, say $a$. Promoting $a$ with either other member to the first two positions does not lower $a$ and therefore preserves its selection. Thus $a$ must win both its binary comparisons, contradicting the cycle. A complete strict relation with no directed three-cycle is transitive. Also the original social choice is its top: for any original selected $a$, promoting $a$ and any $b$ preserves $a$, so it wins every binary comparison.

It remains to prove two-voter dictatorship for this binary relation. Choose any conflict between $a,b$. Suppose voter 1 prefers $a$ to $b$, voter 2 prefers $b$ to $a$, and the social relation follows voter 1. Say voter 1 wins this ordered comparison. For any third alternative $c$, consider the two profile patterns

$$
\begin{array}{c|cc}
&\text{voter 1}&\text{voter 2}\\\hline
\text{pattern I}&a\succ b\succ c&b\succ c\succ a\\
\text{pattern II}&c\succ a\succ b&b\succ c\succ a
\end{array}
$$

with other alternatives below the triple. In pattern I, the social relation has $a\succ b$ by independence and $b\succ c$ by unanimity, hence $a\succ c$. This proves that voter 1 wins the conflict $a$ against $c$. In pattern II, it has $c\succ a$ by unanimity and $a\succ b$ by independence, hence $c\succ b$, proving that voter 1 also wins $c$ against $b$.

Thus winning $a$ against $b$ implies winning $a$ against every third $c$ and every such $c$ against $b$. Applying the implication to $a$ against $c$ gives $b$ against $c$, and then to $b$ against $c$ gives $b$ against $a$. The implication therefore supplies both directions of all pairs involving the original alternatives and any new one. For an arbitrary ordered pair $x,y$ distinct from a fixed base alternative $a$, use the already obtained win of $x$ against $a$ and the third alternative $y$ to get the win of $x$ against $y$. Hence voter 1 wins every conflict. Unanimous comparisons also follow its preference, so the social relation is always voter 1's full order, and the social choice is its top.

If the initially chosen conflict follows voter 2, swap the voter roles in the same argument. We have therefore proved **every onto two-voter [strategyproof](../../../../../../strategyproofness.md) rule with at least three alternatives is dictatorial**. This [two-voter dictatorship from binary choice](../../../../../../two-voter-dictatorship-from-binary-choice.md) proof establishes the required special case without assuming the general theorem's conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
