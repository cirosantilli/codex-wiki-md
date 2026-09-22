<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Serve customers in **[nondecreasing](../../../../../nondecreasing-function.md) service time**, with ties broken arbitrarily. The objective in the source includes each customer's own service time, so these are completion times, not only delays before service begins. If the order is $\sigma$, then

$$
T=\sum_{j=1}^{n}(n-j+1)t_{\sigma(j)}.
$$

To prove optimality, consider adjacent service times $a>b$ after an elapsed time $P$. Their contributions before an exchange are $(P+a)+(P+a+b)$; after the exchange they are $(P+b)+(P+b+a)$. The total decreases by $a-b>0$. Earlier customers are unaffected, and later customers begin after the same combined duration $a+b$ as before, so their completion times are unchanged.

Repeatedly exchanging adjacent inversions reaches a [nondecreasing](../../../../../nondecreasing-function.md) order without increasing the objective. Hence that order is optimal. Sorting takes **$O(n\log n)$** time in a [comparison model](../../../../../comparison-model.md), followed by a linear traversal to produce the order or compute the total. Equal service times give zero exchange difference and do not affect optimality. If waiting time were instead defined before service, subtracting the order-independent total service time would give the same optimal order.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
