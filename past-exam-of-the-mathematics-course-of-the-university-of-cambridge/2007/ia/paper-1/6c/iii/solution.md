<h1 id="6c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $P\mathbf x=(\mathbf n\cdot\mathbf x)\mathbf n$ be the axial [orthogonal projection](../../../../../../orthogonal-projection.md) and $N\mathbf x=\mathbf n\times\mathbf x$. Then $NP=PN=0$, while the [vector](../../../../../../vector.md) triple-product identity gives $N^2=P-I$. The map is $aP+a(I-P)+bN$. Its inverse is $P/a$ on the axis. On the perpendicular [plane](../../../../../../plane.md),

$$
(aI-bN)(aI+bN)=a^2I-b^2N^2=(a^2+b^2)I.
$$

Thus the [inverse of an axis-angle linear map](../../../../../../inverse-of-an-axis-angle-linear-map.md) is

$$
\mathbf x=\frac{P\mathbf x'}a+\frac{a(I-P)\mathbf x'-bN\mathbf x'}{a^2+b^2},
$$

or, in the requested [vector](../../../../../../vector.md) form,

$$
\boxed{\mathbf x=\frac{a\mathbf x'-b(\mathbf n\times\mathbf x')+(b^2/a)(\mathbf n\cdot\mathbf x')\mathbf n}{a^2+b^2}.}
$$

The denominators are nonzero because $a,b>0$. Multiplication on each invariant component verifies the [matrix inverse](../../../../../../matrix-inverse.md) without choosing a coordinate frame.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
