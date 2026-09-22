<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The operator $R$ is the [midpoint parity operator](../../../../../midpoint-parity-operator.md) about $a/2$. The angle-subtraction identity gives

$$
R\psi_n(x)=\sqrt{\frac2a}\sin\left(n\pi-\frac{n\pi x}{a}\right)=\boxed{(-1)^{n+1}\psi_n(x).}
$$

Consequently $HR\psi_n=RH\psi_n=E_n(-1)^{n+1}\psi_n$. The sine functions form a complete [orthonormal basis](../../../../../orthonormal-basis.md) of $L^2(0,a)$, so the simultaneous diagonal action implies commutation on the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md)'s [operator domain](../../../../../operator-domain.md). More directly, $R$ preserves the [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and $(R\psi)''(x)=\psi''(a-x)$; hence $HR\psi=RH\psi$ whenever $H\psi$ is defined. This checks the domain as well as the differential expressions.

For arbitrary $f,g\in L^2(0,a)$, use $y=a-x$ in the [inner product](../../../../../inner-product-split.md):

$$
\langle f,Rg\rangle=\int_0^a f(x)^*g(a-x)\,dx=\int_0^a f(a-y)^*g(y)\,dy=\langle Rf,g\rangle.
$$

Also $\|Rf\|=\|f\|$, so $R$ is bounded and defined everywhere. The identity therefore proves $\boxed{R^*=R}$, with no extra domain restriction. In particular $R$ is a [self-adjoint operator](../../../../../self-adjoint-operator.md); $R^2=I$ also makes it a [unitary operator](../../../../../unitary-operator.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
