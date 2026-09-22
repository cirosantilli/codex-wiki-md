<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At $a=\pi$, the nonzero [homogeneous solution](../../../../../homogeneous-solution.md) $e^{-x}\sin x$ satisfies both zero [boundary conditions](../../../../../boundary-condition.md). Thus the [boundary value problem](../../../../../boundary-value-problem-split.md) has a nontrivial [kernel](../../../../../kernel-of-a-linear-map-split.md) and cannot have an inverse for arbitrary forcing.

More directly, the [adjoint operator](../../../../../adjoint-operator.md) has the zero-endpoint [homogeneous solution](../../../../../homogeneous-solution.md) $w(x)=e^x\sin x$. If an ordinary [Green's function](../../../../../green-s-function-split.md) existed, the [integration by parts](../../../../../integration-by-parts.md) identity would imply

$$
0=\int_0^\pi w(x)\mathcal L_xg(x,\xi)\,dx
=\int_0^\pi w(x)\delta(x-\xi)\,dx=w(\xi).
$$

But $w(\xi)\ne0$ for $0<\xi<\pi$. This contradiction rules out the [Green's function](../../../../../green-s-function-split.md) for the unmodified operator. It is the [Fredholm alternative](../../../../../fredholm-alternative.md) obstruction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
