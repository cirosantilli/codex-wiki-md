<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Sort once by nondecreasing end time, then retain the most recent meeting:
```
Meetings(intervals):
    sort intervals by nondecreasing end
    result = []
    haveMeeting = false
    for (s,e) in intervals:
        if not haveMeeting or s > lastMeeting:
            lastMeeting = e
            append e to result
            haveMeeting = true
    return result
```
When an interval is inspected, $\texttt{lastMeeting}\leq e$ because of the sorted end order. Therefore the interval is already covered exactly when $s\leq\texttt{lastMeeting}$; otherwise it is the earliest-ending uncovered interval and the algorithm chooses its end. This proves that the scan implements greedy strategy 2. The strict test `s > lastMeeting` correctly treats equality as covered for [closed intervals](../../../../../closed-real-interval.md).

The [sorting](../../../../../sorting.md) costs $O(n\log n)$ comparisons, and the scan costs $O(n)$, with $O(k)$ space for the output and constant scan state. Including an empty input, the overall bound is **$O(n\log(n+1))$ time**, conventionally $O(n\log n)$ for $n\geq2$. Additional sorting space depends on the selected [sorting algorithm](../../../../../sorting-algorithm.md). Part (d) proves that the returned number of meetings is minimum.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
