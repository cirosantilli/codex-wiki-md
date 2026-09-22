<h1 id="8f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose first that $|A_n|=1$ for every $n>N$. Then an element of $B$ is determined by its first $N$ coordinates, so $B$ is in bijection with

$$
A_1\times\cdots\times A_N.
$$

A finite [Cartesian product](../../../../../../cartesian-product.md) of countable sets is countable by repeated application of the diagonal enumeration in part (b)(i). Hence $B$ is countable.

Conversely, suppose infinitely many factors contain at least two elements. Choose increasing indices $n_1<n_2<\cdots$ and distinct elements

$$
a_j^0,a_j^1\in A_{n_j}.
$$

Fix one element in every remaining factor. Each [binary sequence](../../../../../../bitstream.md) $\varepsilon=(\varepsilon_1,\varepsilon_2,\ldots)$ then defines an element of $B$ by placing $a_j^{\varepsilon_j}$ in coordinate $n_j$ and the fixed element elsewhere. This map is injective.

The set $\{0,1\}^{\mathbb N}$ is uncountable by [Cantor's diagonal argument](../../../../../../cantor-s-diagonal-argument.md): from any proposed list of binary sequences, form a new sequence whose $j$th digit differs from the $j$th digit of the $j$th listed sequence. It is absent from the list. Thus $B$ contains an uncountable subset and cannot be countable.

Therefore

$$
\boxed{
B\text{ is countable }\Longleftrightarrow
\exists N\ \forall n>N,\ |A_n|=1}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8F](../../8f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
