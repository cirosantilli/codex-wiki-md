<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Two source scales obtained from [dimensional analysis](../../../../../../dimensional-analysis.md) are

$$
\boxed{L_M=\frac{M_0^{3/4}}{B_0^{1/2}},\qquad L_Q=\frac{Q_0^{3/5}}{B_0^{1/5}}}.
$$

The [jet length](../../../../../../jet-length.md) $L_M$ measures how far source [momentum](../../../../../../momentum.md) remains important relative to buoyancy-generated [momentum](../../../../../../momentum.md). The [source-volume length of a turbulent plume](../../../../../../source-volume-length-of-a-turbulent-plume.md) $L_Q$ measures how far imposed source volume remains important relative to entrained volume. Numerical constants and [entrainment coefficient](../../../../../../entrainment-coefficient.md) factors depend on the chosen normalization. From the equations here the useful exact volume-growth scale is $\ell_Q=[Q_0^3/(20\alpha^4B_0)]^{1/5}$; the pure-similarity height whose flux equals $Q_0$ is $5\ell_Q/3$. A momentum crossover likewise contains a factor of order $\alpha^{-1/2}L_M$. The source radius $Q_0/\sqrt{M_0}$ is another useful geometrical combination, but it does not replace the two buoyancy/source crossover comparisons.

Integrate the differential relation from part (a) with finite source values:

$$
M^{5/2}-M_0^{5/2}=\frac{5B_0}{8\alpha}(Q^2-Q_0^2).
$$

Define

$$
\boxed{c=1-\frac{8\alpha M_0^{5/2}}{5B_0Q_0^2}}.
$$

This [plume flux-balance invariant](../../../../../../plume-flux-balance-invariant.md) rearranges to

$$
\boxed{\frac{8\alpha M^{5/2}}{5B_0Q_0^2}+c=\frac{Q^2}{Q_0^2}}.
$$

Use it to express $\sqrt M=[5B_0Q_0^2/(8\alpha)]^{1/5}[(Q/Q_0)^2-c]^{1/5}$, and substitute into $Q'=2\alpha\sqrt M$. The coefficient satisfies $(2\alpha/Q_0)^5[5B_0Q_0^2/(8\alpha)]=20\alpha^4B_0/Q_0^3$, giving

$$
\boxed{\frac1{Q_0}\frac{dQ}{dz}=\left(\frac{20\alpha^4B_0}{Q_0^3}\right)^{1/5}\left(\frac{Q^2}{Q_0^2}-c\right)^{1/5}}.
$$

With positive source fluxes, $c<1$. For $c<0$ the source has excess [momentum](../../../../../../momentum.md) relative to [pure plume balance](../../../../../../pure-plume-balance.md), so it is a momentum-dominated [forced plume](../../../../../../forced-plume.md). For $c=0$ it is already in [pure plume balance](../../../../../../pure-plume-balance.md), and the exact solution is the pure similarity translated to a finite [plume virtual origin](../../../../../../plume-virtual-origin.md). For $0<c<1$ the source has deficient [momentum](../../../../../../momentum.md) relative to its buoyancy and volume fluxes, a [lazy plume](../../../../../../lazy-plume.md). Here “forced” in the broad sense merely means finite source fluxes; this sign classification distinguishes its jet-like and lazy branches. At large height, finite $cQ_0^2/Q^2$ vanishes and every positive branch approaches [pure plume balance](../../../../../../pure-plume-balance.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
