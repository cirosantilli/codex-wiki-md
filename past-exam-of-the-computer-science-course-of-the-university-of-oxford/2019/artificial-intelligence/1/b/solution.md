<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Iterative deepening depth-first search](../../../../../iterative-deepening-depth-first-search.md) increases a bound on the number of actions, usually through $0,1,2,\ldots$. [Iterative lengthening search](../../../../../iterative-lengthening-search.md) instead bounds accumulated [path cost](../../../../../path-cost.md); after an unsuccessful pass, its next bound is the least [path cost](../../../../../path-cost.md) among the rejected [search nodes](../../../../../search-node.md). Thus it can distinguish shallow expensive paths from deeper cheap ones.

Both repeatedly perform [depth-first search](../../../../../depth-first-search.md) and retain its small active-path storage, trading repeated work for avoiding a large [search frontier](../../../../../search-frontier.md). With unit [step costs](../../../../../step-cost.md) their bounds coincide. With unequal positive [step costs](../../../../../step-cost.md), [iterative deepening depth-first search](../../../../../iterative-deepening-depth-first-search.md) finds a solution with the fewest actions, while [iterative lengthening search](../../../../../iterative-lengthening-search.md), under the termination conditions discussed next, finds one of least total cost. Real-valued [path costs](../../../../../path-cost.md) can make [iterative lengthening search](../../../../../iterative-lengthening-search.md) perform many more passes than the depth-bounded method.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
