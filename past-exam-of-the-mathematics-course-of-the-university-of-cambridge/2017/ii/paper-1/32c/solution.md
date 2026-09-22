<h1 id="32c/solution">Solution</h1>

↑ **Parent:** [32C](../32c.md)

Invert the operator definitions to obtain $a=\sqrt{m\omega/(2\hbar)}\,\hat x+i\hat p/\sqrt{2\hbar m\omega}$ and the adjoint formula for $a^\dagger$. The [canonical commutation relation](../../../../../canonical-commutation-relation.md) yields $[a,a^\dagger]=1$, with $[a,a]=[a^\dagger,a^\dagger]=0$. Substitution gives

$$
\boxed{H=\hbar\omega\left(a^\dagger a+\tfrac12\right)}.
$$

Write $N=a^\dagger a\ge0$. Since $[N,a]=-a$ and $[N,a^\dagger]=a^\dagger$, these are lowering and raising operators. Applying $a$ to a [ground state](../../../../../ground-state.md) would lower its [energy](../../../../../energy.md) unless it vanishes, so $a|0\rangle=0$. From the normalized unique [ground state](../../../../../ground-state.md) construct

$$
\boxed{|n\rangle=\frac{(a^\dagger)^n}{\sqrt{n!}}|0\rangle,
\qquad E_n=\hbar\omega(n+\tfrac12),\quad n=0,1,\ldots}.
$$

The commutator gives the factorial normalization and $a|n\rangle=\sqrt n|n-1\rangle$. For any [energy](../../../../../energy.md) eigenstate, repeated lowering cannot pass below $N=0$; positivity of each lowered [norm](../../../../../norm.md) forces its $N$ [eigenvalue](../../../../../eigenvalue.md) to be a nonnegative integer and lowering eventually reaches the [ground state](../../../../../ground-state.md). Its uniqueness then yields the entire eigenstate ladder. The usual oscillator on the real line has discrete complete spectrum because its potential is confining, so these states span its [Hilbert space](../../../../../hilbert-space-split.md).

For the perturbation $\lambda W$ with $W=\hbar\omega(a^2+a^{\dagger2})$, nondegenerate [time-independent perturbation theory](../../../../../time-independent-perturbation-theory.md) gives $E_n'=E_n+\lambda W_{nn}+\lambda^2\sum_{m\ne n}|W_{mn}|^2/(E_n-E_m)+O(\lambda^3)$. The first-order term vanishes. Only $m=n-2,n+2$ contribute, with squared [matrix](../../../../../matrix.md) elements $(\hbar\omega)^2n(n-1)$ and $(\hbar\omega)^2(n+1)(n+2)$ respectively. Thus

$$
\boxed{E_n'=\hbar\omega(n+\tfrac12)-\lambda^2\hbar\omega(2n+1)+O(\lambda^3)}.
$$

The absent downward transition for $n=0,1$ is automatically represented by $n(n-1)=0$. Direct substitution also gives

$$
H'=\frac{1-2\lambda}{2m}\hat p^2+\frac{m\omega^2(1+2\lambda)}2\hat x^2.
$$

For $|\lambda|<1/2$ this is another oscillator with mass $m'=m/(1-2\lambda)$ and frequency $\omega'=\omega\sqrt{1-4\lambda^2}$. Therefore

$$
\boxed{E_n'=\hbar\omega\sqrt{1-4\lambda^2}\,(n+\tfrac12)}.
$$

Its expansion is $E_n[1-2\lambda^2+O(\lambda^4)]$, agreeing with the perturbative result and sharpening its remainder. At the excluded endpoints confinement is lost; beyond them the quadratic [Hamiltonian](../../../../../hamiltonian.md) is not bounded below.

## ↑ Ancestors (10)

1. [32C](../32c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
