<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With initial threshold zero and unit [step costs](../../../../../step-cost.md), the thresholds are $0,1,\ldots,d$, so **there are $d+1$ passes**. Starting the first pass at one instead omits the zero-threshold pass when the root is not a goal.

At depth $i$, at most $b^i$ [search nodes](../../../../../search-node.md) are admitted in each pass with threshold at least $i$. Across all passes, the full-to-cutoff visit bound is

$$
V(b,d)=\sum_{i=0}^{d}(d+1-i)b^i.
$$

This is attained when the only depth-$d$ goal is visited last. If a [goal test](../../../../../goal-test.md) occurs before expansion, the goal is visited but not expanded, giving the corresponding worst-case expansion count

$$
\boxed{E(b,d)=\sum_{i=0}^{d}(d+1-i)b^i-1.}
$$

For $b\ne1$, the visit bound is $V(b,d)=[b^{d+2}-(d+2)b+d+1]/(b-1)^2$, hence the worst-case number expanded is **$\Theta(b^d)$ for fixed $b>1$**. For $b=1$, it is $\Theta(d^2)$. An earlier goal reduces the final pass, so its exact count cannot be inferred from $b,d$ alone. Children generated and immediately rejected above a threshold are not counted as expanded; counting those generated nodes adds the corresponding branching overhead.

## ↑ Ancestors (11)

1. [D](../d.md)
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
