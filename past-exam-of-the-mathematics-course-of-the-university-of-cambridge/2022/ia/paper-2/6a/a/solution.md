<h1 id="6a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The multivariable [chain rule](../../../../../../chain-rule.md) gives, at $(x,y)=(a+t\cos\gamma,b+t\sin\gamma)$,

$$
g'(t)=f_x\cos\gamma+f_y\sin\gamma,
$$



$$
g''(t)=f_{xx}\cos^2\gamma
+2f_{xy}\sin\gamma\cos\gamma
+f_{yy}\sin^2\gamma.
$$

Sufficient conditions for a strict local minimum at $t=0$ are $g'(0)=0$ and $g''(0)>0$.

At a [stationary point](../../../../../../stationary-point.md), $g'(0)=0$ in every direction. Its second derivative is the quadratic form of the [Hessian matrix](../../../../../../hessian-matrix.md). If

$$
f_{yy}>0,\qquad f_{xx}f_{yy}-f_{xy}^2>0,
$$

then completing the square gives

$$
f_{xx}u^2+2f_{xy}uv+f_{yy}v^2
=f_{yy}\left(v+\frac{f_{xy}}{f_{yy}}u\right)^2
+\frac{f_{xx}f_{yy}-f_{xy}^2}{f_{yy}}u^2>0
$$

for every nonzero direction $(u,v)$. The Hessian is therefore [positive definite](../../../../../../positive-definite-matrix.md), and the stationary point is a strict local minimum.

## ↑ Ancestors (11)

1. [A](../a.md)
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
