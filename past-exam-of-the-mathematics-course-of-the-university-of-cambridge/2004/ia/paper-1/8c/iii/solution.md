<h1 id="8c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A direct construction, valid for every $0\leq t<1$, is

$$
\boxed{\begin{aligned}
a_1&=(1,0,0),\\
a_2&=(t,\sqrt{1-t^2},0),\\
a_3&=\left(t,\ t\sqrt{\frac{1-t}{1+t}},\
\sqrt{\frac{(1-t)(1+2t)}{1+t}}\right).
\end{aligned}}
$$

The first coordinates give $a_1\cdot a_2=a_1\cdot a_3=t$, and

$$
a_2\cdot a_3=t^2+t(1-t)=t.
$$

The first two norms are one. For the third,

$$
|a_3|^2=t^2+\frac{t^2(1-t)+(1-t)(1+2t)}{1+t}=1.
$$

Thus the required [Gram matrix](../../../../../../gram-matrix.md) is $(1-t)I+t\mathbf1\mathbf1^T$. The column [matrix](../../../../../../matrix.md) is upper triangular and has [determinant](../../../../../../determinant.md)

$$
\boxed{\det(a_1\ a_2\ a_3)=(1-t)\sqrt{1+2t}>0,}
$$

so these [vectors](../../../../../../vector.md) are [linearly independent](../../../../../../linear-independence.md). This is an explicit instance of [unit vectors with a common inner product](../../../../../../unit-vectors-with-a-common-inner-product.md); at $t=0$ it reduces to the standard [orthonormal basis](../../../../../../orthonormal-basis.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8C](../../8c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
