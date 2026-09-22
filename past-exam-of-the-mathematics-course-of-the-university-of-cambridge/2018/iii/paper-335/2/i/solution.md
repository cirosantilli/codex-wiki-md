<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [time reversal acoustics](../../../../../../time-reversal-acoustics.md), the array records the incoming signal, reverses each recorded time trace, and re-emits it through the same medium. This is [phase conjugation](../../../../../../phase-conjugation.md) in the frequency domain. For the [time-harmonic wave](../../../../../../time-harmonic-wave.md) convention $e^{-i\omega t}$, reversing a real time trace replaces its positive-frequency [wave amplitude](../../../../../../wave-amplitude.md) by its [complex conjugate](../../../../../../complex-conjugate.md). The medium must remain unchanged between recording and re-emission.

Let $f(\mathbf z)=\Psi_0(0,\mathbf z)$ and $G_L(\boldsymbol\zeta,\mathbf z)=G(L,\boldsymbol\zeta;0,\mathbf z)$, with the chosen source and array normalizations incorporated into the [Green function](../../../../../../green-s-function.md). Let $a(\boldsymbol\zeta)\geq0$ be the array's aperture weight, equal to the indicator of its receiving region for an ideal uniform array. The recorded field is

$$
R(\boldsymbol\zeta)=\int_{\mathbb R^2}G_L(\boldsymbol\zeta,\mathbf z')f(\mathbf z')\,d\mathbf z'.
$$

By [wave reciprocity](../../../../../../wave-reciprocity.md), back-propagation has the same [Green function](../../../../../../green-s-function.md) with the source and receiver exchanged. Therefore the physically re-emitted, back-propagated [wave amplitude](../../../../../../wave-amplitude.md) is

$$
K_A(\mathbf z,\mathbf z')=\int_{\mathbb R^2}a(\boldsymbol\zeta)G_L(\boldsymbol\zeta,\mathbf z)\overline{G_L(\boldsymbol\zeta,\mathbf z')}\,d\boldsymbol\zeta.
$$



$$
\boxed{\Psi_B(0,\mathbf z)=\int_{\mathbb R^2}K_A(\mathbf z,\mathbf z')\overline{f(\mathbf z')}\,d\mathbf z'.}
$$

If $Hf=R$ and $P_A$ multiplies by $a$, then $\Psi_B=H^TP_A\overline{Hf}$, where $T$ denotes the transpose without conjugation. Taking a final [complex conjugate](../../../../../../complex-conjugate.md) instead defines the adjoint reconstruction $\overline{\Psi_B}=H^*P_AHf$. This distinction prevents an erroneous conjugation in the [time reversal operator](../../../../../../time-reversal-operator.md).

For a localized [Gaussian beam](../../../../../../gaussian-beam.md) or [acoustic point source](../../../../../../acoustic-point-source.md) in a homogeneous medium, a finite [aperture](../../../../../../aperture.md) admits a limited range of angles. The focal width is of order $\lambda L/A$ when $A$ denotes the aperture diameter. In a [random medium](../../../../../../random-medium.md), [multiple scattering](../../../../../../multiple-scattering.md) creates paths with a larger angular spread. Each reversed path retraces its route, and the paths interfere constructively at the source. This can produce a larger [effective aperture in time reversal](../../../../../../effective-aperture-in-time-reversal.md) and a narrower focus, even though the unreversed field has a complicated [speckle pattern](../../../../../../speckle-pattern.md).

This comparison concerns a homogeneous reference medium; a deterministic heterogeneous medium can also provide useful [multipath propagation](../../../../../../multipath-propagation.md). Suitable scale limits or frequency and spatial averaging can make refocusing [self-averaging](../../../../../../self-averaging.md). Such [self-averaging](../../../../../../self-averaging.md) is not automatic for every monochromatic source and every random realization. [Wave absorption](../../../../../../wave-absorption.md), changing medium parameters, unresolved paths or poor array coverage can spoil refocusing. With complete capture of the propagating modes and a lossless [unitary operator](../../../../../../unitary-operator.md) $H$, ideal adjoint reconstruction is already exact in either medium. **Random scattering can improve finite-aperture [wave focusing](../../../../../../wave-focusing.md) through angular diversity.** See the regime-dependent analysis in [Statistical stability in time reversal](https://arxiv.org/abs/cond-mat/0206095).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
