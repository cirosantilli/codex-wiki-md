<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use outward radial [mass flux](../../../../../../mass-flux.md) $\mathcal F=2\pi r\Sigma u_r$ and outward stress-carried angular-momentum flux $\mathcal G$. The PDF includes a second conservation equation omitted from the converted TeX:

$$
\partial_t(\Sigma h)+\frac1{2\pi r}\partial_r(\mathcal Fh+\mathcal G)=-T.
$$

Together with [mass conservation](../../../../../../mass-conservation.md), $\Sigma_t+(2\pi r)^{-1}\mathcal F_r=-S$, it fixes the signs of the wind terms. Subtract h times the mass equation, noting that the prescribed $h(r)$ is independent of time. One obtains

$$
\mathcal F\frac{dh}{dr}+\frac{\partial\mathcal G}{\partial r}=2\pi r(Sh-T).
$$

The [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) in this outward-flux convention is $\mathcal G=-2\pi\bar\nu\Sigma r^3\Omega'$. Thus, where $h'\ne0$,

$$
\mathcal F=2\pi(h')^{-1}\left[\partial_r(\bar\nu\Sigma r^3\Omega')+r(Sh-T)\right].
$$

Putting this result back into mass conservation gives

$$
\boxed{\Sigma_t=-\frac1r\partial_r\left\{(h')^{-1}\left[\partial_r(\bar\nu\Sigma r^3\Omega')+r(Sh-T)\right]\right\}-S.}
$$

The derivation requires a fixed rotation law; it would acquire additional terms if h evolved independently in time.

For [Keplerian rotation](../../../../../../keplerian-disk.md), $h=\sqrt{GMr}$, $h'=h/(2r)$, and $r^3\Omega'=-(3/2)h$. With $T=qSh$, the radial flux becomes

$$
\mathcal F=-6\pi\sqrt r\,\partial_r(\sqrt r\bar\nu\Sigma)-4\pi(q-1)r^2S.
$$

Consequently the [wind-loaded Keplerian disk evolution](../../../../../../wind-loaded-keplerian-disk-evolution.md) equation is

$$
\boxed{\Sigma_t=\frac3r\partial_r\left[\sqrt r\,\partial_r(\sqrt r\bar\nu\Sigma)\right]+\frac1r\partial_r[2(q-1)r^2S]-S.}
$$

The final term removes mass locally. The extra flux term describes the disc's radial response when the outflow removes more or less than the local [specific angular momentum](../../../../../../specific-angular-momentum.md). In particular, $q=1$ cancels this additional transport term without canceling the local mass sink.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
