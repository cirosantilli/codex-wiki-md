<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define $k_0=\omega/c_0$ and use the [outgoing acoustic square-root branch](../../../../../../outgoing-acoustic-square-root-branch.md)

$$
\gamma^2=k^2-k_0^2,\qquad \operatorname{Re}\gamma>0\quad\text{for }\operatorname{Im}\omega<0.
$$

For positive real frequency reached from below, $\gamma=i\sqrt{k_0^2-k^2}$ on the propagating interval and is positive real for $|k|>k_0$. The outgoing field in the lower fluid has [pressure](../../../../../../pressure.md) amplitude $B e^{\gamma y}$, since $y<0$. If $\eta=\widehat\eta e^{i\omega t-ikx}$, the shared [normal velocity](../../../../../../normal-velocity.md) is $i\omega\widehat\eta$. The [linear homentropic acoustic equations](../../../../../../linear-homentropic-acoustic-equations.md) therefore give

$$
i\omega\widehat\eta=-\frac{\gamma B}{i\omega\rho_0},\qquad
B=\frac{\rho_0\omega^2}{\gamma}\widehat\eta.
$$

This lower-fluid wave is outgoing; no additional incoming sound is included in defining the impedance seen by the upper fluid.

Put $K_s=Tk^2-m\omega^2$. The sheet's [force balance](../../../../../../force-balance.md) gives $K_s\widehat\eta=-P+B$, hence $P=(\rho_0\omega^2/\gamma-K_s)\widehat\eta$. Its prescribed downward [velocity](../../../../../../velocity.md) amplitude is $V=-i\omega\widehat\eta$. Thus the [tensioned-sheet acoustic impedance](../../../../../../tensioned-sheet-acoustic-impedance.md) is

$$
\boxed{Z(k,\omega)=\frac{i\rho_0\omega}{\gamma}-\frac{i}{\omega}(Tk^2-m\omega^2)=Z_f+Z_s.}
$$

The first term is the lower fluid's [normal acoustic impedance](../../../../../../normal-acoustic-impedance.md), and the second is the sheet's inertial and [elastic-sheet tension](../../../../../../elastic-sheet-tension.md) response. For a real propagating angle, $Z_f=\rho_0c_0/\sin\theta$.

At fixed nonzero frequency and fixed wavenumber, $m\to\infty$ gives $|Z|\to\infty$, a zero-velocity, in-phase reflecting boundary. At fixed $k\ne0$, $T\to\infty$ gives the same reflection limit, but there is an important exception: **[elastic-sheet tension](../../../../../../elastic-sheet-tension.md) does not resist the spatially uniform mode $k=0$**. At normal incidence, the impedance remains $\rho_0c_0+im\omega$ however large the [elastic-sheet tension](../../../../../../elastic-sheet-tension.md) is. With $m=0$ this mode is transparent. By contrast, arbitrarily large [mass](../../../../../../mass.md) resists even a spatially uniform oscillation. These fixed-frequency limits exclude a simultaneously tuned structural resonance.

If $m=T=0$, $Z=Z_f$ and $R=0$. The identical fluids are effectively joined across a massless, untensioned interface: [pressure](../../../../../../pressure.md) and [normal velocity](../../../../../../normal-velocity.md) continue without reflection. This is the matched case, rather than the pressure-release case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
