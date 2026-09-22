<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [game tree](../../../../../game-tree.md) alternates **MAX nodes for joint robot choices and CHANCE nodes for joint monster outcomes**. An interior MAX node has at most $25$ children; an interior CHANCE node at most $4^2=16$. A terminal safe meeting has [utility](../../../../../utility.md) one and capture has [utility](../../../../../utility.md) zero. With no specified preference for speed, the objective is to maximize the [probability](../../../../../probability.md) of eventual safe meeting.

Use **[expectimax](../../../../../expectimax.md)**: maximize at MAX nodes and take the [expected value](../../../../../expected-value-split.md) at CHANCE nodes. For nonterminal states, its finite-horizon backup is

$$
V_{t+1}(s)=
\begin{cases}
\displaystyle\max_a V_t(T(s,a)),&\tau=\mathrm R,\\[3pt]
\displaystyle\sum_{s'}P(s'\mid s)V_t(s'),&\tau=\mathrm M.
\end{cases}
$$

Here the horizon counts half-turns, terminal values stay fixed at zero or one, and $V_0$ is zero at nonterminal states. This computes the best chance of success within the horizon. Maximizing the worst monster outcome would solve a different problem from the stipulated random movement.

Because waiting and movement cycles can repeat states, the infinite [game tree](../../../../../game-tree.md) need not terminate. For the unbounded objective, use [value iteration](../../../../../value-iteration.md) on the finite state [graph](../../../../../graph-split.md), starting from terminal-success indicators as above: $V_t$ increases to the optimal eventual-success [probability](../../../../../probability.md). A reachability-policy method or sufficiently long finite-horizon policies can extract the actions; arbitrary tie choices in the limiting equations must not select a policy that waits forever instead of realizing the value. Alternatively impose an explicit finite horizon and use depth-limited [expectimax](../../../../../expectimax.md), stating that changed objective. No method guarantees success with [probability](../../../../../probability.md) one from every initial configuration.

## ↑ Ancestors (11)

1. [I](../i.md)
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
