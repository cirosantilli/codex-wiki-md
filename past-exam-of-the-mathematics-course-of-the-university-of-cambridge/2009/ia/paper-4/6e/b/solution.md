<h1 id="6e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the universe $\Omega=\{B\subseteq A:|B|=k\}$ and define the exact-occupancy events $E_i=\{B\in\Omega:|B\cap A_i|=3\}$. The desired collection is $\bigcup_{i=1}^kE_i$, so apply [inclusion-exclusion](../../../../../../inclusion-exclusion-principle.md) to these events.

Fix $r$ distinct block indices. For $B$ to belong to the intersection of their events, it must contain exactly three elements in each selected block. There are $\binom m3^r$ ways to make those choices. None of the other elements in these selected blocks may be included; the remaining $k-3r$ elements must come from the $n-rm$ elements outside the selected blocks. Thus

$$
\left|E_{i_1}\cap\cdots\cap E_{i_r}\right|=\binom m3^r\binom{n-rm}{k-3r}.
$$

There are $\binom kr$ choices of block indices, and the intersection is empty when $3r>k$. Substitution into [inclusion-exclusion](../../../../../../inclusion-exclusion-principle.md) gives

$$
\boxed{|\mathcal B|=\sum_{r=1}^{\lfloor k/3\rfloor}(-1)^{r-1}\binom kr\binom m3^r\binom{n-rm}{k-3r}.}
$$

Here [binomial coefficients](../../../../../../binomial-coefficient.md) with a lower argument exceeding a nonnegative upper argument are zero. In particular, when $m<3$ every event is empty, and when $k<3$ the sum is empty; both give the correct answer zero. The subtraction of entire selected blocks, not merely the $3r$ chosen elements, is what enforces exact rather than at-least-three occupancy. This is [inclusion-exclusion for exact block occupancy](../../../../../../inclusion-exclusion-for-exact-block-occupancy.md) with the number of blocks and subset size both equal to $k$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
