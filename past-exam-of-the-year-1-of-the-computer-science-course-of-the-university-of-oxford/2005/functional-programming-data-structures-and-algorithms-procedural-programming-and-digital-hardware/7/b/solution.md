<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each merge consumes and copies a total of $n$ elements, so its [time complexity](../../../../../time-complexity.md) is $\Theta(n)$. Hence

$$
T(1)=\Theta(1),\qquad
T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n).
$$

At any level of the recursion tree, all active subranges are disjoint and together contain at most $n$ elements. The total work per level is therefore $O(n)$, and halving gives $O(\log n)$ levels. In fact the full run performs $\Theta(n\log n)$ work for $n\geq2$.

The shared work [array](../../../../../array-data-structure.md) holds $n$ elements, and the depth-first recursion has $O(\log n)$ simultaneous activation records with a constant number of scalar variables each. No recursive call allocates a fresh [array](../../../../../array-data-structure.md). Therefore

$$
\boxed{\text{time }\Theta(n\log n),\qquad
\text{auxiliary space }\Theta(n)+O(\log n)=\Theta(n).}
$$

The work [array](../../../../../array-data-structure.md) is counted in the auxiliary [space complexity](../../../../../space-complexity.md) even though the caller supplies it. If its actual allocated capacity is $M>n$, the reserved storage is $\Theta(M+\log n)$; choosing capacity $n$ gives the stated bound.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
