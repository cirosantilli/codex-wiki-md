<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Identify $A$ with its image under $\alpha$. In a language naming every element of $B$, use the same names for elements of $A$ in the two sets of sentences

$$
\operatorname{Diag}(B)\cup\operatorname{ElDiag}(A).
$$

This union is consistent. To see finite satisfiability, conjoin the finitely many diagram facts about $B$ into a [quantifier-free formula](../../../../../../quantifier-free-formula.md) $\delta(\mathbf a,\mathbf b)$ and the finitely many elementary-diagram facts about $A$ into $\psi(\mathbf a)$, where the elements in $\mathbf b$ have names outside $A$. Since $B\models\exists\mathbf y\,\delta(\mathbf a,\mathbf y)$, the [1-embedding](../../../../../../existential-embedding.md) property gives a witnessing tuple in $A$. Interpret the finitely many new names by that tuple. The resulting expansion of $A$ satisfies $\delta$ as well as $\psi$.

By [compactness theorem](../../../../../../compactness-theorem.md), a model $C$ of this union exists. Its named copy of $B$ gives an embedding $\beta:B\to C$, while its named copy of $A$ is elementary. Consequently

$$
\boxed{\beta\alpha:A\longrightarrow C\text{ is elementary}.}
$$

The naming ensures that the two maps agree on the original copy of $A$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
