# Tournament selection of the three largest elements

↑ **Parent:** [Comparison tournament](comparison-tournament.md)

After a balanced [comparison tournament](comparison-tournament.md), the second-largest element is the [maximum](maximum-of-a-subset-of-a-total-order.md) among the winner's $m$ direct losers. The third-largest must have lost directly to the winner or to that second-largest element: no smaller element could defeat it. Excluding the known top two leaves at most $(m-1)+(m-1)$ candidates, because the second-largest won at most $m-1$ earlier comparisons. The three stages use at most $(n-1)+(m-1)+(2m-3)$ key comparisons, proving the displayed bound. Defeat records must retain their earlier subtrees; keeping only the overall winner's direct-loser values discards information used by the last stage.

## ↑ Ancestors (5)

1. [Comparison tournament](comparison-tournament.md)
2. [Selection algorithm](selection-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/5/c/solution.md)
