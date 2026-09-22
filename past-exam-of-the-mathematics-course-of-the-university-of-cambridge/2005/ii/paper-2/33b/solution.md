<h1 id="33b/solution">Solution</h1>

↑ **Parent:** [33B](../33b.md)

For a normalized trial state in the quadratic-form domain of a [self-adjoint](../../../../../self-adjoint-operator.md) [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) bounded below, its [expectation](../../../../../expected-value.md) of $H$ is at least the ground [energy](../../../../../energy.md) $E_0$. Minimizing this [Rayleigh quotient](../../../../../rayleigh-quotient.md) over a tractable trial family therefore supplies an upper bound.

For the two states, set $a_\pm=(a_1\pm a_2)/\sqrt2$. Their quotient is

$$
\frac{(E+\epsilon)a_+^2+(E-\epsilon)a_-^2}
{(1+s)a_+^2+(1-s)a_-^2}.
$$

The strict assumption $\epsilon<sE$ excludes $|s|=1$, since equality in the overlap Cauchy-Schwarz bound would then force the two states to be proportional and $\epsilon=sE$. Thus $|s|<1$. The two generalized [eigenvalues](../../../../../eigenvalue.md) are $(E\pm\epsilon)/(1\pm s)$, and their difference has the sign of $\epsilon-sE$. The symmetric trial is the lower one, so

$$
\boxed{E_0\leq\frac{E+\epsilon}{1+s}.}
$$

For the single attractive delta well, the supplied [wavefunction](../../../../../wave-function.md) has [norm](../../../../../norm.md) one because $\int\lambda e^{-2\lambda|x|}\,dx=1$. Its [kinetic energy](../../../../../kinetic-energy.md) in quadratic-form notation is $\hbar^2\int|\psi_1'|^2/(2m)=\hbar^2\lambda^2/(2m)$, and its [delta potential](../../../../../delta-potential.md) [energy](../../../../../energy.md) is $-K|\psi_1(0)|^2=-K\lambda$. With $\lambda=mK/\hbar^2$ this gives

$$
\boxed{E_B=-K\lambda/2.}
$$

Its derivative jump is $\psi_1'(0+)-\psi_1'(0-)=-2\lambda\psi_1(0)$, exactly the delta [boundary condition](../../../../../boundary-condition.md), so it is an eigenstate. A decaying [bound state](../../../../../bound-state.md) on the two half-lines must have a common decay rate fixed by this same jump; there is only this one negative-energy state, confirming it is the [ground state](../../../../../ground-state.md).

For $R>0$, integrate the overlap on the three regions $x<0$, $0<x<R$, $x>R$. Put $a=\lambda R$. The result is

$$
\boxed{s=(1+a)e^{-a},\qquad
E=E_B-K\lambda e^{-2a},\qquad
\epsilon=E_Bs-K\lambda e^{-a}.}
$$

The second equality is the single-well [energy](../../../../../energy.md) plus the extra delta [expectation](../../../../../expected-value.md); the third follows by applying either single-well [eigenvalue](../../../../../eigenvalue.md) equation in the cross [matrix](../../../../../matrix.md) element. Moreover $\epsilon-sE=K\lambda e^{-a}[(1+a)e^{-2a}-1]<0$, so the preceding bound applies. Substitution gives

$$
\boxed{E_0(R)\leq E_B\left[1+\frac{2e^{-\lambda R}(1+e^{-\lambda R})}{1+(1+\lambda R)e^{-\lambda R}}\right].}
$$

For widely separated wells, each localized orbital is close to an isolated-well [ground state](../../../../../ground-state.md) and the low-energy subspace is accurately their span; the symmetric combination captures the leading tunneling [energy](../../../../../energy.md) lowering. In the limit both exact and trial energies approach $E_B$. This illustrates electronic molecular binding: sharing an orbital between attractive centers can lower its [energy](../../../../../energy.md) below the separated-center value. A full equilibrium bond length would also require the repulsion of the positive centers.

## ↑ Ancestors (10)

1. [33B](../33b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
