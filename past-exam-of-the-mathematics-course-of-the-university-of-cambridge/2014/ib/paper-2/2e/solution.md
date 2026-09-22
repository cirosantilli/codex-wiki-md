<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

An even [permutation](../../../../../permutation.md) in the [alternating group](../../../../../alternating-group.md) $A_6$ has one of the cycle types listed below. In the [symmetric group](../../../../../symmetric-group.md), a type with $m_j$ cycles of length $j$ has centralizer order $\prod_j j^{m_j}m_j!$ and class size $6!/\prod_j j^{m_j}m_j!$: commuting permutations can rotate each cycle and exchange equal-length cycles.

An $S_6$ [conjugacy class](../../../../../conjugacy-class.md) remains one $A_6$ class if its centralizer contains an odd permutation. Otherwise it splits into two equal classes, since the centralizer is already contained in the index-two subgroup $A_6$. This is the [alternating conjugacy class splitting criterion](../../../../../alternating-conjugacy-class-splitting-criterion.md). For the nonsplitting nonidentity types here, odd commuting permutations are respectively a constituent transposition, a transposition of fixed points, the interchange of two 3-cycles, and the constituent 4-cycle. For a 5-cycle with one fixed point, the centralizer is its cyclic group of order five and contains only even permutations.

Thus the [conjugacy classes of the alternating group on six letters](../../../../../conjugacy-classes-of-the-alternating-group-on-six-letters.md) are:

$$
\begin{array}{c|c|c}
\text{cycle type}&\text{representative}&\text{class size in }A_6\\ \hline
1^6&1&1\\
2^2\,1^2&(12)(34)&45\\
3\,1^3&(123)&40\\
3^2&(123)(456)&40\\
4\,2&(1234)(56)&90\\
5\,1&(12345)&72\\
5\,1&(12345)^2&72
\end{array}
$$

The two 5-cycle representatives lie in different classes. A relabelling that conjugates a 5-cycle to its square acts on its five positions as multiplication by two modulo five, a 4-cycle on the nonzero positions, hence is odd. Every other such conjugator differs by an even centralizer element. The sizes sum to $360=|A_6|$, so the list is exhaustive.

For [simplicity of the alternating group on six letters](../../../../../simplicity-of-the-alternating-group-on-six-letters.md), let $N$ be a [normal subgroup](../../../../../normal-subgroup.md). It contains the identity and is a union of full [conjugacy classes](../../../../../conjugacy-class.md); also $|N|$ divides $360$ by [Lagrange's theorem](../../../../../lagrange-s-theorem.md). A proper subgroup has order at most $180$.

If the class of size 45 is absent, $|N|$ is odd. The odd divisors of $360$ are $1,3,5,9,15,45$. A nontrivial union has order at least 41, but no selection of the even class sizes sums to $44$, so order 45 is impossible. Thus $N=\{1\}$ in this case.

If the size-45 class is present, write $|N|=46+40a+90b+72c$ with $0\le a,c\le2$ and $0\le b\le1$. The possible values at most $180$ are $46,86,118,126,136,158,176$, none dividing $360$. Hence no proper nontrivial [normal subgroup](../../../../../normal-subgroup.md) exists:

$$
\boxed{A_6\text{ is simple}.}
$$

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
