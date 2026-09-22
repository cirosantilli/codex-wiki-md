<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Totality of the [binary relation](../../../../../binary-relation.md) is expressed by

$$
\boxed{\tau=\forall x\forall y\,(R(x,y)\lor R(y,x)).}
$$

When $R$ is already an order, this adds comparability and makes it a [total order](../../../../../total-order.md). In fact this [first-order sentence](../../../../../first-order-sentence.md) alone entails $\rho=\forall xR(x,x)$.

By the definition of [semantic entailment](../../../../../semantic-entailment.md), $\tau\models\rho$ means that every [first-order structure](../../../../../first-order-structure.md) satisfying $\tau$ also satisfies $\rho$. Let $\mathcal M$ be any such [first-order structure](../../../../../first-order-structure.md), and let $a$ be any element of its [domain of a first-order structure](../../../../../domain-of-a-first-order-structure.md). The instance of $\tau$ with $x=y=a$ gives $R(a,a)\lor R(a,a)$, which is true only if $R(a,a)$ is true. Since $a$ was arbitrary, $\mathcal M\models\forall xR(x,x)$. Therefore

$$
\boxed{\tau\models\rho.}
$$

There is no exception for $x=y$ in the displayed totality axiom; that case is exactly what forces the [reflexive relation](../../../../../reflexive-relation.md) property.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
