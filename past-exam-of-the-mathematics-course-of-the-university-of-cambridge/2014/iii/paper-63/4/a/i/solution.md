<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../../../fourier-transform.md) convention $\widehat w(E)=\int_{\mathbb R}w(t)e^{itE}dt$. Since $w\geq0$, it is real, so $\widehat w(-E)=\widehat w(E)^*$. The positive-frequency cutoff therefore also eliminates frequencies at or below $-\Delta$. Normalization gives $\int w=\widehat w(0)=1$.

For [spectral filtering of Hamiltonian terms](../../../../../../../spectral-filtering-of-hamiltonian-terms.md), choose

$$
\boxed{A^{(Z)}=\int_{\mathbb R}w(t)e^{itH}h_Ze^{-itH}dt.}
$$

In an energy [eigenbasis](../../../../../../../eigenbasis.md), its [matrix elements](../../../../../../../matrix-element.md) are

$$
\langle\phi_i|A^{(Z)}|\phi_j\rangle=\widehat w(E_i-E_j)\langle\phi_i|h_Z|\phi_j\rangle.
$$

At $i=j=0$ the frequency is zero, so the normalization preserves the ground-state expectation:

$$
\boxed{\langle\phi_0|A^{(Z)}|\phi_0\rangle=\langle\phi_0|h_Z|\phi_0\rangle.}
$$

The [spectral filter](../../../../../../../spectral-filter.md) is a positive weighted average of [unitary conjugations](../../../../../../../unitary-conjugation.md); in particular the integral is bounded in [operator norm](../../../../../../../operator-norm.md) by $\|h_Z\|$. We can choose it even without an extra assumed tail bound: the [evenization of a nonnegative bandlimited filter](../../../../../../../evenization-of-a-nonnegative-bandlimited-filter.md) proved in part (e) produces another admissible [spectral filter](../../../../../../../spectral-filter.md) with the same type of positive-time decay. Make that choice consistently in all the filtered terms and shell definitions below.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 63](../../../../paper-63-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
