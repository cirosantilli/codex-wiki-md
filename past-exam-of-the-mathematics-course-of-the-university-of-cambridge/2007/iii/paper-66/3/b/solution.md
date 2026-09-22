<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To derive the [nonrelativistic electron-degeneracy pressure in a hydrogen-helium mixture](../../../../../../nonrelativistic-electron-degeneracy-pressure-in-a-hydrogen-helium-mixture.md), take fully ionized [hydrogen](../../../../../../hydrogen.md) and [helium](../../../../../../helium.md) with [hydrogen mass fraction](../../../../../../hydrogen-mass-fraction.md) $X$, the [Electron](../../../../../../electron.md) [number density](../../../../../../number-density.md) is

$$
n_e=\frac{X\rho}{m_p}+2\frac{(1-X)\rho}{4m_p}=\frac{(1+X)\rho}{2m_p}.
$$

Here [helium](../../../../../../helium.md) nuclei have [mass](../../../../../../mass.md) $4m_p$ in the approximation used in the question. Filling the two spin states of each [momentum](../../../../../../momentum.md) mode up to the [Fermi momentum](../../../../../../fermi-momentum.md) $p_0$ gives

$$
n_e=\int_0^{p_0}\frac{8\pi p^2}{h^3}dp=\frac{8\pi p_0^3}{3h^3},\qquad p_0=h\left(\frac{3n_e}{8\pi}\right)^{1/3}.
$$

The isotropic [momentum](../../../../../../momentum.md) flux gives [pressure](../../../../../../pressure.md) $\frac13\int pv\,dn$. For nonrelativistic [Electrons](../../../../../../electron.md) $v=p/m_e$, so the [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md) is

$$
\begin{aligned}
P_e&=\frac13\int_0^{p_0}\frac{p^2}{m_e}\frac{8\pi p^2}{h^3}dp=\frac{8\pi p_0^5}{15m_eh^3}\\
&=\frac{h^2}{5m_e}\left(\frac3{8\pi}\right)^{2/3}n_e^{5/3}.
\end{aligned}
$$

Substitute the composition-dependent $n_e$ and simplify powers of two:

$$
\boxed{P_e=K\rho^{5/3},\qquad K=\left(\frac3{2\pi}\right)^{2/3}\frac{h^2(1+X)^{5/3}}{40m_em_p^{5/3}}.}
$$

Comparing $5/3=1+1/n$ gives **the [polytropic index](../../../../../../polytropic-index.md) $n=3/2$**. The result assumes complete [Electron](../../../../../../electron.md) degeneracy, $p_0\ll m_ec$, and negligible nuclear [mass](../../../../../../mass.md) corrections.

Now adopt the stated approximate partially degenerate [equation of state](../../../../../../equation-of-state.md), keeping composition and hence $K,\mu$ fixed during contraction. Set $q=m/M$ and define the mass-averaged [temperature](../../../../../../temperature.md) $\overline T_M=\int_0^1T\,dq$. The [stellar virial theorem](../../../../../../stellar-virial-theorem.md) from part (a) gives

$$
3K\int_0^1\rho^{2/3}dq+\frac{3\mathcal R}{\mu}\overline T_M=-\frac{\Omega}{M}.
$$

For an index-$3/2$ [stellar polytrope](../../../../../../stellar-polytrope.md), the permitted gravitational-energy formula is $\Omega=-6GM^2/(7R)$. Also, using $\bar\rho=3M/(4\pi R^3)$,

$$
\rho^{2/3}=\frac{M^{2/3}}{R^2}\left(\frac{3\rho}{4\pi\bar\rho}\right)^{2/3}.
$$

Thus, with $A=3K\int_0^1[3\rho/(4\pi\bar\rho)]^{2/3}dq$,

$$
\boxed{\overline T_M=\frac{2\mu GM}{7\mathcal RR}-\frac{\mu A M^{2/3}}{3\mathcal RR^2}.}
$$

The normalized [density](../../../../../../density.md) $\rho/\bar\rho$ is a fixed function of $q$ for this homologous polytropic structure. Therefore its integral and $K$ fix $A$, which is independent of $M$ and $R$ for a common composition. The mean here is mass-weighted, rather than a volume average.

For the [mass-averaged temperature maximum in a partially degenerate polytrope](../../../../../../mass-averaged-temperature-maximum-in-a-partially-degenerate-polytrope.md), put $\alpha=2\mu GM/(7\mathcal R)$ and $\delta=\mu A M^{2/3}/(3\mathcal R)$, both positive. As a function of $s=1/R$ the [temperature](../../../../../../temperature.md) is the concave quadratic

$$
\overline T_M=\alpha s-\delta s^2=\frac{\alpha^2}{4\delta}-\delta\left(s-\frac\alpha{2\delta}\right)^2.
$$

It reaches its maximum when $R=2\delta/\alpha=7A M^{-1/3}/(3G)$, with

$$
\boxed{\overline T_{M,\max}=\frac{\alpha^2}{4\delta}=\frac{3\mu G^2M^{4/3}}{49\mathcal RA}.}
$$

At large [radius](../../../../../../radius.md), contraction increases the [temperature](../../../../../../temperature.md) as in a thermally supported [star](../../../../../../star.md). Once [Electron](../../../../../../electron.md) degeneracy provides a sufficiently large fraction of the support, further contraction can lower the thermal [temperature](../../../../../../temperature.md). The formal zero-temperature [radius](../../../../../../radius.md) is $R_{\mathrm{deg}}=\delta/\alpha=R_{\max}/2$, with $R_{\mathrm{deg}}\propto M^{-1/3}$. The continuation to negative temperatures would be unphysical; the adopted sequence only describes its positive-temperature part.

The [contraction-limited central temperature](../../../../../../contraction-limited-central-temperature.md) has the same [mass](../../../../../../mass.md) scaling. Indeed, if the total polytropic [pressure](../../../../../../pressure.md) is $P=K_{\mathrm{tot}}\rho^{5/3}$, the approximate [equation of state](../../../../../../equation-of-state.md) gives $T=(\mu/\mathcal R)(K_{\mathrm{tot}}-K)\rho^{2/3}$. The fixed [density](../../../../../../density.md) profile therefore fixes $T_c/\overline T_M$. A sufficiently small [mass](../../../../../../mass.md) never reaches the central [temperature](../../../../../../temperature.md) required for sustained [hydrogen burning](../../../../../../hydrogen-burning.md), producing a [hydrogen-burning minimum mass](../../../../../../hydrogen-burning-minimum-mass.md). Such an object becomes a cooling, degeneracy-supported [brown dwarf](../../../../../../brown-dwarf.md) instead of settling onto the [main sequence](../../../../../../main-sequence.md). More massive contracting objects can ignite [hydrogen](../../../../../../hydrogen.md) before reaching this degeneracy-limited maximum. This conclusion uses the nonrelativistic, fixed-composition model; it does not require extrapolation into the relativistic regime.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
