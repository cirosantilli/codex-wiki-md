<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In a [Young-diagram hook](../../../../../../../hook-of-a-young-diagram.md), the cell $(i,j)$ has $\lambda_i-j$ cells to its right and $\lambda'_j-i$ below it. Summing the arm lengths row by row and the leg lengths column by column gives

$$
\sum_{(i,j)\in\lambda}h_{i,j}
=\sum_{(i,j)\in\lambda}\bigl((j-1)+(i-1)+1\bigr)
=\sum_{(i,j)\in\lambda}(i+j-1).
$$

Adding the content $c_{i,j}=j-i$ turns the summand on the right into $2j-1$. Since $\sum_{j=1}^m(2j-1)=m^2$, summing each row proves

$$
\sum_{(i,j)\in\lambda}(h_{i,j}+c_{i,j})
=\sum_i\lambda_i^2.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 160](../../../../paper-160-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
