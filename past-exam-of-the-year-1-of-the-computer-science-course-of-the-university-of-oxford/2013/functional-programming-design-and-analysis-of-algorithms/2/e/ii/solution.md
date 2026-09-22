<h1 id="2/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $S_j=\ell_1+\cdots+\ell_j$, with $S_0=0$. At the $j$th step of the [left fold](../../../../../../left-fold.md), the left operand of [list concatenation](../../../../../../list-concatenation.md) is the accumulated prefix of length $S_{j-1}$. Fully forcing these concatenations repeatedly copies earlier elements. Including the traversal of the outer [list](../../../../../../list-abstract-data-type.md) and the whole output spine gives

$$
\boxed{T_{\mathrm{left}}=\Theta\!\left(k+N+\sum_{j=1}^{k-1}S_j\right)
=\Theta\!\left(k+N+\sum_{t=1}^{k-1}(k-t)\ell_t\right).}
$$

For singleton inner [lists](../../../../../../list-abstract-data-type.md), this becomes $\Theta(1+2+\cdots+(k-1))=\Theta(k^2)$, whereas the [right fold](../../../../../../list-fold.md) takes $\Theta(k)$. More generally, for equal positive length $r$, the [left fold](../../../../../../left-fold.md) takes $\Theta(rk^2+k)$.

An $O(kN+k)$ bound is tight in the worst case over length distributions, but is not a tight formula for every distribution: if all $N$ elements occur only in the final inner [list](../../../../../../list-abstract-data-type.md), all earlier accumulators are empty and the cost is $\Theta(k+N)$. [Lazy evaluation](../../../../../../lazy-evaluation.md) changes when the work happens; it does not remove repeated prefix traversal when the whole result is demanded.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
