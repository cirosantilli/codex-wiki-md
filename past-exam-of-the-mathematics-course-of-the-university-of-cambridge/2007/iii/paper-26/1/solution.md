<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Here an [ultralimit](../../../../../ultralimit.md) in the model-theoretic sense is a [model-theoretic ultralimit](../../../../../model-theoretic-ultralimit.md): start with a [first-order structure](../../../../../first-order-structure.md), take successive [ultrapowers](../../../../../ultrapower.md) along their diagonal [elementary embeddings](../../../../../elementary-embedding.md), and take the [directed limit of elementary embeddings](../../../../../directed-limit-of-elementary-embeddings.md) of that chain. The [elementary chain theorem](../../../../../elementary-chain-theorem.md), proved by induction on formulas after identifying the embeddings with inclusions, makes every stage elementary in the limit. This definition concerns structures, rather than the topological [ultrafilter limit](../../../../../ultralimit.md).

We first prove the needed [Frayne embedding lemma](../../../../../frayne-embedding-lemma.md). If $C\equiv D$, every finite subset of the [elementary diagram of a structure](../../../../../elementary-diagram-of-a-structure.md) $D$ can be realized in $C$: existentially quantify its finitely many named elements, and use [elementary equivalence](../../../../../elementary-equivalence.md). Index by finite diagram fragments, choose such realizations, and extend the filter of cones requiring each diagram formula to an [ultrafilter](../../../../../ultrafilter.md). For each $d\in D$, let $f_d$ give its chosen coordinate realizations, filling unspecified coordinates arbitrarily. The [Łoś theorem](../../../../../los-theorem.md) shows that $d\mapsto[f_d]$ is an [elementary embedding](../../../../../elementary-embedding.md) of $D$ into an [ultrapower](../../../../../ultrapower.md) of $C$. The formulas $c_d\neq c_e$ ensure injectivity.

There is a relative version: if $C\preceq D$, keep all named elements from $C$ constant in every coordinate. Each finite diagram fragment is realizable in $C$ over those parameters by elementarity, so the resulting embedding extends the diagonal embedding of $C$ into its [ultrapower](../../../../../ultrapower.md).

Now use [alternating ultrapowers give isomorphic ultralimits](../../../../../alternating-ultrapowers-give-isomorphic-ultralimits.md). First embed $B$ into an [ultrapower](../../../../../ultrapower.md) $A_1$ of $A$. Apply the relative lemma to $B\preceq A_1$, embedding $A_1$ into an [ultrapower](../../../../../ultrapower.md) $B_1$ of $B$ over its diagonal copy. Next embed $B_1$ into an [ultrapower](../../../../../ultrapower.md) $A_2$ of $A_1$ over $A_1$, and continue. After coherent identifications this gives

$$
B\preceq A_1\preceq B_1\preceq A_2\preceq B_2\preceq\cdots.
$$

Each $A_{n+1}$ is an [ultrapower](../../../../../ultrapower.md) of $A_n$ along its diagonal embedding, and each $B_{n+1}$ is an [ultrapower](../../../../../ultrapower.md) of $B_n$ likewise. The two subsequences are cofinal in the same chain of [elementary substructures](../../../../../elementary-substructure.md), so their limits are the same union. Hence $\boxed{A\equiv B\Longrightarrow A_\infty\cong B_\infty}$. No isomorphism theorem for single [ultrapowers](../../../../../ultrapower.md) has been assumed.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
