<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Countability of the forcing and uncountability of $Y$ are understood internally in $M$ and $M[G]$, respectively. This matters because the model itself is externally countable. Choose a name $\dot Y\in M$ and a ground-model set $A\in M$ containing every ground-model element that can occur in $Y$. Such an $A$ exists: the rank of $\dot Y$ bounds the ranks of its values, so a sufficiently high $V_\theta^M$ contains $Y\subseteq M$.

For $p\in P$, ground-model [axiom schema of separation](../../../../../../../axiom-schema-of-specification.md) and the [forcing definability lemma](../../../../../../../forcing-definability-lemma.md) give

$$
X_p=\{a\in A:p\Vdash\check a\in\dot Y\}\in M.
$$

By the [forcing truth lemma](../../../../../../../forcing-truth-lemma.md),

$$
Y=\bigcup_{p\in G}X_p.
$$

If every $X_p$ for $p\in G$ were countable in $M$, it would remain countable in $M[G]$, where $G\subseteq P$ is countable. Then $Y$ would be countable, contrary to the hypothesis. Thus some $p\in G$ has $X_p$ uncountable in $M$; otherwise its ground-model enumeration would still enumerate it in the extension. Let $X=X_p$. Every one of its members is forced by $p$ into $Y$, so

$$
\boxed{X\in M,\quad M\models|X|>\aleph_0,\quad
M[G]\models X\subseteq Y.}
$$

The [countable chain condition for forcing](../../../../../../../countable-chain-condition-for-forcing.md) also preserves its uncountability. Separativity is not needed for this particular argument. This is the [ground-model uncountable subset lemma for countable forcing](../../../../../../../ground-model-uncountable-subset-lemma-for-countable-forcing.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
