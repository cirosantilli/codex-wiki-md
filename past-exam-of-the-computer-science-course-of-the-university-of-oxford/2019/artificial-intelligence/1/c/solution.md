<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start the threshold at zero and let $C^*$ be the least solution cost. Suppose an unsuccessful pass has threshold $L<C^*$. Along an optimal action [sequence](../../../../../sequence.md), take the first prefix whose [path cost](../../../../../path-cost.md) exceeds $L$. Its preceding prefix is explored, so that rejected prefix contributes to the next-threshold calculation. Positive [step costs](../../../../../step-cost.md) imply that its cost is at most $C^*$. Therefore the next threshold is also at most $C^*$.

By [induction](../../../../../mathematical-induction.md), no threshold used before the first solution exceeds $C^*$. A returned [goal state](../../../../../goal-state.md) therefore has cost at most $C^*$; by the definition of $C^*$ it cannot cost less. **The first returned solution is optimal.**

The termination qualification matters. In a finitely branching problem with [step costs](../../../../../step-cost.md) at least $\epsilon>0$, a threshold $L$ admits only depths up to $\lfloor L/\epsilon\rfloor$, so each pass is finite and only finitely many [path costs](../../../../../path-cost.md) precede $C^*$. These conditions establish completeness as well. Strict positivity alone on an arbitrary infinite tree is insufficient: an infinite branch with costs $1/2,1/4,1/8,\ldots$ can remain below a finite threshold and trap [depth-first search](../../../../../depth-first-search.md). The optimality argument above is valid whenever the required passes terminate; a finite graph with finitely many strictly positive action costs supplies a uniform positive lower bound.

## ↑ Ancestors (11)

1. [C](../c.md)
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
