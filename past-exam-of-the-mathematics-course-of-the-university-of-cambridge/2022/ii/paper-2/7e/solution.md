<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Choose paths from $0$ to $z$ in the cut plane and deform them continuously with the endpoint, never crossing the specified cut. With $0\leq\arg z<2\pi$, use the sheet reached from the positive real axis; when an endpoint is moved into the left half-plane, the path passes around the upper endpoint $i$ of the cut. The cut makes all such admissible paths homotopic with fixed endpoints, so the integral is single valued and its endpoint derivative is $(1+z^2)^{-1/2}$; hence it is [analytic](../../../../../holomorphic-function.md).

For $z=-\sinh u$, continue the endpoint counterclockwise from the positive real axis through the upper half-plane. In

$$
\operatorname{Arcsinh}z
=\log\!\left(z+\sqrt{1+z^2}\right),
$$

the continued square root equals $-\cosh u$ at $z=-\sinh u$. The logarithm is reached with argument $\pi$, and therefore

$$
\boxed{\operatorname{Arcsinh}(-\sinh u)=u+i\pi}.
$$

The identities

$$
\sinh(w+2\pi i)=\sinh w,\qquad
\sinh((2k+1)\pi i-w)=\sinh w
$$

show directly why continuation without an argument restriction is multivalued. The complete set of values of the [multivalued inverse hyperbolic sine](../../../../../multivalued-inverse-hyperbolic-sine.md) at $\sinh u$ is

$$
\boxed{u+2\pi ik\quad\hbox{and}\quad
-u+(2k+1)\pi i,\qquad k\in\mathbb Z}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
