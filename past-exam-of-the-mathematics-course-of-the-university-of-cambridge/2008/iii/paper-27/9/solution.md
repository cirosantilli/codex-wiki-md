<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

An [ultrapower](../../../../../ultrapower.md) $A^I/\mathcal U$ comes with its diagonal [elementary embedding](../../../../../elementary-embedding.md) $a\mapsto[i\mapsto a]$, by the [Łoś theorem](../../../../../los-theorem.md). A [model-theoretic ultralimit](../../../../../model-theoretic-ultralimit.md) is the direct limit of successive [ultrapowers](../../../../../ultrapower.md) along these diagonal embeddings, with elementary unions at limit stages. It is not a topological [ultrafilter](../../../../../ultrafilter.md) limit. We prove the needed embedding lemma with parameters and then build the isomorphism.

If $A\equiv B$, name every element $b\in B$ by a constant $c_b$ and let $D(B)$ be its [elementary diagram of a structure](../../../../../elementary-diagram-of-a-structure.md): all sentences true in this fully named structure. For each finite $F\subseteq D(B)$, the conjunction mentions finitely many constants. Its existential closure in the original language is true in $B$, hence in $A$. Choose an interpretation of those constants in $A$ making $F$ true, and give unmentioned constants arbitrary values. Index these interpretations by $I=[D(B)]^{<\omega}$. Extend the filter of finite-diagram cones to an [ultrafilter](../../../../../ultrafilter.md) $\mathcal U$.

Map each $b$ to the class of its coordinate interpretations. Every diagram formula holds on the cone containing it, so the Łoś theorem says this map preserves every formula, including negated equalities between distinct named elements. It is therefore an [elementary embedding](../../../../../elementary-embedding.md)

$$
\boxed{B\longrightarrow A^I/\mathcal U.}
$$

This is the [Frayne embedding lemma](../../../../../frayne-embedding-lemma.md). Its relative version is crucial: if $A\prec C$, interpret all constants naming elements of $A$ constantly by those same elements. Every finite fragment of the diagram of $C$ with these fixed parameters is realized in $A$, since its existential closure with parameters from $A$ is true in $C$ and elementarity transfers it to $A$. The same construction embeds $C$ into an [ultrapower](../../../../../ultrapower.md) of $A$ while extending exactly the diagonal embedding of $A$.

Now start with $A\equiv B$. Embed $B$ into an [ultrapower](../../../../../ultrapower.md) $A_1$ of $A$. Apply the relative lemma to $B\prec A_1$ to embed $A_1$ into an [ultrapower](../../../../../ultrapower.md) $B_1$ of $B$, extending the diagonal map on $B$. Apply it to $A_1\prec B_1$ to embed $B_1$ into an [ultrapower](../../../../../ultrapower.md) $A_2$ of $A_1$, extending the diagonal map on $A_1$. Continue alternately. Replace structures by isomorphic copies to turn these [elementary embeddings](../../../../../elementary-embedding.md) into inclusions; the commuting identities supplied by the relative lemma give

$$
B\prec A_1\prec B_1\prec A_2\prec B_2\prec A_3\prec\cdots.
$$

In this common chain the map $A_n\to A_{n+1}$ is its [ultrapower](../../../../../ultrapower.md) diagonal, and so is $B_n\to B_{n+1}$. The initial $A\to A_1$ is also diagonal. The union of the $A$-stages and the union of the $B$-stages are cofinal unions of the same chain, hence are the same structure after these coherent identifications. The [elementary chain theorem](../../../../../elementary-chain-theorem.md) follows by induction on formulas, with every finite tuple and every existential witness lying in some sufficiently late stage. It shows this union is elementary over all its stages. Thus the two constructed ultralimits are isomorphic.

Conversely every successive [ultrapower](../../../../../ultrapower.md) and elementary union preserves the original complete theory. If ultralimits of $A$ and $B$ are isomorphic, they satisfy the same sentences, and their [elementary embeddings](../../../../../elementary-embedding.md) of the original structures give $A\equiv B$. Therefore

$$
\boxed{A\equiv B\quad\Longleftrightarrow\quad
\text{$A$ and $B$ have isomorphic model-theoretic ultralimits}.}
$$

This proves [Frayne theorem](../../../../../alternating-ultrapowers-give-isomorphic-ultralimits.md) by an explicit alternating construction; it does not assume the stronger theorem about isomorphic single [ultrapowers](../../../../../ultrapower.md) or any cardinal-arithmetic hypothesis.

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
