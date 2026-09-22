<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

For

$$
L(x,y,y')=y'^2-y^2-2y\sin x,
$$

the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\frac d{dx}\frac{\partial L}{\partial y'}
-\frac{\partial L}{\partial y}=0.
$$

Here this becomes

$$
2y''+2y+2\sin x=0,
\qquad\text{or}\qquad
y''+y=-\sin x.
$$

Because the forcing is resonant with the complementary solution, a particular integral is $(x/2)\cos x$. Hence

$$
y=A\cos x+B\sin x+\frac x2\cos x,
$$

and

$$
y'=-A\sin x+B\cos x+\frac12\cos x-\frac x2\sin x.
$$

The [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) give

$$
y'(0)=B+\frac12=0,
\qquad
y'(\pi/2)=-A-\frac\pi4=0.
$$

Thus

$$
\boxed{
y(x)=-\frac\pi4\cos x-\frac12\sin x+\frac x2\cos x}.
$$

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
