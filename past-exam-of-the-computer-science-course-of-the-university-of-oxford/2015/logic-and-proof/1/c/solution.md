<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the single [Boolean clause](../../../../../clause-of-a-boolean-formula.md)

$$
\boxed{F=P\lor Q\lor R.}
$$

This is a [3-CNF formula](../../../../../3-cnf-formula.md). Suppose a [2-CNF formula](../../../../../2-cnf-formula.md) $K$ were [logically equivalent](../../../../../logical-equivalence.md) to $F$. Every [Boolean clause](../../../../../clause-of-a-boolean-formula.md) $C$ of $K$ would then be a consequence of $F$.

Consider any nontautological [Boolean clause](../../../../../clause-of-a-boolean-formula.md) $C$ containing at most two [Boolean literals](../../../../../boolean-literal.md). Choose a [Boolean valuation](../../../../../boolean-valuation.md) falsifying its [Boolean literals](../../../../../boolean-literal.md). At least one of $P,Q,R$ does not occur in $C$; assign that [Boolean variable](../../../../../boolean-variable.md) true. The resulting [Boolean valuation](../../../../../boolean-valuation.md) satisfies $F$ while falsifying $C$. This contradicts $F\models C$. An empty [Boolean clause](../../../../../clause-of-a-boolean-formula.md) also cannot be a consequence of the satisfiable $F$.

Consequently every [Boolean clause](../../../../../clause-of-a-boolean-formula.md) of $K$ would have to be a tautology. Their [logical conjunction](../../../../../logical-conjunction.md) would be true under every [Boolean valuation](../../../../../boolean-valuation.md), whereas $F$ is false when $P=Q=R=0$. This proves that no such $K$ exists.

The argument even allows additional ordinary [Boolean variables](../../../../../boolean-variable.md) in $K$: at most two [Boolean literals](../../../../../boolean-literal.md) still leave one of $P,Q,R$ free to be made true. Introducing extra variables together with [existential quantification](../../../../../existential-quantification.md) would change the requested notion of [logical equivalence](../../../../../logical-equivalence.md), so it is not a way around the argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
