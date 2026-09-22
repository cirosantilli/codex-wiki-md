<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The answer is $\Theta(n^2)$.** Partition all but at most one point into $m=\lfloor n/2\rfloor$ disjoint pairs and take all unions of two pairs. There are $\binom m2=\Theta(n^2)$ such four-sets, and two distinct unions intersect in zero or two points. The [Ray-Chaudhuri–Wilson theorem](../../../../../../ray-chaudhuri-wilson-theorem.md) gives the upper bound $O(n^2)$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
