<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first value is the tournament winner $M$. Find the second value $s$ by taking the [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) of the direct-loser set $\operatorname{second}(S)$, retaining its associated tournament record.

The third-largest value must have lost directly to either $M$ or $s$: any other value is smaller and could not defeat it. Therefore it belongs to

$$
C=\bigl(\operatorname{second}(S)\setminus\{s\}\bigr)
\ \cup\ \{r.\mathrm{key}:r\in s.\mathrm{losers}\}.
$$

Conversely, every value in $C$ is distinct from $M,s$. Thus **the third-largest value is $\max C$**. This is [tournament selection of the three largest elements](../../../../../tournament-selection-of-the-three-largest-elements.md); it uses the retained defeat records while computing the requested three-part partition.

Three largest elements exist only for $n\geq3$. With the paper's power-of-two assumption this means $n\geq4$. The partition in part (b) remains meaningful for $n=2$, but a third output cannot be supplied in that case.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
