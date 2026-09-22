<h1 id="18f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The initial [wavefunction](../../../../../../wave-function.md) has unit norm, since $\int_0^a(2/a)\sin^2(\pi x/a)\,dx=1$. On its nonzero half, $-\hbar^2\psi''/(2m)=E_*\psi$ with $E_*=\hbar^2\pi^2/(2ma^2)$. A small domain qualification is important: the [derivative](../../../../../../derivative.md) jumps at zero, so the state is not in the operator domain of the Dirichlet [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md). Its finite energy [expectation value](../../../../../../expectation-value.md) is nevertheless defined by the [quadratic form of a positive quantum Hamiltonian](../../../../../../quadratic-form-of-a-positive-quantum-hamiltonian.md). The [energy form of a half-well sine state](../../../../../../energy-form-of-a-half-well-sine-state.md) gives

$$
\langle E\rangle=\frac{\hbar^2}{2m}\int_{-a}^a|\psi'(x)|^2dx
=\frac{\hbar^2}{2m}\frac{2\pi^2}{a^3}\int_0^a\cos^2(\pi x/a)\,dx
=\boxed{\frac{\hbar^2\pi^2}{2ma^2}}.
$$

This is also the rigorous weak interpretation of the printed $\int\psi H\psi$. Indeed the distributional second [derivative](../../../../../../derivative.md) is $\psi''=-(\pi/a)^2\psi+\sqrt{2/a}(\pi/a)\delta_0$ inside the well. The [Dirac delta](../../../../../../dirac-delta-function.md) term pairs to zero because $\psi(0)=0$. One should not instead conclude that this state is an [energy eigenstate](../../../../../../energy-eigenstate.md) from its equation on just the positive half.

Its coefficients in the full-well [energy eigenstates](../../../../../../energy-eigenstate.md) are

$$
a_n=\frac{\sqrt2}{a}\int_0^a\sin\frac{\pi x}{a}\sin\frac{n\pi(x+a)}{2a}\,dx.
$$

For even $n$, sine [orthogonality](../../../../../../orthogonal-vectors.md) gives $a_2=-1/\sqrt2$ and all other even coefficients zero. For $n=2p+1$, set $u=x/a$ and use $\sin[n\pi(u+1)/2]=(-1)^p\cos(n\pi u/2)$. Product-to-sum integration then gives

$$
\int_0^1\sin\pi u\cos\frac{n\pi u}{2}\,du=\frac{4}{\pi(4-n^2)},\qquad
\boxed{a_{2p+1}=\frac{4\sqrt2(-1)^p}{\pi[4-(2p+1)^2]}}.
$$

Since these coefficients are $O(n^{-2})$, $\sum_nE_n|a_n|^2$ converges, confirming that the state has finite energy. With $E_n=n^2E_1$, the spectral expression is

$$
\langle E\rangle=\frac12E_2+\frac{32E_1}{\pi^2}\sum_{p=0}^{\infty}\frac{(2p+1)^2}{[(2p+1)^2-4]^2}.
$$

The kinetic-energy [quadratic form](../../../../../../quadratic-form.md) equals this spectral sum: expanding the weak [derivative](../../../../../../derivative.md) in the corresponding orthonormal cosine modes and using [Parseval's identity](../../../../../../parseval-identity.md) gives $\int|\psi'|^2=\sum_nk_n^2|a_n|^2$. Equating it to the directly integrated value $4E_1$ proves

$$
\boxed{1=\frac12+\frac8{\pi^2}\sum_{p=0}^{\infty}\frac{(2p+1)^2}{[(2p+1)^2-4]^2}}.
$$

In contrast, $\sum_nE_n^2|a_n|^2$ diverges, consistently showing why $H\psi$ is not an ordinary square-integrable [vector](../../../../../../vector.md) even though the energy expectation is finite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18F](../../18f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
