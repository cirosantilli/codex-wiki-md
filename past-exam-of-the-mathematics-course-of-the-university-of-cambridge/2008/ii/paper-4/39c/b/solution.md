<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The given vectors satisfy

$$
y_{k+2}=2y_{k+1}-2y_k,
$$

and $y_k,y_{k+1}$ are [independent](../../../../../../independent-random-variables.md), so their span is invariant under $A$. On that plane the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $\lambda^2-2\lambda+2$. Therefore

$$
\boxed{\lambda_\pm=1\pm i,\qquad
v_\pm=y_{k+1}-(1\mp i)y_k=(1\pm i,2\pm i,3\pm i)^T.}
$$

Indeed $Av_\pm=y_{k+2}-(1\mp i)y_{k+1}=(1\pm i)v_\pm$. No third [eigenvalue](../../../../../../eigenvalue.md) is determined by these data.

The displayed $x_k=(1,1,1)$ has norm $\sqrt3$, although a large-$k$ normalized iterate should have norm one. This harmless source normalization is resolved by dividing all three displayed vectors by $\sqrt3$; the recurrence, [eigenvalues](../../../../../../eigenvalue.md) and [eigenvector](../../../../../../eigenvector.md) directions are unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
