<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $z=x+iy$, $r=|z|$, and $L=(4\pi)^{-1}\log(x^2+y^2)$. The [Wirtinger derivatives](../../../../../wirtinger-derivatives.md) satisfy $4\partial_{\bar z}\partial_z=\Delta$. Away from zero, ordinary differentiation gives

$$
4\partial_z L=2(\partial_x-i\partial_y)L
=\frac{x-iy}{\pi(x^2+y^2)}=\frac1{\pi z}.
$$

This equality also holds for [distributional derivatives](../../../../../distributional-derivative.md). To check that no [Dirac delta distribution](../../../../../dirac-delta-function.md) was lost at zero, integrate by parts outside the disk $r\leq\varepsilon$ against a [test function](../../../../../test-function.md). The new [boundary term](../../../../../boundary-term.md) has absolute value at most $C\varepsilon|\log\varepsilon|\|\phi\|_\infty\to0$. Both $L$ and its displayed first [derivatives](../../../../../derivative.md), of size $O(r^{-1})$, are [locally integrable functions](../../../../../locally-integrable-function.md) in two dimensions, so the remaining integrals converge to their full-plane values.

Using the supplied [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md) identity $\Delta L=\delta_0$, and commutation of [distributional derivatives](../../../../../distributional-derivative.md), now gives

$$
\boxed{E=4\partial_zL=\frac1{\pi z},\qquad
\partial_{\bar z}E=4\partial_{\bar z}\partial_zL=\Delta L=\delta_0.}
$$

Thus the [Cauchy kernel fundamental solution](../../../../../cauchy-kernel-fundamental-solution.md) has exactly the required normalization.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
