# Paper 320

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_320.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_320.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 320](paper-320.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose intrinsic Cartesian coordinates in which the [oblate spheroid](../../../galaxy.md#oblate-spheroid) is

$$
X^2+Y^2+\frac{Z^2}{q^2}=1.
$$

Let $\ell$ be distance along the line of sight and let $y$ be the sky coordinate in the plane containing the line of sight and the symmetry axis. A rotation through the inclination $i$ gives

$$
Y=y\cos i-\ell\sin i,
\qquad
Z=y\sin i+\ell\cos i.
$$

Substitution into the ellipsoid equation and minimization over $\ell$, equivalently requiring the quadratic in $\ell$ to have zero discriminant on the projected boundary, gives

$$
X^2+\frac{y^2}{\cos^2i+q^2\sin^2i}=1.
$$

Therefore the [projected axis ratio of an oblate spheroid](../../../galaxy.md#projected-axis-ratio-of-an-oblate-spheroid) is

$$
\boxed{Q^2=\cos^2i+q^2\sin^2i}.
$$

It correctly gives $Q=1$ face-on and $Q=q$ edge-on.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Uniform orientation on the [unit sphere](../../../topology.md#unit-sphere) means that probability is proportional to the solid-angle element

$$
d\Omega=\sin i\,di\,d\varphi.
$$

Because the minor axis is unoriented, it is enough to take $0\leq i\leq\pi/2$. After integration over the azimuth and normalization,

$$
\boxed{p_i(i)=\sin i,
\qquad 0\leq i\leq\frac\pi2}.
$$

Equivalently, the [random variable](../../../random-variable.md) $\mu=\cos i$ has the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At fixed intrinsic ratio $q$, part a gives

$$
Q^2=q^2+(1-q^2)\mu^2,
\qquad
\mu=\sqrt{\frac{Q^2-q^2}{1-q^2}}.
$$

Since $\mu$ is uniform, the [change-of-variables formula for a probability density](../../../continuous-probability-distribution.md#change-of-variables-formula-for-a-probability-density) yields the conditional [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
\boxed{
\mathcal P(Q\mid q)
=\frac{d\mu}{dQ}
=\frac{Q}{\sqrt{1-q^2}\sqrt{Q^2-q^2}},
\qquad q\leq Q\leq1}.
$$

The inverse-square-root singularity at $Q=q$ is integrable, and direct integration gives one.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For an intrinsic [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $\mathcal P(q)$, the [law of total probability](../../../probability-theory.md#law-of-total-probability) averages the conditional density from part c. An object observed with ratio $Q$ can only have $q\leq Q$, so

$$
\boxed{
\mathcal P(Q)
=Q\int_0^Q
\frac{\mathcal P(q)}{\sqrt{1-q^2}\sqrt{Q^2-q^2}}\,dq,
\qquad 0<Q<1}.
$$

This is an [Abel transform](../../../functional-analysis.md#abel-transform) of $\mathcal P(q)/\sqrt{1-q^2}$. Its normalization follows by reversing the order of integration and using $\int_q^1\mathcal P(Q\mid q)dQ=1$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) $\mathcal P(q)=1$, substitute $q=Q\sin\theta$ into part d:

$$
\mathcal P(Q)
=Q\int_0^{\pi/2}
\frac{d\theta}{\sqrt{1-Q^2\sin^2\theta}}
=\boxed{QK(Q)},
$$

where $K$ is the [complete elliptic integral of the first kind](../../../complex-analysis.md#complete-elliptic-integral-of-the-first-kind). Both $Q$ and $K(Q)$ increase on $(0,1)$; indeed $\mathcal P(Q)\sim\pi Q/2$ near zero and diverges logarithmically as $Q\uparrow1$. Thus the apparent distribution is strongly skewed toward higher $Q$: projection makes many intrinsically flattened systems look round.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

With

$$
\mathcal P(q)=\frac4\pi\sqrt{1-q^2},
$$

the factor $\sqrt{1-q^2}$ cancels from the [Abel transform](../../../functional-analysis.md#abel-transform):

$$
\mathcal P(Q)
=\frac{4Q}{\pi}\int_0^Q\frac{dq}{\sqrt{Q^2-q^2}}
=\frac{4Q}{\pi}\cdot\frac\pi2.
$$

Hence

$$
\boxed{\mathcal P(Q)=2Q,
\qquad 0\leq Q\leq1}.
$$

This [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is normalized and again favors rounder projections.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

For an ordinary intrinsic density, inversion of the [Abel transform](../../../functional-analysis.md#abel-transform) gives

$$
\mathcal P(q)
=\frac{2\sqrt{1-q^2}}\pi
\frac d{dq}\int_0^q
\frac{\mathcal P(Q)}{\sqrt{q^2-Q^2}}\,dQ.
$$

If $\mathcal P(Q)=1$, the integral is $\pi/2$ for every $q>0$, so its derivative vanishes. The missing probability is an endpoint atom: all systems must be infinitely thin,

$$
\boxed{\mathcal P(q)=\delta(q)}.
$$

Indeed, putting $q=0$ directly into part c gives $\mathcal P(Q\mid0)=1$. Thus a uniform apparent-axis-ratio distribution corresponds to a [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function) of ideal zero-thickness disks, rather than to a regular intrinsic density.

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

**Yes.** Even under random orientation, a population concentrated at one nonzero intrinsic ratio $q_0$ has

$$
\mathcal P(Q)=
\frac{Q}{\sqrt{1-q_0^2}\sqrt{Q^2-q_0^2}},
\qquad q_0<Q<1,
$$

which decreases from an integrable divergence at the lowest allowed value $Q=q_0$. It is therefore skewed toward the lower end of its support. More generally, a sufficiently narrow intrinsic distribution can retain such low-$Q$ peaks after the mixture in part d.

If the random-orientation assumption is relaxed, preferentially edge-on selection makes $\cos i$ concentrate near zero and hence makes $Q$ concentrate near $q$. Dust extinction, surface-brightness selection, or alignment by environment can instead bias the sample in either direction. Triaxial or prolate galaxy shapes also invalidate the [projected axis ratio of an oblate spheroid](../../../galaxy.md#projected-axis-ratio-of-an-oblate-spheroid) formula and can produce other low-$Q$ distributions.

## 2

↑ **Parent:** [Paper 320](paper-320.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $\mu=GM$ and $s=\sqrt{b^2+r^2}$. The [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass) of the [spherical isochrone model](../../../galaxy.md#spherical-isochrone-model) obeys

$$
\frac{d\Phi}{dr}=\frac{\mu r}{s(b+s)^2}.
$$

The spherical [Poisson equation](../../../partial-differential-equation.md#poisson-equation) therefore gives

$$
\begin{aligned}
\rho(r)
&=\frac1{4\pi Gr^2}\frac d{dr}
\left(r^2\frac{d\Phi}{dr}\right)\\
&=\frac{M}{4\pi s(b+s)^2}
\left(3-\frac{r^2}{s^2}
-\frac{2r^2}{s(b+s)}\right).
\end{aligned}
$$

Its small-radius [asymptotic expansion](../../../analysis.md#asymptotic-expansion) is

$$
\boxed{
\rho(r)=\frac{3M}{16\pi b^3}
-\frac{5Mr^2}{16\pi b^5}+O(r^4)},
\qquad r\ll b,
$$

so the model has a finite-density core. At large radius,

$$
\boxed{
\rho(r)=\frac{Mb}{2\pi r^4}
-\frac{3Mb^2}{4\pi r^5}+O(r^{-6})},
\qquad r\gg b.
$$

The $r^{-4}$ envelope has finite total mass $M$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a bound orbit let $E<0$ be the specific energy and $L$ the specific angular momentum. Introduce the dimensionless radius suggested in the question,

$$
x=-\frac{\mu}{b\Phi(r)}
=\frac{b+\sqrt{b^2+r^2}}b,
\qquad
r^2=b^2x(x-2).
$$

The radial energy equation becomes

$$
\dot x^2
=\frac{-2E(x-x_-)(x_+-x)}{b^2(x-1)^2},
$$

where $x_-$ and $x_+$ are the two [turning points](../../../classical-mechanics.md#turning-point). Comparing coefficients gives

$$
x_-+x_+=2-\frac{\mu}{bE}.
$$

The time from periapsis to apoapsis is

$$
\begin{aligned}
\frac{T_r}{2}
&=\frac b{\sqrt{-2E}}
\int_{x_-}^{x_+}
\frac{x-1}{\sqrt{(x-x_-)(x_+-x)}}\,dx\\
&=\frac{\pi b}{\sqrt{-2E}}
\left(\frac{x_-+x_+}{2}-1\right)
=\frac{\pi\mu}{(-2E)^{3/2}}.
\end{aligned}
$$

Thus the radial [orbital period](../../../classical-mechanics.md#orbital-period) is

$$
\boxed{T_r=\frac{2\pi GM}{(-2E)^{3/2}}}.
$$

It depends on $E$ but not on $L$, which is the defining isochrone property.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

During half a radial oscillation,

$$
\Delta\phi_{1/2}
=\frac{L}{b\sqrt{-2E}}
\int_{x_-}^{x_+}
\frac{x-1}{x(x-2)\sqrt{(x-x_-)(x_+-x)}}\,dx.
$$

Use

$$
\frac{x-1}{x(x-2)}=\frac12\left(\frac1x+\frac1{x-2}\right)
$$

and the two root products

$$
x_-x_+=\frac{L^2+4\mu b}{-2Eb^2},
\qquad
(x_--2)(x_+-2)=\frac{L^2}{-2Eb^2}.
$$

The stated elementary integrals then give the azimuthal advance over one radial period:

$$
\boxed{\Delta\phi
=\pi\left(1+\frac{L}{\sqrt{L^2+4GMb}}\right)}.
$$

Consequently the [frequency ratio of the spherical isochrone model](../../../galaxy.md#frequency-ratio-of-the-spherical-isochrone-model) is

$$
\boxed{
\frac{T_r}{T_\phi}
=\frac{\Omega_\phi}{\Omega_r}
=\frac12\left(1+\frac{L}{\sqrt{L^2+4GMb}}\right)},
$$

or equivalently $T_\phi/T_r=2/(1+L/\sqrt{L^2+4GMb})$.

Deep in the constant-density core, $L^2\ll4GMb$ and $\Omega_\phi/\Omega_r\to1/2$, as for an isotropic [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion): the radius completes two oscillations per revolution. Far outside the core, $L^2\gg4GMb$ for the corresponding circular scale and the ratio tends to one, recovering the closed [Kepler orbit](../../../classical-mechanics.md#kepler-orbit). Intermediate orbits undergo apsidal precession because the ratio is generally not rational.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [radial action](../../../classical-mechanics.md#radial-action) is

$$
J_r=\frac1\pi\int_{r_-}^{r_+}
\sqrt{2[E-\Phi(r)]-\frac{L^2}{r^2}}\,dr.
$$

With the variable $x$ from part b this becomes

$$
J_r=\frac{b\sqrt{-2E}}{2\pi}
\int_{x_-}^{x_+}
\left(\frac1x+\frac1{x-2}\right)
\sqrt{(x-x_-)(x_+-x)}\,dx.
$$

Applying the supplied integral twice, with $c=0$ and $c=2$, and using the root sum and products from parts b and c gives

$$
\boxed{
J_r=\frac{GM}{\sqrt{-2E}}
-\frac12\left(L+\sqrt{L^2+4GMb}\right)}.
$$

This is the [radial action of the spherical isochrone model](../../../galaxy.md#radial-action-of-the-spherical-isochrone-model). Rearranging,

$$
\frac{2GM}{\sqrt{-2E}}
=2J_r+L+\sqrt{L^2+4GMb},
$$

and squaring yields the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) in [action-angle variables](../../../classical-mechanics.md#action-angle-variables):

$$
\boxed{
H(J_r,L)
=-\frac{2(GM)^2}
{\left(2J_r+L+\sqrt{L^2+4GMb}\right)^2}}.
$$

As a check, differentiating this Hamiltonian gives $\Omega_r=(-2E)^{3/2}/(GM)$ and the frequency ratio found in part c.

## 3

↑ **Parent:** [Paper 320](paper-320.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

At fixed radius, use spherical coordinates in velocity space with polar angle $\alpha$ measured from the radial direction:

$$
v_r=v\cos\alpha,
\qquad
v_t=v\sin\alpha,
\qquad
L=rv\sin\alpha.
$$

The [galactic distribution function](../../../galaxy.md#galactic-distribution-function) and volume element give angular weight

$$
L^{p-2}d^3v
\propto \sin^{p-1}\alpha\,d\alpha\,d\varphi.
$$

All dependence on $v$, $r$, and $g(E)$ cancels from ratios of second moments. Symmetry in the tangential plane gives

$$
\frac{\sigma_\theta^2}{\sigma_r^2}
=\frac{\sigma_\phi^2}{\sigma_r^2}
=\frac{\frac12\int_0^\pi\sin^{p+1}\alpha\,d\alpha}
{\int_0^\pi\cos^2\alpha\sin^{p-1}\alpha\,d\alpha}.
$$

Writing the angular integrals as [beta function](../../../complex-analysis.md#beta-function) integrals and using the [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence),

$$
\frac12
\frac{B((p+2)/2,1/2)}{B(p/2,3/2)}
=\frac p2.
$$

Therefore, for every admissible energy factor $g$,

$$
\boxed{\sigma_\theta^2=\sigma_\phi^2
=\frac p2\sigma_r^2}.
$$

Equivalently, the [velocity-anisotropy parameter](../../../galaxy.md#velocity-anisotropy-parameter) is the constant $\beta=1-p/2$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $\Psi=-\Phi=GM(r^p+a^p)^{-1/p}$. The spherical [Poisson equation](../../../partial-differential-equation.md#poisson-equation) gives the [hypervirial model](../../../galaxy.md#hypervirial-model) density

$$
\boxed{
\rho(r)=\frac{(p+1)Ma^p}{4\pi}
\frac{r^{p-2}}{(r^p+a^p)^{2+1/p}}}
=\frac{(p+1)Ma^p}{4\pi(GM)^{2p+1}}
r^{p-2}\Psi^{2p+1}.
$$

For the proposed [hypervirial distribution function](../../../galaxy.md#hypervirial-distribution-function), write $\mathcal E=-E=\Psi-v^2/2$ and $n=(3p+1)/2$. Direct velocity integration gives

$$
\begin{aligned}
\rho
&=A r^{p-2}
\int_0^{\sqrt{2\Psi}}v^p
(\Psi-v^2/2)^n\,dv
\int_0^{2\pi}d\varphi
\int_0^\pi\sin^{p-1}\alpha\,d\alpha\\
&=A\,2^{(p+1)/2}\pi^{3/2}
\frac{\Gamma(p/2)\Gamma(3(p+1)/2)}
{\Gamma(2p+2)}
r^{p-2}\Psi^{2p+1}.
\end{aligned}
$$

Matching this expression to the density fixes

$$
\boxed{
A=\frac{(p+1)a^p\Gamma(2p+2)}
{2^{(p+5)/2}\pi^{5/2}G^{2p+1}M^{2p}
\Gamma(p/2)\Gamma(3(p+1)/2)}}.
$$

This coefficient is positive for $0<p\leq2$, so the distribution function self-consistently generates the stated density and potential.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The density has the form

$$
\rho=C r^{p-2}\Psi^{2p+1},
\qquad
\beta=1-\frac p2.
$$

Insert the ansatz $\sigma_r^2=k\Psi$ into the [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation)

$$
\frac{d(\rho\sigma_r^2)}{dr}
+\frac{2\beta}{r}\rho\sigma_r^2
=\rho\frac{d\Psi}{dr}.
$$

The radial-power derivative cancels the anisotropy term because $p-2+2\beta=0$, leaving $k(2p+2)=1$. Thus

$$
\boxed{
\sigma_r^2=\frac{\Psi}{2(p+1)},
\qquad
\sigma_\theta^2=\sigma_\phi^2
=\frac{p\Psi}{4(p+1)}}.
$$

Their sum is independent of $p$:

$$
\langle v^2\rangle
=\sigma_r^2+\sigma_\theta^2+\sigma_\phi^2
=\frac\Psi2=-\frac\Phi2.
$$

Therefore the local kinetic-energy density and gravitational potential-energy density are

$$
K=\frac12\rho\langle v^2\rangle=-\frac14\rho\Phi,
\qquad
W=\frac12\rho\Phi,
$$

and they satisfy the [local virial relation of the hypervirial model](../../../galaxy.md#local-virial-relation-of-the-hypervirial-model)

$$
\boxed{2K+W=0}
$$

at every radius. This pointwise identity is not generic. The ordinary [virial theorem](../../../classical-mechanics.md#virial-theorem) constrains suitable global integrals, with boundary terms when the system is truncated, but does not normally impose a virial balance shell by shell.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
