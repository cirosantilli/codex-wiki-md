<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $O=\int d[\bar\psi,\psi]e^{-\sum\bar\psi\psi}|\psi\rangle\langle\psi|$. For bosons the measure is $\prod_n d\operatorname{Re}\psi_n\,d\operatorname{Im}\psi_n/\pi$ over $\mathbb C$ in each mode, with $\bar\psi_n=\psi_n^*$. For fermions it is an ordered [Berezin integral](../../../../../../berezin-integral.md) over independent $\bar\psi_n,\psi_n$; choose $\int d\bar\psi\,d\psi\,\bar\psi\psi=-1$, so $\int d\bar\psi\,d\psi\,e^{-\bar\psi\psi}=1$.

For one bosonic mode, $a|\psi\rangle=\psi|\psi\rangle$ and $\langle\psi|a=\partial_{\bar\psi}\langle\psi|$. [Integration by parts](../../../../../../integration-by-parts.md) in the Gaussian measure gives $aO=Oa$; the conjugate argument gives $a^\dagger O=Oa^\dagger$. Boundary terms vanish because of the Gaussian weight.

For one fermionic mode, put $n=a^\dagger a$ and move Grassmann coefficients to the left. The weighted projector is

$$
W=e^{-\bar\psi\psi}|\psi\rangle\langle\psi|=(1-n)-\psi a^\dagger+\bar\psi a-\bar\psi\psi I.
$$

Its ordinary [commutators](../../../../../../commutator.md) are $[a,W]=-a+\psi I$ and $[a^\dagger,W]=a^\dagger-\bar\psi I$. Their [Berezin integrals](../../../../../../berezin-integral.md) vanish, so again $[a,O]=[a^\dagger,O]=0$. Equivalently the sole surviving coefficient in $\int W$ is $-\bar\psi\psi I$, giving $I$ directly.

The modes factorize. In the irreducible [Fock space](../../../../../../fock-space.md) representation, commuting with every creation and annihilation operator makes $O$ a scalar multiple of the identity. Its vacuum matrix element is the normalized Gaussian integral, equal to one. Thus the [coherent-state resolution of identity](../../../../../../coherent-state-resolution-of-identity.md) is

$$
\boxed{\int d[\bar\psi,\psi]e^{-\sum_n\bar\psi_n\psi_n}|\psi\rangle\langle\psi|=I}.
$$

For infinitely many modes, this argument first uses a finite-mode regulator.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
