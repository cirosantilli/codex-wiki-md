<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Polydispersity](../../../../polydispersity.md) means that a sample contains chains of different [molar masses](../../../../molar-mass.md) or lengths. Let $n_i$ count chains with [molar mass](../../../../molar-mass.md) $M_i$. The [number-average molar mass](../../../../number-average-molar-mass.md) gives every chain equal weight, while the [weight-average molar mass](../../../../weight-average-molar-mass.md) weights a chain population by its contribution to total [mass](../../../../mass.md):

$$
\boxed{M_n=\frac{\sum_i n_iM_i}{\sum_i n_i},\qquad
M_w=\frac{\sum_i n_iM_i^2}{\sum_i n_iM_i}.}
$$

Writing $w_i=n_iM_i/\sum_jn_jM_j$ makes the latter interpretation explicit: $M_w=\sum_iw_iM_i$. Large chains therefore influence $M_w$ more strongly. If brackets denote an average over chain number,

$$
\frac{M_w}{M_n}=\frac{\langle M^2\rangle}{\langle M\rangle^2}
=1+\frac{\operatorname{Var}(M)}{\langle M\rangle^2}\geq1.
$$

The ratio is [molar-mass dispersity](../../../../molar-mass-dispersity.md), conventionally written Đ. It equals one only when every chain has the same [molar mass](../../../../molar-mass.md). Different distributions can share the same ratio, so it does not specify the full distribution.

For a [freely jointed chain](../../../../ideal-chain.md), write the end-to-end vector as the sum of $N$ independently oriented steps $\mathbf b_i$, each of fixed length $a$. [Isotropy](../../../../isotropy.md) gives $\langle\mathbf b_i\rangle=\mathbf0$, and [independence](../../../../independent-random-variables.md) gives $\langle\mathbf b_i\cdot\mathbf b_j\rangle=0$ for $i\ne j$. Hence

$$
\langle R^2\rangle=
\sum_{i,j=1}^N\langle\mathbf b_i\cdot\mathbf b_j\rangle
=\sum_{i=1}^N a^2,
\qquad \boxed{\langle R^2\rangle=Na^2.}
$$

The root-mean-square [end-to-end distance of a polymer chain](../../../../end-to-end-distance-of-a-polymer-chain.md) is $a\sqrt N$, although the mean vector is zero. Its [polymer contour length](../../../../polymer-contour-length.md) is $L=Na$, an upper bound on extension; it is not the typical unforced end-to-end length.

Stiffness correlates neighboring bond directions, so the discarded cross terms need not vanish. A [freely rotating chain](../../../../freely-rotating-chain.md) fixes the angle $\theta$ between successive forward bond vectors but leaves torsion uniformly distributed. Set $q=\cos\theta$, so $\langle\mathbf b_i\cdot\mathbf b_{i+s}\rangle=a^2q^s$. Then

$$
\langle R^2\rangle=Na^2+2a^2\sum_{s=1}^{N-1}(N-s)q^s
=Na^2\left[\frac{1+q}{1-q}
-\frac{2q(1-q^N)}{N(1-q)^2}\right],\qquad |q|<1.
$$

For a chain long compared with its orientational correlation range, the [characteristic ratio of a freely rotating chain](../../../../characteristic-ratio-of-a-freely-rotating-chain.md) approaches $C_\infty=(1+q)/(1-q)$. Positive forward persistence increases the mean-square size and gives the [Kuhn length of a freely rotating chain](../../../../kuhn-length-of-a-freely-rotating-chain.md) $b_K=aC_\infty$. A chemical internal bond angle is supplementary to the forward-vector angle used here, so substituting that internal angle requires $q=-\cos\theta_{\rm internal}$. For $q\to1$ at fixed $N$, the finite sum tends to $N^2a^2$, the rigid-rod result; taking the long-chain limit first would incorrectly predict an unbounded size. Real torsional energy preferences can be represented by a [rotational isomeric state model](../../../../rotational-isomeric-state-model.md), with weighted torsional states and correlations beyond independent free rotations.

A [worm-like chain](../../../../worm-like-chain.md) describes continuously varying local orientation. For unit tangent $\mathbf t(s)$ and bending stiffness $\kappa$, its elastic [energy](../../../../energy-split.md) is $E_b=(\kappa/2)\int_0^L|d\mathbf t/ds|^2ds$. In three spatial dimensions the [persistence length](../../../../persistence-length.md) is $\ell_p=\kappa/(k_BT)$ and

$$
\langle\mathbf t(s)\cdot\mathbf t(s')\rangle=e^{-|s-s'|/\ell_p}.
$$

Since $\mathbf R=\int_0^L\mathbf t(s)\,ds$, integrating the tangent correlation gives the [end-to-end distance of a worm-like chain](../../../../end-to-end-distance-of-a-worm-like-chain.md):

$$
\boxed{\langle R^2\rangle=
2\ell_pL-2\ell_p^2(1-e^{-L/\ell_p}).}
$$

For $L\ll\ell_p$, expansion gives $\langle R^2\rangle=L^2-L^3/(3\ell_p)+\cdots$, approaching a straight rod. For $L\gg\ell_p$, it gives $\langle R^2\rangle\simeq2\ell_pL$, the long-chain [ideal chain](../../../../ideal-chain.md) result with [Kuhn length](../../../../kuhn-length.md) $2\ell_p$. These models isolate stiffness; long-range [excluded volume](../../../../excluded-volume.md) can additionally swell an isolated chain in a [good solvent](../../../../good-solvent.md). When coarse-graining, a chemical repeat count and a count of independent statistical steps must not be silently interchanged.

<a id="4/image-stiff-chain-crossover-and-distinct-polymer-brush-density-scalings"></a>
![](../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1-chain-and-brush-scaling.png)

**[Figure 4](#4/image-stiff-chain-crossover-and-distinct-polymer-brush-density-scalings). Stiff-chain crossover and distinct polymer brush density scalings**.

The first panel shows the exact [worm-like chain](../../../../worm-like-chain.md) crossover between a rod and a long flexible coil. The second compares original normalized scaling curves for a uniform [polymer brush](../../../../polymer-brush.md); their prefactors have been chosen for illustration and do not fit the exam's experimental points.

For a [good solvent](../../../../good-solvent.md), consider long flexible [grafted polymer chains](../../../../grafted-polymer-chain.md) with [grafting density](../../../../grafting-density.md) $\sigma$ and lateral spacing $D\sim\sigma^{-1/2}$. At high coverage, $D$ is smaller than the isolated coil size, and adjacent chains cannot retain their unperturbed conformations. A scaling model divides each chain into [concentration blobs](../../../../concentration-blob.md) of diameter $D$. Inside one blob the chain retains good-solvent statistics,

$$
D\sim ag^{3/5},\qquad g\sim(D/a)^{5/3},
$$

using the [Flory approximation](../../../../flory-approximation.md) exponent $3/5$. The $N/g$ blobs per chain form a stretched sequence approximately normal to the surface. The [good-solvent brush height](../../../../good-solvent-brush-height.md) therefore obeys

$$
h\sim\frac NgD\sim Na^{5/3}D^{-2/3},\qquad
\boxed{h\sim Na(\sigma a^2)^{1/3}.}
$$

Here $a$ and $N$ refer to consistently chosen effective segments, whose microscopic properties are held fixed as chain length changes. The result is a scaling law with an undetermined order-one prefactor, not a fully specified height in nanometres.

A complementary free-energy balance per chain is

$$
\frac{F}{k_BT}\sim\frac{h^2}{Na^2}+\frac{vN^2\sigma}{h},
$$

where $v>0$ is effective segment [excluded volume](../../../../excluded-volume.md). The first term is the chain [entropy](../../../../entropy-split.md) cost of stretching and the second is the cost of crowding segments into a layer of volume $h/\sigma$ per chain. Minimization gives $h^3\sim vN^3a^2\sigma$; with $v\sim a^3$ it recovers the same height. The blob argument incorporates good-solvent correlations more directly. Both descriptions require overlapping chains, many segments per chain, and heights below the [polymer contour length](../../../../polymer-contour-length.md); the power law cannot be extrapolated to infinite grafting density.

In the printed experimental graph, the vertical axis is $hD^2/(10^6\,\mathrm{\mathring A^3})$ and the horizontal axis is $M/10^5$. The approximately straight trend through the origin therefore means **$hD^2\propto M$**. Since $D^{-2}\sim\sigma$ and $M$ is proportional to chain length for a fixed repeat chemistry,

$$
\boxed{h\propto M\sigma\propto N\sigma\qquad\text{(poor solvent).}}
$$

The dashed guide rises by roughly $1.8$–$1.9$ vertical units over six horizontal units, corresponding to $hD^2/M$ of order $3\,\mathrm{\mathring A^3}$ per unit of the plotted $M$. This is an approximate graphical slope, not a fitted material constant; the graph does not specify a numerical monomer count or a repeat-unit volume from which an absolute brush height could independently be calculated.

The [poor-solvent brush height](../../../../poor-solvent-brush-height.md) has a simple volume argument. Let $v_0$ be the volume per repeat and $\phi$ the roughly fixed polymer [volume fraction](../../../../volume-fraction.md) within a dense uniform layer. There are $N\sigma$ repeats per substrate [area](../../../../surface-area.md), so

$$
\phi h=N\sigma v_0,\qquad
\boxed{h\simeq\frac{Nv_0\sigma}{\phi}.}
$$

For fixed poor-solvent conditions, $\phi$ is approximately independent of $N$ and $\sigma$, giving the observed linear grafting-density dependence. Polymer–polymer contacts are favored and the layer becomes relatively compact; in a [good solvent](../../../../good-solvent.md), favorable solvent contact and segment repulsion instead produce a swollen layer whose stretching and osmotic costs balance at the weaker $\sigma^{1/3}$ dependence. Sparse isolated [polymer globules](../../../../polymer-globule.md) or lateral segregation fall outside the uniform-brush model.

The cited experimental paper's abstract independently reports these two scaling laws, but identifies polydimethylsiloxane chains on porous [silicon dioxide](../../../../silicon-dioxide.md), rather than the [polystyrene](../../../../polystyrene.md) system named in the exam. The solution uses the printed axes to infer the exponents and does not treat that material identification as verified experimental provenance.[Physical Review Letters 66 (1991), 719–722, abstract: neutron-scattering measurement, chemical system, and good- versus poor-solvent thickness scaling](../../../../characterization-of-the-brush-regime-for-grafted-polymer-layers-at-the-solid-liquid-interface-by-p-auroy-and-others.md)

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
