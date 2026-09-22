<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $\forall_2$ denotes [universal-existential sentences](../../../../../../universal-existential-sentence.md), with quantifier-free matrix and possibly empty blocks. Add constants for $A$ and consider

$$
\Sigma=T\cup\operatorname{Diag}(A)\cup
\{\neg\exists\mathbf y\,\theta(\mathbf c_a,\mathbf y):
\theta\text{ quantifier-free and }A\models\neg\exists\mathbf y\,\theta(\mathbf a,\mathbf y)\}.
$$

We show that $\Sigma$ is consistent. Suppose a finite subset is inconsistent. Combine its diagram facts as $\delta(\mathbf c)$ and its finitely many negative existential facts as $\neg\exists\mathbf y_j\,\theta_j(\mathbf c,\mathbf y_j)$. Replacing the new constants by a variable tuple gives the consequence

$$
T\models\forall\mathbf x\left(\delta(\mathbf x)\longrightarrow
\bigvee_{j=1}^m\exists\mathbf y_j\,\theta_j(\mathbf x,\mathbf y_j)\right).
$$

This is equivalent to a universal-[existential sentence](../../../../../../existential-sentence.md): move all the existential blocks to the front of the disjunction, using the usual nonempty-domain convention. If there are no negative existential facts, the consequence is simply $\forall\mathbf x\,\neg\delta$. By hypothesis $A$ satisfies the displayed consequence. Its named tuple satisfies $\delta$ but none of the existential alternatives, a contradiction.

A model $B$ of $\Sigma$ contains a diagram copy of $A$. Every [existential formula](../../../../../../existential-formula.md) false in $A$ is still false in $B$; every one true in $A$ is preserved by the embedding. Thus

$$
\boxed{A\preccurlyeq_1 B\models T.}
$$

Both preservation and reflection are required here; the atomic diagram alone would give only an ordinary embedding.

## ↑ Ancestors (11)

1. [C](../c.md)
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
