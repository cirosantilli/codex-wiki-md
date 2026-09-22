<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $p_1(z)$ denote the [Eulerian perturbation of a fluid variable](../../../../../eulerian-perturbation-of-a-fluid-variable.md) that is the [pressure](../../../../../pressure.md) amplitude, and keep $\rho$ constant. The [linearized Euler equations](../../../../../linearized-euler-equations.md) and [incompressible flow](../../../../../incompressible-flow.md) constraint are

$$
ik(U-c)u+U'w=-\frac{ikp_1}{\rho},\qquad
ik(U-c)w=-\frac{p_1'}\rho,\qquad
iku+w'=0.
$$

The last equation gives $u=iw'/k$. Substituting it into the first yields

$$
\boxed{p_1=\frac{i\rho}{k}\left[(c-U)w'+U'w\right].}
$$

Differentiating this formula and using the vertical momentum equation produces the [Rayleigh equation for inviscid shear flow](../../../../../rayleigh-equation-for-inviscid-shear-flow.md):

$$
\boxed{(U-c)(w''-k^2w)-U''w=0.}
$$

For a growing [normal mode](../../../../../normal-mode.md), $c$ is nonreal, so $U-c$ never vanishes on the real $z$ axis. In each open region the base [velocity](../../../../../velocity.md) is constant or linear and $U''=0$; therefore $w''-k^2w=0$. Decay away from the layer selects $e^{-kz}$ above and $e^{kz}$ below, while both exponentials are retained inside. Conveniently normalize these as

$$
w(z)=\begin{cases}
A e^{-k(z-d)},&z\ge d,\\
B e^{-k(z-d)}+C e^{k(z+d)},&-d<z<d,\\
D e^{k(z+d)},&z\le-d.
\end{cases}
$$

These are the spatially localized discrete modes relevant to instability, rather than all possible generalized neutral disturbances at a [critical layer in a shear flow](../../../../../critical-layer-in-a-shear-flow.md).

At each corner $U$ is continuous and $U'$ jumps. The two sides have the same normal [velocity](../../../../../velocity.md) and [normal stress](../../../../../normal-stress.md): there is no membrane, density jump or singular external force supplying a [pressure](../../../../../pressure.md) jump. Thus $w$ and $p_1$ must be continuous. The [pressure](../../../../../pressure.md) formula proves the required continuity of **$(c-U)w'+U'w$**. This is [pressure matching at a piecewise-linear shear interface](../../../../../pressure-matching-at-a-piecewise-linear-shear-interface.md); it does not require $w'$ to be continuous. Equivalently integrating the [Rayleigh equation for inviscid shear flow](../../../../../rayleigh-equation-for-inviscid-shear-flow.md) through a corner gives $(U-c)[w']=[U']w$.

Write $\alpha=kd$, $y=c/U_0$, and $E=e^{2\alpha}$. Continuity of normal [velocity](../../../../../velocity.md) gives

$$
A=B+EC,\qquad D=EB+C.
$$

At $z=d$, the outside [derivatives](../../../../../derivative.md) are $w'_+=-kA$, $U'_+=0$, while the inside [derivatives](../../../../../derivative.md) are $w'_-=-kB+kEC$, $U'_-=U_0/d$. Hence [pressure](../../../../../pressure.md) matching reduces to

$$
B+E(1-2\alpha+2\alpha y)C=0.
$$

Similarly at $z=-d$, the outside [derivative](../../../../../derivative.md) is $kD$ and the inside [derivative](../../../../../derivative.md) is $-kEB+kC$. Matching gives

$$
E(1-2\alpha-2\alpha y)B+C=0.
$$

The two equations can be written as

$$
\begin{pmatrix}
1-2\alpha+2\alpha y&e^{-2\alpha}\\
e^{-2\alpha}&1-2\alpha-2\alpha y
\end{pmatrix}
\begin{pmatrix}C\\B\end{pmatrix}=0.
$$

A nonzero mode therefore requires

$$
(1-2\alpha)^2-4\alpha^2y^2-e^{-4\alpha}=0,
\qquad
\boxed{\frac{c^2}{U_0^2}=\frac{(2\alpha-1)^2-e^{-4\alpha}}{4\alpha^2}.}
$$

This is the [dispersion relation](../../../../../dispersion-relation.md) for the [unbounded piecewise-linear shear layer](../../../../../unbounded-piecewise-linear-shear-layer.md).

With the phase convention $e^{ik(x-ct)}$, positive $\operatorname{Im}c$ gives exponential temporal growth. Since the displayed $c^2$ is real, a growing/decaying pair occurs precisely when

$$
|2\alpha-1|<e^{-2\alpha}.
$$

For $0<\alpha\le1/2$, $e^{-2\alpha}>1-2\alpha$ by the strict exponential tangent inequality, so every such mode is unstable. For $\alpha\ge1/2$, define $f(\alpha)=2\alpha-1-e^{-2\alpha}$. Its [derivative](../../../../../derivative.md) $2+2e^{-2\alpha}$ is positive, while $f(1/2)<0$ and $f(1)>0$. There is consequently exactly one root in that interval, and

$$
\boxed{0<kd<\alpha_s\text{ is unstable},\qquad
2\alpha_s-1=e^{-2\alpha_s},\qquad
\tfrac12<\alpha_s<1,quad\alpha_s\simeq0.63923227.}
$$

At the cutoff the discrete roots merge at $c=0$; above it the roots are real and have no exponential growth. The physical wavelengths in the unstable band satisfy $\lambda_x=2\pi/k>2\pi d/\alpha_s\simeq9.83d$.

This is a finite-thickness [Kelvin-Helmholtz instability](../../../../../kelvin-helmholtz-instability.md): long disturbances roll up the layer and draw [kinetic energy](../../../../../kinetic-energy.md) from its shear. The off-diagonal $e^{-2kd}$ terms describe coupling of the two [vorticity](../../../../../vorticity.md) discontinuities. Short disturbances decay across the layer before strongly coupling its edges and are neutral. Indeed at $kd\to\infty$ the two phase speeds approach the [velocities](../../../../../velocity.md) $\pm U_0$ of the separated edges. At $kd\to0$, expansion of the numerator gives $c^2/U_0^2\to-1$, recovering the [vortex sheet](../../../../../vortex-sheet.md) result $c=\pm iU_0$; the growth rate then behaves as $k|U_0|$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
