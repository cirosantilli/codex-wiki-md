<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use balls $a,b$, buckets $1,2$, transition index $k$ and the grounded [action schemas](../../../../../action-schema.md) from (a). Under a sequential encoding, one example [successor-state axiom](../../../../../successor-state-axiom.md) is

$$
\boxed{\operatorname{In}(a,1)_{k+1}\leftrightarrow
\operatorname{Drop}(a,1)_k\lor
\bigl(\operatorname{In}(a,1)_k\land\neg\operatorname{Pick}(a,1)_k\bigr).}
$$

Ball $a$ is in bucket $1$ afterwards exactly when it is dropped there now, or it was there and is not picked up. Actions involving other balls or arm movement leave this fact unchanged. This is both an effect rule and a persistence rule, rather than an implication that permits spontaneous appearances.

An example [action precondition axiom](../../../../../action-precondition-axiom.md) is

$$
\boxed{\operatorname{Pick}(a,1)_k\to
\operatorname{In}(a,1)_k\land\operatorname{At}(1)_k\land\operatorname{Empty}_k.}
$$

A selected pick action must have the ball, arm and empty hand in the appropriate current state. The static type conditions have already been satisfied by [action grounding](../../../../../action-grounding.md).

An example [action exclusion axiom](../../../../../action-exclusion-axiom.md) is

$$
\boxed{\neg\bigl(\operatorname{Pick}(a,1)_k\land\operatorname{Pick}(b,1)_k\bigr).}
$$

The single arm cannot pick up both balls in one step. For a serial encoding include such an exclusion for every pair of distinct action occurrences at one layer; with at-most-one rather than exactly-one actions, a layer may idle. Initial-state clauses, goal clauses and corresponding [successor-state axioms](../../../../../successor-state-axiom.md) for all other [planning fluents](../../../../../planning-fluent.md) complete the plan-as-[SAT](../../../../../boolean-satisfiability-problem.md) construction. The plan-as-[SAT](../../../../../boolean-satisfiability-problem.md) approach was introduced by [Henry Kautz](../../../../../henry-kautz.md) and [Bart Selman](../../../../../bart-selman.md) in 1992.[ECAI 1992, pp. 359–363; author-hosted publication listing](../../../../../planning-as-satisfiability-by-henry-kautz-and-bart-selman.md)

## ↑ Ancestors (11)

1. [E](../e.md)
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
