<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Uniform knots give translation invariance $N_{i,k}(x)=N_{0,k}(x-i)$. Put $v_{k,j}=N_{0,k}(j)$ and set missing values to zero. The recurrence in part (a) gives the exact numerical recursion

$$
\boxed{v_{k,j}=\frac{jv_{k-1,j}+(k-j)v_{k-1,j-1}}{k-1}.}
$$

The order-two starting row is $(0,1,0)$. For example, the order-four middle value is $(2\cdot\frac12+2\cdot\frac12)/3=2/3$, and the order-six central value is $(3\cdot\frac{11}{24}+3\cdot\frac{11}{24})/5=66/120$. Iteration gives the requested array, listing $N_{0,k}(0),\ldots,N_{0,k}(k)$:

$$
\boxed{\begin{array}{c|rrrrrrr}
2&0&1&0&&&&\\
3&0&\frac12&\frac12&0&&&\\
4&0&\frac16&\frac46&\frac16&0&&\\
5&0&\frac1{24}&\frac{11}{24}&\frac{11}{24}&\frac1{24}&0&\\
6&0&\frac1{120}&\frac{26}{120}&\frac{66}{120}&\frac{26}{120}&\frac1{120}&0
\end{array}}
$$

The symmetry follows from reflection of the uniform [Cardinal B-spline](../../../../../../cardinal-b-spline.md) about the midpoint of its support. The row sums equal one, consistent with sampling the uniform partition of unity. These are partition-normalized values; normalizing each spline to have peak one would produce a different array.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
