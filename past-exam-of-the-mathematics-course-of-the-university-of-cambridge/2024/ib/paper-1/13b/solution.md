<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

Continuity at $x=\xi$ is automatic in the proposed expression. Integrating the differential equation through $x=\xi$ gives the [derivative](../../../../../derivative.md) jump

$$
G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=1.
$$

Thus

$$
c(\xi)\left[y_1(\xi)y_2'(\xi)-y_1'(\xi)y_2(\xi)\right]=1.
$$

In terms of the [Wronskian](../../../../../wronskian.md)

$$
W(x)=y_1(x)y_2'(x)-y_1'(x)y_2(x),
$$

one has

$$
\boxed{c(\xi)=\frac1{W(\xi)}}.
$$

The [boundary conditions](../../../../../boundary-condition.md) hold because $y_1'(0)=0$ and $y_2'(1)=0$.

The [Abel identity](../../../../../abel-s-identity.md) gives $W'=-\alpha W$. If $\alpha=0$, the Wronskian and hence $c$ are constant. The two branches of the displayed formula are then interchanged by $x\leftrightarrow\xi$, proving

$$
\boxed{G(x,\xi)=G(\xi,x)}.
$$

This is the symmetry of the [Neumann Green function for a second-order ordinary differential equation](../../../../../neumann-green-function-for-a-second-order-ordinary-differential-equation.md) in the self-adjoint case.

For $G''-G=\delta(x-\xi)$, choose

$$
y_1(x)=\cosh x,
\qquad
y_2(x)=\cosh(1-x).
$$

Their Wronskian is

$$
W=-\cosh x\sinh(1-x)-\sinh x\cosh(1-x)=-\sinh1.
$$

Writing $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$ gives

$$
\boxed{G(x,\xi)=-\frac{\cosh x_<\cosh(1-x_>)}{\sinh1}}.
$$

The solution of the inhomogeneous problem is $y(x)=\int_0^1G(x,\xi)\xi\,d\xi$. Equivalently, solving directly gives

$$
y(x)=A\cosh x+B\sinh x-x.
$$

The two Neumann conditions yield $B=1$ and

$$
A=\frac{1-\cosh1}{\sinh1}=-\tanh\frac12.
$$

Therefore

$$
\boxed{y(x)=\sinh x-\tanh\left(\frac12\right)\cosh x-x}.
$$

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
