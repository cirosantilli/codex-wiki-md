<h1 id="3/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [Gelfand–Tsetlin basis](../../../../../../../gelfand-tsetlin-basis.md) spans $V^\lambda$, and the scalar computed on its vectors depends only on the shape. Thus

$$
\boxed{X_2\cdots X_nw=\begin{cases}(-1)^k k!(n-k-1)!\,w&\lambda=(n-k,1^k),\\0&\lambda\text{ not a hook},\end{cases}}
$$

for every $w\in V^\lambda$. The product is the sum of the $(n-1)!$ permutations in the [conjugacy class](../../../../../../../conjugacy-class.md) of an $n$-cycle. Taking [traces](../../../../../../../matrix-trace.md) therefore gives $(n-1)!\chi^\lambda((n))$ equal to the displayed scalar times $\dim V^\lambda$.

For a [hook partition](../../../../../../../hook-partition.md), a [standard Young tableau](../../../../../../../standard-young-tableau.md) is uniquely determined by the choice of its $k$ entries below the top cell, selected from $\{2,\ldots,n\}$. The column and the remaining row are then forced to increase. Hence $\dim V^{(n-k,1^k)}=\binom{n-1}{k}$, and cancellation of the factorials yields

$$
\boxed{\chi^\lambda((n))=\begin{cases}(-1)^k&\lambda=(n-k,1^k),\\0&\lambda\text{ not a hook}.\end{cases}}
$$

This uses the [central character value of a conjugacy-class sum](../../../../../../../central-character-value-of-a-conjugacy-class-sum.md) and tableau counting, without a character rule for removing [rim hooks](../../../../../../../rim-hook.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
