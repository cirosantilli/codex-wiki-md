<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

All $n$ [singular values](../../../../../singular-value.md) are positive, so $\Sigma$ and $V$ are [invertible matrices](../../../../../invertible-matrix.md) and $A$ has [matrix rank](../../../../../matrix-rank.md) $n$. The [image of a linear map](../../../../../image-of-a-linear-map.md) is therefore

$$
\boxed{\operatorname{range}(A)=\operatorname{span}\{u_1,\ldots,u_n\},}
$$

with those columns furnishing an [orthonormal basis](../../../../../orthonormal-basis.md). Also $Ax=0$ implies $\Sigma V^Tx=0$ and hence $x=0$. Thus

$$
\boxed{\ker A=\{0\},\qquad\text{its basis is the empty set}.}
$$

Finally $A^Tz=V\Sigma U^Tz=0$ exactly when $U^Tz=0$. The remaining columns of the full [orthogonal matrix](../../../../../orthogonal-matrix.md) span this [orthogonal complement](../../../../../orthogonal-complement.md):

$$
\boxed{\ker A^T=\operatorname{range}(U_\perp),\qquad
\text{a basis consists of the }m-n\text{ columns of }U_\perp.}
$$

If $m=n$, this last [null space](../../../../../kernel-of-a-linear-map-split.md) also equals $\{0\}$ and has the empty basis.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
