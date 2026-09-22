<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A sentence $\forall\bar x\,\exists\bar y\,\varphi(\bar x,\bar y)$ with quantifier-free $\varphi$ is preserved by a union of an embedding chain: a tuple $\bar a$ occurs at some stage, a witness $\bar b$ exists at that stage, and quantifier-free formulas are preserved in the union. Thus every forall-exists axiomatized theory is [inductive](../../../../../../inductive-first-order-theory.md).

Conversely, let $T_0$ contain all forall-exists consequences of $T$ and suppose $M\models T_0$. The diagram-and-compactness sandwich lemma says that one can construct

$$
M=M_0\subseteq N_0\subseteq M_1\subseteq N_1\subseteq\cdots
$$

where every $N_i\models T$ and every $M_i\preccurlyeq M_{i+1}$. For completeness, the first extension is obtained by adding to $T$ the diagram of $M_i$ together with all universal formulas over $M_i$ true there. A finite inconsistency would give a forall-exists consequence of $T$ false in $M_i$. The resulting extension embeds into an elementary extension $M_{i+1}$ by the method of diagrams.

The $N_i$ form an embedding chain and have the same union $N$ as the $M_i$. By the assumed preservation, $N\models T$; by the [elementary chain theorem](../../../../../../elementary-chain-theorem.md), $M\preccurlyeq N$. Hence $M\models T$, so $T_0\models T$. The two theories are equivalent, proving the characterization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
