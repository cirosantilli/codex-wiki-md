<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A corrected [STRIPS](../../../../../strips.md) model can fix object roles in the action names, leaving only room parameters to instantiate. Use the same $a,w,g,r$ and introduce static $\operatorname{pitfree}(z)$ and $\operatorname{exit}(z)$ facts, plus a [planning fluent](../../../../../planning-fluent.md) $\operatorname{clear}(z)$ meaning “no live monster occupies $z$”. Unlike the supplied adjacency relation, let $\operatorname{adj}$ describe all geometrically adjacent rooms; safety is then explicit rather than hidden by missing [edges](../../../../../edge-of-a-graph.md).

Initially the agent, monster and gold have their specified locations, $\operatorname{have}(a,r)$, $\operatorname{alive}(w)$ and $\operatorname{active}$ hold, $\operatorname{exit}(s_{11})$ holds, $\operatorname{pitfree}$ holds at every room except $s_{12}$, and $\operatorname{clear}$ holds at every room except $s_{23}$. All unlisted facts are false by the [closed-world assumption](../../../../../closed-world-assumption.md). The following positive [preconditions](../../../../../precondition.md), add lists and delete lists are a complete action specification:

$$
\begin{array}{c|l|l|l}
\text{action}&\text{preconditions}&\text{add}&\text{delete}\\\hline
\operatorname{Walk}(y,z)&\begin{gathered}\operatorname{active},\operatorname{at}(a,y),\operatorname{adj}(y,z),\\\operatorname{pitfree}(z),\operatorname{clear}(z)\end{gathered}&\operatorname{at}(a,z)&\operatorname{at}(a,y)\\[3pt]
\operatorname{Fire}(y,z)&\begin{gathered}\operatorname{active},\operatorname{at}(a,y),\operatorname{adj}(y,z),\\\operatorname{at}(w,z),\operatorname{alive}(w),\operatorname{have}(a,r)\end{gathered}&\begin{gathered}\operatorname{dead}(w),\\\operatorname{clear}(z)\end{gathered}&\begin{gathered}\operatorname{alive}(w),\\\operatorname{have}(a,r)\end{gathered}\\[3pt]
\operatorname{Collect}(z)&\begin{gathered}\operatorname{active},\operatorname{at}(a,z),\\\operatorname{at}(g,z)\end{gathered}&\operatorname{have}(a,g)&\operatorname{at}(g,z)\\[3pt]
\operatorname{Leave}(z)&\begin{gathered}\operatorname{active},\operatorname{at}(a,z),\\\operatorname{exit}(z),\operatorname{have}(a,g)\end{gathered}&\operatorname{exited}&\operatorname{active}
\end{array}
$$

Require $\operatorname{exited}$ as the goal. If reaching the exit suffices, omit $\operatorname{Leave}$ and use the original two goal facts. Instantiating these schemata over the finite room [set](../../../../../set-split.md) gives ordinary ground [STRIPS](../../../../../strips.md) actions.

Only $a$ moves, only $g$ is collectible and only $r$ can be fired at $w$. No action changes the monster’s location; its corpse can stay there, while $\operatorname{clear}$ records that it is harmless. The gold stays at its original room until collection. The arrow is consumed by its only use. By [mathematical induction](../../../../../mathematical-induction.md) on plan length, every applicable action preserves the [planning state invariant](../../../../../planning-state-invariant.md) that the active agent occupies one pit-free room without a live monster. Consequently every solution is a safe execution. The plan in part a, followed by $\operatorname{Leave}(s_{11})$, is one such execution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
