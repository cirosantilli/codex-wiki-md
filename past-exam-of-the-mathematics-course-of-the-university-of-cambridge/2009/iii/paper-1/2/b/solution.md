<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The allowed algebraic characterization is the [Boone-Higman theorem](../../../../../../boone-higman-theorem.md):

$$
\boxed{G\text{ finitely generated has soluble word problem}
\ \Longleftrightarrow\ G\hookrightarrow S\hookrightarrow P,
\quad S\text{ simple},\quad P\text{ finitely presented}.}
$$

The [simple group](../../../../../../simple-group.md) $S$ need not itself be finitely presented. The primary statement is Theorem I of [An algebraic characterization of groups with soluble word problem](https://www.cambridge.org/core/journals/journal-of-the-australian-mathematical-society/article/an-algebraic-characterization-of-groups-with-soluble-word-problem1/748FFD937CEA3727E812C8CDB9CC59B9). In particular, a finitely generated [group](../../../../../../group-split.md) with insoluble [word problem for a group](../../../../../../word-problem-for-groups.md) cannot embed in any finitely presented simple group: otherwise take that group as both $S$ and $P$ in the characterization.

Use the following effective form of the permitted [Messuage lemma for groups](../../../../../../messuage-lemma-for-groups.md). Given a [finite group presentation](../../../../../../finite-group-presentation.md) of $K$ and a word $w$, one can algorithmically write a finite presentation $K_w$ such that $w=1$ in $K$ implies $K_w=1$, while $w\ne1$ implies that $K$ embeds in $K_w$. The construction is performed without first deciding whether $w$ is trivial. A collapse-and-embedding lemma with these properties is also stated as Lemma 5.13 in [Combinatorial Group Theory](https://www.macs.hw.ac.uk/~lc45/Teaching/kggt/miller.pdf). No proof of that allowed lemma is needed here.

Fix a finitely presented [group](../../../../../../group-split.md) $U$ with insoluble [word problem for a group](../../../../../../word-problem-for-groups.md), whose existence is allowed. For each input word $w$ in its generators, construct $U_w$ by the lemma and then form the finite presentation of

$$
P_w=U_w*C_2.
$$

If $w=1$, then $P_w\cong C_2$, which is a nontrivial [simple group](../../../../../../simple-group.md). If $w\ne1$, the lemma embeds $U$ in $U_w$, and the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md) embeds $U_w$ in $P_w$. If $P_w$ were simple, it would be a finitely presented simple group containing $U$, contradicting the characterization. Hence

$$
\boxed{P_w\text{ is simple}\ \Longleftrightarrow\ w=1\text{ in }U.}
$$

An algorithm deciding simplicity from arbitrary finite presentations would therefore solve the insoluble [word problem for a group](../../../../../../word-problem-for-groups.md) in $U$. This proves **simplicity of finitely presented groups is algorithmically undecidable**. Using $C_2$ avoids any convention about whether the trivial group is called simple.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
