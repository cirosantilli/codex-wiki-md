<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A fixed [array](../../../../../../array-data-structure.md) containing the distinct seen [integers](../../../../../../integer-split.md) needs capacity at most $N$, because at most one new distinct value is introduced per result entry. Its auxiliary space is therefore **$O(N)$**, rather than the bitmap's $O(M)$ universe storage. A size field identifies the occupied prefix; insertion first checks membership, and appends only when absent.

An unsorted occupied prefix needs linear membership scans, giving **$O(N^2)$ total work** by the same summation as in the original version. Keeping it sorted permits [binary search](../../../../../../binary-search.md) membership in $O(\log N)$, but inserting a new value can shift $O(N)$ entries, so the overall worst-case upper bound remains quadratic. Unlike a bitmap, the space cost depends on the number of stored values rather than their largest possible numerical magnitude. Compared with part (a)(ii), this extra set [array](../../../../../../array-data-structure.md) also duplicates information already present in the output prefix; its principal benefit is a separate set interface, not an automatic asymptotic speedup.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
