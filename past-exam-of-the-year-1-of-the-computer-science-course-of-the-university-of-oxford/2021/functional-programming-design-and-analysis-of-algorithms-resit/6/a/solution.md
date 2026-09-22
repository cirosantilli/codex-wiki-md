<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat [array](../../../../../array-data-structure.md) entries as indexed occurrences, so equal numerical values may be selected independently. Put $S=\sum_{j=1}^{n}a_j\leq nk$. Reject $s<0$ or $s>S$. Define $D_i(t)$ to mean that some [subset](../../../../../subset.md) of the first $i$ indices sums to $t$. The base is $D_0(0)=\mathrm{True}$ and all other base entries are false. Considering whether index $i$ is selected gives

$$
D_i(t)=D_{i-1}(t)\lor\bigl(t\geq a_i\ \land\ D_{i-1}(t-a_i)\bigr).
$$

Only $0\leq t\leq s$ is needed, because all entries are positive. A one-dimensional implementation is
```
subsetSum(A, s):
    S = sum of A
    if s < 0 or s > S: return false
    D[0..s] = false
    D[0] = true
    for each indexed entry a in A:
        for t from s down to a:
            D[t] = D[t] or D[t-a]
    return D[s]
```
Descending updates make both right-hand-side values belong to the previous [list prefix](../../../../../prefix-of-a-list.md): when updating $t$, the smaller location $t-a$ has not yet been updated for this entry. This prevents using the same occurrence repeatedly. [Induction](../../../../../mathematical-induction.md) on the [list prefix](../../../../../prefix-of-a-list.md) proves the recurrence and the returned answer.

The time is $O(n(s+1))\subseteq O(n^2k)$ for nonempty input with $k\geq1$, and space is $O(s+1)\subseteq O(nk)$. More generally one may fill through $S$ and answer every target from the same table. For a two-way equal partition, reject odd $S$; otherwise ask for target $S/2$. A selected [subset](../../../../../subset.md) with that sum leaves its complement with the same sum. These are bounds [polynomial](../../../../../polynomial-split.md) in the numerical bound $k$; without that bound the method is pseudopolynomial in a binary-encoded unrestricted target.[Chapter 3, §3.8, Subset Sum: include/exclude states and memoization](../../../../../dynamic-programming-by-jeff-erickson.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
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
