<h1 id="32d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [spatial translation operator](../../../../../../spatial-translation-operator.md) is $U(\alpha)=e^{-i\alpha\widehat p/\hbar}$. From $[\widehat x,\widehat p]=i\hbar$ and the preceding central-commutator result,

$$
\boxed{[\widehat x,U(\alpha)]=\alpha U(\alpha).}
$$

Thus $\widehat xU|x\rangle=U\widehat x|x\rangle+\alpha U|x\rangle=(x+\alpha)U|x\rangle$, consistent with $U|x\rangle=|x+\alpha\rangle$. Since $\langle x|U=\langle x-\alpha|$, the translated [wavefunction](../../../../../../wave-function.md) is $\boxed{\psi(x-\alpha)}$.

For the [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator.md), the [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) give $\widehat p=i\sqrt{m\hbar\omega/2}(a^\dagger-a)$. Put $s=\alpha\sqrt{m\omega/(2\hbar)}$. The central [commutator](../../../../../../commutator.md) of $sa^\dagger$ and $-sa$ is $s^2$, so

$$
U=e^{s(a^\dagger-a)}=e^{-s^2/2}e^{sa^\dagger}e^{-sa}.
$$

As $a|0\rangle=0$ and $(a^\dagger)^n|0\rangle=\sqrt{n!}|n\rangle$,

$$
U|0\rangle=e^{-s^2/2}\sum_{n=0}^\infty\frac{s^n}{\sqrt{n!}}|n\rangle.
$$

Taking position [wavefunctions](../../../../../../wave-function.md) proves

$$
\boxed{\psi_0(x-\alpha)=e^{-m\omega\alpha^2/(4\hbar)}\sum_{n=0}^\infty\left(\frac{m\omega}{2\hbar}\right)^{n/2}\frac{\alpha^n}{\sqrt{n!}}\psi_n(x).}
$$

The coefficient squares sum to $e^{-s^2}\sum_n s^{2n}/n!=1$, checking normalization of this [coherent state](../../../../../../coherent-state.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32D](../../32d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
