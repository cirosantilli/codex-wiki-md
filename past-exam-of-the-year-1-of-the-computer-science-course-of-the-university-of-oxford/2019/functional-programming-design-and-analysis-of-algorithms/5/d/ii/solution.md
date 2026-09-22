<h1 id="5/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $n=1$, return its sole index without a query. Otherwise first evaluate $f(t,t,\ldots,t)$ for $t=1,\ldots,d$ until two different outputs are found. Part i says these outputs are precisely $f_i(t)$, so two values $a,b$ with $f_i(a)\ne f_i(b)$ must exist. This uses at most $d$ calls to the [function-evaluation oracle](../../../../../../function-oracle.md).

Maintain a candidate index [set](../../../../../../set-split.md) $S$, initially all indices. Split $S$ into two nearly equal pieces and choose one, $H$. Query the input that is $b$ on $H$ and $a$ everywhere else. Its output equals $f_i(b)$ exactly when $i\in H$, and otherwise equals $f_i(a)$. Retain the indicated half and repeat until one index remains.

The [loop invariant](../../../../../../loop-invariant.md) is $i\in S$, and the witness outputs keep each test unambiguous. There are at most $\lceil\log_2 n\rceil$ splitting queries. The total is **at most $d+\lceil\log_2n\rceil$ evaluations**, which is $O(d\log n)$ for $n\ge2$, and in fact a stronger additive bound. Only oracle calls are being counted; explicitly constructing each query vector can require $O(n)$ ordinary work. This is [identification of a unique essential variable](../../../../../../identification-of-a-unique-essential-variable.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
