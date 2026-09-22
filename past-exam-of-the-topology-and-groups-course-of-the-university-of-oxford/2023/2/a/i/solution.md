<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [group presentation](../../../../../group-presentation.md) of $G$ consists of a [set](../../../../../set-split.md) $S$ of symbols and a [subset](../../../../../subset.md) $R\subseteq F(S)$ of [relators](../../../../../relator.md), together with a [group isomorphism](../../../../../group-isomorphism.md)

$$
\boxed{G\cong\langle S\mid R\rangle:=F(S)/\langle\!\langle R\rangle\!\rangle.}
$$

Here $F(S)$ is the [free group](../../../../../free-group.md) on $S$, and $\langle\!\langle R\rangle\!\rangle$ is the [normal closure](../../../../../normal-closure.md) of $R$. The images of $S$ form a [generating set of a group](../../../../../generating-set-of-a-group.md); the [relators](../../../../../relator.md) prescribe which words become the [identity element](../../../../../identity-element.md).

For the [canonical presentation of a group](../../../../../canonical-presentation-of-a-group.md), use one symbol $s_g$ for every [group element](../../../../../group-element.md) $g\in G$. The [universal property of a free group](../../../../../universal-property-of-a-free-group.md) gives a [surjective](../../../../../surjective-function.md) [group homomorphism](../../../../../group-homomorphism.md)

$$
\varepsilon:F(\{s_g:g\in G\})\longrightarrow G,\qquad s_g\longmapsto g.
$$

Let $R(G)=\ker\varepsilon$, namely all words whose evaluation in $G$ is the [identity element](../../../../../identity-element.md). Then

$$
\boxed{G\cong\langle s_g\ (g\in G)\mid R(G)\rangle.}
$$

Indeed $R(G)$ is already a [normal subgroup](../../../../../normal-subgroup.md), so its [normal closure](../../../../../normal-closure.md) is itself, and the [first isomorphism theorem](../../../../../first-isomorphism-theorem.md) identifies the resulting [quotient group](../../../../../quotient-group.md) with $G$. This is the course's [canonical presentation of a group](../../../../../canonical-presentation-of-a-group.md).

An equivalent, smaller collection of [relators](../../../../../relator.md) is $s_gs_hs_{gh}^{-1}$ for all $g,h\in G$. These encode the multiplication table. They imply $s_1=1$ and $s_g^{-1}=s_{g^{-1}}$, so every word reduces to the single symbol recording its product. This proves directly that they normally generate $R(G)$, although the canonical collection above consists of every word in that [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology and groups course of the University of Oxford](../../../../split.md)
6. [Topology and groups course of the University of Oxford](../../../../../topology-and-groups-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
