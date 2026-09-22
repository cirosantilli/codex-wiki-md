<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [first-order theory](../../../../../first-order-theory.md) in a fixed [first-order signature](../../../../../first-order-signature.md) is a set of [first-order sentences](../../../../../first-order-sentence.md). Under the closed-theory convention used in the question, it contains all its [semantic entailments](../../../../../semantic-entailment.md): $T\models\theta$ implies $\theta\in T$. One can equivalently begin with a set of axioms and take its closure under consequence.

A [complete theory](../../../../../complete-theory.md) is a consistent [first-order theory](../../../../../first-order-theory.md) that decides every [first-order sentence](../../../../../first-order-sentence.md) $\theta$ in its [first-order signature](../../../../../first-order-signature.md):

$$
\boxed{T\models\theta\quad\text{or}\quad T\models\neg\theta.}
$$

Consistency ensures that exactly one of these alternatives holds.

A [decidable theory](../../../../../decidable-theory.md) is one for which an [algorithm](../../../../../algorithm-split.md) always terminates and determines whether a given [first-order sentence](../../../../../first-order-sentence.md) is a consequence:

$$
\boxed{\{\theta:T\models\theta\}\text{ is decidable}.}
$$

If the [first-order theory](../../../../../first-order-theory.md) is already closed under consequence, this is its membership problem. It is a condition on the consequences, not merely on whether the chosen set of axioms has a decidable membership test.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
