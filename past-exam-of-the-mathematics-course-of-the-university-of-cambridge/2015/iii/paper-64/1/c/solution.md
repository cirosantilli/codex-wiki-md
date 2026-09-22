<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [Rayleigh-Jeans spectrum of a finite blackbody disk](../../../../../../rayleigh-jeans-spectrum-of-a-finite-blackbody-disk.md), the [Rayleigh-Jeans law](../../../../../../rayleigh-jeans-law.md) replaces $(e^{h\nu/(kT)}-1)^{-1}$ by $kT/(h\nu)$. Here $h$ is the [Planck constant](../../../../../../planck-constant.md) and $k$ the [Boltzmann constant](../../../../../../boltzmann-constant.md). The [multitemperature blackbody disk](../../../../../../multitemperature-blackbody-disk.md) therefore has

$$
F_\nu\sim\frac{k}{h}\nu^2\int_{r_*}^{r_{\rm out}}rT(r)\,dr,\qquad\boxed{F_\nu\propto\nu^2.}
$$

For example, setting $R=r_{\rm out}/r_*$ makes its [frequency](../../../../../../frequency.md)-independent coefficient proportional to the finite dimensionless integral

$$
T_{\rm in}r_*^2\int_1^R y^{1/4}(1-y^{-1/2})^{1/4}\,dy.
$$

Although the exact [effective temperature](../../../../../../effective-temperature.md) vanishes at the inner edge, the very narrow cold rim where the [Rayleigh-Jeans law](../../../../../../rayleigh-jeans-law.md) fails makes a negligible contribution in this limit. More formally, after dividing the integrand by $\nu^2$, the inequality $e^x-1\geq x$ bounds it by $(k/h)rT$, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) justifies the result even at that edge.

At large [radius](../../../../../../radius.md), $T\propto r^{-3/4}$, and the contribution per logarithmic interval is $r^2T\propto r^{5/4}$. **The outer disk dominates the low-[frequency](../../../../../../frequency.md) emission** because its much greater area outweighs its lower [effective temperature](../../../../../../effective-temperature.md).

For intermediate frequencies use the allowed power-law approximation to the [effective temperature](../../../../../../effective-temperature.md) and introduce

$$
x=\frac{h\nu}{kT(r)}=\frac{h\nu}{kT_{\rm in}}\left(\frac r{r_*}\right)^{3/4}.
$$

Then

$$
r\,dr=\frac43r_*^2\left(\frac{kT_{\rm in}}{h\nu}\right)^{8/3}x^{5/3}\,dx,
$$

so

$$
F_\nu\propto\nu^{1/3}\int_{h\nu/(kT_{\rm in})}^{h\nu/(kT_{\rm out})}\frac{x^{5/3}}{e^x-1}\,dx.
$$

The lower limit is much smaller than one and the upper limit much larger than one. Extending them to zero and infinity leaves a constant: near zero the integrand behaves as $x^{2/3}$, and at infinity it decays exponentially. Hence **the intermediate spectrum** is

$$
\boxed{F_\nu\propto\nu^{1/3}.}
$$

This is the [one-third spectrum of a multitemperature disk](../../../../../../one-third-spectrum-of-a-multitemperature-disk.md). Much of the emission comes from radii where $kT(r)$ is of order $h\nu$, moving inward as the [frequency](../../../../../../frequency.md) rises. With the exact inner-edge profile, a broad intermediate interval also requires [frequency](../../../../../../frequency.md) well below $kT_{\max}/h$; the supplied approximation captures its slope away from the hottest annuli.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
