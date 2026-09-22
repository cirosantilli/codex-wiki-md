<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Include all four positions and a turn marker:

$$
s=(p,q,z_1,z_2,\tau),\qquad\tau\in\{\mathrm{R},\mathrm{M}\}.
$$

The initial marker is $\mathrm{R}$. There are at most $2n^8$ such states before terminal compression. The two robots form one maximizing team in the [adversarial search](../../../../../adversarial-search.md) representation. At an R state their actions are joint legal moves, including waiting, with deterministic successor positions and marker M. At an M state the monster outcome is a pair of legal cardinal moves, producing marker R.

Check termination initially and after each simultaneous pair of moves. A state is a failure if $\{p,q\}\cap\{z_1,z_2\}\ne\varnothing$. Otherwise it is a success if $p=q$. **Collision takes priority over meeting**, so meeting on an occupied room fails. A safe meeting ends immediately, before a further monster response. Room swaps without a shared position at a checked boundary are neither capture nor meeting.

The monsters move randomly, so their nodes are **chance nodes**, not minimizing decisions. Under independent uniform legal moves, if monster $j$ currently has $d_j$ available destinations, each joint outcome has [probability](../../../../../probability.md) $1/(d_1d_2)$. If several commands produce the same state, add their [probabilities](../../../../../probability.md). This specifies a stochastic [game tree](../../../../../game-tree.md), equivalently a [Markov decision process](../../../../../markov-decision-process.md) for the robot team. Uniform legal moves and independent monsters are explicit boundary/joint-law conventions; uniform attempted directions with blocked moves staying put is another convention, with different boundary [transition probabilities](../../../../../transition-probability.md) but the same search method. For the one-cell grid, a monster with no legal move stays; all four initial positions then coincide and the instance immediately fails.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
