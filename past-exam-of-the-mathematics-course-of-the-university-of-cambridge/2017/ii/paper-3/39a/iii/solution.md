<h1 id="39a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Two consecutive steps multiply by the [polynomial](../../../../../../polynomial-split.md) of the symmetric [matrix](../../../../../../matrix.md)

$$
 P(A)=(A-s_0I)(A-s_1I),\qquad P(\lambda)=\lambda^2-\lambda+\frac18
 =\frac18T_2(2\lambda-1).
$$

The [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) bound on $[0,1]$ gives $|P(\lambda)|\leq1/8$, and the actual endpoints $0,1$ attain it. At the dominant [eigenvalue](../../../../../../eigenvalue.md), $P(1+\epsilon)=1/8+\epsilon+\epsilon^2$. Thus

$$
\boxed{\rho^2=\frac1{1+8\epsilon+8\epsilon^2},\qquad
 \rho=1-4\epsilon+O(\epsilon^2).}
$$

For a small prescribed error $\delta$ relative to a fixed initial-component factor $C$, the number of [matrix](../../../../../../matrix.md)-[vector](../../../../../../vector.md) iterations is approximately $\log(C/\delta)/(-\log\rho)$. The three leading denominators are $\epsilon,2\epsilon,4\epsilon$. Therefore **the iteration counts are in the ratio $1:1/2:1/4$**: the single shift halves and the alternating double shift quarters the leading count. A pair of double-shift steps costs two [matrix](../../../../../../matrix.md)-[vector](../../../../../../vector.md) products, already accounted for by using $\rho$ per iteration rather than $\rho^2$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [39A](../../39a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
