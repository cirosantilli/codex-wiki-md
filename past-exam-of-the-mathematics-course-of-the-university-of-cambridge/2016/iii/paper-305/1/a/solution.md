<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The operator $b^s(p)$ is a [fermionic annihilation operator](../../../../../../fermionic-annihilation-operator.md) for a particle with momentum $\mathbf p$ and spin label $s$; $d^{s\dagger}(p)$ is a [fermionic creation operator](../../../../../../fermionic-creation-operator.md) for the corresponding [antiparticle](../../../../../../antiparticle.md). The c-number [Dirac spinors](../../../../../../dirac-spinor.md) $u^s(p)$ and $v^s(p)$ solve the positive-energy particle and antiparticle equations respectively. They supply the spinor wavefunctions in the [mode expansion of a Dirac field](../../../../../../mode-expansion-of-a-dirac-field.md); they are not creation or annihilation operators.

Apply the specified [parity](../../../../../../parity.md) transformation to the two operators in the [mode expansion of a Dirac field](../../../../../../mode-expansion-of-a-dirac-field.md):

$$
\widehat P\psi(x)\widehat P^{-1}=\eta_P\sum_{p,s}\left[b^s(p_P)u^s(p)e^{-ip\cdot x}-d^{s\dagger}(p_P)v^s(p)e^{ip\cdot x}\right].
$$

Relabel $k=p_P$. The momentum sum is unchanged, $p\cdot x=k\cdot x_P$, and the spinor identities give $u^s(p)=\gamma^0u^s(k)$ and $v^s(p)=-\gamma^0v^s(k)$. The two minus signs in the antiparticle term cancel. Therefore

$$
\boxed{\widehat P\psi(x)\widehat P^{-1}=\eta_P\gamma^0\psi(x_P).}
$$

Taking the [Hermitian conjugate](../../../../../../hermitian-conjugation.md) and using $(\gamma^0)^\dagger=\gamma^0$, $(\gamma^0)^2=1$ in the [Dirac adjoint](../../../../../../dirac-adjoint.md) yields

$$
\boxed{\widehat P\bar\psi(x)\widehat P^{-1}=\eta_P^*\bar\psi(x_P)\gamma^0.}
$$

The unit-modulus intrinsic-parity phase cancels from all neutral [fermion bilinears](../../../../../../fermion-bilinear.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
