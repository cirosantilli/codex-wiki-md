<h1 id="24h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Regard the space of real $n\times n$ [matrices](../../../../../../matrix.md) as $\mathbb R^{n^2}$, and use the smooth [determinant](../../../../../../determinant.md) map. For invertible $A$, factor $A+tH=A(I+tA^{-1}H)$. Expanding the [determinant](../../../../../../determinant.md) to first order gives

$$
d(\det)_A(H)=\det(A)\operatorname{tr}(A^{-1}H),
$$

since the linear coefficient of $\det(I+tK)$ is the sum of the diagonal entries of $K$. At every $A$ with [determinant](../../../../../../determinant.md) one, taking $H=A$ makes this [derivative](../../../../../../derivative.md) $n\ne0$. Thus one is a [regular value](../../../../../../regular-value.md), and part (ii) makes $\operatorname{SL}(n,\mathbb R)$ a [submanifold](../../../../../../submanifold.md) of [dimension](../../../../../../dimension-vector-space.md) $n^2-1$.

Its [tangent space](../../../../../../tangent-space.md) is the kernel of this [differential](../../../../../../differential-of-a-smooth-map.md). At the identity,

$$
\boxed{T_I\operatorname{SL}(n,\mathbb R)=\{H:\operatorname{tr}H=0\}=\mathfrak{sl}(n,\mathbb R).}
$$

Indeed tangent [derivatives](../../../../../../derivative.md) of curves with constant [determinant](../../../../../../determinant.md) lie in that kernel, and the local regular-value coordinates show every kernel [vector](../../../../../../vector.md) is tangent to the level set.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [24H](../../24h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
