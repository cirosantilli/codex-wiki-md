<h1 id="question-1/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Write the [centroid](../../../../../../../centroid.md) as $\overline{\mathbf r}=\overline x\,\mathbf i+\overline y\,\mathbf j$. The region has [reflection symmetry](../../../../../../../reflection-symmetry.md) in the $y$-axis: replacing $\theta$ by $\pi-\theta$ changes $x$ to $-x$ and preserves $y$ and $dA$. Thus [symmetry in integration](../../../../../../../symmetry-in-integration.md) gives

$$
\iint_Rx\,dA=0,\qquad\overline x=0.
$$

For the other [first moment of area](../../../../../../../first-moment-of-area.md), use $y=r\sin\theta$ in [polar coordinates](../../../../../../../polar-coordinates.md):

$$
\iint_Ry\,dA
=\int_0^\pi\int_0^{\sin^2\theta}r^2\sin\theta\,dr\,d\theta
=\frac13\int_0^\pi\sin^7\theta\,d\theta
=\frac{32}{105}.
$$

Here the last [integral](../../../../../../../integral-split.md) has the value allowed in the paper. Dividing the [first moment of area](../../../../../../../first-moment-of-area.md) by the [area](../../../../../../../surface-area.md) found in [i](../i.md) gives

$$
\boxed{(\overline x,\overline y)=\left(0,\frac{512}{315\pi}\right)},
\qquad
\boxed{\overline{\mathbf r}=\frac{512}{315\pi}\,\mathbf j}.
$$

The positive vertical coordinate agrees with the fact that the entire region lies above the $x$-axis.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [Question 1](../../../question-1.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
