<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**The comparator alone cannot generally reproduce informed [A-star search](../../../../../a-star-search.md) priorities. A valid weaker fallback is [uniform-cost search](../../../../../uniform-cost-search.md), namely [A-star search](../../../../../a-star-search.md) with $h=0$.** The issue is that ordering $h^*(n)$ and $h^*(m)$ does not supply the numerical difference needed to compare $g(n)+h^*(n)$ with $g(m)+h^*(m)$.

For example, take accumulated costs $g(n)=5$, $g(m)=1$. Remaining costs $h^*(n)=1$, $h^*(m)=2$ rank $n$ ahead under $\kappa$ but give total estimates $6$ and $3$, so informed [A-star search](../../../../../a-star-search.md) selects $m$. Remaining costs $1$ and $10$ give the same pairwise comparator ranking but totals $6$ and $11$, selecting $n$. Thus the comparator's ordering cannot simply replace the cardinal [heuristic function](../../../../../heuristic-function.md) inside $f=g+h$.

If “do [A-star search](../../../../../a-star-search.md)” includes choosing any available [admissible heuristic](../../../../../admissible-heuristic.md), set it identically to zero and prioritize by the known accumulated cost $g$. Apply the [goal test](../../../../../goal-test.md) on removal from the [search frontier](../../../../../search-frontier.md). This is complete and optimal under the stated finiteness and step-cost assumptions, but it does not recover the unavailable perfect-[heuristic function](../../../../../heuristic-function.md) ordering or its search reduction. The distinction is between implementing the informed priority from $\kappa$ and retaining the algorithm's guarantees through this uninformed special case.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
