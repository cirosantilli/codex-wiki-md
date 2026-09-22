<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $D[j]$ be the minimum number of jumps from index zero to index $j$, with $\infty$ denoting an unreachable position. The [minimum forward-jump dynamic programming](../../../../../minimum-forward-jump-dynamic-programming.md) recurrence is

$$
\boxed{D[0]=0,\qquad D[j]=1+\min_{\substack{0\le i<j\\i+A[i]\ge j}}D[i]\quad(1\le j<n),}
$$

where the minimum of an empty set is $\infty$ and $1+\infty=\infty$. Compute it in increasing index order:

```
D[0] = 0
for j = 1, ..., n-1:
    D[j] = INFINITY
    for i = 0, ..., j-1:
        if D[i] != INFINITY and A[i] >= j-i:
            D[j] = min(D[j], D[i] + 1)
return D[n-1]
```

For [algorithm correctness](../../../../../algorithm-correctness.md), classify any route to $j>0$ by its penultimate index $i$. Every jump advances, so $i<j$, and legality requires $A[i]\ge j-i$. By the [principle of optimality](../../../../../principle-of-optimality.md), a shortest prefix to $i$ can be used; this gives the lower bound represented by the recurrence. Conversely, a minimizing reachable predecessor supplies an actual route of length $D[i]+1$, proving attainability. [Mathematical induction](../../../../../mathematical-induction.md) on $j$ therefore proves every stored value correct.

There are $n(n-1)/2$ predecessor tests, and two arrays are unnecessary when only the number is required. Thus

$$
\boxed{\text{time }\Theta(n^2),\qquad\text{auxiliary space }\Theta(n).}
$$

For the source example, the computed [array](../../../../../array-data-structure.md) is

$$
D=[0,1,1,2,2,2,3,3,3,3,4].
$$

When $n=1$, zero jumps are needed even if the lone entry is zero. An unreachable final position returns $\infty$. Testing `A[i] >= j-i` also avoids forming a potentially overflowing sum `i + A[i]` in bounded implementations. A faster frontier-based [algorithm](../../../../../algorithm-split.md) is possible, but the displayed method directly supplies the requested [dynamic programming](../../../../../dynamic-programming.md) solution.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
