<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

On a suitable dense domain of smooth rapidly decreasing [wave functions](../../../../../wave-function.md), the canonical [commutator](../../../../../commutator.md) is $[x,p]=i\hbar$. Expanding the two [ladder operators](../../../../../ladder-operator.md) gives

$$
[a,a^\dagger]=\frac12\left[\beta x+\frac{ip}{\beta\hbar},\beta x-\frac{ip}{\beta\hbar}\right]
=\frac12(1+1)=1.
$$

Their sum and difference give

$$
\boxed{x=\frac{a+a^\dagger}{\sqrt2\beta},\qquad
p=\frac{\beta\hbar}{i\sqrt2}(a-a^\dagger).}
$$

Direct multiplication, retaining the operator order, gives

$$
a^\dagger a=\frac12\left[\beta^2x^2+\frac{p^2}{\beta^2\hbar^2}+\frac{i[x,p]}\hbar\right]
=\frac12\left[\beta^2x^2+\frac{p^2}{\beta^2\hbar^2}-1\right].
$$

Using $\beta^2=m\omega/\hbar$ identifies the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md):

$$
\boxed{H=\hbar\omega(a^\dagger a+\tfrac12).}
$$

For any admissible [wave function](../../../../../wave-function.md), adjointness gives

$$
\langle\Psi,H\Psi\rangle=\hbar\omega\left(\|a\Psi\|^2+\tfrac12\|\Psi\|^2\right)
\geq\tfrac12\hbar\omega\|\Psi\|^2.
$$

For the conventional normalized state $\|\Psi\|=1$, this is the stated lower bound $E\geq\hbar\omega/2$. For an unnormalized [function](../../../../../function-split.md) the [norm](../../../../../norm.md) factor must be retained; rescaling a [wave function](../../../../../wave-function.md) cannot leave its unnormalized [energy](../../../../../energy.md) [integral](../../../../../integral.md) bounded below by a fixed positive number.

Equality holds exactly when $a\Psi_0=0$. In position representation this equation is $(\beta x+\beta^{-1}\partial_x)\Psi_0=0$, whose normalized square-integrable solution is

$$
\boxed{\Psi_0(x)=\left(\frac{\beta^2}{\pi}\right)^{1/4}e^{-\beta^2x^2/2},\qquad E_0=\tfrac12\hbar\omega.}
$$

This construction establishes existence of a state attaining the bound, and hence proves that it is the [ground state](../../../../../ground-state.md).

The [commutator](../../../../../commutator.md) $[a,a^\dagger]=1$ implies $[H,a^\dagger]=\hbar\omega a^\dagger$. Repeatedly commuting through the product gives

$$
H(a^\dagger)^n\Psi_0=(a^\dagger)^nH\Psi_0+n\hbar\omega(a^\dagger)^n\Psi_0
=\hbar\omega(n+\tfrac12)(a^\dagger)^n\Psi_0.
$$

These [vectors](../../../../../vector.md) are nonzero: the identity $a(a^\dagger)^n\Psi_0=n(a^\dagger)^{n-1}\Psi_0$ gives their [norm](../../../../../norm.md) squared $n!$ by induction. Therefore

$$
\boxed{\Psi_n=\frac{(a^\dagger)^n}{\sqrt{n!}}\Psi_0,\qquad E_n=(n+\tfrac12)\hbar\omega.}
$$

For time-dependent stationary states multiply each spatial eigenfunction by $e^{-iE_nt/\hbar}$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
