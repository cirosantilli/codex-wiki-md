<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the two history [D flip-flops](../../../../../d-flip-flop.md) and add an output [D flip-flop](../../../../../d-flip-flop.md) with previous value $q=z_{n-1}$. Its next value $q^+=z_n$ is one if all three inputs are one, or if the output was one and at least one of the three inputs is one. In the latter case the samples are not all zero, so the previous one must be retained. This gives

$$
\boxed{q^+=abc+aq+bq+cq,\qquad q_{\rm initial}=0.}
$$

If $abc=111$, the first product sets the output. If $abc=000$, every product vanishes and the output clears. For every mixed input triple, at least one of $aq,bq,cq$ equals $q$, so the output is retained. Feed this [sum of products](../../../../../disjunctive-normal-form.md) to the output D input, use $b^+=a,c^+=b$ for the history, and use [asynchronous clear](../../../../../asynchronous-clear.md) or an appropriate initialization to establish $q=0$.

Minimality can be seen directly from the [truth table](../../../../../truth-table.md). At $q=0$, the only one-entry is $abc=111$, forcing the product $abc$ or a narrower term. At $q=1$, the triples $100$, $010$ and $001$ must all produce one; combining any two in one product would also admit $000$, which must produce zero. Thus three more products are needed. The displayed four products achieve the minimum; removing any [Boolean literal](../../../../../boolean-literal.md) from $abc,aq,bq,cq$ would include a zero-entry.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
