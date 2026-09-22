<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Expanding and taking [partial derivatives](../../../../../../../partial-derivative.md) gives the [gradient](../../../../../../../gradient.md) and [Hessian matrix](../../../../../../../hessian-matrix.md)

$$
\nabla f=\begin{pmatrix}2x+2y^2+4x^3+4xy\\4xy+4y^3+2x^2+2y\end{pmatrix},
\qquad
H=\begin{pmatrix}2+12x^2+4y&4x+4y\\4x+4y&2+12y^2+4x\end{pmatrix}.
$$

At $p_0=(-1,0)^T$, these are $\nabla f(p_0)=(-6,2)^T$ and

$$
H(p_0)=\begin{pmatrix}14&-4\\-4&-2\end{pmatrix},\qquad \det H(p_0)=-44\ne0.
$$

Thus the [Newton step](../../../../../../../newton-step.md) solves

$$
\begin{pmatrix}14&-4\\-4&-2\end{pmatrix}
\begin{pmatrix}s_x\\s_y\end{pmatrix}
=\begin{pmatrix}6\\-2\end{pmatrix}.
$$

The second equation gives $s_y=1-2s_x$; substituting into the first gives $22s_x=10$. Hence

$$
s_x=\frac5{11},\qquad s_y=\frac1{11},\qquad
\boxed{(x_1,y_1)=\left(-\frac6{11},\frac1{11}\right).}
$$

At $p_*=(-1/2,-1/2)^T$, however,

$$
\nabla f(p_*)=0,\qquad
H(p_*)=\begin{pmatrix}3&-4\\-4&3\end{pmatrix}.
$$

The [eigenvalues](../../../../../../../eigenvalue.md) of this [Hessian matrix](../../../../../../../hessian-matrix.md) are $-1$ in direction $(1,1)$ and $7$ in direction $(1,-1)$. It is invertible but indefinite. Thus the [Newton step](../../../../../../../newton-step.md) is zero, and

$$
\boxed{(x_n,y_n)=\left(-\frac12,-\frac12\right)\quad\text{for every }n.}
$$

This illustrates that [stationary points are fixed points of Newton's method](../../../../../../../stationary-points-are-fixed-points-of-newton-s-method.md). Here the fixed point is a **[saddle point of a scalar function](../../../../../../../saddle-point-of-a-scalar-function.md)**, not a [local minimum](../../../../../../../local-minimum.md). Indeed, direct substitution along the two [eigenvector](../../../../../../../eigenvector.md) directions gives

$$
\begin{aligned}
f(-\tfrac12+t,-\tfrac12+t)&=\frac18-t^2+2t^4,\\
f(-\tfrac12+t,-\tfrac12-t)&=\frac18+7t^2+2t^4.
\end{aligned}
$$

For sufficiently small nonzero $t$, one direction decreases $f$ and the other increases it. The [global minimum](../../../../../../../global-minimum.md) is instead zero: the sum of squares vanishes at $(0,0)$ and $(-1,-1)$. These are the only real zeros, since $x=-y^2$ and $y=-x^2$ imply $y(y^3+1)=0$. Thus a zero [gradient](../../../../../../../gradient.md) is an insufficient stopping certificate for [minimization problem](../../../../../../../minimization-problem.md) without classifying the [stationary point](../../../../../../../stationary-point.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics IV resit](../../../../mathematics-iv-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
