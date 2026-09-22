<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A small [loss cone](../../../../../../loss-cone.md) does not by itself specify its supply rate. Introduce a characteristic orbital radius $r$, an [orbital period](../../../../../../orbital-period.md) $P\sim r/v$, the number $N_r$ of stars on the relevant energy range, and their local number density $n$. Weak encounters of [impact parameter](../../../../../../impact-parameter.md) $b$ give velocity kicks of order $Gm/(bv)$. Summing their squared kicks over encounter rate $2\pi b\,db\,nv$ gives

$$
\frac{d\langle\Delta v^2\rangle}{dt}
\sim\frac{G^2m^2n\log\Lambda}{v},
\qquad
\boxed{t_{\rm rel}\sim\frac{v^3}{G^2m^2n\log\Lambda}.}
$$

Here $\log\Lambda$ is the [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md). This derives the [stellar relaxation time](../../../../../../stellar-relaxation-time.md) relevant to angular-momentum scattering, up to the velocity-averaging constants.

Let $J_c^2\sim GM_Hr$ and define the dimensionless cone size $\mathcal R_{\rm lc}=J_{\rm lc}^2/J_c^2\sim R_{\rm sch}/r$. In one period, [two-body relaxation](../../../../../../two-body-relaxation.md) changes $J^2$ by order $J_c^2P/t_{\rm rel}$, so the refilling parameter is

$$
q\sim\frac{P}{t_{\rm rel}\mathcal R_{\rm lc}}.
$$

If refilling is sufficiently rapid to keep the cone populated, an isotropic fraction of order $\mathcal R_{\rm lc}$ reaches its absorbing pericentre each orbit. The full-cone rate is

$$
\boxed{\Gamma_{\rm full}\equiv-\dot N_r
\sim\frac{N_r\mathcal R_{\rm lc}}P
\sim\frac{N_r}P\frac{R_{\rm sch}}r.}
$$

If $q\ll1$, the cone is depleted and capture is diffusion-limited. At fixed orbital energy, the two transverse angular-momentum coordinates have an approximately two-dimensional diffusion equation. Its steady radial solution between the absorbing boundary $J_{\rm lc}$ and the reservoir $J_c$ satisfies

$$
\frac1J\frac d{dJ}\left(J\frac{df}{dJ}\right)=0,
\qquad f(J)\propto\frac{\log(J/J_{\rm lc})}{\log(J_c/J_{\rm lc})}.
$$

The gradient supplies a constant inward flux. With diffusion coefficient of order $J_c^2/t_{\rm rel}$ and reservoir population $N_r$, this gives

$$
\boxed{\Gamma_{\rm empty}\sim
\frac{N_r}{t_{\rm rel}\log(1/\mathcal R_{\rm lc})}.}
$$

Constants of two depend on using $J$ or $J^2$ and on the definition of $t_{\rm rel}$. A rough interpolation uses the slower of the orbital draining and diffusion-supply rates; an accurate transition requires an orbit-averaged diffusion calculation. These are the [empty and full loss-cone capture rates](../../../../../../empty-and-full-loss-cone-capture-rates.md). In particular, multiplying $N_r/t_{\rm rel}$ by the cone's tiny solid-angle fraction would incorrectly treat diffusive feeding as independent isotropic redraws.

For a one-zone black-hole-dominated cluster with $N_r\sim N$, $n\sim N/r^3$ and $v^2\sim GM_H/r$,

$$
t_{\rm rel}\sim\frac{(M_H/m)^2}{N\log\Lambda}P,
\qquad
\Gamma_{\rm empty}\sim\frac{N^2\log\Lambda}{(M_H/m)^2P\log(r/R_{\rm sch})}.
$$

The mass ingestion rate is $\dot M_H\simeq m\Gamma$. A radially extended cluster requires summing the energy-dependent fluxes, not replacing every radius by the same $r$. **No numerical capture rate follows from $N,m,M_H$ alone:** its radius/density, orbital distribution and refilling regime are required. The displayed relations are the requested estimates with those physical scales explicit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
