<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Specify the path convention before integrating the [neutral-hydrogen column-density distribution](../../../../../../neutral-hydrogen-column-density-distribution.md). Write $f_z=\partial^2\mathcal N/(\partial N\partial z)$ and $f_X=\partial^2\mathcal N/(\partial N\partial X)$, with [absorption distance](../../../../../../absorption-distance.md) satisfying

$$
\frac{dX}{dz}=\frac{H_0}{H(z)}(1+z)^2,\qquad f_z=f_X\frac{dX}{dz}.
$$

The lower panel of the preceding sketch shows the approximate decrease of $f$ with $N=N_{\rm HI}$ near $z=3$. Ordinary forest columns are roughly described by $f\propto N^{-\beta}$, $\beta\sim1.5$, but the slope changes through partially shielded [Lyman limit systems](../../../../../../lyman-limit-system.md) and high-column [damped Lyman-alpha systems](../../../../../../damped-lyman-alpha-system.md). No single slope should be extrapolated through all these regimes. In logarithmic bins the number is $N\ln(10)f$, whereas their neutral mass contribution is proportional to $N^2f$; confusing these two weightings would give a wrong baryon inventory.

To derive the [neutral gas density from an absorption distribution](../../../../../../neutral-gas-density-from-an-absorption-distribution.md), a redshift interval $dz$ has proper light-path length $d\ell=c\,dz/[(1+z)H]$. The sum of neutral [hydrogen](../../../../../../hydrogen.md) columns per path length estimates the mean proper number density:

$$
\overline n_{\rm HI}(z)=\frac{(1+z)H(z)}c\int Nf_z(N,z)\,dN.
$$

The proper [mass density](../../../../../../density.md) is $m_H\overline n_{\rm HI}$; division by $(1+z)^3$ converts it to a comoving mass density. Thus, with today's [critical density](../../../../../../critical-density.md) $\rho_{\rm crit,0}=3H_0^2/(8\pi G)$,

$$
\boxed{\Omega_{\rm HI}(z)=\frac{m_HH(z)}{c\rho_{\rm crit,0}(1+z)^2}\int Nf_z\,dN
=\frac{H_0m_H}{c\rho_{\rm crit,0}}\int Nf_X\,dN.}
$$

A representative finite-sample estimator replaces the last integral by $\sum_j N_j/\Delta X$, with completeness and selection corrections. This defines a comoving inventory divided by today's [critical density](../../../../../../critical-density.md); a fraction of the instantaneous critical density has a different normalization. Neutral gas including accompanying helium is obtained by multiplying by a specified mass correction, approximately $1.3$; hydrogen-only $\Omega_{\rm HI}$ must not silently include it.

At $z\sim3$ the observed neutral inventory is of order $10^{-3}$, far below the [cosmological baryon density](../../../../../../cosmological-baryon-density.md) of order $0.04$–$0.05$ for $h\sim0.7$. High-column [damped Lyman-alpha systems](../../../../../../damped-lyman-alpha-system.md) contribute most of this neutral mass although weak forest lines dominate the counts; for $\beta=1.5$ the mass per logarithmic column interval increases as $N^{1/2}$ in the forest regime. The small neutral inventory therefore does not imply a small total gas inventory: the [intergalactic medium](../../../../../../intergalactic-medium.md) contains a large ionized baryon reservoir invisible to a neutral-only count. Recovering that reservoir requires an ionization correction and a gas-density model. The survey normalization and high-column contribution are described in [the neutral-gas inventory analysis](https://ned.ipac.caltech.edu/level5/Sept05/Wolfe/Wolfe2.html).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
