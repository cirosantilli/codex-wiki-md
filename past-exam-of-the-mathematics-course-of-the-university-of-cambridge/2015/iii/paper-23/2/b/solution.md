<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T_\forall$ denote the [universal consequences of a theory](../../../../../../universal-consequences-of-a-theory.md): all universal [first-order sentences](../../../../../../first-order-sentence.md) entailed by $T$. A [first-order structure](../../../../../../first-order-structure.md) satisfies $T_\forall$ exactly when it embeds into a model of $T$, by the [compactness theorem](../../../../../../compactness-theorem.md) applied to its [diagram of a structure](../../../../../../diagram-mathematical-logic.md).

The theory has [algebraically prime models](../../../../../../algebraically-prime-extension.md) if, for every $\mathcal A\models T_\forall$, there are $\mathcal P\models T$ and a [structure embedding](../../../../../../structure-embedding.md) $i:\mathcal A\to\mathcal P$ such that every [structure embedding](../../../../../../structure-embedding.md) $j:\mathcal A\to\mathcal N$, $\mathcal N\models T$, factors as $j=h\circ i$ for some [structure embedding](../../../../../../structure-embedding.md) $h:\mathcal P\to\mathcal N$. Neither $i$ nor $h$ is required to be elementary.

For $\mathcal M\subseteq\mathcal N$, [simple closure](../../../../../../simple-closure.md) means that every existential [quantifier-free formula](../../../../../../quantifier-free-formula.md) over $M$ which has a witness in $N$ has one in $M$:

$$
\mathcal N\models\exists x\,\theta(x,\bar a)\quad\Longrightarrow\quad
\mathcal M\models\exists x\,\theta(x,\bar a),\qquad \bar a\in M.
$$

Now take two models $\mathcal M,\mathcal N\models T$ with common [substructure](../../../../../../substructure-of-a-first-order-structure.md) $\mathcal A$. Since $A$ embeds into $M$, it satisfies $T_\forall$. Choose its [algebraically prime extension](../../../../../../algebraically-prime-extension.md) $\mathcal P$, and embed $P$ into both $M$ and $N$ over $A$.

If $\exists x\,\theta(x,\bar a)$ holds in $M$, the image of $P$ in $M$ is a model of $T$. The assumed [simple closure](../../../../../../simple-closure.md) of this image transfers a witness from $M$ into $P$. Its embedding into $N$ then transfers the [quantifier-free formula](../../../../../../quantifier-free-formula.md) and its witness into $N$. Thus the hypothesis of [QET1](../../../../../../existential-common-substructure-test-for-quantifier-elimination.md) is satisfied. **The second test follows: $T$ has [quantifier elimination](../../../../../../quantifier-elimination.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
