<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The numerical contour length is $L=Nb_0=10^{10}\times10^{-8}\,\mathrm m=100\,\mathrm m$, and $k_BT=4.14\times10^{-21}\,\mathrm J$. Begin with a three-dimensional [freely jointed chain](../../../../../../ideal-chain.md) in which each chemical [monomer](../../../../../../monomer.md) is also an independent statistical link of length $b_0$. This neglects [excluded volume](../../../../../../excluded-volume.md), hydrodynamic effects on equilibrium statistics, and stretching of the chemical backbone.

An applied [force](../../../../../../force.md) $F$ gives a one-link [canonical partition function](../../../../../../canonical-partition-function.md)

$$
Z_1=2\pi\int_{-1}^{1}e^{\xi u}du=4\pi\frac{\sinh\xi}{\xi},\qquad \xi=\frac{Fb_0}{k_BT}.
$$

The mean extension is $z=k_BT\partial_F\log Z_1^N=Nb_0(\coth\xi-1/\xi)$. Expanding the [Langevin function](../../../../../../langevin-function.md) at small [force](../../../../../../force.md) gives $z=Nb_0^2F/(3k_BT)+O(F^3)$. The [three-dimensional entropic chain stiffness](../../../../../../three-dimensional-entropic-chain-stiffness.md) is thus

$$
\boxed{k_s=\frac{3k_BT}{Nb_0^2}=1.242\times10^{-14}\,\mathrm{N\,m^{-1}}.}
$$

The unforced root-mean-square end-to-end distance is $\sqrt N b_0=10^{-3}\,\mathrm m$, not the contour length. This response is entropic straightening of a fluctuating coil. Axial stretching of a straight material rod instead has stiffness $EA/L$, and is a different phenomenon. Aqueous solvent does not by itself prove ideal-chain statistics: a good-solvent [self-avoiding walk](../../../../../../self-avoiding-walk.md) has a different coil size and susceptibility. The estimate above states explicitly the model under which the supplied link data suffice.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
