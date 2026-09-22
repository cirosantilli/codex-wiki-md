<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Increasing here means nondecreasing, so equal neighbors remain in the same run. Change only the suffix-reset test:

```
best = 0; run = 0; bestStart = 0
for i = 0,...,n-1:
    if i == 0 or a[i] < a[i-1]: run = 1
    else: run = run+1
    if run > best:
        best = run; bestStart = i-run+1
return (bestStart,best)
```

After index $i$, `run` is the longest nondecreasing suffix of the prefix and the recorded interval is a longest nondecreasing segment seen so far. The adjacent-comparison condition implies the all-pairs condition by transitivity. The scan uses **$O(n)$ time and $O(1)$ auxiliary space**. Empty input yields length zero because no nonempty increasing segment exists.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
