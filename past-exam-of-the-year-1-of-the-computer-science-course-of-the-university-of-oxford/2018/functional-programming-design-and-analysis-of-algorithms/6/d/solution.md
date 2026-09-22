<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each physical item may enter neither knapsack or exactly one of them. Let $F_i(a,b)$ be the largest combined value using the first $i$ items with remaining capacity limits $a,b$. Initialize $F_0(a,b)=0$ and compute

$$
F_i(a,b)=\max\begin{cases}
F_{i-1}(a,b),\\
v_i+F_{i-1}(a-w_i,b)&\text{if }w_i\leq a,\\
v_i+F_{i-1}(a,b-w_i)&\text{if }w_i\leq b.
\end{cases}
$$

An infeasible alternative is omitted. The three alternatives classify the placement of item $i$ exhaustively. Every reference uses row $i-1$, ensuring that no item is placed in both knapsacks. Removing item $i$ from an optimum and applying [optimal substructure](../../../../../optimal-substructure.md) proves the [recurrence relation](../../../../../recurrence-relation.md).

**The optimum is $F_n(W_1,W_2)$**, with time $O(n(W_1+1)(W_2+1))$, conventionally $O(nW_1W_2)$ for positive capacities. Two successive layers require $O((W_1+1)(W_2+1))$ space; keep predecessor decisions or recompute them if the actual allocations are wanted. The stipulated uniqueness of values and weights is unnecessary for correctness. The capacity-indexed algorithm is [pseudopolynomial](../../../../../pseudopolynomial-time.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
