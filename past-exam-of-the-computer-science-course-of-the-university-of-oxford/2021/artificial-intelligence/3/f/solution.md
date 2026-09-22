<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**Use backward deletion of achieved goal requirements; this decides [precondition](../../../../../precondition.md)-free ground [STRIPS](../../../../../strips.md) [planning](../../../../../planning.md) in [polynomial time](../../../../../polynomial-time.md).** Let $I$ be the initial set of true facts, $G$ the positive conjunctive goal set and $\mathcal A$ the [ground actions](../../../../../ground-action.md). Assume the usual disjoint add and delete lists; if both lists contain a fact, first normalize the net effect according to the action semantics.

Maintain residual goal set $R=G$ and an initially empty list $L$. While $R\nsubseteq I$, look for an action $a$ satisfying

$$
\boxed{\operatorname{Del}(a)\cap R=\varnothing,
\qquad \operatorname{Add}(a)\cap R\ne\varnothing.}
$$

If no such action exists, reject. Otherwise record $a$ in $L$ and replace $R$ by $R\setminus\operatorname{Add}(a)$. When $R\subseteq I$, return the actions in reverse order of recording. All actions are applicable because their [precondition](../../../../../precondition.md) sets are empty.

For soundness, the selected action can be put last in a [plan](../../../../../plan.md) for the current residual goals: it supplies the removed goals and deletes none of the goals still being required. Reversing all recorded selections makes the final state satisfy the original $G$.

For completeness, suppose $R$ is not already satisfied initially but a [plan](../../../../../plan.md) achieves it. Consider the last action in that [plan](../../../../../plan.md) that changes any fact of $R$. Its effective changes cannot delete any member of $R$, because no later action repairs it; it must add at least one member. Thus a candidate exists. Moreover any candidate chosen by the algorithm is safe: removing some requirements gives a subset of $R$, so a [plan](../../../../../plan.md) for $R$, if one exists, also establishes the smaller goal set. Appending the chosen last action then restores the removed requirements without harming the rest. [Mathematical induction](../../../../../mathematical-induction.md) therefore preserves solvability during all choices.

Each successful iteration removes at least one residual goal, so there are at most $|G|$ iterations and the returned [plan](../../../../../plan.md) has at most $|G|$ actions. Scanning all actions and their effect lists per iteration is polynomial in the input size, for example $O(|G|\,|\mathcal A|\,|P|)$ with simple fact-set representations over $P$. Merely taking the union of all add effects would be unsound, since actions can delete each other's achievements. This algorithm is the [last-achiever algorithm for precondition-free planning](../../../../../last-achiever-algorithm-for-precondition-free-planning.md).

## ↑ Ancestors (11)

1. [F](../f.md)
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
