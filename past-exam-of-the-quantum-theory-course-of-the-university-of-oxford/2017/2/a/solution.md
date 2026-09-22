<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a smooth [wavefunction](../../../../wave-function-split.md) $f$, the [position operator](../../../../position-operator.md) and [momentum operator](../../../../momentum-operator.md) give

$$
[X,P]f=-i\hbar xf'+i\hbar(xf)'=i\hbar f.
$$

Thus the [canonical commutation relation](../../../../canonical-commutation-relation.md) is $\boxed{[X,P]=i\hbar I}$. Since $X$ and $P$ are [self-adjoint operators](../../../../self-adjoint-operator.md) and $m,\omega$ are real, the [adjoint operator](../../../../adjoint-operator.md) of $a_-$ is

$$
\boxed{a_+=P+im\omega X.}
$$

Expanding the products in the stated order is essential:

$$
\begin{aligned}
a_+a_-&=P^2+m^2\omega^2X^2+im\omega[X,P]=2mH-m\hbar\omega,\\
a_-a_+&=P^2+m^2\omega^2X^2-im\omega[X,P]=2mH+m\hbar\omega.
\end{aligned}
$$

Subtracting gives $\boxed{[a_-,a_+]=2m\hbar\omega I}$. These identities initially hold on smooth rapidly decaying functions, which contain the [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md) [energy eigenstates](../../../../energy-eigenstate.md) used below.

The factorization also proves a lower bound: for a normalized [energy eigenstate](../../../../energy-eigenstate.md) $H\psi=E\psi$,

$$
0\leq\|a_-\psi\|^2=\langle\psi,a_+a_-\psi\rangle=2m\left(E-\frac12\hbar\omega\right).
$$

Therefore $E\geq E_0:=\hbar\omega/2$. The [commutator product rule](../../../../commutator-product-rule.md), applied to $H=a_+a_-/(2m)+E_0$, gives

$$
[H,a_+]=\hbar\omega a_+,\qquad [H,a_-]=-\hbar\omega a_-.
$$

So a nonzero application of the [creation operator](../../../../creation-operator.md) $a_+$ raises the [energy eigenvalue](../../../../energy-eigenvalue-split.md) by $\hbar\omega$, while the [annihilation operator](../../../../annihilation-operator.md) $a_-$ lowers it by the same amount.

Begin with any [energy eigenstate](../../../../energy-eigenstate.md), whose existence is assumed. Repeated lowering must terminate: otherwise it would eventually produce a nonzero [energy eigenstate](../../../../energy-eigenstate.md) below $E_0$, contradicting the lower bound. More explicitly, if $(E-E_0)/(\hbar\omega)=N+r$ with integer $N\geq0$ and $0\leq r<1$, the first $N$ lowering steps are nonzero. If $r>0$, one further step is also nonzero by its positive squared [norm](../../../../norm.md) and has energy $E_0+(r-1)\hbar\omega<E_0$, an impossibility. Thus $r=0$ and the last state satisfies $a_-\psi_0=0$. This proves

$$
\boxed{E_n=\left(n+\frac12\right)\hbar\omega,\qquad n=0,1,2,\ldots.}
$$

Every level exists as well: $\|a_+\psi_n\|^2=2m(E_n+\hbar\omega/2)=2m\hbar\omega(n+1)>0$, so repeated raising from $\psi_0$ never vanishes. The same factorization bounds the [energy expectation](../../../../energy-expectation.md) of any normalized state in the [one-dimensional harmonic oscillator form domain](../../../../one-dimensional-harmonic-oscillator-form-domain.md) below by $E_0$, proving that the terminated state really is a [ground state](../../../../ground-state.md).

To find its [probability density](../../../../probability-density.md), solve the first-order equation

$$
(P-im\omega X)\psi_0=-i\left(\hbar\psi_0'+m\omega x\psi_0\right)=0.
$$

Its solutions are $\psi_0=C_0\exp[-m\omega x^2/(2\hbar)]$. With $\alpha=m\omega/\hbar>0$, the supplied [Gaussian integral](../../../../gaussian-integral.md) gives

$$
1=|C_0|^2\int_{-\infty}^{\infty}e^{-\alpha x^2}\,dx=|C_0|^2\sqrt{\frac\pi\alpha}.
$$

Taking $C_0=(\alpha/\pi)^{1/4}$ fixes an irrelevant [global phase](../../../../global-phase.md). Consequently

$$
\boxed{|\psi_0(x)|^2=\sqrt{\frac{m\omega}{\pi\hbar}}\exp\left(-\frac{m\omega x^2}{\hbar}\right).}
$$

The [ground-state energy](../../../../ground-state-energy.md) is positive even though the potential minimum is zero: it is the oscillator's [zero-point energy](../../../../zero-point-energy.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
