<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A [model-theoretic ultralimit](../../../../../model-theoretic-ultralimit.md) is the direct limit of a chain of successive [ultrapowers](../../../../../ultrapower.md) along their diagonal elementary maps. It is not the topological notion of a limit along an [ultrafilter](../../../../../ultrafilter.md). We first prove the precise relative embedding lemma needed to synchronize two such limits.

If $A\prec B$, then $B$ embeds elementarily into an [ultrapower](../../../../../ultrapower.md) of $A$, with the embedding restricting on $A$ to its diagonal map. To prove this [Frayne embedding lemma](../../../../../frayne-embedding-lemma.md), use the elementary diagram of $B$ with the elements of $A$ treated as named parameters. Every finite fragment $\Delta$ of that diagram has a realization in $A$: replace its finitely many names from $B\setminus A$ by variables and existentially quantify their conjunction. It is true in $B$, and hence true in $A$ by elementarity. Choose these simultaneous realizations for each finite fragment, keeping every parameter from $A$ interpreted as itself; give unmentioned names an arbitrary default in the nonempty $A$.

On the index set of finite fragments, extend the filter of cones $\{\Delta:\Delta\supseteq\Gamma\}$ to an [ultrafilter](../../../../../ultrafilter.md) $U$. For each $b\in B$, let $g_b(\Delta)$ be its value in the chosen coordinate realization. Every diagram sentence is satisfied on its cone, so the [Łoś theorem](../../../../../los-theorem.md) makes $b\mapsto[g_b]$ an [elementary embedding](../../../../../elementary-embedding.md) $B\to A^I/U$. Inequalities in the diagram ensure injectivity. If $b\in A$, all its coordinates equal $b$, giving exactly the diagonal map.

There is also the initial version: if merely $A\equiv B$, then $A$ embeds elementarily into an [ultrapower](../../../../../ultrapower.md) of $B$. A finite fragment of the elementary diagram of $A$, with all its names replaced by variables, yields an existential sentence true in $A$ and hence in $B$. The identical finite-fragment and cone construction therefore proves this version without already assuming an embedding.

Start with $A_0=A$. Use the initial version to place $A_0$ elementarily in an [ultrapower](../../../../../ultrapower.md) $B_0$ of $B$. Relabel embedded copies so we can regard the elementary maps as inclusions. Apply the relative version to $A_0\prec B_0$ to obtain an [ultrapower](../../../../../ultrapower.md) $A_1$ of $A_0$ containing $B_0$, and whose inclusion of $A_0$ is its diagonal map. Next apply it to $B_0\prec A_1$ to obtain an [ultrapower](../../../../../ultrapower.md) $B_1$ of $B_0$ containing $A_1$, again fixing the earlier diagonal inclusion. Continuing gives an elementary chain

$$
A_0\prec B_0\prec A_1\prec B_1\prec A_2\prec B_2\prec\cdots.
$$

The common union $C$ is elementary over every stage by the [elementary chain theorem](../../../../../elementary-chain-theorem.md), and

$$
C=\bigcup_{n<\omega}A_n=\bigcup_{n<\omega}B_n.
$$

The first presentation is a [model-theoretic ultralimit](../../../../../model-theoretic-ultralimit.md) of $A$. The second, preceded by the initial diagonal embedding of $B$ into $B_0$, is a [model-theoretic ultralimit](../../../../../model-theoretic-ultralimit.md) of $B$. Each consecutive same-letter inclusion is precisely the corresponding [ultrapower](../../../../../ultrapower.md) diagonal map, not just an unspecified [elementary embedding](../../../../../elementary-embedding.md). Thus the two limits are identified with the same structure $C$, proving

$$
\boxed{A\equiv B\ \Longrightarrow\ A\text{ and }B\text{ have isomorphic model-theoretic ultralimits}.}
$$

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
