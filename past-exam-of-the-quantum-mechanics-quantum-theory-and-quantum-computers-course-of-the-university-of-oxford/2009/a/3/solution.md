<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With the specified ladder-operator [normalization](../../../../normalization.md), $A_+^\dagger=A_-$ and

$$
A_+A_-=P^2+m^2\omega^2X^2-m\hbar\omega=2mH-m\hbar\omega.
$$

Therefore $\|A_-\psi\|^2=2m(E-\hbar\omega/2)\|\psi\|^2\geq0$. This proves $\boxed{E\geq\hbar\omega/2}$, with equality exactly when $A_-\psi=0$. In position representation this equation is $\hbar\psi'+m\omega x\psi=0$, whose general solution is

$$
\boxed{\psi(x)=C\exp[-m\omega x^2/(2\hbar)].}
$$

For a unit vector $|C|=(m\omega/\pi\hbar)^{1/4}$; its phase is arbitrary. The [commutators](../../../../commutator.md) $[H,A_\pm]=\pm\hbar\omega A_\pm$ make $A_+$ raise and $A_-$ lower energies by $\hbar\omega$. Repeated raising of the Gaussian produces all levels $(n+1/2)\hbar\omega$. Conversely lowering any nonzero [energy](../../../../energy-split.md) [eigenvector](../../../../eigenvector.md) must eventually terminate, since otherwise it would produce an [energy](../../../../energy-split.md) below the lower bound. A terminating vector is annihilated by $A_-$ and hence has [energy](../../../../energy-split.md) $\hbar\omega/2$. Thus no other [eigenvalues](../../../../eigenvalue.md) occur.

Bilinearity of the two-dimensional [commutators](../../../../commutator.md) gives

$$
[P_\theta,X_\varphi]=-i\hbar(\cos\theta\cos\varphi+\sin\theta\sin\varphi)\mathbf1=-i\hbar\cos(\theta-\varphi)\mathbf1,
$$

while all momentum-momentum and position-position [commutators](../../../../commutator.md) remain zero. Equal angles give a canonical position-momentum pair. Perpendicular angles give commuting components, which belong to independent coordinate directions.

The orthogonal coordinates $X_+=(X_1+X_2)/\sqrt2$, $X_-=(X_1-X_2)/\sqrt2$ preserve the kinetic sum, and

$$
5(X_1^2+X_2^2)-8X_1X_2=X_+^2+9X_-^2.
$$

Hence $\boxed{\omega_+=\omega,\quad\omega_-=3\omega}$ and $H=H_++H_-$. Every cross-mode position/momentum pair commutes, so $[H_+,H_-]=0$. On the tensor-product oscillator basis,

$$
E=\hbar\omega(n_++\tfrac12)+3\hbar\omega(n_-+\tfrac12)=(n_++3n_-+2)\hbar\omega.
$$

For each $N\geq0$, allowed pairs have $n_-=0,1,\ldots,\lfloor N/3\rfloor$ and $n_+=N-3n_-$. Thus

$$
\boxed{E_N=(N+2)\hbar\omega,\qquad g_N=\lfloor N/3\rfloor+1.}
$$

Each pair contributes one product [eigenvector](../../../../eigenvector.md); counting them accounts for the [energy-level degeneracy](../../../../energy-level-degeneracy.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
