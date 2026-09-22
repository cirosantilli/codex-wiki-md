<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Meaning of the mixing [free energy](../../../thermodynamic-free-energy.md).** The supplied expression is the [Flory–Huggins solution theory](../../../flory-huggins-solution-theory.md) mixing [free energy](../../../thermodynamic-free-energy.md) _per lattice site_, or per solvent-sized reference cell. Although the question calls it “per particle,” it cannot mean per [polymer](../../../polymer-split.md) molecule: one chain occupies $N$ sites. Let the site volume be $v_0$, the total number of sites be $M=V/v_0$, and the chain and solvent counts be $n_p,n_s$, so

$$
M=Nn_p+n_s,\qquad\phi=\frac{Nn_p}{M},\qquad F_{\rm mix}=Mk_BT\,g(\phi),
$$

where

$$
g(\phi)=\frac\phi N\ln\phi+(1-\phi)\ln(1-\phi)+\chi\phi(1-\phi).
$$

The first term is the [polymer](../../../polymer-split.md)'s translational [entropy of mixing](../../../entropy-of-mixing.md). Its factor $1/N$ expresses that $N$ connected segments translate as one molecule. The second is the solvent's translational mixing [entropy](../../../entropy-split.md). Both are negative in the mixing [free energy](../../../thermodynamic-free-energy.md) for $0<\phi<1$, favoring mixing.

The final term is a mean-field excess contact contribution. The [Flory interaction parameter](../../../flory-interaction-parameter.md) $\chi$ measures the relative preference for unlike polymer-solvent contacts compared with like contacts. In the simplest lattice model with coordination number $z$ and pair energies $\epsilon_{ps},\epsilon_{pp},\epsilon_{ss}$,

$$
\chi=\frac z{k_BT}\left[\epsilon_{ps}-\frac{\epsilon_{pp}+\epsilon_{ss}}2\right].
$$

Positive $\chi$ penalizes unlike contacts and promotes separation; negative $\chi$ favors them. Effective real-solution values can also include non-enthalpic effects, so their [temperature](../../../temperature-split.md) dependence need not be exactly a constant divided by $T$. The subsequent derivatives assume composition-independent $\chi$ as in the supplied model.

**[Osmotic pressure](../../../osmotic-pressure.md) and the special value one half.** At fixed chain count, $\partial\phi/\partial V=-\phi/V$. Differentiating $F_{\rm mix}=(V/v_0)k_BTg(\phi)$ with respect to volume, relative to the pure-solvent reference, gives

$$
\pi=\frac{k_BT}{v_0}[\phi g'(\phi)-g(\phi)].
$$

The resulting [osmotic pressure in Flory-Huggins solution theory](../../../osmotic-pressure-in-flory-huggins-solution-theory.md) is

$$
\boxed{\frac{\pi v_0}{k_BT}
=-\ln(1-\phi)-\left(1-\frac1N\right)\phi-\chi\phi^2
=\frac\phi N+\left(\frac12-\chi\right)\phi^2
+\frac{\phi^3}{3}+O(\phi^4).}
$$

The leading term is the ideal [osmotic pressure](../../../osmotic-pressure.md) of chains, since their [number density](../../../number-density.md) is $\phi/(Nv_0)$. At $\chi=1/2$ the second-virial term vanishes: effective two-segment attraction and excluded-volume repulsion balance. This is the [theta solvent](../../../theta-solvent.md) condition for a sufficiently long dilute chain; the positive third-order contribution remains, so a finite-concentration solution is not a completely noninteracting gas. The site-volume factor is necessary to give physical [pressure](../../../pressure-split.md) units.

For $\chi<1/2$, the effective pair [excluded volume](../../../excluded-volume.md) is positive. In a [good solvent](../../../good-solvent.md), the isolated chain expands relative to a Gaussian coil, with $R\sim bN^\nu$, $\nu\simeq0.588$ or $3/5$ in the [Flory approximation](../../../flory-approximation.md). For $\chi>1/2$, attraction wins in a [poor solvent](../../../poor-solvent.md) and a sufficiently long chain collapses toward a dense [polymer globule](../../../polymer-globule.md), with asymptotic size $R\propto N^{1/3}$. Close to the theta condition, finite-chain crossover effects matter. At $\chi=1/2$, $R\sim bN^{1/2}$ to leading scaling order. This theta criterion is not the exact finite-$N$ phase-separation critical point; the lattice model has $\phi_c=1/(1+\sqrt N)$ and $\chi_c=(1+1/\sqrt N)^2/2$.

**Overlap concentration.** The [polymer overlap concentration](../../../polymer-overlap-concentration.md) is reached when there is roughly one isolated coil in its own pervaded volume. If the coil size is $R$ and a [repeat unit](../../../repeat-unit.md) occupies volume $v_0$,

$$
\phi^*\sim\frac{Nv_0}{R^3}.
$$

With $R\sim bN^\nu$, the general scaling law is

$$
\boxed{\phi^*\sim\frac{v_0}{b^3}N^{1-3\nu}.}
$$

The usual single-segment-volume estimate $v_0\sim b^3$ gives $\phi^*\sim N^{1-3\nu}$: $N^{-1/2}$ in a [theta solvent](../../../theta-solvent.md), approximately $N^{-4/5}$ in a [good solvent](../../../good-solvent.md), and order one for compact globules. A coil has no sharp surface, so choosing a [radius of gyration](../../../radius-of-gyration.md) or a geometric coil volume changes numerical prefactors.

For the stated [polystyrene](../../../polystyrene.md) at $N=1500$ and $\chi=1/2$, the conventional scaling estimate is

$$
\boxed{\phi^*\sim N^{-1/2}=1500^{-1/2}=0.0258\simeq2.6\%.}
$$

This is a volume-fraction estimate, not a molar concentration. It uses the implicit site-volume approximation; the question does not provide an independent repeat-unit volume to determine a more precise prefactor.

**Semidilute length scale.** Beyond overlap, a [semidilute polymer solution](../../../semidilute-polymer-solution.md) is characterized locally by a [concentration blob](../../../concentration-blob.md) size $\xi$. Suppose one blob contains $g$ statistical units. At the theta condition the subchain is Gaussian, so $\xi\sim b\sqrt g$, while matching its internal concentration to the bulk gives $\phi\sim gv_0/\xi^3$. Eliminating $g$ gives the [concentration-blob size in a theta solvent](../../../concentration-blob-size-in-a-theta-solvent.md):

$$
\boxed{\xi\sim\frac{v_0}{b^2\phi}\sim\frac b\phi
\quad\text{when }v_0\sim b^3.}
$$

Using the supplied [statistical step length](../../../statistical-segment-length.md) $b=0.67\,\mathrm{nm}$ and $\phi=0.05$,

$$
\boxed{\xi\sim\frac{0.67}{0.05}\,\mathrm{nm}=13.4\,\mathrm{nm}\simeq13\,\mathrm{nm}.}
$$

The same convention gives $g\sim\phi^{-2}=400<N=1500$, and the whole [ideal chain](../../../ideal-chain.md) has $R\sim b\sqrt N\simeq26\,\mathrm{nm}$. Thus the blob is smaller than the chain. Because $\phi/\phi^*\simeq1.94$ is only modestly above overlap, the value is a scaling estimate in a crossover region, not a precision asymptotic measurement. A [statistical step length](../../../statistical-segment-length.md) is not automatically a physical monomer diameter: if $v_0$ differs from $b^3$, the more general estimates are $\phi^*\sim(v_0/b^3)N^{-1/2}$ and $\xi\sim v_0/(b^2\phi)$, with the missing prefactor left explicit.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2017](../../2017-split.md)
3. [Past exam of the soft condensed matter course of the University of Cambridge](../../split.md)
4. [Soft Condensed Matter course of the University of Cambridge](../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
