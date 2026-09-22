<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $U$ be all [universal sentences](../../../../../../universal-sentence.md) true in $C$. The theory $T\cup U$ is consistent. Indeed, if a finite conjunction $u$ of sentences from $U$ were inconsistent with $T$, then $T\models\neg u$. A finite conjunction of [universal sentences](../../../../../../universal-sentence.md) is universal, so its negation is equivalent to an [existential sentence](../../../../../../existential-sentence.md). By the hypothesis $C$ would satisfy $\neg u$, whereas it satisfies $u$.

Choose $A\models T\cup U$. Now expand the language by names for every element of $C$ and consider its [elementary diagram](../../../../../../elementary-diagram-of-a-structure.md) $\operatorname{ElDiag}(C)$. Its universal consequences in the original language are exactly $U$: any such consequence is true in the named copy of $C$, while any original-language sentence true in $C$ already belongs to its elementary diagram. Part (b), applied to $A$ and this expanded theory, gives a [structure embedding](../../../../../../structure-embedding.md) of $A$ into a model $D$ of $\operatorname{ElDiag}(C)$. The named copy of $C$ is an [elementary substructure](../../../../../../elementary-substructure.md) of $D$. Identifying that copy with $C$, we obtain

$$
\boxed{A\models T,\qquad A\hookrightarrow D,\qquad C\preccurlyeq D.}
$$

Thus the required target is an [elementary extension](../../../../../../elementary-extension.md) of $C$, although $C$ itself need not be a model of $T$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
