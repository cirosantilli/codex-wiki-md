<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a quadratic uniform [B-spline](../../../../../b-spline.md) segment on a unit [spline knot](../../../../../spline-knot.md) interval. This choice is useful because adjacent pieces can later share [de Boor points](../../../../../de-boor-point.md) at simple, equally spaced [spline knots](../../../../../spline-knot.md). Its three active basis pieces on local $t\in[0,1]$ are

$$
b_0(t)=\frac{(1-t)^2}{2},\qquad
b_1(t)=\frac{1+2t-2t^2}{2},\qquad
b_2(t)=\frac{t^2}{2}.
$$

They follow from the [Cox-de Boor recurrence](../../../../../cox-de-boor-recursion-formula.md) for degree two and consecutive integer [spline knots](../../../../../spline-knot.md). If the three [de Boor points](../../../../../de-boor-point.md) are $D_0,D_1,D_2$, then the equivalent [Bézier curve](../../../../../bezier-curve.md) handles are

$$
A=\frac{D_0+D_1}{2},\qquad B=D_1,\qquad
C=\frac{D_1+D_2}{2}.
$$

One can verify this conversion simply by substituting these expressions into the [Bernstein basis](../../../../../bernstein-basis.md) formula and collecting each $D_i$. Solving gives

$$
\boxed{D_0=2A-B=(-4,-1),\qquad D_1=B=(0,1),\qquad D_2=2C-B=(0,-1).}
$$

The desired [matrix](../../../../../matrix.md) representation is therefore

$$
\boxed{F(t)=\frac12[t^2\ t\ 1]
\begin{pmatrix}1&-2&1\\-2&2&0\\1&1&0\end{pmatrix}
\begin{pmatrix}-4&-1\\0&1\\0&-1\end{pmatrix}.}
$$

The left row is again the monomial row, the middle [matrix](../../../../../matrix.md) contains the monomial [coefficients](../../../../../coefficient.md) of $b_0,b_1,b_2$, and the right [matrix](../../../../../matrix.md) lists the [de Boor points](../../../../../de-boor-point.md). Unlike the [Bézier curve](../../../../../bezier-curve.md) basis [matrix](../../../../../matrix.md), the constant row averages two handles. A clamped [B-spline](../../../../../b-spline.md) with repeated end [spline knots](../../../../../spline-knot.md) could instead reuse $A,B,C$ directly; the simple uniform convention above specifies which representation is being used and supplies the shared handles required for the extension.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
