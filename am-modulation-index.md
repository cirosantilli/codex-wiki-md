# AM modulation index

↑ **Parent:** [Amplitude modulation](amplitude-modulation.md)

In the single-[sinusoid](sinusoid.md) [AM](amplitude-modulation.md) voltage model, $m$ is the peak fractional excursion of the signed multiplying factor from its mean value $1$. At $m=0$ there is only the [carrier wave](carrier-wave.md); at $m=0.5$ its multiplying factor ranges from $0.5$ to $1.5$; at $m=1$ it just touches zero. For $0\leq m\leq1$, the [wave envelope](envelope-waves.md) extrema are

$$
E_{\max}=A(1+m),\qquad E_{\min}=A(1-m),\qquad
m=\frac{E_{\max}-E_{\min}}{E_{\max}+E_{\min}}.
$$

The last equality follows by adding and subtracting the first two. An [oscilloscope](oscilloscope.md) estimate uses local carrier peaks near the message extrema and needs enough carrier cycles to approximate those bounds. Consistent local [peak-to-peak amplitude](peak-to-peak-amplitude.md) readings give the same ratio because their common factor of two cancels. Mixing a peak reading with a peak-to-peak reading does not.

For $A=2\,\mathrm V$ and $m=0.5$, the [wave envelope](envelope-waves.md) ranges from $1$ to $3\,\mathrm V$, giving $(3-1)/(3+1)=0.5$. These are model values. At $m=1.4$, the signed factor has minimum $-0.4$, but the nonnegative [wave envelope](envelope-waves.md) reaches zero at its sign changes; the extrema formula would misleadingly report $1$. It cannot measure the true depth of [overmodulation](overmodulation.md) from the folded envelope alone.

## ↑ Ancestors (3)

1. [Amplitude modulation](amplitude-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Amplitude modulation](amplitude-modulation.md)
