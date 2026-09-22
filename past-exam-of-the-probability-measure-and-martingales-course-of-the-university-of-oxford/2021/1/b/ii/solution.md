<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Retain the binary [random variables](../../../../../random-variable-split.md) $B_j=\mathbf1_{\{U_j\leq X_{j-1}\}}$. Iterating the recursion gives

$$
2^nX_n=x+\sum_{j=1}^n2^{j-1}B_j.
$$

Each binary history determines the full vector $(X_0,\ldots,X_n)$, so its [sigma-algebra](../../../../../sigma-algebra.md) is finite by the [sigma-algebra of a finite-valued random vector](../../../../../sigma-algebra-of-a-finite-valued-random-vector.md). Conversely, because $0<x<1$, the integer $2^nX_n-x$ uniquely determines the digits $B_1,\ldots,B_n$; also $B_j=2X_j-X_{j-1}$. Thus

$$
\mathcal F_n^X=\sigma(B_1,\ldots,B_n)=\sigma(X_n).
$$

All $2^n$ binary histories have positive [probability](../../../../../probability.md). By [independence](../../../../../independent-random-variables.md) of the driving [uniform random variables](../../../../../uniform-random-variable.md), along a fixed finite history every intermediate state is in $(0,1)$, so each subsequent conditional branch [probability](../../../../../probability.md), either $X_{j-1}$ or $1-X_{j-1}$, is strictly positive. It follows that $\mathcal F_n^X$ has $2^n$ nonempty fibres, each an [atom of a sigma-algebra](../../../../../atom-of-a-sigma-algebra.md), and exactly $2^{2^n}$ elements.

[Adaptedness](../../../../../adapted-process.md) from the preceding part gives $\mathcal F_n^X\subseteq\mathcal F_n$. For $n\geq1$, however, $\mathcal F_n$ contains the [events](../../../../../event.md) $\{U_1\leq t\}$ for every $t\in[0,1]$. They have distinct [probabilities](../../../../../probability.md) $t$, so there are infinitely many distinct such [events](../../../../../event.md). Consequently the finite [sigma-algebra](../../../../../sigma-algebra.md) $\mathcal F_n^X$ cannot equal $\mathcal F_n$. **The inclusion is strict for every $n\geq1$.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
