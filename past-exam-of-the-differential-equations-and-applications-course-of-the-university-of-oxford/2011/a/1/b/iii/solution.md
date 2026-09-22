<h1 id="a/1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under $y=e^{-2x}v$, the left [Robin boundary condition](../../../../../../robin-boundary-condition.md) becomes $v'(0)-v(0)=0$ and the right [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) becomes $v(1)=0$. Choose

$$
v_L(x)=\cos(\pi x)+\frac1\pi\sin(\pi x),\qquad v_R(x)=\sin(\pi x).
$$

Their [Wronskian](../../../../../../wronskian.md) $v_Lv_R'-v_L'v_R$ is the constant $\pi$. For $y_L=e^{-2x}v_L$ and $y_R=e^{-2x}v_R$, it is $W_y(x)=\pi e^{-4x}$. The coefficient enforcing the derivative jump four is $4/W_y(\xi)$. Writing $x_< =\min(x,\xi)$ and $x_>=\max(x,\xi)$, the [Green's function](../../../../../../green-s-function-split.md) is

$$
\boxed{g(x,\xi)=\frac4\pi e^{2\xi-2x}\left[\cos(\pi x_<)+\frac1\pi\sin(\pi x_<)\right]\sin(\pi x_>).}
$$

The endpoint conditions, continuity and derivative jump follow directly from this [Wronskian](../../../../../../wronskian.md) construction. Its exponential factor also shows why the kernel need not be symmetric in the unweighted inner product.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
