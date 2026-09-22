<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For two classes, write $m(x)=\min\{p_1(x),p_2(x)\}$, the conditional Bayes error. The nearest-neighbour label and the test label become conditionally independent draws from the same local class distribution, so the limiting conditional error of [one-nearest-neighbour classification](../../../../../../one-nearest-neighbour-classification.md) is

$$
2p_1(x)p_2(x)=2m(x)(1-m(x)).
$$

The assumption gives $c\leq m(x)\leq1/2-c$. Its excess over the conditional Bayes error is

$$
2m(1-m)-m=m(1-2m)\geq2c^2>0.
$$

After taking expectations, the limiting risk remains at least $2c^2$ above the Bayes risk, so one-nearest-neighbour classification is not consistent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
