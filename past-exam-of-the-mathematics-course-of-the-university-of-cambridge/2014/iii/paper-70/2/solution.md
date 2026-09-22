<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $F=F_s>0$ and constant [entrainment parameter](../../../../../entrainment-coefficient.md) $\alpha>0$. The printed integrals are normalized by $\pi$, so a [top-hat plume model](../../../../../top-hat-plume-model.md) has $Q=b^2w$, $M=b^2w^2$ and $F=b^2wg'$; the physical area is still $\pi b^2$. Keeping this normalization avoids spurious factors of $\pi$ in the flux equations.

Eliminate height between the two flux balances. The [plume flux-balance invariant](../../../../../plume-flux-balance-invariant.md) follows from

$$
\frac{dM}{dQ}=\frac{FQ}{2\alpha M^{3/2}},\qquad
\frac{d(M^{5/2})}{dQ}=\frac{5FQ}{4\alpha},
$$

so

$$
\boxed{M^{5/2}-\lambda Q^2=C,\qquad
\lambda=\frac{5F}{8\alpha},\qquad C=M_s^{5/2}-\lambda Q_s^2.}
$$

For positive fluxes, both $M$ and $Q$ increase. In particular $Q'\geq2\alpha\sqrt{M_s}>0$, so $Q\to\infty$ as $z\to\infty$. Therefore $C/(\lambda Q^2)\to0$, whatever the finite source imbalance, and $M\sim\lambda^{2/5}Q^{4/5}$. Integrating $Q'\sim2\alpha\lambda^{1/5}Q^{2/5}$ gives the attracting [similarity solution](../../../../../similarity-solution.md)

$$
\boxed{Q\sim\frac{6\alpha}{5}\left(\frac{9\alpha F}{10}\right)^{1/3}z^{5/3},\qquad
M\sim\left(\frac{9\alpha F}{10}\right)^{2/3}z^{4/3}.}
$$

This proves [attraction to pure plume similarity](../../../../../attraction-to-pure-plume-similarity.md) for physical positive source fluxes. Sources with a vanishing initial volume or [momentum flux](../../../../../momentum-flux.md) enter the positive regime immediately and can be obtained by the corresponding limiting solutions; a point buoyancy source has the same similarity form with zero virtual-origin offset. The statement assumes positive [buoyancy flux](../../../../../buoyancy-flux.md): a jet with $F=0$ is a different asymptotic problem.

Define the [plume balance parameter](../../../../../plume-balance-parameter.md)

$$
\Gamma=\frac{5FQ^2}{8\alpha M^{5/2}}.
$$

[Pure plume balance](../../../../../pure-plume-balance.md) means $\Gamma=1$ at each height, or equivalently $C=0$: momentum, buoyancy and [entrainment](../../../../../fluid-entrainment.md) have their similarity relation, even when the source has finite radius. A [forced plume](../../../../../forced-plume.md) has $\Gamma<1$, meaning excess momentum relative to this balance; a [lazy plume](../../../../../lazy-plume.md) has $\Gamma>1$, meaning insufficient momentum. The invariant ensures that the sign of the imbalance is preserved while $\Gamma\to1$. In particular, a strictly positive source remains pure at every height precisely when

$$
\boxed{M_s^{5/2}=\frac{5F_s}{8\alpha}Q_s^2.}
$$

For this source the exact solution is the same similarity form with $z$ replaced by $Z=z+z_0$. Writing $a=(9\alpha F_s/10)^{1/3}$,

$$
Q=\frac{6\alpha}{5}aZ^{5/3},\qquad M=a^2Z^{4/3},\qquad
b=\frac{Q}{\sqrt M}=\frac{6\alpha}{5}Z.
$$

Thus the [radius growth of an axisymmetric pure plume](../../../../../radius-growth-of-an-axisymmetric-pure-plume.md) is $b'=6\alpha/5$ and the [plume virtual origin](../../../../../plume-virtual-origin.md) lies at $-z_0$, with $z_0=5b_s/(6\alpha)$. Equivalently, in terms of top-hat source properties, [pure plume balance](../../../../../pure-plume-balance.md) is $g_s'b_s/w_s^2=8\alpha/5$.

For the stated source-to-source geometry, the relevant horizontal distance is $L_s$. Consequently the edge criterion is $b_m=L_s$, rather than the radius at which two expanding edges first touch. Since $b(z)=b_s+6\alpha z/5$,

$$
\boxed{z_m=\frac5{6\alpha}\left[L_s-\left(\frac{8\alpha}{5F_s}\right)^{1/5}Q_s^{3/5}\right],\qquad b_m=L_s.}
$$

Here $b_s=Q_s/\sqrt{M_s}=\lambda^{-1/5}Q_s^{3/5}$. A positive merging height requires $L_s>b_s$; equality puts it at the source, while an already wider source satisfies the geometric condition from the start. The no-interaction premise extrapolates independent plumes even though their edges would first touch earlier, when each radius is $L_s/2$.

Use $M^{5/2}=\lambda Q^2$ with $Q=b^2w$ and $M=b^2w^2$ to get $F_s=(8\alpha/5)bw^3$. The individual plume properties at the specified height are therefore

$$
\boxed{w_m=\left(\frac{5F_s}{8\alpha L_s}\right)^{1/3},\qquad
g_m'=\left(\frac{8\alpha}{5}\right)^{1/3}F_s^{2/3}L_s^{-5/3}.}
$$

The source volume flux affects the height through the virtual origin, but it does not affect these properties at a prescribed radius in an exactly [pure plume](../../../../../pure-plume.md).

For the stipulated [merger of two equal pure plumes](../../../../../merger-of-two-equal-pure-plumes.md), the new radius is $b_c=\sqrt2\,b_m$. This factor is outside $b_m$, as required by the area. Since speed and [reduced gravity](../../../../../reduced-gravity-split.md) are held fixed, the merged fluxes are $Q_c=2Q_m$, $M_c=2M_m$ and $F_c=2F_s$. Their balance parameter is

$$
\boxed{\Gamma_c=\frac{5(2F_s)(2Q_m)^2}{8\alpha(2M_m)^{5/2}}=\sqrt2>1.}
$$

**The immediate combined plume is lazy.** The same result follows from $\Gamma=5g'b/(8\alpha w^2)$: enlarging the radius at fixed $g',w$ increases this parameter.

At fixed $w_m,g_m'$, the radius required for [pure plume balance](../../../../../pure-plume-balance.md) is

$$
\boxed{b_p=\frac{8\alpha w_m^2}{5g_m'}=b_m=L_s,\qquad \pi b_p^2=\pi L_s^2.}
$$

That is half the stipulated combined area $2\pi L_s^2$. This [fixed-speed pure-plume merger and flux conservation](../../../../../fixed-speed-pure-plume-merger-and-flux-conservation.md) comparison exposes the limitation of demanding immediate pure balance with unchanged speed and [reduced gravity](../../../../../reduced-gravity-split.md): reducing the area to this value would also halve all three merged fluxes. A conservative merger must instead adjust its properties and begin out of pure balance. Under the given constant-entrainment equations, the resulting [lazy plume](../../../../../lazy-plume.md) subsequently approaches the attracting [similarity solution](../../../../../similarity-solution.md) with total [buoyancy flux](../../../../../buoyancy-flux.md) $2F_s$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
