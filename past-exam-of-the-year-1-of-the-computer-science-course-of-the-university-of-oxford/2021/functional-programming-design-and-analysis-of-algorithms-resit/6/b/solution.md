<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S$ again be the total. Reject unless $S$ is divisible by three, and put $h=S/3$. Define $D_i(x,y)$ to mean that the first $i$ occurrences can be assigned to three groups so that the first two groups have sums $x$ and $y$. Their third sum is already determined by the processed [list prefix](../../../../../prefix-of-a-list.md) sum minus $x+y$, so it need not be stored as another coordinate.

Initialize $D_0(0,0)$ true and all other states false. For each reachable state, assign the next occurrence to exactly one group:
```
threeEqualParts(A):
    S = sum of A
    if S mod 3 != 0: return false
    h = S/3
    D[0..h,0..h] = false
    D[0,0] = true
    for each indexed entry a in A:
        Next[0..h,0..h] = false
        for x from 0 to h:
            for y from 0 to h:
                if D[x,y]:
                    Next[x,y] = true
                    if x+a <= h: Next[x+a,y] = true
                    if y+a <= h: Next[x,y+a] = true
        D = Next
    return D[h,h]
```
The three transitions put the occurrence in the third, first or second group, respectively. Using a fresh layer prevents reusing it. Conversely, deleting the last occurrence from any valid [list prefix](../../../../../prefix-of-a-list.md) assignment leaves exactly one predecessor state, so [induction](../../../../../mathematical-induction.md) proves completeness as well as soundness. At the final state $(h,h)$, the third sum is $S-2h=h$, giving precisely the required disjoint partition.

There are $(h+1)^2$ states per layer and a constant number of transitions per state. Thus the time is **$O(n(h+1)^2)\subseteq O(n^3k^2)$**, and rolling layers use **$O((h+1)^2)\subseteq O(n^2k^2)$** space for nonempty inputs. The source mentions an additional [integer](../../../../../integer-split.md) $s$ in this part, but it does not occur in the stated equal-partition condition; the required target is determined by $S$. Empty groups are allowed by the stated [subset](../../../../../subset.md) formulation.

## ↑ Ancestors (12)

1. [B](../b.md)
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
