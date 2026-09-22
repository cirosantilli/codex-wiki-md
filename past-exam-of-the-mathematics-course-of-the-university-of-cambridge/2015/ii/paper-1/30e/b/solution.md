<h1 id="30e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose

$$
\boxed{u_n(x,y)=\frac1n\cos(nx)\cosh(ny),\qquad
v_n(x,y)=-\frac1n\sin(nx)\sinh(ny)}.
$$

Direct differentiation gives $u_{ny}=v_{nx}$ and $v_{ny}=-u_{nx}$. Both functions are smooth and $2\pi$-periodic in $x$, with initial data $f_n(x)=n^{-1}\cos nx$, $v_n(x,0)=0$. Their squared norms are

$$
\int_0^{2\pi}|f_n|^2dx=\frac\pi{n^2}\to0,\qquad
\int_0^{2\pi}|u_n(x,y)|^2dx=\frac\pi{n^2}\cosh^2(ny)\to\infty
$$

for every fixed $y\ne0$. Thus **continuous dependence on the initial data fails in this $L^2$ topology**, even on smooth analytic data. The [Cauchy problem for a partial differential equation](../../../../../../cauchy-problem.md) is ill-posed in the sense of [Hadamard well-posedness](../../../../../../well-posed-problem.md); existence of analytic solutions from the preceding theorem does not supply stability for an elliptic Cauchy problem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30E](../../30e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
