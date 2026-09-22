<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p_t(z)=(2\pi t)^{-1/2}e^{-z^2/(2t)}$ be the [heat kernel](../../../../../../heat-kernel.md) for $u_t=\frac12u_{xx}$. The symmetry of the [Gaussian distribution](../../../../../../normal-distribution.md) gives the method-of-images formula

$$
v(t,x)=\int_0^\infty f(y)\bigl(p_t(x-y)+p_t(x+y)\bigr)dy.
$$

This is the [Neumann heat kernel on a half-line](../../../../../../neumann-heat-kernel-on-a-half-line.md). [Differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) shows that $v\in C^{1,2}$ for $t,x>0$ and that $v_t=\frac12v_{xx}$. At $x=0$, the two differentiated kernel terms cancel, so $v_x(t,0)=0$. The [Gaussian approximate identity](../../../../../../gaussian-approximate-identity.md) gives $v(t,x)\to f(x)$ as $t\downarrow0$, while the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives continuity up to $x=0$. Finally $|v(t,x)|\leq\lVert f\rVert_\infty$, which is stronger than the required exponential bound. Thus $v$ satisfies every condition in the displayed boundary-value problem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
