<h1 id="section-a-ii/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [positive photoresist](../../../../../../positive-photoresist.md), let $D_0$ be the largest exposure preserving the initial film thickness and $D_c$ the clearing dose. The [photoresist contrast](../../../../../../photoresist-contrast.md) is $\gamma=1/\log_{10}(D_c/D_0)$. An aerial image $I=\bar I[1+M\cos(2\pi\nu x)]$ can clear its maxima while retaining its minima only if

$$
\frac{1+M}{1-M}\geq\frac{D_c}{D_0}=10^{1/\gamma},\qquad
M\geq M_c=\frac{10^{1/\gamma}-1}{10^{1/\gamma}+1}.
$$

Thus $M_c=0.6991$ and $0.2006$ for the lower- and higher-contrast materials. Reading those levels on the supplied [modulation transfer function](../../../../../../modulation-transfer-function.md) gives **maximum normalized [spatial frequencies](../../../../../../spatial-frequency.md) approximately $\nu/\nu_0=0.40$ and $0.60$**, respectively. The stated partial coherence is already represented by that curve; do not multiply the read [frequencies](../../../../../../frequency.md) by another coherence factor.

The unambiguous pattern dimensions are full pitch $P=1/(x\nu_0)$ and equal line/space width $w=P/2$, where $x$ is the read normalized [frequency](../../../../../../frequency.md). To convert the paper's Rayleigh-frequency label into [lengths](../../../../../../length.md), explicitly use the circular-pupil [Rayleigh criterion](../../../../../../rayleigh-criterion.md) $d_R=0.61\lambda/NA$ and $\nu_0=1/d_R$. With the ArF vacuum wavelength $193\ \mathrm{nm}$ and the stated [numerical aperture](../../../../../../numerical-aperture.md), $d_R=235.5\ \mathrm{nm}$, giving

$$
\begin{array}{c|cc}
\gamma&P\ (\mathrm{\mu m})&w\ (\mathrm{\mu m})\\\hline
1.33&0.589&0.294\\
5.66&0.392&0.196
\end{array}
$$

**The higher-contrast material resolves a line/space feature about two-thirds as wide.** The pitch and half-pitch distinction matters: the point-separation [Rayleigh criterion](../../../../../../rayleigh-criterion.md) is not itself an equal-line/space width. If a course defines $\nu_0$ as an optical cutoff rather than $1/d_R$, use that specified [frequency](../../../../../../frequency.md) in $w=1/(2x\nu_0)$; the normalized graph readings and their ratio are unchanged. No absolute clearing dose is provided.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Section A(ii)](../../../section-a-ii.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
