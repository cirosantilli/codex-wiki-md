<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inside the [infinite square well](../../../../infinite-square-well.md), the [time-independent Schrödinger equation](../../../../time-independent-schrodinger-equation.md) and [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) are

$$
-\frac{\hbar^2}{2m}\psi''=E\psi\quad(0<x<a),\qquad \psi(0)=\psi(a)=0,
$$

and the [wavefunction](../../../../wave-function-split.md) vanishes outside the interval. For a nonzero state, [integration by parts](../../../../integration-by-parts.md) gives

$$
E\int_0^a|\psi|^2\,dx=\frac{\hbar^2}{2m}\int_0^a|\psi'|^2\,dx>0.
$$

The strict inequality follows because a function with zero derivative and zero endpoint values is zero. Put $k=\sqrt{2mE}/\hbar$. The general solution is $A\sin kx+B\cos kx$; the first [boundary condition](../../../../boundary-condition.md) gives $B=0$, and the second gives $ka=n\pi$, $n=1,2,\ldots$. Since $\int_0^a\sin^2(n\pi x/a)\,dx=a/2$, the normalized [energy eigenstates](../../../../energy-eigenstate.md) and [eigenvalues](../../../../eigenvalue.md) are

$$
\boxed{\psi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}{a},\qquad E_n=\frac{n^2\pi^2\hbar^2}{2ma^2},\quad n\geq1.}
$$

The normalization fixes the magnitude of the coefficient; its arbitrary [global phase](../../../../global-phase.md) has been chosen real and positive.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
