<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $p=a+bx$. [orthogonality](../../../../../orthogonal-vectors.md) of the residual to $1,x$ gives

$$
\frac a2+\frac b3=\int_0^1x\sqrt{1-x^2}dx=\frac13,
$$



$$
\frac a3+\frac b4=\int_0^1x^2\sqrt{1-x^2}dx=\frac\pi{16}.
$$

The first integral follows from $t=1-x^2$; for the second use $x=\sin\theta$, giving $\int_0^{\pi/2}\sin^2\theta\cos^2\theta\,d\theta=\pi/16$. The coefficient [matrix](../../../../../matrix.md) has determinant $1/72$, so solving yields

$$
\boxed{p(x)=6-\frac{3\pi}{2}
+\left(\frac{9\pi}{4}-8\right)x.}
$$

Part (a) proves this is the unique best weighted $L^2$ approximation. The weight $x$ is essential; using ordinary unweighted [normal equations](../../../../../normal-equation.md) would give different coefficients.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
