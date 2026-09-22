<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**As literally stated, the claim is false.** Give player one two pure actions, with [payoffs](../../../../../payoff.md) one and zero against every opposing action. A [mixed strategy](../../../../../mixed-strategy.md) assigning probability one to the first action has exactly that action's [payoffs](../../../../../payoff.md), so very weakly dominates it under the printed non-strict inequality. The other pure action nevertheless fails to dominate it.

The intended statement becomes true if the mixture gives positive [probability](../../../../../probability.md) to some distinct action, equivalently $p_i<1$. Fix any opposing pure [strategy profile](../../../../../strategy-profile.md) at which $s_i$ pays one. Since all [payoffs](../../../../../payoff.md) are in $\{0,1\}$,

$$
1\leq\sum_jp_ju_1(s_j,s_{-1})\leq\sum_jp_j=1.
$$

Equality forces every positive-probability supported action to pay one there. At a profile where $s_i$ pays zero, every other action already pays at least zero. Therefore every action in the [support of a mixed strategy](../../../../../support-of-a-mixed-strategy.md) is no worse than $s_i$ against every opposing profile. Choosing a distinct supported action proves the corrected conclusion: **nontrivial mixed [very weak dominance](../../../../../very-weakly-dominated-strategy.md) implies very weak domination by a distinct pure action**. This proof does not insert the missing support condition silently.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
