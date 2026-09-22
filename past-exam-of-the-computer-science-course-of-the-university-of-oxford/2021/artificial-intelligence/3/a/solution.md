<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Use location, holding and hand-capacity [planning fluents](../../../../../planning-fluent.md), together with static object types.** Write $\operatorname{In}(b,k)$, $\operatorname{Holding}(b)$, $\operatorname{At}(k)$ and $\operatorname{Empty}$ for a ball's bucket, the held ball, the arm's location and an empty hand. Static predicates $\operatorname{Ball}(b)$, $\operatorname{Bucket}(k)$ and $\operatorname{Different}(k,\ell)$ identify types and distinct buckets. The latter can equivalently be a [action grounding](../../../../../action-grounding.md) restriction.

For typed parameters, the [STRIPS](../../../../../strips.md) actions are

$$
\begin{array}{c|l|l|l}
\text{Action}&\text{Preconditions}&\text{Add}&\text{Delete}\\\hline
\operatorname{Pick}(b,k)&\operatorname{In}(b,k),\operatorname{At}(k),\operatorname{Empty}&\operatorname{Holding}(b)&\operatorname{In}(b,k),\operatorname{Empty}\\
\operatorname{Drop}(b,k)&\operatorname{Holding}(b),\operatorname{At}(k)&\operatorname{In}(b,k),\operatorname{Empty}&\operatorname{Holding}(b)\\
\operatorname{Move}(k,\ell)&\operatorname{At}(k),\operatorname{Different}(k,\ell)&\operatorname{At}(\ell)&\operatorname{At}(k)
\end{array}
$$

Untyped notation adds the appropriate $\operatorname{Ball}$ and $\operatorname{Bucket}$ facts to every [precondition](../../../../../precondition.md) set. Static type and inequality facts have no add or delete effects. A state is a set of true ground facts under the [closed-world assumption](../../../../../closed-world-assumption.md), and an applicable action produces $(S\setminus\operatorname{Del})\cup\operatorname{Add}$.

Start from a physically valid state: each ball is in exactly one bucket or held; at most one ball is held; the arm is at exactly one bucket; and $\operatorname{Empty}$ is true exactly when no ball is held. The operators preserve these [planning state invariants](../../../../../planning-state-invariant.md). In particular, picking requires an empty hand, dropping releases the held ball, and moving deletes the old arm location. Moving while holding a ball is permitted, so a separate carried-ball movement action is unnecessary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
