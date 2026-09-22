# Permanent (mathematics)

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permanent_(mathematics))

The [permanent of a matrix](permanent-mathematics.md) adds the products obtained by choosing one entry in each row and one in each column. For an $n\times n$ [matrix](matrix.md) $A=(a_{ij})$ with entries in the [real numbers](real-number.md) or [complex numbers](complex-number.md),

$$
\operatorname{perm}A=\sum_{\sigma\in S_n}\prod_{i=1}^n a_{i,\sigma(i)}.
$$

Here each [permutation](permutation.md) $\sigma$ chooses column $\sigma(i)$ in row $i$, and the [symmetric group](symmetric-group.md) $S_n$ lists every such [bijection](bijection.md). The formula resembles the [Leibniz formula for determinants](leibniz-formula-for-determinants.md), but omits the [sign of a permutation](sign-of-a-permutation.md). For a two-by-two [matrix](matrix.md),

$$
\operatorname{perm}\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad+bc,
\qquad
\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc.
$$

The absence of alternating signs makes the [permanent of a matrix](permanent-mathematics.md) particularly useful for counting allowed assignments.

For a zero-one [matrix](matrix.md), let rows represent people, columns represent jobs, and $a_{ij}=1$ mean that person $i$ can do job $j$. This is the [biadjacency matrix](biadjacency-matrix.md) of a [bipartite graph](bipartite-graph-split.md). A product in the permanent is one exactly when all the selected assignments are allowed; otherwise it is zero. Each surviving [permutation](permutation.md) assigns every person a different job, which is a [perfect matching](perfect-matching.md). Thus the permanent counts [perfect matchings](perfect-matching.md). This interpretation and the definition are given in [Yufei Zhao, Probabilistic Methods in Combinatorics, §10.2, pp. 178–179](https://ocw.mit.edu/courses/18-226-probabilistic-methods-in-combinatorics-fall-2022/mit18_226_f22_lec_full.pdf).

For a fully enumerated example, take

$$
A=\begin{pmatrix}1&1&0\\1&1&1\\0&1&1\end{pmatrix}.
$$

Among the six [permutations](permutation.md) of three columns, exactly three give nonzero products: $(1,2,3)$, $(1,3,2)$ and $(2,1,3)$. These tuples list the chosen column in each successive row. Each product is one, so $\operatorname{perm}A=3$. Their [permutation signs](sign-of-a-permutation.md) are $+1,-1,-1$, giving $\det A=-1$. The diagram displays all three allowed assignments.

<a id="image-three-allowed-one-to-one-assignments-contribute-positively-to-the-permanent-while-their-permutation-signs-give-a-determinant-of-minus-one"></a>
![](permanent-perfect-matching-assignments.png)

**[Figure 19](#image-three-allowed-one-to-one-assignments-contribute-positively-to-the-permanent-while-their-permutation-signs-give-a-determinant-of-minus-one). Three allowed one-to-one assignments contribute positively to the permanent, while their permutation signs give a determinant of minus one**.

A zero [determinant](determinant.md) need not mean that no assignment exists. The two-by-two all-ones [matrix](matrix.md) has permanent $2$ and [determinant](determinant.md) $0$: its two assignments cancel in the determinant. The [nonzero determinant criterion for a perfect matching](perfect-matching-from-a-nonzero-determinant.md) is sufficient for existence, but the converse fails for a fixed zero-one [matrix](matrix.md).

For nonnegative entries, the permanent instead sums assignment weights, with each assignment weighted by the product of its selected entries. It is then a total weight rather than necessarily an [integer](integer-split.md) count. With arbitrary entries in the [real numbers](real-number.md) or [complex numbers](complex-number.md), even the permanent can have cancellation; the counting interpretation specifically uses zero-one entries. The [permanent as probability of distinct independent choices](permanent-as-probability-of-distinct-independent-choices.md) gives another useful nonnegative interpretation.

There are $n!$ terms in the defining sum, linking direct evaluation to the [factorial](factorial.md). For the all-ones $n\times n$ [matrix](matrix.md), every term is one and the permanent is exactly $n!$; the [identity matrix](identity-matrix.md) has permanent one. Finding one allowed assignment and counting all allowed assignments are different questions. Their relationship to [computational complexity theory](computational-complexity-theory.md) was studied in [L. G. Valiant, The complexity of computing the permanent, Theoretical Computer Science 8(2), 189–201, 1979](https://www.sciencedirect.com/science/article/pii/0304397579900446). The elementary sum is useful for small examples, while the existing [dense permanent approximation](dense-permanent-approximation.md) describes a more specialized way of estimating large counts.

**Table of contents**

- [Ryser's formula for the permanent](ryser-s-formula-for-the-permanent.md)
- [Permanent as probability of distinct independent choices](permanent-as-probability-of-distinct-independent-choices.md)
- [Dense permanent approximation](dense-permanent-approximation.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
