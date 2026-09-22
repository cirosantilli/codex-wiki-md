<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $\sin l\ne0$, use [variation of parameters](../../../../../variation-of-parameters.md) with the [homogeneous solutions](../../../../../homogeneous-solution.md) $\cos x,\sin x$, whose [Wronskian](../../../../../wronskian.md) is one. Write $y=A(x)\cos x+B(x)\sin x$ and impose $A'\cos x+B'\sin x=0$. The [differential equation](../../../../../differential-equation-split.md) gives $-A'\sin x+B'\cos x=f$, hence

$$
A'=-f\sin x,\qquad B'=f\cos x.
$$

After integrating from zero and using the left [boundary condition](../../../../../boundary-condition.md),

$$
y(x)=C\sin x+\int_0^x\sin(x-t)f(t)\,dt.
$$

The right [boundary condition](../../../../../boundary-condition.md) determines

$$
C=-\frac1{\sin l}\int_0^l\sin(l-t)f(t)\,dt,
$$

so the unique solution is

$$
\boxed{y(x)=\int_0^x\sin(x-t)f(t)\,dt
-\frac{\sin x}{\sin l}\int_0^l\sin(l-t)f(t)\,dt.}
$$

Combining the two [integrals](../../../../../integral-split.md) gives $y(x)=\int_0^lG(x,t)f(t)\,dt$, with [Green's function](../../../../../green-s-function-split.md)

$$
\boxed{G(x,t)=-\frac1{\sin l}
\begin{cases}
\sin x\sin(l-t),&0\leq x\leq t,\\
\sin t\sin(l-x),&t\leq x\leq l.
\end{cases}}
$$

It is symmetric in $x,t$, as expected from [self-adjointness](../../../../../self-adjoint-operator.md), and has zero endpoint values. At $x=t$ it is continuous, while its first [derivative](../../../../../derivative.md) obeys the [jump condition](../../../../../jump-condition.md)

$$
G_x(t^+,t)-G_x(t^-,t)
=\frac{\sin t\cos(l-t)+\cos t\sin(l-t)}{\sin l}=1.
$$

Thus $(\partial_x^2+1)G=\delta(x-t)$, with the positive normalization of the [Dirac delta function](../../../../../dirac-delta-function.md) required for $\mathcal Ly=f$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
