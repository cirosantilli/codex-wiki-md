<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The algorithm is $\boxed{\text{incorrect: it can return true for a non-entailed ground atom}}$. Its recursive calls return only Booleans. They do not return and propagate the [first-order substitutions](../../../../../first-order-substitution.md) obtained while satisfying earlier rule premises.

Take distinct constants $a,b,c$, facts

$$
\mathcal F=\{P(a),Q(b)\},
$$

and the single [Datalog](../../../../../datalog.md) rule

$$
P(x)\land Q(x)\to H(c).
$$

Ask for $H(c)$. The head matches the goal without binding $x$. In line 15, the recursive call for $P(x)$ succeeds by [first-order unification](../../../../../first-order-unification.md) with $P(a)$, but returns only `true`. The next recursive call still receives $Q(x)$ with $x$ unbound, and succeeds by [first-order unification](../../../../../first-order-unification.md) with $Q(b)$. Neither subgoal is the visited head $H(c)$, so the visited test does not stop these calls. Both recursive results are `true`, and the algorithm returns `true` for $H(c)$.

However, the [least Herbrand model](../../../../../least-herbrand-model.md) is just $\{P(a),Q(b)\}$. No single constant makes both $P(x)$ and $Q(x)$ true, so the rule cannot derive $H(c)$. The two individually successful premises need one consistent [first-order substitution](../../../../../first-order-substitution.md). A correct [backward chaining](../../../../../backward-chaining.md) procedure must thread answer [first-order substitutions](../../../../../first-order-substitution.md) through the remaining premises and backtrack when they cannot be extended; [forward chaining](../../../../../forward-chaining.md) on ground [Datalog](../../../../../datalog.md) instances is another way to avoid this error.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
