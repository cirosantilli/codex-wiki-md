<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Messuage lemma for groups](../../../../../../messuage-lemma-for-groups.md) is the following effective collapse-versus-embedding statement: from a [finite group presentation](../../../../../../finite-group-presentation.md) for $K$ and a word $w$, one can algorithmically write a finite presentation $K_w$ such that $w=1$ in $K$ makes $K_w$ trivial, whereas $w\ne1$ makes the specified copy of $K$ embed in $K_w$. It can also be arranged that the image of $w$ normally generates $K_w$. We use this lemma as an assumed construction, as requested; the construction of its presentation does not require deciding which case applies.

Let $P$ be a [finitely presented group](../../../../../../finitely-presented-group.md) with insoluble [word problem for a group](../../../../../../word-problem-for-groups.md), whose existence is allowed. Set $K=P*\langle z\rangle$, with $z$ of infinite order. It is finitely presented, and the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md) embeds both $P$ and the infinite cyclic factor. Thus an input word $w$ from $P$ is trivial in $K$ exactly when it is trivial in $P$, while $K$ is certainly infinite.

Apply the [Messuage lemma for groups](../../../../../../messuage-lemma-for-groups.md) to this $K,w$. If $w=1$ in $P$, the constructed group $K_w$ is trivial and hence finite. If $w\ne1$, it contains $K$ and is infinite. Consequently

$$
\boxed{K_w\text{ is infinite}\quad\Longleftrightarrow\quad w\ne1\text{ in }P.}
$$

A hypothetical algorithm deciding infinitude from arbitrary [finite group presentations](../../../../../../finite-group-presentation.md) would therefore decide every input word in $P$, a contradiction. **There is no such algorithm.** The infinite cyclic free factor ensures the reduction does not need an additional assumption about the size of $P$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
