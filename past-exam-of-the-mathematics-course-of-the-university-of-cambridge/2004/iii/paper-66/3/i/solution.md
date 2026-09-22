<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The factor called $N$ in the formula must be the stellar [number density](../../../../../../number-density.md) $n$, not a dimensionless count. Indeed $\sigma^3/(G^2m^2)$ has dimensions time per volume, so a density in the denominator is essential. If $N_*$ is the population in a representative volume $V$, then $n=N_*/V$.

For a weak encounter between equal-mass [stars](../../../../../../star.md), let $u$ be the asymptotic relative [speed](../../../../../../speed.md) and $b$ the [impact parameter](../../../../../../impact-parameter.md). In the straight-line impulse approximation, one star's transverse kick is

$$
\Delta v_\perp=\int_{-\infty}^{\infty}\frac{Gmb\,dt}{(b^2+u^2t^2)^{3/2}}=\frac{2Gm}{bu}.
$$

The other receives the opposite kick, so the relative-velocity change is $\Delta u_\perp=4Gm/(bu)$. Encounters in $(b,b+db)$ occur at rate $2\pi b\,db\,nu$. Independent random kicks add in squared magnitude, giving

$$
D_v:=\frac{d\langle|\Delta\mathbf v|^2\rangle}{dt}=\frac{8\pi nG^2m^2}{u}\int_{b_{\min}}^{b_{\max}}\frac{db}{b}=\frac{8\pi nG^2m^2\ln\Lambda}{u},\qquad D_u=4D_v.
$$

This is the [random-walk derivation of stellar relaxation](../../../../../../random-walk-derivation-of-stellar-relaxation.md). The [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md) is $\ln\Lambda=\ln(b_{\max}/b_{\min})$. The upper cutoff is the size or inhomogeneity scale beyond which independent local encounters are inappropriate. The lower cutoff is of order the strong-deflection scale $G(2m)/u^2$, or a larger stellar-size/softening scale if applicable. A self-gravitating system commonly has $\Lambda$ of order its total number of stars; that population count is distinct from $n$ in the diffusion rate.

To state the numerical convention explicitly, use representative encounter speed $u=\sqrt2\sigma$ and define the relaxation estimate from the relative-velocity diffusion rate with reference squared velocity $3\sigma^2$. This gives

$$
\boxed{T_R:=\frac{3\sigma^2}{D_u}=\frac{3}{16\pi\sqrt2}\frac{\sigma^3}{nG^2m^2\ln\Lambda}.}
$$

This recovers the printed coefficient under a specified convention. There is no convention-independent exact numerical prefactor determined by a representative one-dimensional velocity alone. Using the single-star diffusion rate with the same $3\sigma^2$ reference instead gives four times this time; averaging over a full velocity distribution also changes the prefactor. The [relaxation time conventions in stellar dynamics](../../../../../../relaxation-time-conventions-in-stellar-dynamics.md) must therefore distinguish single-star and relative kicks. **The physical scaling is $T_R\propto\sigma^3/(nG^2m^2\ln\Lambda)$, and the printed $N$ must be interpreted as number density.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
