<h1 id="analysis/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrate $e^{iz}/z$ around the upper half-disc with the upper half-disc of radius $\varepsilon$ about [zero](../../../../../zero-of-a-function.md) removed. The real segments run from $-R$ to $-\varepsilon$ and $\varepsilon$ to $R$; the small semicircle is clockwise. There are no poles inside this indented [contour](../../../../../complex-integration-contour.md).

The large arc contribution tends to [zero](../../../../../zero-of-a-function.md): its modulus is at most $\int_0^\pi e^{-R\sin\theta}\,d\theta$, which tends to [zero](../../../../../zero-of-a-function.md) by [dominated convergence](../../../../../dominated-convergence-theorem.md). On the small arc $z=\varepsilon e^{i\theta}$, $\theta$ decreases from $\pi$ to [zero](../../../../../zero-of-a-function.md), so its integral tends to $\int_\pi^0i\,d\theta=-i\pi$. The [contour](../../../../../complex-integration-contour.md) theorem consequently gives

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{e^{ix}}x\,dx=i\pi.
$$

Taking imaginary parts is legitimate for each truncated integral. The imaginary integrand $\sin x/x$ is continuous at [zero](../../../../../zero-of-a-function.md) after assigning its limiting value one, so the inner indentation can be removed. Therefore

$$
\boxed{\lim_{R\to\infty}\int_{-R}^{R}\frac{\sin x}{x}\,dx=\pi.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [Analysis](../../../analysis.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
