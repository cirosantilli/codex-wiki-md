<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret limit points as subsequential limits, including a value repeated infinitely often. Let $L$ be the common nonempty compact cluster set. Boundedness implies $\operatorname{dist}(a_n,L)\to0$ and likewise for $b_n$: otherwise a subsequence staying a fixed distance away would have a convergent further subsequence whose limit both belongs to $L$ and stays away from it.

Construct a matching of indices in alternating steps. At step $2j-1$ choose the least unused index $m$ in the first sequence. Choose a nearest point $\ell\in L$ to $a_m$ and an unused index $n$ in the second sequence with $|b_n-\ell|<1/j$. Such indices exist infinitely often because $\ell$ is a subsequential limit. Pair $m$ with $n$; their values differ by at most $\operatorname{dist}(a_m,L)+1/j$. At step $2j$ choose the least unused second-sequence index and match it to an unused first-sequence index within $1/j$ of a nearest point of $L$. This gives the analogous bound with $b_n$.

Every index is used exactly once: no step reuses an index, and by step $2j$ at least the first $j$ indices in each sequence have been used. Hence the produced lists are permutations satisfying

$$
\boxed{k\in\{m_1,\ldots,m_{2k}\}\cap\{n_1,\ldots,n_{2k}\}.}
$$

The indices actively chosen as least unused tend to infinity on their respective odd and even steps. Their distances to $L$ therefore tend to zero, and $1/j\to0$. The two matching estimates prove **$\boxed{|a_{m_k}-b_{n_k}|\to0}$**. The cluster-set convention is important here; accumulation points of the set of distinct values would ignore infinite repetitions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
