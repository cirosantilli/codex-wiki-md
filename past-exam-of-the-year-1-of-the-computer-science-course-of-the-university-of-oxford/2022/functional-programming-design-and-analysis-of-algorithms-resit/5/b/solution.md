<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Maintain the two largest entries of each segment, counting repeated values as separate entries. A singleton returns its value and a sentinel $-\infty$ for its missing runner-up. Split a longer segment into two nonempty halves, recursively obtain $(m_L,s_L)$ and $(m_R,s_R)$, and combine them by

$$
(m,s)=\begin{cases}
(m_L,\max(s_L,m_R)),&m_L\ge m_R,\\
(m_R,\max(m_L,s_R)),&m_L<m_R.
\end{cases}
$$

For example, an implementation on an indexed [sequence](../../../../../sequence.md) can use:
```
top2(lo, hi):
    if hi-lo == 1: return (a[lo], -infinity)
    mid = (lo+hi)//2
    (mL,sL) = top2(lo,mid)
    (mR,sR) = top2(mid,hi)
    if mL >= mR: return (mL, max(sL,mR))
    else:        return (mR, max(mL,sR))
```
The result is `top2(0,n)`. The global maximum is one of the two child maxima. Once its side is identified, the global second maximum is either that side's runner-up or the other side's maximum; the displayed formula exhausts these possibilities. This proves the [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) by [induction](../../../../../mathematical-induction.md) on segment length. There are $n$ leaves and $n-1$ constant-cost combinations, so its [time complexity](../../../../../time-complexity.md) is **$\Theta(n)$**, with $O(\log n)$ recursive stack space for balanced splits. A `Maybe` value can replace the formal sentinel for a generic ordered element type. If both largest entries are equal, both are returned; a second _distinct_ value is a different specification.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
