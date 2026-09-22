<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Propagate an entire [utility](../../../../../utility.md) pair from a child chosen to maximize the component of the player whose turn it is.** This is the two-player case of [max-n search](../../../../../max-n-search.md). At a terminal node let $V(s)=(U_A(s),U_B(s))$. At an A-node choose

$$
s^*\in\operatorname*{arg\,max}_{s'\in\operatorname{Children}(s)}V_A(s'),
\qquad V(s)=V(s^*),
$$

and at a B-node replace $V_A$ by $V_B$. Do not maximize the two coordinates independently: their separate maxima may belong to incompatible outcomes. Fix a tie rule, such as the first child in the specified order. The rule recursively gives a [pure strategy](../../../../../pure-strategy.md) [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md) in a finite [perfect-information game](../../../../../perfect-information-game.md): [backward induction](../../../../../backward-induction.md) makes the moving player's selected continuation a best response at every node.[§3.4, entire utility tuples selected by the moving player's component](../../../../../cs-188-stochastic-and-general-game-notes.md)

In the original Figure 2, each of the three children of the root belongs to B. The left B-node prefers its first leaf because $1>0$, the middle B-node prefers its first leaf because $2>-2$, and the right B-node prefers its second leaf because $3>1$. Their propagated [utility](../../../../../utility.md) pairs, from left to right, are

$$
(1,1),\qquad(-1,2),\qquad(-1,3).
$$

At the root A compares $1,-1,-1$ and chooses the left child. Thus **the root pair is $(1,1)$**, with play following the root's left branch and then that B-node's first branch. No tie affects this outcome.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
