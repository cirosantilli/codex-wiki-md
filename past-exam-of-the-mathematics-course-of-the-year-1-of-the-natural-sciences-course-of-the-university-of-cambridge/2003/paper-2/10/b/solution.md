<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $c=\cos\theta$, $s=\sin\theta$. Since $\theta$ is constant, the [multivariable chain rule](../../../../../multivariable-chain-rule.md) gives $\partial_x=c\partial_u-s\partial_v$ and $\partial_y=s\partial_u+c\partial_v$. Applying these operators twice to a twice continuously differentiable [function](../../../../../function-split.md) gives

$$
g_{xx}=c^2g_{uu}-2csg_{uv}+s^2g_{vv},\qquad g_{yy}=s^2g_{uu}+2csg_{uv}+c^2g_{vv}.
$$

The mixed terms cancel and $c^2+s^2=1$, so

$$
\boxed{g_{xx}+g_{yy}=g_{uu}+g_{vv}.}
$$

This is [rotational invariance of the Laplacian](../../../../../rotational-invariance-of-the-laplacian.md): an [orthogonal change of coordinates](../../../../../orthogonal-change-of-coordinates.md) preserves the [trace](../../../../../matrix-trace.md) of the [Hessian matrix](../../../../../hessian-matrix.md). A nonconstant angle would introduce additional [derivatives](../../../../../derivative.md) and is not covered by this constant rotation calculation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
