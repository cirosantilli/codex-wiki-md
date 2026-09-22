<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The nonzero endpoint data contribute to the [Fredholm alternative](../../../../../fredholm-alternative.md) condition. With $w=e^x\sin x$, the same [integration by parts](../../../../../integration-by-parts.md) identity gives

$$
\int_0^\pi w\mathcal Ly\,dx
=[wy'-w'y+2wy]_0^\pi
=-w'(\pi)y(\pi)+w'(0)y(0)=1.
$$

For the specified forcing the left side is $A\int_0^\pi\sin^2x\,dx=A\pi/2$. Hence

$$
\boxed{A=\frac2\pi}.
$$

To verify sufficiency, set $y=e^{-x}u$. Direct [differentiation](../../../../../differentiation.md) gives $\mathcal Ly=e^{-x}(u''+u)$. At this value of $A$, a [particular solution](../../../../../particular-solution.md) of $u''+u=(2/\pi)\sin x$ is $-(x/\pi)\cos x$. The complete family obeying the two [boundary conditions](../../../../../boundary-condition.md) is

$$
\boxed{y(x)=e^{-x}\left[\left(1-\frac{x}{\pi}\right)\cos x+C\sin x\right],\qquad C\in\mathbb R}.
$$

The arbitrary constant records the one-dimensional [kernel](../../../../../kernel-of-a-linear-map-split.md); existence does not imply uniqueness here.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
