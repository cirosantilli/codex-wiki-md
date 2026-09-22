<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the two populations have settling speeds $w_1\gg w_2>0$ and [particle volume fractions](../../../../../../particle-volume-fraction.md) $c_1,c_2$. In the same mixed box their scalar equations are $\dot c_j=-w_jc_j/h$, while the common [reduced gravity](../../../../../../reduced-gravity-split.md) is $g'=b_1c_1+b_2c_2$ after neglecting thermal [buoyancy](../../../../../../buoyancy.md). Both populations are carried by the same radius and depth:

$$
\dot R=\mathsf F\sqrt{(b_1c_1+b_2c_2)h},\qquad h=\mathcal V/(\pi R^2).
$$

The coarse ash deposits rapidly near the source; the fine ash remains aloft longer, sustains the current's [buoyancy](../../../../../../buoyancy.md) and is carried farther. The composition of the deposit therefore fines outward. Since the remaining fine ash drives the flow transporting both classes, the runout is not obtained by superposing two independent monodisperse currents.

Define the [settling exposure for a particle size distribution](../../../../../../settling-exposure-for-a-particle-size-distribution.md) $J=\int_0^t ds/h(s)$. Then $c_j=c_{j0}e^{-w_jJ}$ and

$$
R_\infty^4-R_0^4=4\mathsf F(\mathcal V/\pi)^{3/2}\int_0^\infty\sqrt{b_1c_{10}e^{-w_1J}+b_2c_{20}e^{-w_2J}}\,dJ.
$$

The [integral](../../../../../../integral.md) is finite when both settling speeds are positive. Each deposited mass is $\Sigma_j(r)=\rho_{pj}w_j\int_{t_a(r)}^\infty c_j(t)\,dt$; their sum is the total deposit, with a coarse proximal component and a finer distal tail. If the actual hot-gas [density](../../../../../../density.md) deficit is retained, early loss of coarse ash can make $g'$ vanish and loft the remaining fine-rich cloud, shortening its ground-hugging reach relative to this particle-only calculation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
