<h1 id="13c/solution">Solution</h1>

↑ **Parent:** [13C](../13c.md)

For a variation $y+\varepsilon\eta$,

$$
\left.\frac d{d\varepsilon}I[y+\varepsilon\eta]\right|_{\varepsilon=0}
=\int_0^{x_0}\left(F_y\eta+F_{y'}\eta'\right)dx.
$$

Integration by parts gives

$$
\delta I=\left[F_{y'}\eta\right]_0^{x_0}
+\int_0^{x_0}\left(F_y-\frac d{dx}F_{y'}\right)\eta\,dx.
$$

For fixed endpoints, $\eta(0)=\eta(x_0)=0$. The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{\frac d{dx}F_{y'}-F_y=0}.
$$

A solution makes the first variation vanish for every admissible variation, so it is a stationary candidate; whether it is a minimum or maximum is decided by higher variations. If endpoint values are free, $\eta$ is arbitrary there, and the boundary term instead vanishes under the natural conditions

$$
\boxed{F_{y'}(0)=F_{y'}(x_0)=0}.
$$

Thus the same Euler-Lagrange solution is stationary for all free-endpoint variations. These are the [natural boundary conditions for a free endpoint](../../../../../natural-boundary-conditions-for-a-free-endpoint.md).

For

$$
F=y'^2+z'^2+2yz,
$$

the two equations are

$$
\boxed{y''=z,\qquad z''=y}.
$$

Set $u=y+z$ and $v=y-z$. Then

$$
u''=u,
\qquad
v''=-v.
$$

The conditions $y(0)=z(0)=0$ give

$$
u=A\sinh x,
\qquad
v=B\sin x,
$$

and hence the most general solution is

$$
\boxed{
y=\frac12(A\sinh x+B\sin x),
\qquad
z=\frac12(A\sinh x-B\sin x)}.
$$

Free conditions at $x_0$ are $y'(x_0)=z'(x_0)=0$. Adding and subtracting them gives

$$
A\cosh x_0=0,
\qquad
B\cos x_0=0.
$$

Thus $A=0$. The zero solution exists for every $x_0$, while nonzero solutions exist precisely when

$$
\boxed{x_0=\left(k+\frac12\right)\pi,
\qquad k=0,1,2,\ldots}.
$$

For those values they form the one-parameter family

$$
\boxed{y=C\sin x,
\qquad z=-C\sin x},
$$

where $C$ is arbitrary. This is the [free-endpoint normal mode of a coupled variational functional](../../../../../free-endpoint-normal-mode-of-a-coupled-variational-functional.md).

## ↑ Ancestors (10)

1. [13C](../13c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
