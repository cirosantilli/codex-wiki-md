<h1 id="17b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $p=0$ and $\lambda=1$, the [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation.md) is $y''''=y$, whose general solution is

$$
y=A\cos x+B\sin x+C\cosh x+D\sinh x.
$$

By the stated parity reduction, an [even](../../../../../../even-function.md) eigenfunction has the form $y=A\cos x+C\cosh x$. The conditions $y(c)=y'(c)=0$ have a nonzero solution exactly when

$$
\det\begin{pmatrix}
\cos c&\cosh c\\
-\sin c&\sinh c
\end{pmatrix}=0,
$$

that is,

$$
\cos c\sinh c+\sin c\cosh c=0.
$$

An [odd](../../../../../../odd-function.md) eigenfunction has the form $y=B\sin x+D\sinh x$, and the corresponding determinant gives

$$
\cos c\sinh c-\sin c\cosh c=0.
$$

Thus $\lambda=1$ is an eigenvalue precisely under one of the two stated conditions.

<a id="17b/c/image-the-fourth-order-eigenvalue-condition-and-its-roots"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4-fourth-order-eigenvalue-condition.png)

**[Figure 1](#17b/c/image-the-fourth-order-eigenvalue-condition-and-its-roots). The fourth-order eigenvalue condition and its roots**.

For the minus sign, division by $\cos c\cosh c$ away from $c=\pi/2$ gives $\tan c=\tanh c$. On $(0,\pi/2)$, $\tan c>\tanh c$ for $c>0$, while on $(\pi/2,\pi)$ their signs differ, so there is no root. For the plus sign the equation is

$$
\tan c=-\tanh c.
$$

There is no root in $(0,\pi/2)$. On $(\pi/2,\pi)$, the function $\tan c+\tanh c$ increases strictly from $-\infty$ to $\tanh\pi>0$, so it has exactly one root by the [intermediate value theorem](../../../../../../intermediate-value-theorem.md). Numerically,

$$
\boxed{c\approx2.365020372}.
$$

**Hence the combined $\pm$ condition has exactly one solution in $0<c<\pi$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
