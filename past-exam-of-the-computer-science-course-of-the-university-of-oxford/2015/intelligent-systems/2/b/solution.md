<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use two [STRIPS](../../../../../strips.md) [action schemas](../../../../../action-schema.md), for a destination topped by a coin and for an empty destination. In both, $x$ is a coin, $s,t$ are distinct stack constants, and $y$ is either a different coin or $g$. In the first, $z$ is a coin distinct from $x$ and, when $y$ is a coin, also distinct from $y$. These are restrictions on [action grounding](../../../../../action-grounding.md), so no new type or inequality [predicates](../../../../../predicate.md) are needed.

For $\operatorname{MoveToCoin}(x,y,z,s,t)$, use

$$
\begin{aligned}
\operatorname{Pre}={}&\{\operatorname{Topmost}(x,s),\operatorname{OnTop}(x,y),
\operatorname{Topmost}(z,t),\operatorname{Smaller}(x,z)\},\\
\operatorname{Del}={}&\{\operatorname{Topmost}(x,s),\operatorname{OnTop}(x,y),
\operatorname{Topmost}(z,t)\},\\
\operatorname{Add}={}&\{\operatorname{Topmost}(y,s),\operatorname{OnTop}(x,z),
\operatorname{Topmost}(x,t)\}.
\end{aligned}
$$

For $\operatorname{MoveToEmpty}(x,y,s,t)$, use

$$
\begin{aligned}
\operatorname{Pre}={}&\{\operatorname{Topmost}(x,s),\operatorname{OnTop}(x,y),
\operatorname{Topmost}(g,t)\},\\
\operatorname{Del}={}&\{\operatorname{Topmost}(x,s),\operatorname{Topmost}(g,t)\}
\cup\begin{cases}\{\operatorname{OnTop}(x,y)\},&y\ne g,\\\varnothing,&y=g,\end{cases}\\
\operatorname{Add}={}&\{\operatorname{Topmost}(y,s),\operatorname{Topmost}(x,t)\}
\cup\begin{cases}\{\operatorname{OnTop}(x,g)\},&y\ne g,\\\varnothing,&y=g.\end{cases}
\end{aligned}
$$

The last cases are a compact notation for two ordinary [action schemas](../../../../../action-schema.md), one with $y$ a coin and one with $y=g$. In the second case, $\operatorname{OnTop}(x,g)$ already holds and is left unchanged: the same ground object represents the base of every stack. Its stack identity is carried by $\operatorname{Topmost}$, so moving a singleton stack to an empty location still changes two top markers even though its support remains $g$.

Each [ground action](../../../../../ground-action.md) applies only if $\operatorname{Pre}\subseteq S$ and updates the [STRIPS](../../../../../strips.md) state by

$$
\boxed{S'=(S\setminus\operatorname{Del})\cup\operatorname{Add}.}
$$

The [preconditions](../../../../../precondition.md) require the moved coin to be exposed and the destination to be either exposed or empty. A coin destination additionally requires the moved coin to be smaller. The delete list removes its old support relation when that support changes, removes its old source-top marker, and removes the destination's old top marker. The add list exposes its former support and installs it as the destination top.

To prove that no incorrect [plans](../../../../../plan.md) arise, induct on the action history. Initially every coin has exactly one support; the stacks are disjoint decreasing chains ending at $g$; and each stack has exactly one correct top marker. An applicable action removes just the top coin from one such chain and attaches it to a different chain, or creates a singleton chain. The size [precondition](../../../../../precondition.md) preserves decreasing order; distinct stack parameters prevent moving onto one's own stack; and updating both top markers preserves their accuracy. The unchanged chain segments retain their support relations. These [planning state invariants](../../../../../planning-state-invariant.md) therefore hold after every action. Only the $k$ named stacks can be used, enforcing the stack limit.

Conversely, every legal physical move has a source top $x$, a uniquely determined former support $y$, and either an empty target or a target top $z$ larger than $x$. The corresponding [ground action](../../../../../ground-action.md) has exactly these [preconditions](../../../../../precondition.md) and effects. Thus the encoding permits all legal moves and preserves physical legality from the initial state.[Printed p. 3, Question 2(a–b), prescribed objects and predicates](../../../../../intelligent-systems-examination-paper-by-the-university-of-oxford-2015.md)

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
