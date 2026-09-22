<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

A set is [countable](../../../../../countable-set.md) if it is finite or bijects with a subset of $\mathbb N$. For any $f:X\to\mathcal P(X)$, the [Cantor diagonal argument](../../../../../cantor-diagonal-argument.md) set $D=\{x:x\notin f(x)\}$ differs from every $f(y)$ at $y$. Hence no such map is surjective. Binary sequences are indicator functions of subsets of $\mathbb N$, so $\{0,1\}^{\mathbb N}\cong\mathcal P(\mathbb N)$ is uncountable.

Every member of $L$ corresponds to a unique permutation $(a_0,a_1,\ldots)$ of $\mathbb N$, with $F_n=\{a_0,\ldots,a_{n-1}\}$. Let $p(j)$ be the position of $j$.

For $L_0$, $p(n)<n$ eventually. Choose $N$ after which this holds and then $m$ larger than all $p(0),\ldots,p(N-1)$. The $m$ positions $0,\ldots,m-1$ would contain all $m+1$ values $0,\ldots,m$, a contradiction. Thus **$L_0$ is empty**, hence countable.

For $L_1$, $p(n)\leq n$ eventually. For every sufficiently large $m$, all values $0,\ldots,m$ occur in positions $0,\ldots,m$, so this initial segment is invariant. Comparing consecutive invariant initial segments gives $p(m)=m$ eventually. These are the finite-support permutations, of which there are countably many. Hence **$L_1$ is countable**.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
