<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The coordinate [tangent vectors](../../../../../tangent-vector-split.md) are the partial [derivatives](../../../../../derivative.md) of the position [vector](../../../../../vector.md):

$$
\boxed{\begin{aligned}
\mathbf h_r&=(\sin\alpha\cos\beta,\sin\alpha\sin\beta,\cos\alpha),\\
\mathbf h_\alpha&=(r\cos\alpha\cos\beta,r\cos\alpha\sin\beta,-r\sin\alpha),\\
\mathbf h_\beta&=(-(1+r\sin\alpha)\sin\beta,(1+r\sin\alpha)\cos\beta,0).
\end{aligned}}
$$

Their pairwise [dot products](../../../../../dot-product.md) vanish. Their lengths, the [scale factors of orthogonal coordinates](../../../../../scale-factors-of-orthogonal-coordinates.md), are $1,r,1+r\sin\alpha$. Since $R<1$, the last is positive throughout the body. Thus these [circular torus coordinates](../../../../../circular-torus-coordinates.md) are **orthogonal wherever $r>0$**; at $r=0$ the cross-section angle degenerates, as in ordinary [polar coordinates](../../../../../polar-coordinates.md).

The ordered [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\boxed{J=\det\frac{\partial(x,y,z)}{\partial(r,\alpha,\beta)}=\mathbf h_r\cdot(\mathbf h_\alpha\times\mathbf h_\beta)=r(1+r\sin\alpha).}
$$

Its sign is positive for $r>0$, so the [volume](../../../../../volume.md) element is $dV=r(1+r\sin\alpha)\,dr\,d\alpha\,d\beta$. The coordinate degeneracy on the central [circle](../../../../../circle.md) has zero [volume](../../../../../volume.md) and does not obstruct [volume](../../../../../volume.md) [integration](../../../../../integral-split.md).

<a id="1/a/image-circular-torus-coordinates-and-their-orthogonal-tangent-directions"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1-q1-torus-coordinates.png)

**[Figure 1](#1/a/image-circular-torus-coordinates-and-their-orthogonal-tangent-directions). Circular torus coordinates and their orthogonal tangent directions**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
