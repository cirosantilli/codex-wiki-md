<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [model-theoretic ultralimit](../../../../../model-theoretic-ultralimit.md) is the elementary direct limit of a chain of successive [ultrapowers](../../../../../ultrapower.md) along their diagonal embeddings. We will build two such chains with isomorphic limits. This is not a topological [ultrafilter](../../../../../ultrafilter.md) limit and does not require the stronger claim that one [ultrapower](../../../../../ultrapower.md) of each structure is already isomorphic.

First prove the [Frayne embedding lemma](../../../../../frayne-embedding-lemma.md), including the relative form needed to make the diagrams commute. If $C\equiv D$, expand the language by constants naming every element of $D$, and let $\operatorname{ED}(D)$ be its complete elementary diagram. Index by finite subsets $s$ of this diagram. The finitely many constants in $s$ can be interpreted in $C$ so that $s$ holds: existentially quantifying them gives a sentence true in $D$ and hence in $C$. Choose such interpretations, and give unused constants an arbitrary fixed value in the nonempty domain of $C$.

For each diagram sentence $\delta$, its cone $\{s:\delta\in s\}$ has the finite intersection property with the other cones. Extend the generated filter to an [ultrafilter](../../../../../ultrafilter.md) $U$. For $d\in D$, let $f_d(s)$ be its chosen interpretation at coordinate $s$. The map

$$
e:D\longrightarrow C^J/U,\qquad d\longmapsto[f_d]_U
$$

is elementary by Łoś: every formula true of a tuple from $D$, or its negation, is a diagram sentence and holds on its corresponding cone. In particular distinct named elements stay distinct.

If $C\preceq D$, the construction can keep every constant naming $c\in C$ equal to that same $c$ at every coordinate. For a finite diagram fragment, existentially quantify just the names outside $C$; the resulting formula with parameters in $C$ is true in $D$, hence true in $C$. Thus the finite realizations still exist with all those old names fixed. Consequently

$$
\boxed{e:D\longrightarrow C^J/U\text{ is elementary and }e(c)=[\text{constant }c]\text{ for }c\in C.}
$$

This relative extension of the diagonal map is the essential strengthening.

Now let $A_0\equiv B_0$. The nonrelative lemma embeds $B_0$ into an [ultrapower](../../../../../ultrapower.md) $A_1$ of $A_0$. Identify the image with a copy of $B_0$ inside $A_1$. Since $B_0\preceq A_1$, the relative lemma embeds $A_1$ into an [ultrapower](../../../../../ultrapower.md) $B_1$ of $B_0$ extending its diagonal map. Rename this larger structure so that the displayed copy of $A_1$ is a literal [elementary substructure](../../../../../elementary-substructure.md). Next apply the relative lemma over $A_1\preceq B_1$ to embed $B_1$ into an [ultrapower](../../../../../ultrapower.md) $A_2$ of $A_1$ fixing its diagonal copy. Continue alternately. We obtain a coherent elementary chain

$$
B_0\preceq A_1\preceq B_1\preceq A_2\preceq B_2\preceq\cdots,
$$

with $A_0\preceq A_1$ as well. Each inclusion $A_n\to A_{n+1}$ is, up to these coherent identifications, the diagonal embedding into its [ultrapower](../../../../../ultrapower.md); the same holds for $B_n\to B_{n+1}$. It is the relative clause, not merely the existence of arbitrary [elementary embeddings](../../../../../elementary-embedding.md), which guarantees this.

By the [elementary chain theorem](../../../../../elementary-chain-theorem.md), the unions of the two subsequences are elementary limits. They are the same structure: each $A_n$ lies in a subsequent $B_n$, and each $B_n$ lies in $A_{n+1}$. Hence the [alternating ultrapowers give isomorphic ultralimits](../../../../../alternating-ultrapowers-give-isomorphic-ultralimits.md) construction proves

$$
\boxed{A_0\equiv B_0\Longrightarrow A_\infty\cong B_\infty.}
$$

Conversely each [ultrapower](../../../../../ultrapower.md) and each elementary direct limit has the same first-order theory as its starting structure. Isomorphic ultralimits therefore imply $A_0\equiv B_0$ as well. Thus the conclusion exactly characterizes [elementary equivalence](../../../../../elementary-equivalence.md) at the level of ultralimits.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
