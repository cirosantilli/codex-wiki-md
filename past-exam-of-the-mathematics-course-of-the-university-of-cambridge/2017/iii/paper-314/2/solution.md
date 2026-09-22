<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $v=|u_r|>0$ for the radial [speed](../../../../../speed.md) and distinguish the central mass $M$ from the [Mach number](../../../../../mach-number.md) $\mathcal M=v/c$. In each smooth nonzero-flow region, [mass conservation](../../../../../mass-conservation.md), the [adiabatic equation of state](../../../../../adiabatic-equation-of-state.md), and the [Bernoulli equation](../../../../../bernoulli-equation.md) give

$$
j=r^2\rho v=\frac{|\dot M|}{4\pi}>0,\qquad p=K\rho^{3/2},\qquad c^2=\frac32K\rho^{1/2},\qquad
\mathcal E=\frac{v^2}{2}+2c^2-\frac{GM}{r}.
$$

Here $K>0$ is constant on a smooth [isentropic flow](../../../../../isentropic-flow.md) branch, $c$ is the [adiabatic sound speed](../../../../../adiabatic-sound-speed.md), and $\mathcal E$ is the [Bernoulli function](../../../../../bernoulli-function.md). Either sign of $u_r$ is possible. The positive-radius nondimensionalization in the question requires $\mathcal E>0$; flows with $\mathcal E\leq0$ do not have these positive $r_s,x,\lambda$ and require another scaling.

Indeed, the supplied [adiabatic process](../../../../../adiabatic-process.md) equations give $D(p\rho^{-3/2})/Dt=0$, so $K$ is spatially constant along a steady nonzero radial [fluid flow](../../../../../fluid-flow.md). The [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) is $c^2=(\partial p/\partial\rho)_s$, and the [specific enthalpy](../../../../../specific-enthalpy.md) is $h=c^2/(\gamma-1)=2c^2$. The radial [Euler momentum equation](../../../../../euler-equations-for-an-inviscid-fluid.md), $v\,dv/dr=-\rho^{-1}dp/dr-GM/r^2$, integrates to $\mathcal E$ because $dh=dp/\rho$ on this [isentropic flow](../../../../../isentropic-flow.md) branch.

Put $D=[j(3K/2)^2]^{2/5}$. Eliminating the [mass density](../../../../../density.md) from the [continuity equation](../../../../../continuity-equation.md) gives

$$
c^2=D r^{-4/5}\mathcal M^{-2/5}.
$$

With $y=\mathcal M^{2/5}$, the [Bernoulli equation](../../../../../bernoulli-equation.md) becomes

$$
\mathcal E+\frac{GM}{r}=\frac D2 r^{-4/5}(y^4+4/y).
$$

Therefore the physical constants of the [spherical polytropic flow with adiabatic exponent three halves](../../../../../spherical-polytropic-flow-with-adiabatic-exponent-three-halves.md) are

$$
\boxed{r_s=\frac{GM}{4\mathcal E},\qquad \lambda=\frac{[j(3K/2)^2]^{2/5}}{2\mathcal E r_s^{4/5}},\qquad
\lambda F(y)=F(x),\quad F(t)=t^4+\frac4t,\quad x=(r/r_s)^{1/5}.}
$$

For $t>0$, $F'(t)=4(t^5-1)/t^2$, so $F$ decreases from infinity to its unique minimum $F(1)=5$, then increases to infinity. This completely determines the [algebraic curves](../../../../../algebraic-curve.md). For $0<\lambda<1$, there are two disconnected branches at every $x>0$, one [subsonic flow](../../../../../subsonic-flow.md) with $y<1$ and one [supersonic flow](../../../../../supersonic-flow.md) with $y>1$. For $\lambda=1$, the line $y=x$ and a decreasing branch meet at $(1,1)$. Their slopes are $+1$ and $-1$, since the leading expansion is $F(1+\eta)=5+10\eta^2+O(\eta^3)$. For $\lambda>1$, solutions exist only where $F(x)\geq5\lambda$: if $x_-<1<x_+$ solve $F(x_\pm)=5\lambda$, there is a forbidden interval $x_-<x<x_+$. At either endpoint the two branches turn at $y=1$ and have an infinite slope.

A smooth [sonic point](../../../../../sonic-point.md) needs $F'(x)=F'(y)=0$; hence **a regular sonic transition requires $\lambda=1$ and $r=r_s$**. The [critical speed of a polytropic flow](../../../../../critical-speed-of-a-polytropic-flow.md) is then $c_s^2=GM/(2r_s)=2\mathcal E$, and the allowed [mass flux](../../../../../mass-flux.md) is $j=(2\mathcal E)^{5/2}r_s^2/(3K/2)^2$. Here the subscript on $c_s$ denotes evaluation at the [sonic point](../../../../../sonic-point.md), rather than the [isothermal sound speed](../../../../../isothermal-sound-speed.md) convention used in the next solution.

The simple [transonic branch](../../../../../transonic-branch.md) is $y=x$. Direct substitution gives

$$
\boxed{\mathcal M=(r/r_s)^{1/2},\quad v=\sqrt{2\mathcal E},\quad c^2=\frac{GM}{2r},\quad
\rho=\left(\frac{GM}{3Kr}\right)^2,\quad p=K\left(\frac{GM}{3Kr}\right)^3.}
$$

Thus the radial [velocity](../../../../../velocity.md) has constant magnitude, while the [mass density](../../../../../density.md) and [pressure](../../../../../pressure.md) scale as $r^{-2}$ and $r^{-3}$. For an outward [fluid flow](../../../../../fluid-flow.md), this is a [subsonic flow](../../../../../subsonic-flow.md) becoming a [supersonic flow](../../../../../supersonic-flow.md) as its [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) decreases.

On the other [transonic branch](../../../../../transonic-branch.md), $y$ decreases as $x$ increases. At large $r$, the terms $4/y$ and $x^4$ dominate, giving $y\sim4x^{-4}$. At small $r$, the terms $y^4$ and $4/x$ dominate, giving $y\sim4^{1/4}x^{-1/4}$. The resulting [asymptotic expansions](../../../../../asymptotic-expansion.md) are

$$
\begin{aligned}
r\gg r_s:\quad&\mathcal M\sim32(r_s/r)^2,\qquad c^2\longrightarrow\mathcal E/2,\qquad
\rho\longrightarrow\left(\frac{\mathcal E}{3K}\right)^2,\qquad
v\sim32\sqrt{\mathcal E/2}(r_s/r)^2,\\
r\ll r_s:\quad&\mathcal M\sim2^{5/4}(r_s/r)^{1/8},\qquad
c^2\sim\sqrt2\,\mathcal E(r_s/r)^{3/4},\qquad
v\sim\sqrt{\frac{2GM}{r}},\\
&\rho\sim\frac{j}{\sqrt{2GM}}r^{-3/2},\qquad
p\sim K\left(\frac{j}{\sqrt{2GM}}\right)^{3/2}r^{-9/4}.
\end{aligned}
$$

For inward [fluid flow](../../../../../fluid-flow.md), these are the nearly static reservoir at infinity and the inner [free fall](../../../../../free-fall.md) region of [Bondi accretion](../../../../../bondi-accretion.md). The [specific enthalpy](../../../../../specific-enthalpy.md) is smaller than $GM/r$ in the inner limit, which explains [free fall](../../../../../free-fall.md). Reversing the radial [velocity](../../../../../velocity.md) gives a decelerating outflow with the same profiles. The formal small-$r$ limit describes the point-mass model: if the spherical gravitating body has a finite surface, the exterior solution stops there.

A stationary, nonradiative [normal shock wave](../../../../../normal-shock-wave.md) conserves the [mass flux](../../../../../mass-flux.md) and the sum $v^2/2+h$, while the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) is continuous across its thin layer. Hence $\mathcal E$ and $r_s$ are unchanged. The [entropy production in a perfect-gas shock](../../../../../entropy-production-in-a-perfect-gas-shock.md) increases $K=p/\rho^{3/2}$, so

$$
\boxed{\frac{\lambda_2}{\lambda_1}=\left(\frac{K_2}{K_1}\right)^{4/5}>1.}
$$

More explicitly, the [Rankine-Hugoniot condition](../../../../../rankine-hugoniot-conditions.md) for $\gamma=3/2$ gives, with upstream $m=\mathcal M_1^2>1$,

$$
\frac{\rho_2}{\rho_1}=\frac{5m}{m+4},\qquad
\frac{p_2}{p_1}=\frac{6m-1}{5},\qquad
\mathcal M_2^2=\frac{m+4}{6m-1}<1.
$$

Thus the [shock wave](../../../../../shock-wave.md) jumps vertically, at the same $x$, from the [supersonic flow](../../../../../supersonic-flow.md) to a [subsonic flow](../../../../../subsonic-flow.md) on a larger-$\lambda$ curve. The figure illustrates an outward flow on $y=x$ with a [shock wave](../../../../../shock-wave.md) at $x=1.4$; the downstream [subsonic flow](../../../../../subsonic-flow.md) has $\lambda\simeq1.224$ and continues to larger $x$. The [shock wave](../../../../../shock-wave.md) radius is an additional boundary-data choice, rather than being determined by the smooth equations alone.

<a id="2/image-transonic-curves-and-a-stationary-shock"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314-flow-curves.png)

**[Figure 1](#2/image-transonic-curves-and-a-stationary-shock). Transonic curves and a stationary shock**. Solid blue curves have $\lambda=1$; grey curves have $\lambda=0.7$; orange curves have the downstream shock value $\lambda>1$. The vertical arrow is a supersonic-to-subsonic jump at fixed radius.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 314](../../paper-314-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
