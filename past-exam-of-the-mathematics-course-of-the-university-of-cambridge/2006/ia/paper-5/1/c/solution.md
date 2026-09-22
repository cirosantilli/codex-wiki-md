<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [merge sort](../../../../../../merge-sort.md) on a list of integers:
```
sml
fun sort xs = mergeSort (op <=) xs;
```
Here `mergeSort` denotes the standard [merge sort](../../../../../../merge-sort.md) implementation: split into two almost equal lists, recursively sort them, and combine them using the [merge algorithm](../../../../../../merge-algorithm.md). Splitting and merging take linear time, and each recursion level has total input length $n$. There are $\Theta(\log n)$ levels, so the worst-case [time complexity](../../../../../../time-complexity.md) is **$\Theta(n\log n)$**. Equivalently, $T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
