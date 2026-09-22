<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the implementations above, the output is
```
0
1
```
In `A`, the [Scala trait linearization](../../../../../scala-trait-linearization.md) sends `insert('a',0)` first to `CapitalisePlugIn`, then to `CharTrackPlugIn`, then to `DocImpl`. The counter [trait](../../../../../trait.md) receives `'A'`, so it does not increment the lowercase `'a'` count. The stored document is `A`.

In `B`, the counter [trait](../../../../../trait.md) receives `'a'`, delegates through `CapitalisePlugIn`, and increments its original argument's counter on return. The stored document is again `A`, but the counter records one lowercase insertion:

$$
\boxed{\mathrm{d1.getCount('a')}=0,\qquad\mathrm{d2.getCount('a')}=1.}
$$

This demonstrates a composition that violates the count-of-current-document [representation invariant](../../../../../representation-invariant.md) for `B`: an earlier counter cannot assume a later transforming [trait](../../../../../trait.md) inserts its argument unchanged. Subsequent deletion also receives uppercase `'A'` and would leave that stale lowercase count. A different valid design could inspect `read(pos)` after insertion to count the actual stored character; that design would produce `0,0`. The stated `0,1` follows the explicit implementation in part (b), whose correctness assumption has now failed in the second composition.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
