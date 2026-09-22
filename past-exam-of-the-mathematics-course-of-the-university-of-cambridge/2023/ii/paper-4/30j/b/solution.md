<h1 id="30j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $X_1<\cdots<X_n$, it suffices to put the threshold between $X_m$ and $X_{m+1}$ for $m=1,\ldots,n-1$. Form the [prefix sums](../../../../../../prefix-sum.md)

$$
A_m=\sum_{i=1}^mY_i,
\qquad
B_m=\sum_{i=1}^mY_i^2.
$$

They take $O(n)$ operations to compute. The minimized squared errors for the two children are

$$
L_m=B_m-\frac{A_m^2}{m},
$$

and

$$
R_m=(B_n-B_m)-\frac{(A_n-A_m)^2}{n-m}.
$$

Each candidate value $L_m+R_m$ therefore takes constant time once the prefix sums are available. Scanning all $n-1$ candidates takes $O(n)$ operations in the sense of [Big O notation](../../../../../../big-o-notation.md), and retaining the minimizing $m$ gives the optimal split.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
