<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Build a balanced [comparison tournament](../../../../../comparison-tournament.md), retaining the record of each value's direct defeats. A record stores a key and a list of records that it directly defeated:
```
tournament(S):
    if |S| = 1:
        return Node(the element of S, [])
    split S into equally sized L and R
    a = tournament(L)
    b = tournament(R)
    if a.key < b.key:
        exchange a and b
    prepend b to a.losers
    return a
```
There is one key comparison at each merge. Because $S$ is a [set](../../../../../set-split.md), all keys are distinct, so the greater winner is unambiguous. Retaining the losing record also retains its own earlier comparison history; it does not merely retain the losing root's value.

Let the returned root have value $M$. Define

$$
\boxed{\max(S)=M,\quad
\operatorname{second}(S)=\{r.\mathrm{key}:r\in\mathrm{root.losers}\},\quad
\operatorname{third}(S)=S\setminus(\{M\}\cup\operatorname{second}(S)).}
$$

The second-largest value can only lose to $M$, so it occurs among those direct losers. This proves the required partition and the exclusion of the second-largest value from the third part. For $n=2^m$, the winner participates in exactly $m$ merges, so $\lvert\operatorname{second}(S)\rvert=m$. The other part can be materialized by marking the original element identities in this list and scanning the original inputs, using $O(n)$ additional operations without more comparisons between keys.

## ↑ Ancestors (12)

1. [B](../b.md)
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
