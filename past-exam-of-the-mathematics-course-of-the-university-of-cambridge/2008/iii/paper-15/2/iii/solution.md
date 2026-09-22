<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Translate each two-element set by its smaller element to write $S_i=\{0,s_i\}$ with $s_i>0$. Translation does not affect any [sumset](../../../../../../sumset.md) cardinality. The pair-sum hypothesis forces the $s_i$ to be distinct, since equal values would give only three pair sums. Relabel so $s_1<\cdots<s_n$.

The [distinct-positive-integer subset-sum lower bound](../../../../../../distinct-positive-integer-subset-sum-lower-bound.md) has a short inductive proof. Suppose the first $n-1$ values have sum $P$, their largest subset sum. Adding $s_n$ creates the $n$ distinct sums $P+s_n$ and $P+s_n-s_i$ for $1\leq i<n$. They are all above $P$, since $s_n>s_i$, and hence are all new. Starting with one sum for no elements and adding $1,2,\ldots,n$ new sums gives

$$
\boxed{|S|\geq1+\frac{n(n+1)}2.}
$$

Equality is attained by $S_i=\{0,i\}$. Their subset sums fill every integer from zero to $n(n+1)/2$, by induction on $n$, and each pair of distinct positive values has four different pair sums. Thus **the bound is best possible for every $n$**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
