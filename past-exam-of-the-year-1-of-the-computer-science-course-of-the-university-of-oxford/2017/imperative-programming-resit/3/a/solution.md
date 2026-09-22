<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Track the length of the constant suffix of the scanned prefix:

```
best = 0; run = 0
for i = 0,...,n-1:
    if i == 0 or a[i] != a[i-1]: run = 1
    else: run = run+1
    if run > best: best = run
return best
```

The condition is evaluated with short-circuit logic, so `a[-1]` is never accessed. After processing index $i$, `run` is the longest [constant segment of an array](../../../../../constant-segment-of-an-array.md) ending there and `best` is the longest anywhere in $a[0:i+1)$. A maximal constant segment either extends the preceding suffix or starts at a changed value, proving the update. Empty input returns zero. Time is **$O(n)$**, with constant auxiliary storage.

## ↑ Ancestors (12)

1. [A](../a.md)
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
