<h1 id="12/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $F$ is [continuously differentiable](../../../../../../continuously-differentiable-function.md) near the point of interest on $F=0$, and that the relevant denominators below are nonzero. The [total differential](../../../../../../total-differential.md) on the surface is

$$
dF=F_x\,dx+F_y\,dy+F_z\,dz=0.
$$

Holding $z$ fixed gives $F_x\,dx+F_y\,dy=0$, so the [implicit function theorem](../../../../../../implicit-function-theorem.md) gives

$$
\left(\frac{\partial y}{\partial x}\right)_z=-\frac{F_x}{F_y},\qquad
\left(\frac{\partial x}{\partial y}\right)_z=-\frac{F_y}{F_x}.
$$

When $F_xF_y\ne0$, their product proves the [reciprocity rule for constrained partial derivatives](../../../../../../reciprocity-rule-for-constrained-partial-derivatives.md):

$$
\boxed{\left(\frac{\partial y}{\partial x}\right)_z
\left(\frac{\partial x}{\partial y}\right)_z=1.}
$$

Similarly, holding $y$ or $x$ fixed gives $(\partial x/\partial z)_y=-F_z/F_x$ and $(\partial z/\partial y)_x=-F_y/F_z$. With $F_xF_yF_z\ne0$, multiply the three ratios:

$$
\boxed{\left(\frac{\partial y}{\partial x}\right)_z
\left(\frac{\partial x}{\partial z}\right)_y
\left(\frac{\partial z}{\partial y}\right)_x
=\left(-\frac{F_x}{F_y}\right)\left(-\frac{F_z}{F_x}\right)\left(-\frac{F_y}{F_z}\right)=-1.}
$$

This is the [cyclic partial derivative identity](../../../../../../cyclic-partial-derivative-identity.md). Nonzero denominators and local differentiable coordinate representations are substantive assumptions: at a singular coordinate representation, a formal cancellation of zero or infinite factors is not a valid proof.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
