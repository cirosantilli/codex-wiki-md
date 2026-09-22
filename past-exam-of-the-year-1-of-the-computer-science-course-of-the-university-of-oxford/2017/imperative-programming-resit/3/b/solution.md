<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Add `bestStart = 0` initially and, whenever a strictly longer run is found, record

```
best = run
bestStart = i-run+1
```

Then $a[\mathrm{bestStart}:\mathrm{bestStart}+\mathrm{best})$ is a plateau of the returned maximum length. Keeping the old answer on equal lengths selects the earliest maximum. The [loop invariant](../../../../../loop-invariant.md) from part (a) gains the assertion that the recorded interval realizes `best`; time and auxiliary-space bounds are unchanged. For empty input use the empty interval at zero.

## ↑ Ancestors (12)

1. [B](../b.md)
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
