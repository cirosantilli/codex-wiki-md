<h1 id="1/j/solution">Solution</h1>

↑ **Parent:** [J](../j.md)

**Solve the finite state [graph](../../../../../graph-split.md) by winning-set [fixed-point iteration](../../../../../fixed-point-iteration.md), treating positions outside both winning regions as draws.** A naive recursive [minimax search](../../../../../minimax-search.md) over histories may run forever around a cycle. Store each ownership-sensitive state once, with a player-to-move flag and all legal successors.

Let $T_A$ and $T_B$ be terminal states where the [propositional formula](../../../../../propositional-formula.md) is true and false, respectively. Initialize $W_A^0=T_A$. Repeatedly add nonterminal positions as follows:

$$
W_A^{k+1}=W_A^k\cup\{s\text{ controlled by }A:\exists s'\in\operatorname{Succ}(s),\ s'\in W_A^k\}
\cup\{s\text{ controlled by }B:\operatorname{Succ}(s)\subseteq W_A^k\}.
$$

For $W_B$, start at $T_B$ and exchange the players in the existential and universal conditions. Terminal states keep their original labels and are excluded from these predecessor rules, avoiding a vacuous all-successors test at a terminal loss. Each process stabilizes after at most $|V|$ strict growth steps; predecessor counters implement both regions via the [winning-position attractor in an infinite game](../../../../../winning-position-attractor-in-an-infinite-game.md) construction in $O(|V|+|E|)$ [graph](../../../../../graph-split.md) time.

The admission round supplies a decreasing rank. At a state controlled by the winning player, choose a successor of smaller rank; at an opposing state, every successor already has smaller rank. Hence these strategies force a finite terminal win. The two winning regions are disjoint. Outside both, each player can keep the play outside the opponent's winning region, so neither can force a terminal win against best defence. Under the convention in (h), assign those remaining positions value $0$; the other regions have values $+1$ and $-1$.

This is a finite [reachability game](../../../../../reachability-game.md) calculation, with [memoryless strategies](../../../../../memoryless-strategy.md) read from successor choices. Merely calling the first back-[edge](../../../../../edge-of-a-graph.md) encountered a draw is unsound: a cycle can have an exit through which one player can force a win.

## ↑ Ancestors (11)

1. [J](../j.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
