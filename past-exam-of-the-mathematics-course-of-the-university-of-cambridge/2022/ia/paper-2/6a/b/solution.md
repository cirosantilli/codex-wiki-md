<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stationary equations are

$$
4x^3-6x+2y=0,\qquad 2x+2y=0.
$$

Thus $y=-x$ and $4x(x^2-2)=0$, giving

$$
(0,0),\qquad(\sqrt2,-\sqrt2),\qquad(-\sqrt2,\sqrt2).
$$

The [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
H=\begin{pmatrix}12x^2-6&2\\2&2\end{pmatrix}.
$$

At either nonzero stationary point,

$$
H=\begin{pmatrix}18&2\\2&2\end{pmatrix},
\qquad \det H=32>0,
$$

so both are strict local minima.

Along a line through the origin,

$$
g(t)=f(t\cos\gamma,t\sin\gamma)
=t^2q(\gamma)+t^4\cos^4\gamma,
$$

where

$$
q(\gamma)=-3\cos^2\gamma
+2\sin\gamma\cos\gamma+\sin^2\gamma.
$$

When $\cos\gamma\ne0$ and $r=\tan\gamma$,

$$
q(\gamma)=\cos^2\gamma(r-1)(r+3).
$$

Consequently the origin is a local minimum along the line when

$$
\boxed{\tan\gamma\leq-3\quad\text{or}\quad\tan\gamma\geq1},
$$

including the equality cases because the positive quartic term then leads. It is also a minimum on the vertical line. It is a local maximum along the line when

$$
\boxed{-3<\tan\gamma<1}.
$$

In the first case the graph is locally bowl-shaped. In the second it initially bends downward from the origin, but the positive quartic term eventually turns it upward, producing the usual double-well profile.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
