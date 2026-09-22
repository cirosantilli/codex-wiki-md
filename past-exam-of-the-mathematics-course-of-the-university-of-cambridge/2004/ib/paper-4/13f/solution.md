<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

The [inverse function theorem](../../../../../inverse-function-theorem.md) says that a continuously differentiable map on an open subset of $\mathbb R^n$ whose derivative at a point is invertible has a continuously differentiable inverse between neighborhoods of that point and its image. The derivative of the inverse is the inverse derivative matrix.

For the given map the [Jacobian matrix](../../../../../jacobian-matrix.md) and its determinant are

$$
Df(x,y)=\begin{pmatrix}1&0\\3x^2-3y&3y^2-3x\end{pmatrix},\qquad \det Df=3(y^2-x).
$$

Hence every point of the nonempty open set

$$
\boxed{U=\{(x,y):x\ne y^2\}}
$$

has a local continuously differentiable inverse. At its image, the derivative of that inverse is

$$
\boxed{D(f^{-1})(f(x,y))=\begin{pmatrix}1&0\\-(x^2-y)/(y^2-x)&1/[3(y^2-x)]\end{pmatrix}.}
$$

At the omitted points a differentiable inverse with differentiable composition cannot exist, since the chain rule would force the singular derivative to be invertible.

To locate the exceptions on the curve, substitute $x=y^2$ into its defining relation. This gives $y^6-2y^3=y^3(y^3-2)=0$. The two exceptional points are therefore

$$
\boxed{(0,0),\quad (2^{2/3},2^{1/3}).}
$$

At any other point $(a,b)$ of the curve, $f(a,b)=(a,0)$ and the local inverse exists. Because the first coordinate of $f$ is $x$, its inverse at $(t,0)$ has the form $(t,h(t))$. The function $h$ is continuously differentiable for $t$ in a sufficiently small interval $I$ containing $a$. Shrink an interval $J$ containing $b$ so that $I\times J$ lies in the inverse neighborhood and $h(I)\subset J$. A point of the curve in that rectangle maps to $(t,0)$, so injectivity forces it to be $(t,h(t))$. Conversely all these inverse images belong to the curve. This proves the requested local graph description by the [inverse function theorem](../../../../../inverse-function-theorem.md), rather than merely asserting an implicit-function conclusion. Differentiating the relation also gives $h'(t)=-(t^2-h(t))/(h(t)^2-t)$ there.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
