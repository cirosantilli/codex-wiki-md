<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The loop divides each feature by its sample maximum, putting features with nonnegative values on comparable scales and improving numerical conditioning for gradient optimization. If exactly one hidden layer must use the [sigmoid function](../../../../../../sigmoid-function.md), use layer 3. Sigmoid derivatives can become small in saturated regions; placing it latest minimizes the number of subsequent gradient multiplications affected by this saturation, while the earlier ReLU layers retain efficient gradient propagation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
