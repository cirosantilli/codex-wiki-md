<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [linear differential operator](../../../../linear-differential-operator.md) $L=D^2+4D+5$, the [characteristic equation](../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $m^2+4m+5=0$, with roots $-2\pm i$. Take the [fundamental system of solutions](../../../../fundamental-system-of-solutions.md)

$$
u(x)=e^{-2x}\cos x,\qquad v(x)=e^{-2x}\sin x,\qquad W(x)=uv'-u'v=e^{-4x}.
$$

The [Wronskian](../../../../wronskian.md) is never zero, so [variation of parameters](../../../../variation-of-parameters.md) is valid on the whole interval. Write a particular solution as $a(x)u(x)+b(x)v(x)$, and impose the auxiliary condition $a'u+b'v=0$. Substitution then gives $a'u'+b'v'=f$. These two equations give

$$
a'=-\frac{vf}{W},\qquad b'=\frac{uf}{W}.
$$

Choosing both [integrals](../../../../integral-split.md) to start at zero makes the resulting particular solution and its first [derivative](../../../../derivative.md) vanish there:

$$
y_p(x)=-u(x)\int_0^x\frac{v(t)f(t)}{W(t)}\,dt+v(x)\int_0^x\frac{u(t)f(t)}{W(t)}\,dt=e^{-2x}\int_0^xe^{2t}\sin(x-t)f(t)\,dt.
$$

A general solution is $Au+Cv+y_p$. The [boundary condition](../../../../boundary-condition.md) at zero sets $A=0$. The condition at $\ell=\pi/2$ gives

$$
C=-\int_0^{\pi/2}e^{2t}\cos t\,f(t)\,dt,
$$

because $\sin\ell=1$ and $\sin(\ell-t)=\cos t$. Combining the two [integrals](../../../../integral-split.md) yields the [Green's function](../../../../green-s-function-split.md) representation

$$
\boxed{y(x)=\int_0^{\pi/2}G(x,t)f(t)\,dt,\qquad G(x,t)=-e^{2(t-x)}\sin(\min(x,t))\cos(\max(x,t)).}
$$

Indeed, for $t<x$ the kernel is $-e^{2(t-x)}\sin t\cos x$, since $\sin(x-t)-\sin x\cos t=-\cos x\sin t$; for $x<t$ it is $-e^{2(t-x)}\sin x\cos t$.

For fixed interior $t$, the [Green's function](../../../../green-s-function-split.md) vanishes at both endpoints, is continuous at $x=t$, solves the homogeneous equation away from $t$, and satisfies

$$
G_x(t^+,t)-G_x(t^-,t)=\sin^2t+\cos^2t=1.
$$

This [derivative](../../../../derivative.md) jump is the normalization required by the leading [coefficient](../../../../coefficient.md) one in $L$. Finally, a [homogeneous solution](../../../../homogeneous-solution.md) satisfying the first [boundary condition](../../../../boundary-condition.md) is $Ce^{-2x}\sin x$, and the second [boundary condition](../../../../boundary-condition.md) at $\pi/2$ forces $C=0$. Thus the [boundary value problem](../../../../boundary-value-problem-split.md) has exactly one solution for every continuous forcing, justifying the unique inverse represented by this kernel.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
