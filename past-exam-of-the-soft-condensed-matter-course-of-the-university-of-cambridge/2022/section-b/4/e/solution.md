<h1 id="section-b/4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

During slow peeling in [atomic force microscopy](../../../../../atomic-force-microscopy.md), $n$ adjusts to minimize the [Helmholtz free energy](../../../../../helmholtz-free-energy.md) at each imposed height. Define the positive binding gain $\mu=k_BT[\epsilon b/\xi-(b/\xi)^2]$ for the adsorbed segment. The [stationary point](../../../../../stationary-point.md) satisfies

$$
0=\left(\frac{\partial F}{\partial n}\right)_z
=\mu-\frac{3k_BTz^2}{2b^2n^2},\qquad
n_*(z)=\frac zb\sqrt{\frac{3k_BT}{2\mu}}.
$$

Since $\partial_n^2F=3k_BTz^2/(b^2n^3)>0$, this is a minimum while $0<n_*<N$. The upward pulling [force](../../../../../force-split.md) is the height [derivative](../../../../../derivative.md) of the minimized [free energy](../../../../../thermodynamic-free-energy.md). The implicit $n_*(z)$ term vanishes because $\partial_nF=0$, giving

$$
f=\frac{dF(n_*(z),z)}{dz}
=\frac{3k_BTz}{b^2n_*}
=\frac{\sqrt{6k_BT\mu}}b.
$$

Using $\xi=2b/\epsilon$,

$$
\boxed{f_{\mathrm{peel}}=\sqrt{\frac32}\,\frac{\epsilon k_BT}{b}.}
$$

It is independent of $z$: extra pulling height releases more [monomers](../../../../../monomer.md) while leaving the fractional extension of the stretched part unchanged. Equivalently $F_{\min}=-N\mu+f_{\mathrm{peel}}z$. This is the [equilibrium peeling force of an adsorbed Gaussian chain](../../../../../equilibrium-peeling-force-of-an-adsorbed-gaussian-chain.md).

The plateau ends when $n_*=N$, at

$$
z_{\mathrm{det}}=Nb\sqrt{\frac{2\mu}{3k_BT}}=\frac{Nb\epsilon}{\sqrt6}.
$$

Thereafter all [monomers](../../../../../monomer.md) are detached and the [Gaussian chain](../../../../../gaussian-chain.md) force is $f=3k_BTz/(Nb^2)$, agreeing continuously with the plateau at $z_{\mathrm{det}}$. Very near the start and final release, finite-chain and junction effects lie outside the blob approximation.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
