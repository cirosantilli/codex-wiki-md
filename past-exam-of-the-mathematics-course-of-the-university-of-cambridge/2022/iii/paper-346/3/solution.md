<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The definition of the [virial radius of a dark-matter halo](../../../../../virial-radius-of-a-dark-matter-halo.md) immediately gives the [virial mass of a dark-matter halo](../../../../../virial-mass-of-a-dark-matter-halo.md)

$$
\boxed{M_v=\frac{4\pi}{3}v\rho_c^0r_v^3.}
$$

In an [Einstein-de Sitter universe](../../../../../einstein-de-sitter-universe.md), spherical collapse gives $v=18\pi^2\simeq178$, conventionally rounded to about $200$.

For the [Navarro--Frenk--White profile](../../../../../navarro-frenk-white-profile.md), put $x=r/r_s=cs$. Direct integration gives

$$
M(r)=4\pi\rho_c^0\delta_{\rm char}r_s^3
\left[\log(1+x)-\frac{x}{1+x}\right].
$$

Using $r_s=r_v/c$ and $\delta_{\rm char}=vc^3g(c)/3$ therefore yields

$$
\boxed{\frac{M(s)}{M_v}=g(c)
\left[\log(1+cs)-\frac{cs}{1+cs}\right].}
$$

At small radius the bracket is $(cs)^2/2+O((cs)^3)$, so $M(r)\propto r^2$, consistent with the central $\rho\propto r^{-1}$ cusp. At large radius it is $\log(cs)-1+o(1)$, so the mass diverges logarithmically unless the halo is truncated.

The primordial free streaming of [warm dark matter](../../../../../warm-dark-matter.md) erases small-scale density fluctuations and lowers the central phase-space density, tending to replace the smallest, earliest cold-dark-matter cusps by shallower central profiles or cores.

Since $V_v^2=GM_v/r_v$, the spherical potential that vanishes at infinity is

$$
\Phi(s)=-g(c)V_v^2\frac{\log(1+cs)}s.
$$

Indeed, $r\,d\Phi/dr=GM(r)/r$, and normalization at $s=1$ requires

$$
\boxed{g(c)=\left[\log(1+c)-\frac{c}{1+c}\right]^{-1}.}
$$

The [circular speed](../../../../../circular-speed.md) is consequently

$$
\boxed{V^2(s)=V_v^2\frac{g(c)}s
\left[\log(1+cs)-\frac{cs}{1+cs}\right].}
$$

It rises as $s^{1/2}$ near the centre, peaks at $r\simeq2.16r_s$, and then declines approximately as $\sqrt{\log r/r}$. Increasing the [concentration of a dark-matter halo](../../../../../concentration-of-a-dark-matter-halo.md) moves the peak inward in units of $r_v$ and raises it relative to $V_v$. Thus an NFW curve can be fairly broad but is not exactly a [flat galaxy rotation curve](../../../../../flat-galaxy-rotation-curve.md); stellar and gas contributions matter when comparing with an observed [galaxy rotation curve](../../../../../galaxy-rotation-curve.md).

Lower-mass haloes typically collapse earlier, when the cosmic background density is larger. Their characteristic inner densities are consequently larger relative to the present virial density, producing the [mass-concentration relation of dark-matter haloes](../../../../../mass-concentration-relation-of-dark-matter-haloes.md) in which concentration decreases weakly with mass.

For a mass smaller by $1024=2^{10}$,

$$
M_v\simeq9.8\times10^8M_\odot,
\qquad
r_v=200\,1024^{-1/3}\ {\rm kpc}\simeq19.8\ {\rm kpc},
$$

and $c=10\,1024^{0.1}=20$. Hence

$$
\boxed{r_s=r_v/c\simeq0.99\ {\rm kpc}.}
$$

A halo of roughly $10^9M_\odot$ and kiloparsec scale naturally hosts a [dwarf galaxy](../../../../../dwarf-galaxy.md), possibly an extremely faint one if star formation is inefficient.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
