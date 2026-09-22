<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

The [unit vectors](../../../../../unit-vector.md) of [plane polar coordinates](../../../../../plane-polar-coordinates.md) obey $\dot{\mathbf e}_r=\dot\theta\mathbf e_\theta$ and $\dot{\mathbf e}_\theta=-\dot\theta\mathbf e_r$, as follows by differentiating their Cartesian sine/cosine components. Since $\mathbf x=r\mathbf e_r$,

$$
\boxed{\dot{\mathbf x}=\dot r\mathbf e_r+r\dot\theta\mathbf e_\theta}.
$$

At a regular point of nonzero [speed](../../../../../speed.md), rotating this [velocity vector](../../../../../velocity-vector.md) through a right angle produces a [normal vector](../../../../../normal-vector.md). Thus, up to its orientation,

$$
\mathbf n=\pm\frac{r\dot\theta\mathbf e_r-\dot r\mathbf e_\theta}{\sqrt{\dot r^2+r^2\dot\theta^2}}.
$$

Its scalar product with $\mathbf x$ gives the distance from the origin to the [tangent line](../../../../../tangent-line.md):

$$
p=|\mathbf x\cdot\mathbf n|=\frac{r^2|\dot\theta|}{\sqrt{\dot r^2+r^2\dot\theta^2}}.
$$

Where $r$ is a differentiable function of $\theta$ and $\dot\theta\ne0$, substitute $\dot r=(dr/d\theta)\dot\theta$ to obtain

$$
\boxed{\frac{r^2}{p^2}=1+\frac1{r^2}\left(\frac{dr}{d\theta}\right)^2}.
$$

A choice of principal normal is undefined on a locally straight segment, but the perpendicular normal line and the tangent-distance formula remain meaningful.

For a [central force](../../../../../central-force.md), the torque vanishes. Use physical signed [angular momentum](../../../../../angular-momentum.md) $h=mr^2\dot\theta$, with $h\ne0$. The preceding geometric formula implies $|h|=mpv$, where $v=|\dot{\mathbf x}|$. [Conservation of energy](../../../../../conservation-of-energy.md) gives $E=mv^2/2+V(r)$. Eliminate $v$ to obtain the [pedal equation for a central-force orbit](../../../../../pedal-equation-for-a-central-force-orbit.md):

$$
\boxed{\frac1{p^2}=\frac{2m[E-V(r)]}{h^2}}.
$$

Equivalently the radial [energy](../../../../../energy.md) equation is

$$
\frac12m\dot r^2+V_{\rm eff}(r)=E,\qquad V_{\rm eff}(r)=V(r)+\frac{h^2}{2mr^2}.
$$

On an outward radial branch, divide $\dot\theta=h/(mr^2)$ by $\dot r=\sqrt{2[E-V_{\rm eff}]/m}$ and integrate:

$$
\boxed{\theta(r)-\theta(r_0)=\int_{r_0}^r\frac{h\,ds}{s^2\sqrt{2m[E-V_{\rm eff}(s)]}}}.
$$

On an inward radial branch the integrand acquires a minus sign. At a turning point the two branches must be joined; the quoted positive-root integral is a local branch representation, not a single global time-parametrized orbit.

For $V=c/r^2$ with $c>0$, define

$$
C=c+\frac{h^2}{2m},\qquad r_{\min}=\sqrt{\frac CE},\qquad \beta=\frac{\sqrt{h^2+2mc}}{|h|}>1.
$$

A finite moving orbit has $E>0$. In the radial integral, set $s=r_{\min}/r$. Because $dr/r^2=-ds/r_{\min}$, the outward integral, measured from the radial minimum, is

$$
\theta-\theta_0=\frac{h}{\sqrt{2mC}}\arccos\left(\frac{r_{\min}}r\right).
$$

Joining the inward and outward branches gives

$$
\boxed{r(\theta)=r_{\min}\sec[\beta(\theta-\theta_0)],\qquad |\theta-\theta_0|<\frac\pi{2\beta}}.
$$

The orientation in time is determined by the sign of $h$. The [repulsive inverse-square potential](../../../../../repulsive-inverse-square-potential.md) generates force $-V'(r)=2c/r^3$, an outward inverse-cube [central force](../../../../../central-force.md), not an inverse-square force. The orbit approaches infinity along two asymptotic directions, turns once at $r_{\min}$ and escapes again. The total polar-angle sweep is $\pi/\beta<\pi$, and the repulsive scattering deflection is

$$
\boxed{\delta=\pi\left(1-\frac1\beta\right)}.
$$

The [effective potential](../../../../../effective-potential.md) $C/r^2$ decreases strictly to zero, so it admits no finite circular or bounded orbit. The sketch shows this [scattering in a repulsive inverse-square potential](../../../../../scattering-in-a-repulsive-inverse-square-potential.md). In the radial case $h=0$, the formulas dividing by $h$ are inapplicable; the direction is fixed, the turning radius is $\sqrt{c/E}$ and the particle reverses on the same ray.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
