<h1 id="9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The assertion is **true**. Write $A=L(\alpha)$ and $B=L(\beta)$. The semantics of [regular expressions](../../../../../regular-expression.md) reduce the claim to

$$
(A^*B^*)^*=(A\cup B)^*,
$$

where juxtaposition is [concatenation of formal languages](../../../../../concatenation-of-formal-languages.md) and a star is the [Kleene star](../../../../../kleene-star.md).

Every element of $A^*B^*$ is a finite concatenation of members of $A\cup B$, so belongs to $(A\cup B)^*$. Concatenating any finite number of such elements still belongs to $(A\cup B)^*$, proving $(A^*B^*)^*\subseteq(A\cup B)^*$.

Conversely, $A\subseteq A^*B^*$ because one may take a single member of $A$ followed by the empty [string](../../../../../string.md) from $B^*$. Likewise $B\subseteq A^*B^*$ by taking the empty [string](../../../../../string.md) from $A^*$. Hence any finite concatenation of members of $A\cup B$ lies in $(A^*B^*)^*$. The empty [string](../../../../../string.md) belongs to both sides. Thus

$$
\boxed{L((\alpha^*\beta^*)^*)=L((\alpha+\beta)^*).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [9](../../9.md)
3. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
