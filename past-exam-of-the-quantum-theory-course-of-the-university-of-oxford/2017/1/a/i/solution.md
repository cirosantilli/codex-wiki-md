<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Inside the [infinite square well](../../../../../infinite-square-well.md), the [Schrödinger equation](../../../../../schrodinger-equation.md) and [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) are

$$
i\hbar\frac{\partial\Psi}{\partial t}=-\frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2},\qquad 0<x<a,\qquad \Psi(0,t)=\Psi(a,t)=0.
$$

The [wavefunction](../../../../../wave-function-split.md) vanishes outside the box. These walls constrain its values, not its first derivatives: requiring both to vanish at an endpoint would eliminate all the nonzero stationary solutions.

For a nonzero separated solution, [separation of variables](../../../../../separation-of-variables.md) gives

$$
i\hbar\frac{T'}T=-\frac{\hbar^2}{2m}\frac{\psi''}\psi=E,\qquad T(t)=T(0)e^{-iEt/\hbar},\qquad -\frac{\hbar^2}{2m}\psi''=E\psi.
$$

The last equation is the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md). Its [energy eigenvalue](../../../../../energy-eigenvalue-split.md) is real. Multiplication by $\psi^*$ and [integration by parts](../../../../../integration-by-parts.md), with the endpoint values zero, gives

$$
E\int_0^a|\psi|^2\,dx=\frac{\hbar^2}{2m}\int_0^a|\psi'|^2\,dx\geq0.
$$

Equality would force $\psi$ to be constant and hence zero, so a nonzero [energy eigenstate](../../../../../energy-eigenstate.md) has $E>0$. Writing $k=\sqrt{2mE}/\hbar$, the general solution is $A\sin kx+B\cos kx$. The left wall gives $B=0$; the right gives $\sin ka=0$. Negative integers reproduce the same functions up to a constant, and $n=0$ gives the zero function, leaving $k=n\pi/a$ for $n=1,2,\ldots$.

Finally $\int_0^a\sin^2(n\pi x/a)\,dx=a/2$. Thus [wavefunction normalization](../../../../../wavefunction-normalization.md) with positive coefficient gives

$$
\boxed{\psi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}{a},\qquad E_n=\frac{n^2\pi^2\hbar^2}{2ma^2},\qquad n\geq1.}
$$

An arbitrary constant [global phase](../../../../../global-phase.md) has no effect on the [quantum state](../../../../../quantum-state.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
