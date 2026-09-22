<h1 id="6a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $Ax=b$ and $h\in\ker A$, symmetry gives $b\cdot h=(Ax)\cdot h=x\cdot Ah=0$, proving necessity. Conversely, expand $b$ in the [orthonormal basis](../../../../../../orthonormal-basis.md) from part (i), with $Ay_i=\lambda_i y_i$. The zero-[eigenvalue](../../../../../../eigenvalue.md) vectors span the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md). If $b$ is [orthogonal](../../../../../../orthogonal-vectors.md) to that kernel, then $b\cdot y_i=0$ whenever $\lambda_i=0$, so the remaining coordinates can be solved independently.

For a nonzero [eigenvalue](../../../../../../eigenvalue.md) and any associated nonzero [eigenvector](../../../../../../eigenvector.md) $v$, symmetry gives $b\cdot v=\lambda x\cdot v$. Thus **the component vector along $v$ is**

$$
\boxed{\operatorname{proj}_v x=\frac{b\cdot v}{\lambda\|v\|^2}v.}
$$

For the unit vectors $y_i$, this coefficient is $(b\cdot y_i)/\lambda_i$. Consequently **the general solution is**

$$
\boxed{x=\sum_{\lambda_i\ne0}\frac{b\cdot y_i}{\lambda_i}y_i
+\sum_{\lambda_i=0}c_i y_i,\qquad c_i\in\mathbb R.}
$$

This proves sufficiency as well as the claimed kernel criterion. If the compatibility condition fails, there is no solution; if it holds, the freedom is exactly an arbitrary kernel vector.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6A](../../6a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
