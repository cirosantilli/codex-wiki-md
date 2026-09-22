<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $r<1$ and construct $g_n$ from the boundary values of $u_n$ on the circle $|z|=r$ as in [ii](../ii.md). By the assumed [locally uniform convergence](../../../../../locally-uniform-convergence.md), those boundary values converge uniformly to $u$. For each $s<r$, the kernel is bounded on $|z|\leq s$, so the same integral shows that $g_n$ converges uniformly there to

$$
g(z)=\frac1{2\pi}\int_0^{2\pi}u(re^{i\theta})\frac{re^{i\theta}+z}{re^{i\theta}-z}\,d\theta.
$$

The [Weierstrass convergence theorem](../../../../../locally-uniform-convergence-of-holomorphic-functions.md) makes $g$ holomorphic. Since $\operatorname{Re}g_n=u_n$, passing to the limit gives $u=\operatorname{Re}g$ on $|z|<r$. The real part of a [holomorphic function](../../../../../holomorphic-function-split.md) is harmonic. As $r<1$ was arbitrary, **$u$ is harmonic throughout the unit disc**. This proves the [locally uniform limit of harmonic functions](../../../../../locally-uniform-limit-of-harmonic-functions.md) theorem without presuming convergence of the derivatives of $u_n$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../../split.md)
6. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
