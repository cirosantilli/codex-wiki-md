<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

The [ladder operators](../../../../../ladder-operator.md) obey $[a,a^\dagger]=1$ and $N=a^\dagger a$ has $[N,a]=-a$, $[N,a^\dagger]=a^\dagger$. Since $\langle\psi,N\psi\rangle=\|a\psi\|^2\geq0$, its [eigenvalues](../../../../../eigenvalue.md) are nonnegative. If $N|\nu\rangle=\nu|\nu\rangle$, lowering gives [eigenvalue](../../../../../eigenvalue.md) $\nu-1$ and squared norm $\nu$. Repeated lowering cannot produce a negative nonzero eigenstate; the norm product $\nu(\nu-1)\cdots$ forces $\nu$ to be an integer. The final lowered state has $a|0\rangle=0$. With a unique ground state all normalized states are

$$
|n\rangle=\frac{(a^\dagger)^n}{\sqrt{n!}}|0\rangle,\qquad
\boxed{E_n=\hbar\omega(n+\tfrac12)},\quad n=0,1,\ldots.
$$

For [time-independent perturbation theory](../../../../../time-independent-perturbation-theory.md), write $H'=H+\lambda W$ with $W=\hbar\omega(a^2+a^{\dagger2})$. The standard first correction is $\lambda\langle n|W|n\rangle$ and the second is $\lambda^2\sum_{j\ne n}|\langle j|W|n\rangle|^2/(E_n-E_j)$. The first vanishes. Only $j=n-2,n+2$ occur, with ladder coefficients $\sqrt{n(n-1)}$ and $\sqrt{(n+1)(n+2)}$, respectively. Therefore

$$
\Delta E_n^{(2)}=\lambda^2\hbar\omega\left[\frac{n(n-1)}2-\frac{(n+1)(n+2)}2\right]
=-\lambda^2\hbar\omega(2n+1).
$$

The downward term is zero for $n<2$.

Inverting the given position/momentum expressions gives

$$
a^2+a^{\dagger2}=\frac{m\omega}{\hbar}\widehat x^2-\frac{\widehat p^2}{m\hbar\omega}.
$$

Thus **$\boxed{\alpha=1-2\lambda,\ \beta=1+2\lambda}$**. For $|\lambda|<1/2$ both are positive, and this is a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) of effective mass $m/\alpha$ and frequency $\omega\sqrt{\alpha\beta}$. Its exact energies are

$$
\boxed{E_n'=\hbar\omega\sqrt{1-4\lambda^2}(n+\tfrac12).}
$$

Expansion gives $E_n'=\hbar\omega(n+1/2)[1-2\lambda^2+O(\lambda^4)]$, agreeing with both perturbative corrections.

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
