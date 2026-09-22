<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a periodic comoving box of volume $L^3$, with $\mathbf k=2\pi\mathbf n/L$. A real field has the expansion

$$
\delta\hat\phi(\mathbf x,t)=\sum_{\mathbf k}\left[w_k(t)\hat a_{\mathbf k}e^{i\mathbf k\cdot\mathbf x}+w_k^*(t)\hat a_{\mathbf k}^\dagger e^{-i\mathbf k\cdot\mathbf x}\right],
$$

where $[\hat a_{\mathbf k},\hat a_{\mathbf q}^\dagger]=\delta_{\mathbf k\mathbf q}$ and the other ladder-operator [commutators](../../../../../../commutator.md) vanish. The coefficient of $e^{i\mathbf k\cdot\mathbf x}$ is therefore $w_k\hat a_{\mathbf k}+w_k^*\hat a_{-\mathbf k}^\dagger$. This opposite momentum is required by reality; the single-oscillator shorthand with the same label on both operators must not be read literally as every traveling-wave [Fourier coefficient](../../../../../../fourier-coefficient.md).

The quadratic action has [canonical momentum](../../../../../../canonical-momentum.md) $\hat\pi=a^3\delta\dot{\hat\phi}$. Its equal-time field [commutator](../../../../../../commutator.md) requires

$$
\boxed{a^3L^3(w_k\dot w_k^*-w_k^*\dot w_k)=i}.
$$

Choose the vacuum annihilated by all $a_{\mathbf k}$ and the subhorizon positive-frequency condition. For constant $H$ and negligible effective [mass](../../../../../../mass.md), put $x=k/(aH)$, $C_k=L^{-3/2}H/\sqrt{2k^3}$. The candidate is $w_k=C_k(i+x)e^{ix}$. Since $\dot x=-Hx$,

$$
\dot w_k=-iHC_kx^2e^{ix},\qquad\ddot w_k=H^2C_k(2ix^2-x^3)e^{ix}.
$$

Direct substitution makes $\ddot w_k+3H\dot w_k+(k^2/a^2)w_k$ identically zero. Its [Wronskian](../../../../../../wronskian.md) is $2iHC_k^2x^3=i/(L^3a^3)$, which has the required normalization. Thus

$$
\boxed{w_k=L^{-3/2}\frac H{\sqrt{2k^3}}\left(i+\frac{k}{aH}\right)e^{ik/(aH)}}.
$$

This is the existing [Bunch-Davies mode normalization in a finite comoving volume](../../../../../../bunch-davies-mode-normalization-in-a-finite-comoving-volume.md). It is exact for a massless minimally coupled test field in de Sitter and the leading approximation for a light slowly evolving field. The homogeneous zero mode needs separate treatment.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
