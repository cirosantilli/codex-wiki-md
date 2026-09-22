<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

A [function](../../../../../function-split.md) $f:D\to\mathbb R$ on a [convex set](../../../../../convex-set.md) $D$ is [convex](../../../../../convex-function.md) when

$$
f((1-t)x+ty)
\leq(1-t)f(x)+tf(y)
$$

for all $x,y\in D$ and $0\leq t\leq1$.

If $f$ is once [differentiable](../../../../../differentiable-function.md), this is equivalent to monotonicity of its [gradient](../../../../../gradient.md):

$$
\boxed{
(\nabla f(x)-\nabla f(y))\cdot(x-y)\geq0
}.
$$

Equivalently, every tangent hyperplane supports the graph:

$$
f(y)\geq f(x)+\nabla f(x)\cdot(y-x).
$$

If $f$ is twice [differentiable](../../../../../differentiable-function.md), convexity is equivalent to the [Hessian matrix](../../../../../hessian-matrix.md) being positive semidefinite throughout $D$.

For

$$
f(x,y)=x^3+y^3+Axy,
$$

the Hessian is

$$
H=
\begin{pmatrix}6x&A\\A&6y\end{pmatrix}.
$$

A real symmetric two-by-two [matrix](../../../../../matrix.md) is positive semidefinite exactly when its two diagonal entries and its [determinant](../../../../../determinant.md) are nonnegative. Thus

$$
x\geq0,\qquad y\geq0,\qquad 36xy-A^2\geq0.
$$

The largest convexity domain is therefore

$$
\boxed{
D_A=\{(x,y):x\geq0,\ y\geq0,\ 36xy\geq A^2\}
}.
$$

For $A\ne0$, its boundary is the hyperbola $y=A^2/(36x)$ in the first quadrant and the domain lies above it. For $A=0$, it is the closed first quadrant. This is the [convexity domain of x cubed plus y cubed plus Axy](../../../../../convexity-domain-of-x-cubed-plus-y-cubed-plus-axy.md).

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
