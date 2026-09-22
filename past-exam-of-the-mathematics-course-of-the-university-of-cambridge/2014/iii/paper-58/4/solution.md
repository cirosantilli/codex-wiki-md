<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $\mu=GM$ and use [energy](../../../../../energy.md) and [angular momentum](../../../../../angular-momentum.md) per unit particle [mass](../../../../../mass.md). The [Kepler orbit](../../../../../kepler-orbit.md) equation is $\ddot{\boldsymbol r}=-\mu\boldsymbol r/r^3$. Hence

$$
\frac d{dt}\left(\frac12|\dot{\boldsymbol r}|^2-\frac\mu r\right)
=\dot{\boldsymbol r}\cdot\ddot{\boldsymbol r}
+\frac{\mu\boldsymbol r\cdot\dot{\boldsymbol r}}{r^3}=0,
\qquad
\dot{\boldsymbol L}=\boldsymbol r\times\ddot{\boldsymbol r}=0.
$$

Thus $E$ and $\boldsymbol L=\boldsymbol r\times\dot{\boldsymbol r}$ are [integrals of motion](../../../../../integral-of-motion.md). Splitting the [velocity](../../../../../velocity.md) into radial and transverse parts, $|\dot{\boldsymbol r}|^2=\dot r^2+L^2/r^2$, gives the [Kepler radial energy equation](../../../../../kepler-radial-energy-equation.md)

$$
\boxed{\frac12\dot r^2+\frac{L^2}{2r^2}=E+\frac\mu r.}
$$

Here $\dot r$ denotes the derivative of the scalar radius, unlike $\dot{\boldsymbol r}$.

For the [Laplace-Runge-Lenz vector](../../../../../laplace-runge-lenz-vector.md), differentiate directly:

$$
\frac d{dt}\left(\dot{\boldsymbol r}\times\boldsymbol L-\mu\frac{\boldsymbol r}{r}\right)
=\ddot{\boldsymbol r}\times\boldsymbol L
-\mu\left(\frac{\dot{\boldsymbol r}}r
-\frac{\boldsymbol r(\boldsymbol r\cdot\dot{\boldsymbol r})}{r^3}\right).
$$

The vector triple-product identity yields

$$
\ddot{\boldsymbol r}\times\boldsymbol L
=-\frac\mu{r^3}\boldsymbol r\times(\boldsymbol r\times\dot{\boldsymbol r})
=\mu\left(\frac{\dot{\boldsymbol r}}r
-\frac{\boldsymbol r(\boldsymbol r\cdot\dot{\boldsymbol r})}{r^3}\right).
$$

The terms cancel, proving **every component of $\boldsymbol A$ is conserved**.

Write $q=\bar r(r)$ and $\tau=\bar t$ for a monotone [radial orbit time transformation](../../../../../radial-orbit-time-transformation.md). The [chain rule](../../../../../chain-rule.md) gives

$$
q'=\frac{dq}{dr}\frac{dt}{d\tau}\dot r.
$$

Impose $q'=(r/q)\dot r$, equivalently

$$
\boxed{\frac rq=\frac{dq}{dr}\frac{dt}{d\tau},\qquad
\frac{d\tau}{dt}=\frac qr\frac{dq}{dr}.}
$$

Multiplying the radial [energy](../../../../../energy.md) equation by $r^2/q^2$ then gives

$$
\boxed{\frac12q'^2+\frac{L^2}{2q^2}
=\frac{r^2}{q^2}\left(E+\frac\mu r\right).}
$$

This is a transformation along each trajectory; the new clock is obtained by integrating its radius-dependent rate.

For the [Kepler–harmonic radial duality](../../../../../kepler-harmonic-radial-duality.md), take the old inverse-radius term as the new constant [energy](../../../../../energy.md), $\bar E=\mu r/q^2$. On a positive-radius branch $\bar E>0$, so

$$
r=\frac{\bar E}{\mu}q^2,\qquad
\frac{d\tau}{dt}=\frac{\mu}{2\bar E r}.
$$

The remaining term is minus the new [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md):

$$
\boxed{\bar\Phi(q)=-E\left(\frac{\bar E}{\mu}\right)^2q^2.}
$$

For $E<0$ this is an attractive isotropic [harmonic oscillator](../../../../../simple-harmonic-motion.md) with $\bar\omega^2=-2E(\bar E/\mu)^2$. For $E>0$ it is an inverted oscillator, and for $E=0$ the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) vanishes. Calling it a confining oscillator therefore requires a bound original [Kepler orbit](../../../../../kepler-orbit.md).

For the [angular reconstruction of a radial orbit transformation](../../../../../angular-reconstruction-of-a-radial-orbit-transformation.md), choose the new angle by $d\bar\theta/d\tau=L/q^2$. The same $L$ then supplies its centrifugal term. From $d\theta/dt=L/r^2$, the transformation is $d\bar\theta/d\theta=(r/q)(dq/dr)$; in the harmonic case this gives $\bar\theta=\theta/2$ up to a constant. Keeping the old angle unchanged would not in general preserve the [angular momentum](../../../../../angular-momentum.md) used in the displayed transformed radial equation.

For the second transformation use the explicit displayed split of the [energy](../../../../../energy.md) terms. It assigns weight $\lambda$ to $E$ and $1-\lambda$ to $\mu/r$; the surrounding printed prose interchanges these weights. Define the transformed quantities consistently by

$$
\boxed{\bar E=\frac{r^2}{q^2}\left[\lambda E+(1-\lambda)\frac\mu r\right],\qquad
\bar\Phi=-\frac{r^2}{q^2}\left[(1-\lambda)E+\lambda\frac\mu r\right].}
$$

Their difference is exactly $(r^2/q^2)(E+\mu/r)$, so they give the same transformed radial [energy](../../../../../energy.md) equation.

Let $a=(1-\lambda)\mu$, $h=\lambda E$, and $\varepsilon=\bar E$. Constancy of the new [energy](../../../../../energy.md) imposes

$$
\varepsilon q^2=hr^2+ar.
$$

For the standard regular isochrone branch take $h>0$, $\varepsilon>0$, and $a\geq0$. The positive-radius root is

$$
\boxed{r(q)=\frac{-a+\sqrt{a^2+4h\varepsilon q^2}}{2h}
=\sqrt{\frac\varepsilon h}\left(\sqrt{q^2+b^2}-b\right),\qquad
b=\frac{a}{2\sqrt{h\varepsilon}}
=\frac{(1-\lambda)GM}{2\sqrt{\lambda E\bar E}}.}
$$

For $q>0$ it is monotone. The corresponding clock is also regular there:

$$
\frac{d\tau}{dt}=\frac{a+2hr}{2\varepsilon r}>0.
$$

With $\alpha=\sqrt{\varepsilon/h}$ and $s=\sqrt{q^2+b^2}$, rationalization gives $r/q^2=\alpha/(s+b)$. Eliminate $r^2/q^2$ using $h r^2/q^2=\varepsilon-a r/q^2$:

$$
\bar\Phi(q)
=-\frac{1-\lambda}{\lambda}\varepsilon
+\mu\frac{1-2\lambda}{\lambda}\frac r{q^2}
=k-\frac{G\bar M}{b+\sqrt{q^2+b^2}},
$$

where one possible identification is

$$
\boxed{k=-\frac{1-\lambda}{\lambda}\bar E,\qquad
G\bar M=GM\frac{2\lambda-1}{\lambda}
\sqrt{\frac{\bar E}{\lambda E}}.}
$$

This is the [Kepler–isochrone radial transformation](../../../../../kepler-isochrone-radial-transformation.md) to the [spherical isochrone model](../../../../../spherical-isochrone-model.md), up to the additive [energy](../../../../../energy.md) constant $k$.

The [attractive branch of the Kepler–isochrone transformation](../../../../../attractive-branch-of-the-kepler-isochrone-transformation.md) requires a suitable parameter domain. The displayed square root needs $\lambda E\bar E>0$, and the positive-root branch used above needs $\lambda E>0$, $\bar E>0$. An attractive regular isochrone also needs $b\geq0$ and $\bar M>0$. For bound original orbits a convenient domain is **$E<0$, $\lambda<0$, $\bar E>0$**: it satisfies all these requirements and gives $\bar E-k=\bar E/\lambda<0$. For $E>0$ one may instead take $1/2<\lambda\leq1$, with $\bar E>0$; these map to unbound attractive isochrone orbits. Other parameter choices can produce a repulsive [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) or a different branch, so no unrestricted real-parameter statement is justified. The singular algebraic case $\lambda=0$ is the harmonic transformation already handled separately. The angular reconstruction $d\bar\theta/d\tau=L/q^2$ likewise completes the isochrone radial solution into a central-force orbit.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
