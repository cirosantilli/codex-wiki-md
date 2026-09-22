<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Build the spherical system by bringing successive thin [spherical shells](../../../../../spherical-shell.md) in from infinity. The interior [mass](../../../../../mass.md) is $M(r)=4\pi\int_0^r s^2\rho(s)\,ds$, and the next shell has $dM=4\pi r^2\rho(r)\,dr$. By the [spherical shell theorem](../../../../../spherical-shell-theorem.md), the interaction [gravitational potential energy](../../../../../gravitational-energy.md) of that shell with the assembled interior is $-GM(r)dM/r$. Each pair of mass elements is counted exactly once in this construction. Integrating gives

$$
\boxed{W=-\int_0^\infty\frac{GM(r)}r\,dM(r)=-4\pi G\int_0^\infty r\rho(r)M(r)\,dr.}
$$

The infinitesimal shell's own energy is of second order in its mass and is accounted for by the limiting pairwise assembly.

For [spherical density projection](../../../../../spherical-density-projection.md), let $z$ run along the [line of sight](../../../../../line-of-sight.md) at projected radius $R$. Spherical symmetry gives

$$
\Sigma(R)=\int_{-\infty}^{\infty}\rho\!\left(\sqrt{R^2+z^2}\right)\,dz.
$$

On $z>0$, use $r=\sqrt{R^2+z^2}$, so $dz=r\,dr/\sqrt{r^2-R^2}$. The two halves of the [line of sight](../../../../../line-of-sight.md) contribute equally, yielding

$$
\boxed{\Sigma(R)=2\int_R^\infty\frac{\rho(r)r}{\sqrt{r^2-R^2}}\,dr.}
$$

To derive the inverse [Abel transform](../../../../../abel-transform.md), set $u=R^2$, $v=r^2$, $F(u)=\Sigma(\sqrt u)$ and $g(v)=\rho(\sqrt v)$. The projection becomes $F(u)=\int_u^\infty g(v)(v-u)^{-1/2}\,dv$. Compose this with the same square-root kernel and exchange the convergent [integrals](../../../../../integral.md):

$$
\begin{aligned}
\int_t^\infty\frac{F(u)}{\sqrt{u-t}}\,du
&=\int_t^\infty g(v)\left[\int_t^v\frac{du}{\sqrt{(u-t)(v-u)}}\right]dv\\
&=\pi\int_t^\infty g(v)\,dv.
\end{aligned}
$$

The inner integral equals $\pi$, as follows from $u=t+(v-t)\sin^2\chi$ with $0<\chi<\pi/2$. Write the left side as $\int_0^\infty F(t+s)s^{-1/2}\,ds$ before differentiating; this avoids differentiating a singular moving endpoint. Under sufficient regularity and decay,

$$
\int_t^\infty\frac{F'(u)}{\sqrt{u-t}}\,du=-\pi g(t).
$$

Finally put $t=r^2,u=R^2$. Since $F'(u)=\Sigma'(R)/(2R)$, this gives the [spherical Abel deprojection](../../../../../spherical-abel-deprojection.md)

$$
\boxed{\rho(r)=-\frac1\pi\int_r^\infty\frac{\Sigma'(R)}{\sqrt{R^2-r^2}}\,dR.}
$$

Next, the [strip density of a spherical system](../../../../../strip-density-of-a-spherical-system.md) is the integral across the projected coordinate perpendicular to the strip:

$$
S(x)=\int_{-\infty}^{\infty}\Sigma\!\left(\sqrt{x^2+y^2}\right)\,dy.
$$

For $x\geq0$, the substitution $R=\sqrt{x^2+y^2}$ on $y>0$ yields

$$
\boxed{S(x)=2\int_x^\infty\frac{\Sigma(R)R}{\sqrt{R^2-x^2}}\,dR.}
$$

There is a particularly simple way to compose these two projections: $S(x)$ integrates the original [mass density](../../../../../density.md) over the whole plane of coordinates $y,z$. Polar coordinates in that plane, with $q^2=y^2+z^2$, give

$$
S(x)=2\pi\int_0^\infty\rho\!\left(\sqrt{x^2+q^2}\right)q\,dq
=2\pi\int_x^\infty\rho(r)r\,dr.
$$

Differentiation now proves

$$
\boxed{S'(x)=-2\pi x\rho(x),\qquad\rho(x)=-\frac{S'(x)}{2\pi x}\quad(x>0).}
$$

The central density, if finite, is obtained by taking the limit as $x\to0$.

To obtain [gravitational binding energy from strip density](../../../../../gravitational-binding-energy-from-strip-density.md), use $S'=-2\pi x\rho$ in the shell-assembly result, and note also that $M'=4\pi x^2\rho=-2xS'$. Two [integrations by parts](../../../../../integration-by-parts.md) then give

$$
\begin{aligned}
W&=2G\int_0^\infty M(x)S'(x)\,dx
=-2G\int_0^\infty S(x)M'(x)\,dx\\
&=4G\int_0^\infty xS(x)S'(x)\,dx
=-2G\int_0^\infty S(x)^2\,dx.
\end{aligned}
$$

Here $[MS]_0^\infty=[xS^2]_0^\infty=0$; the calculation assumes convergent binding energy and sufficient regularity and decay for these boundary terms to vanish. Thus

$$
\boxed{W=-2G\int_0^\infty[S(x)]^2\,dx.}
$$

Only the nonnegative half-axis is integrated, since the [strip density of a spherical system](../../../../../strip-density-of-a-spherical-system.md) is even. Dimensionally, $S$ is mass per length, so the last expression has the units of [energy](../../../../../energy.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
