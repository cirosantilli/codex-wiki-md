# Single-tone FM sidebands

↑ **Parent:** [Frequency modulation](frequency-modulation.md)

A single-tone [FM](frequency-modulation.md) [signal](signal.md) has components displaced from the [carrier wave](carrier-wave.md) [frequency](frequency.md) by integer multiples of the message [frequency](frequency.md). These are temporal sidebands; the [spatial sidebands](spatial-sideband.md) used to perturb a spatial pattern are a related but different setting. To find the temporal components, apply the [Jacobi-Anger expansion](jacobi-anger-expansion.md) to the complex representation:

$$
e^{\mathrm i\beta\sin\theta}=\sum_{k=-\infty}^{\infty}J_k(\beta)e^{\mathrm ik\theta},\qquad
z(t)=A\sum_{k=-\infty}^{\infty}J_k(\beta)e^{2\pi\mathrm i(f_c+kf_m)t}.
$$

Here $J_k$ is a [Bessel function of the first kind](bessel-function-of-the-first-kind.md). The identity follows by setting the generating variable to $e^{\mathrm i\theta}$ in its [generating function](generating-function.md).[Chapter 10, §10.12, equation 10.12.1 and the substitution described in the section notes](nist-digital-library-of-mathematical-functions.md)

Taking the [real part](real-part.md) gives the exact real [signal](signal.md) expansion

$$
s(t)=A\sum_{k=-\infty}^{\infty}J_k(\beta)\cos\bigl(2\pi(f_c+kf_m)t\bigr).
$$

The complex representation has a [Fourier coefficient](fourier-coefficient.md) $AJ_k(\beta)$ at $f_c+kf_m$; the normalized magnitude is $|J_k(\beta)|$. The identity $J_{-k}(\beta)=(-1)^kJ_k(\beta)$ makes upper and lower complex sideband magnitudes equal, but their signs matter when reconstructing the [wave phase](phase-waves.md). A negative coefficient reverses a component's [wave phase](phase-waves.md) by $\pi$; an [amplitude](wave-amplitude.md) display alone hides that information.

For $\beta=5$, original evaluation gives $J_0(5)\approx-0.17760$, $J_1(5)\approx-0.32758$, $J_5(5)\approx0.26114$ and $J_6(5)\approx0.13105$. Thus there are appreciable components at $14$ and $26\,\mathrm{Hz}$, outside the $15$–$25\,\mathrm{Hz}$ range of the [instantaneous frequency](instantaneous-frequency.md). There is no contradiction: [instantaneous frequency](instantaneous-frequency.md) describes the local rate of the combined [wave phase](phase-waves.md), while the [frequency spectrum](frequency-spectrum.md) describes a global [superposition](superposition-principle.md) of constant-[frequency](frequency.md) components.

For the real [signal](signal.md), negative [frequencies](frequency.md) must also be accounted for: a [cosine](cosine.md) at $-f$ equals one at $f$. When $f_c/f_m=20$, the normalized positive-[frequency](frequency.md) [cosine](cosine.md) coefficient at $nf_m$, $n>0$, is exactly $J_{n-20}(\beta)+J_{-n-20}(\beta)$. The second term is extremely small over the plotted range, but the figure includes it. The chosen complex representation need not have a [frequency spectrum](frequency-spectrum.md) supported only at positive [frequencies](frequency.md), even when its specified [instantaneous frequency](instantaneous-frequency.md) is everywhere positive.

<a id="image-fm-sideband-amplitudes-for-three-modulation-indices-at-fixed-carrier-and-message-frequencies"></a>
![](frequency-modulation-sideband-amplitude-comparison.png)

**[Figure 9](#image-fm-sideband-amplitudes-for-three-modulation-indices-at-fixed-carrier-and-message-frequencies). FM sideband amplitudes for three modulation indices at fixed carrier and message frequencies**. Original one-sided cosine-amplitude spectra for $f_c=20\,\mathrm{Hz}$ and $f_m=1\,\mathrm{Hz}$. Shading marks the instantaneous-frequency range, not a spectral cutoff. The middle modulation index is near the first zero of $J_0$; all three modeled envelopes have amplitude $A$. Only a finite set of lines is displayed.

For a nonzero [FM modulation index](fm-modulation-index.md), the ideal [frequency spectrum](frequency-spectrum.md) has infinitely many sidebands. Many become tiny, but drawing only visible lines does not make the exact [signal bandwidth](signal-bandwidth.md) finite. A useful engineering width must state a threshold or a retained-power fraction. For the complex representation, [Parseval's identity](parseval-identity.md) gives a simple check:

$$
\frac{1}{2\pi}\int_0^{2\pi}\bigl|e^{\mathrm i\beta\sin\theta}\bigr|^2\,d\theta
=\sum_{k=-\infty}^{\infty}|J_k(\beta)|^2=1.
$$

At $\beta=5$, the sum through $|k|\leq6$ is approximately $0.99356$. Retaining those complex components captures over $99\%$ of their squared magnitudes and spans $12\,\mathrm{Hz}$ from $14$ to $26\,\mathrm{Hz}$. This is a stated truncation criterion, not an exact cutoff or a universal bandwidth rule. It also explains why a diminished carrier component need not imply a diminished envelope: its contribution has been redistributed among sidebands.

## ↑ Ancestors (3)

1. [Frequency modulation](frequency-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)
