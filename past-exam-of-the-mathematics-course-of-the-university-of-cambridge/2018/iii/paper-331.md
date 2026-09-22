# Paper 331

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_331.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_331.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
    - [iv](#1/c/iv)
      - [Solution](#1/c/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
    - [iii](#3/d/iii)
      - [Solution](#3/d/iii/solution)
    - [iv](#3/d/iv)
      - [Solution](#3/d/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
    - [iv](#4/a/iv)
      - [Solution](#4/a/iv/solution)
    - [v](#4/a/v)
      - [Solution](#4/a/v/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
    - [iv](#4/b/iv)
      - [Solution](#4/b/iv/solution)
    - [v](#4/b/v)
      - [Solution](#4/b/v/solution)
    - [vi](#4/b/vi)
      - [Solution](#4/b/vi/solution)

## 1

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

For [irrotational flow](../../../fluid-mechanics.md#irrotational-flow), $\mathbf u_j=\nabla\phi_j$. An impermeable stationary horizontal wall has zero normal velocity, so the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) is

$$
\boxed{\partial_z\phi_1(x,L_1,t)=0,\qquad\partial_z\phi_2(x,-L_2,t)=0.}
$$

No tangential no-slip condition is imposed on these inviscid fluids.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The interface is material: fluid particles on $F=z-\eta(x,t)=0$ remain there. Its [material derivative](../../../continuum-mechanics.md#material-derivative) therefore vanishes, giving $w_j=\eta_t+u_j\eta_x=D_j\eta/Dt$ on the interface. Since $w_j=\partial_z\phi_j$, this is the [kinematic boundary condition for a free-surface graph](../../../fluid-mechanics.md#kinematic-boundary-condition-for-a-free-surface-graph) on each side. The material derivatives use the respective tangential fluid velocities; they enforce the same moving normal boundary.

The [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation) gives $p_j+\rho_j[\partial_t\phi_j+|\nabla\phi_j|^2/2+gz]=C_j(t)$. Absorb the spatially constant functions $C_j$ into the gauges of the [velocity potentials](../../../fluid-mechanics.md#velocity-potential). Evaluating at $z=\eta$ and subtracting the equations yields the stated [dynamic boundary condition for an inviscid interface](../../../fluid-mechanics.md#dynamic-boundary-condition-for-an-inviscid-interface). [Surface tension](../../../fluid-mechanics.md#surface-tension) supplies the pressure jump, rather than pressure continuity. Thus **the first condition enforces material motion, and the second enforces the Bernoulli pressure balance**.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Use the [linearized boundary condition](../../../fluid-mechanics.md#linearized-boundary-condition): evaluate at $z=0$ and discard products of perturbations. The [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) and [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) become

$$
\partial_z\phi_1=\partial_z\phi_2=\eta_t,\qquad
\rho_1\phi_{1t}-\rho_2\phi_{2t}+g(\rho_1-\rho_2)\eta=-\gamma\eta_{xx}.
$$

[Incompressible flow](../../../fluid-mechanics.md#incompressible-flow) and [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) give the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) for each potential. For a [normal mode](../../../wave-equation.md#normal-mode), the wall conditions select

$$
\phi_1=A_1\cosh[k(z-L_1)]e^{i(kx-\omega t)},\qquad
\phi_2=A_2\cosh[k(z+L_2)]e^{i(kx-\omega t)}.
$$

With $\eta=Be^{i(kx-\omega t)}$, the kinematic conditions give $A_1=i\omega B/[k\sinh(kL_1)]$ and $A_2=-i\omega B/[k\sinh(kL_2)]$. Hence $\widehat\phi_1(0)=i\omega B\coth(kL_1)/k$ and $\widehat\phi_2(0)=-i\omega B\coth(kL_2)/k$. Substitution into the dynamic condition gives the [finite-depth Rayleigh-Taylor dispersion relation](../../../continuum-mechanics.md#finite-depth-rayleigh-taylor-dispersion-relation):

$$
\boxed{\omega^2[\rho_1\coth(kL_1)+\rho_2\coth(kL_2)]=-g(\rho_1-\rho_2)k+\gamma k^3.}
$$

Its denominator is positive. Assuming $g>0$ and $\gamma>0$, negative $\omega^2$ therefore produces a growing branch $\omega=i\sigma$ with $\sigma>0$, as in [Rayleigh-Taylor instability](../../../continuum-mechanics.md#rayleigh-taylor-instability).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Put $A=g(\rho_1-\rho_2)>0$. In the deep-layer limit, the [finite-depth Rayleigh-Taylor dispersion relation](../../../continuum-mechanics.md#finite-depth-rayleigh-taylor-dispersion-relation) gives $\omega^2=(\gamma k^3-Ak)/(\rho_1+\rho_2)$. Its sign changes at

$$
\boxed{k_c=\sqrt{\frac{g(\rho_1-\rho_2)}{\gamma}}.}
$$

The [Rayleigh-Taylor instability](../../../continuum-mechanics.md#rayleigh-taylor-instability) band is $0<k<k_c$; $k=k_c$ is neutral and $k>k_c$ is oscillatory.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For the growing [normal mode](../../../wave-equation.md#normal-mode) in two deep layers,

$$
\sigma^2(k)=\frac{Ak-\gamma k^3}{\rho_1+\rho_2},\qquad A=g(\rho_1-\rho_2).
$$

It vanishes at the endpoints of the unstable band and has its unique interior maximum where $A-3\gamma k^2=0$. Using $k_c=\sqrt{A/\gamma}$ gives

$$
\boxed{\sigma_m=\left[\frac{2A k_c}{3\sqrt3(\rho_1+\rho_2)}\right]^{1/2}.}
$$

This is the maximum exponential [growth rate](../../../wave-equation.md#growth-rate), not the real oscillation frequency.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The stationary-point condition for the squared [growth rate](../../../wave-equation.md#growth-rate) is $A-3\gamma k_m^2=0$. Its second derivative is $-6\gamma k_m/(\rho_1+\rho_2)<0$, so

$$
\boxed{k_m=\frac{k_c}{\sqrt3}=\sqrt{\frac{g(\rho_1-\rho_2)}{3\gamma}}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $L_2\to\infty$, the denominator is $\rho_1\coth(kL_1)+\rho_2>0$. The numerator is unchanged, so the cutoff is exactly independent of depth:

$$
\boxed{k_c=\sqrt{\frac{g(\rho_1-\rho_2)}{\gamma}}.}
$$

This remains exact before taking the thin-layer limit in the [finite-depth Rayleigh-Taylor dispersion relation](../../../continuum-mechanics.md#finite-depth-rayleigh-taylor-dispersion-relation).

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Write $A=g(\rho_1-\rho_2)$ and $\varepsilon=k_cL_1\ll1$. Throughout the unstable band, $kL_1\le\varepsilon$ and $\coth(kL_1)=1/(kL_1)+O(kL_1)$. Since $\rho_2<\rho_1$,

$$
\sigma^2(k)=\frac{Ak-\gamma k^3}{\rho_1\coth(kL_1)+\rho_2}
=\frac{L_1}{\rho_1}(Ak^2-\gamma k^4)[1+O(\varepsilon)].
$$

The leading polynomial is maximized at $k^2=A/(2\gamma)$, where it equals $L_1A^2/(4\rho_1\gamma)$. Thus the [thin-layer Rayleigh-Taylor growth asymptotics](../../../continuum-mechanics.md#thin-layer-rayleigh-taylor-growth-asymptotics) give

$$
\boxed{\sigma_m\sim\frac{g(\rho_1-\rho_2)}2\sqrt{\frac{L_1}{\rho_1\gamma}}.}
$$

This is a leading asymptotic expression; the exact maximum for a small but nonzero layer depth has corrections.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Maximize the leading thin-layer squared [growth rate](../../../wave-equation.md#growth-rate), $(L_1/\rho_1)(Ak^2-\gamma k^4)$. Its positive stationary point obeys $2Ak-4\gamma k^3=0$ and is the unique interior maximum. Therefore

$$
\boxed{k_m\sim\frac{k_c}{\sqrt2}=\sqrt{\frac{g(\rho_1-\rho_2)}{2\gamma}}.}
$$

The maximizing point stays within the thin-layer regime because $k_mL_1\sim k_cL_1/\sqrt2\ll1$.

<h4 id="1/c/iv">iv</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/c/iv)

Use superscripts $T$ and $D$ for the thin-upper-layer and two-deep-layer cases. The cutoff is identical, while

$$
\boxed{\frac{k_m^T}{k_m^D}\sim\sqrt{\frac32},\qquad
\frac{\sigma_m^T}{\sigma_m^D}\sim\left[\frac{3\sqrt3(\rho_1+\rho_2)}{8\rho_1}\,k_cL_1\right]^{1/2}\ll1.}
$$

Thus confinement suppresses the [Rayleigh-Taylor instability](../../../continuum-mechanics.md#rayleigh-taylor-instability) growth strongly, but moves the most amplified disturbance to a somewhat larger [wavenumber](../../../wave-equation.md#wavenumber). The cutoff depends on the gravity-capillary balance, whereas growth depends also on the inertia of the moving layers.

## 2

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

First suppose $c_i\ne0$ and put $F=\widehat w/(U-c)$. The wall condition gives $F(\pm L)=0$. Substitution into the [Rayleigh equation for inviscid shear flow](../../../hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow) gives

$$
[(U-c)^2F']'-k^2(U-c)^2F=0.
$$

Multiply by $\overline F$ and use [integration by parts](../../../calculus.md#integration-by-parts). The resulting [weighted identity for Howard's semicircle theorem](../../../hydrodynamic-stability.md#weighted-identity-for-howard-s-semicircle-theorem) is

$$
\int_{-L}^L(U-c)^2Q\,dz=0,\qquad Q=|F'|^2+k^2|F|^2,\qquad I=\int Q\,dz>0.
$$

Its imaginary part gives $\int UQ=c_rI$, and its real part then gives $\int U^2Q=(c_r^2+c_i^2)I$. Set $a=U_{\min}$ and $b=U_{\max}$. Since $(U-a)(b-U)\ge0$,

$$
0\le\int(U-a)(b-U)Q\,dz
=\bigl[(a+b)c_r-ab-c_r^2-c_i^2\bigr]I.
$$

Completing the square proves [Howard's semicircle theorem](../../../hydrodynamic-stability.md#howard-s-semicircle-theorem):

$$
\boxed{\left(c_r-\frac{U_{\max}+U_{\min}}2\right)^2+c_i^2\le\left(\frac{U_{\max}-U_{\min}}2\right)^2.}
$$

In particular every growing [normal mode](../../../wave-equation.md#normal-mode) lies in the upper semicircle for $k>0$. If $c$ is real and outside $[a,b]$, $F$ is again regular, but the same identity has a strictly positive integrand unless the mode vanishes. Such a neutral mode is impossible. Consequently neutral regular modes also satisfy the bound; no division by $c_i$ is needed for this last conclusion. The nonreal proof avoids critical-level singularities altogether.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Normalize $U$ and $c$ by $U_{\max}$ and write $h=\zeta_L\in(0,1)$, $\alpha=kL>0$. In each open region $U''=0$, so the [Rayleigh equation for inviscid shear flow](../../../hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow) reduces to $\widehat w''-\alpha^2\widehat w=0$ for the nonreal modes of interest. Incorporating the wall conditions from the start, the [bounded piecewise-linear shear layer](../../../hydrodynamic-stability.md#bounded-piecewise-linear-shear-layer) has

$$
\boxed{\begin{aligned}
\widehat w_1&=A\sinh[\alpha(1-\zeta)],\\
\widehat w_2&=B\cosh(\alpha\zeta)+C\sinh(\alpha\zeta),\\
\widehat w_3&=D\sinh[\alpha(1+\zeta)].
\end{aligned}}
$$

These are four independent regional amplitudes before matching. The same expressions extend to noncritical neutral modes and their limits.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Impermeability gives $\widehat w(\pm1)=0$. At $\zeta=\pm h$, the base velocity is continuous but its derivative jumps. The normal velocity and pressure must remain continuous. From incompressibility and the streamwise linearized momentum equation,

$$
\widehat p=\frac{\rho}{ik}\bigl[(U-c)\widehat w_z-U_z\widehat w\bigr].
$$

Therefore, with derivatives now taken in $\zeta$, the [vorticity-jump matching for an inviscid shear flow](../../../hydrodynamic-stability.md#vorticity-jump-matching-for-an-inviscid-shear-flow) is

$$
\boxed{[\widehat w]=0,\qquad[(U-c)\widehat w'-U'\widehat w]=0\quad\text{at }\zeta=\pm h.}
$$

At the upper jump $[U']=-1/h$ and at the lower jump $[U']=1/h$, where brackets mean the limit from larger $\zeta$ minus that from smaller $\zeta$. Equivalently $(U-c)[\widehat w']=[U']\widehat w$ away from $U=c$. Setting $[\widehat w']=0$ would discard the vorticity jumps and give the wrong eigenproblem.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Let $q=\alpha h$, $d=\alpha(1-h)$, and use the four regional amplitudes above. Continuity of $\widehat w$ at the two jumps gives

$$
A\sinh d=B\cosh q+C\sinh q,\qquad
D\sinh d=B\cosh q-C\sinh q.
$$

Pressure continuity, using [vorticity-jump matching for an inviscid shear flow](../../../hydrodynamic-stability.md#vorticity-jump-matching-for-an-inviscid-shear-flow), gives the other two equations:

$$
\begin{aligned}
-\alpha(1-c)(A\cosh d+B\sinh q+C\cosh q)
+\frac{B\cosh q+C\sinh q}{h}&=0,\\
-\alpha(1+c)(-B\sinh q+C\cosh q-D\cosh d)
-\frac{B\cosh q-C\sinh q}{h}&=0.
\end{aligned}
$$

These are the required homogeneous four equations. As a useful reduction, put $X=\tanh q$, $Y=\tanh d$, $H=q(1+XY)$ and $J=q(X+Y)$. Eliminating $A,D$ leaves

$$
\boxed{[(1-c)H-Y]B+[(1-c)J-XY]C=0,\qquad
[(1+c)H-Y]B-[(1+c)J-XY]C=0.}
$$

The vanishing [determinant](../../../linear-algebra.md#determinant) gives $c^2=(H-Y)(J-XY)/(HJ)$, which expands to the printed [dispersion relation](../../../wave-equation.md#dispersion-relation).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For fixed $h\in(0,1)$, $X=\alpha h+O(\alpha^3)$ and $Y=\alpha(1-h)+O(\alpha^3)$. The factored [dispersion relation](../../../wave-equation.md#dispersion-relation) therefore gives

$$
\lim_{\alpha\to0}c^2=2h-1,\qquad
\lim_{\alpha\to\infty}c^2=1,
$$

where the latter follows from $X,Y\to1$ and $c^2\sim(1-1/(2\alpha h))^2$. A real negative $c^2$ yields a growing branch $c=i\sqrt{-c^2}$ for positive $k$. Thus $h<1/2$ gives instability at sufficiently small nonzero wavenumber.

For the converse, monotonicity toward the limiting value one would suffice, as permitted in the question. In fact a direct sign argument avoids this extra assumption. With $q=\alpha h>0$, $X=\tanh q<q$, so $J-XY=qX+(q-X)Y>0$. If $h\ge1/2$, then $q\ge d=\alpha(1-h)$ and $Y=\tanh d<d\le q$. Hence $H-Y=q(1+XY)-Y>0$, so $c^2>0$ for every $\alpha>0$. We obtain the exact [instability threshold for a bounded piecewise-linear shear layer](../../../hydrodynamic-stability.md#instability-threshold-for-a-bounded-piecewise-linear-shear-layer):

$$
\boxed{0<\zeta_L<\frac12\quad\text{is the condition for exponential linear instability}.}
$$

At $\zeta_L=1/2$ the long-wave limiting value is zero, but every finite positive wavenumber has $c^2>0$.

## 3

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Choose a length $\ell$, velocity $U_s$, time $\ell/U_s$, and pressure $\rho U_s^2$, giving [Reynolds number](../../../fluid-mechanics.md#reynolds-number) $Re=U_s\ell/\nu$. Write perturbation velocity as $(u,v,w)$ and let $\mathcal L=\partial_t+U\partial_x-Re^{-1}\nabla^2$. Linearizing the incompressible [Navier-Stokes equations](../../../viscous-fluid-flow.md#navier-stokes-equation) gives

$$
\mathcal Lu+U'v=-p_x,\quad\mathcal Lv=-p_y,\quad\mathcal Lw=-p_z,\quad u_x+v_y+w_z=0.
$$

Taking the divergence gives $\nabla^2p=-2U'v_x$. Applying $\nabla^2$ to the wall-normal momentum equation and using

$$
\nabla^2(Uv_x)=U\nabla^2v_x+2U'v_{xy}+U''v_x
$$

then cancels the pressure derivatives and yields $\mathcal L\nabla^2v-U''v_x=0$. Define wall-normal [vorticity](../../../fluid-mechanics.md#vorticity) $\eta=u_z-w_x$. Applying $\partial_z$ to the streamwise equation minus $\partial_x$ to the spanwise equation gives $\mathcal L\eta=-U'v_z$.

For the assumed [normal modes](../../../wave-equation.md#normal-mode), set $D=d/dy$ and $\kappa^2=\alpha^2+\beta^2$. The two equations become the [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation) and [Squire equation](../../../hydrodynamic-stability.md#squire-equation):

$$
\boxed{[(-i\omega+i\alpha U)(D^2-\kappa^2)-i\alpha U''-Re^{-1}(D^2-\kappa^2)^2]\widehat v=0,}
$$



$$
\boxed{[(-i\omega+i\alpha U)-Re^{-1}(D^2-\kappa^2)]\widehat\eta=-i\beta U'\widehat v.}
$$

At rigid no-slip walls the conditions are $\widehat v=D\widehat v=\widehat\eta=0$ for nonzero horizontal wavenumber.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

An [Orr-Sommerfeld mode](../../../hydrodynamic-stability.md#orr-sommerfeld-mode) has $\widehat v\ne0$ satisfying the [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation), with accompanying vorticity satisfying the forced [Squire equation](../../../hydrodynamic-stability.md#squire-equation). A [Squire mode](../../../hydrodynamic-stability.md#squire-mode) has $\widehat v=0$ and $\widehat\eta\ne0$, so its Squire equation is homogeneous.

For a Squire mode multiply that homogeneous equation by $\overline\eta$ and integrate over the channel. Under the no-slip condition $\eta=0$ at the walls, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
-i\omega\int|\eta|^2dy+i\alpha\int U|\eta|^2dy
=-\frac1{Re}\int(|\eta'|^2+\kappa^2|\eta|^2)dy.
$$

Since $U,\alpha$ are real, taking the real part proves

$$
\boxed{\operatorname{Im}\omega=-\frac{\int(|\eta'|^2+\kappa^2|\eta|^2)dy}{Re\int|\eta|^2dy}<0.}
$$

The numerator is strictly positive for a nontrivial finite-channel mode, and $Re>0$. Thus Squire modes are exponentially damped in the convention $e^{-i\omega t}$. This does not rule out [transient growth from non-normal modes](../../../hydrodynamic-stability.md#transient-growth-from-non-normal-modes) in the coupled system.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

With $U=U_0$ and $\beta=0$, the [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation) factors into constant-coefficient operators:

$$
(D^2-\alpha^2)(D^2-\gamma^2)\widehat v=0,\qquad
\boxed{\gamma^2=\alpha^2+iRe(\alpha U_0-\omega).}
$$

For distinct nonzero characteristic roots, the general solution is

$$
\boxed{\widehat v=a_1e^{\alpha y}+a_2e^{-\alpha y}+a_3e^{\gamma y}+a_4e^{-\gamma y}.}
$$

Either square-root choice for $\gamma$ gives the same solution space. The [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) and impermeability impose $\widehat v=D\widehat v=0$ at each wall.

The displayed exponential basis needs the usual repeated-root qualification. If $\gamma^2=\alpha^2\ne0$, replace it by $(a_1+a_2y)e^{\alpha y}+(a_3+a_4y)e^{-\alpha y}$. If just one root pair is zero, that pair contributes $1,y$; if both pairs are zero, the basis is $1,y,y^2,y^3$. These are the complete limiting cases, not four independent copies of a repeated exponential.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Take $k^*>0$ and positive shear scale $S^*$, with kinematic viscosity $\nu^*$. Choose

$$
y=k^*y^*,\quad x=k^*x^*,\quad t=S^*t^*,\quad U=\frac{k^*U^*}{S^*}=y,\quad c=\frac{k^*c^*}{S^*},\quad
\boxed{Re=\frac{S^*}{\nu^*(k^*)^2}.}
$$

The velocity scale is $S^*/k^*$. A reversed shear can be treated by reversing the corresponding coordinate orientation and mode convention. The dimensional [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation), with $U^{*\prime\prime}=0$, is

$$
(U^*-c^*)(D_*^2-(k^*)^2)\widehat v^*
=\frac{\nu^*}{ik^*}(D_*^2-(k^*)^2)^2\widehat v^*.
$$

Substitution of the scales and cancellation gives

$$
\boxed{(y-c)(D^2-1)\widehat v=-\frac{i}{Re}(D^2-1)^2\widehat v.}
$$

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

In two dimensions at nondimensional streamwise wavenumber one, incompressibility gives $i\widehat u+D\widehat v=0$, so $\widehat u=iD\widehat v$. The spanwise [vorticity](../../../fluid-mechanics.md#vorticity) is the $z$ component of the curl:

$$
\widehat\zeta=i\widehat v-D\widehat u=-i(D^2-1)\widehat v.
$$

Consequently

$$
\boxed{\widehat\omega=(D^2-1)\widehat v=i\widehat\zeta.}
$$

The symbol $\widehat\omega$ here denotes a vorticity amplitude, not the temporal frequency used elsewhere. In dimensional variables, $\widehat\zeta^*=-i(D_*^2-(k^*)^2)\widehat v^*/k^*$, with the same sign convention.

<h4 id="3/d/iii">iii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/d/iii)

Put $W=(D^2-1)\widehat v$ and $\delta^3=Re^{-1}$. The constant-shear [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation) gives

$$
(y-c)W=-i\delta^3(W''-W),\qquad
W''=\left[1+\frac{i(y-c)}{\delta^3}\right]W
=\frac{i(y-c-i\delta^3)}{\delta^3}W.
$$

Let $a=e^{i\pi/6}$ and $Z=a(y-c-i\delta^3)/\delta$. Since $d/dy=(a/\delta)d/dZ$ and $a^3=i$, the equation becomes

$$
\frac{a^2}{\delta^2}W_{ZZ}=\frac{i}{a\delta^2}ZW,\qquad
\boxed{W_{ZZ}-ZW=0.}
$$

This is the [Airy ordinary differential equation](../../../differential-equation.md#airy-ordinary-differential-equation), yielding the [Airy reduction of the Orr-Sommerfeld equation in constant shear](../../../hydrodynamic-stability.md#airy-reduction-of-the-orr-sommerfeld-equation-in-constant-shear). It is distinct from the evolution PDE represented by the existing [Airy equation](../../../integrable-systems.md#airy-equation) article.

<h4 id="3/d/iv">iv</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/d/iv)

Write $W(s)=a_1\operatorname{Ai}(Z(s))+a_2\operatorname{Bi}(Z(s))$, using the independent [Airy functions](../../../differential-equation.md#airy-function). To solve $(D^2-1)\widehat v=W$, the [variation of parameters](../../../differential-equation.md#variation-of-parameters) formula, equivalently a direct convolution, gives the [velocity reconstruction from the Orr-Sommerfeld vorticity](../../../hydrodynamic-stability.md#velocity-reconstruction-from-the-orr-sommerfeld-vorticity):

$$
\boxed{\widehat v(y)=C_+e^y+C_-e^{-y}
+\int_{y_0}^y\sinh(y-s)\left[a_1\operatorname{Ai}(Z(s))+a_2\operatorname{Bi}(Z(s))\right]ds.}
$$

The reference point $y_0$ is arbitrary. Twice differentiating the integral produces $W(y)$ because $\sinh0=0$ and its derivative at zero is one, verifying the formula. The four constants are independent: applying $D^2-1$ to an identically zero combination first forces $a_1=a_2=0$, then the complementary solutions force $C_+=C_-=0$. The boundary conditions would be $\widehat v(y_j)=D\widehat v(y_j)=0$, $j=1,2$. Their compatibility selects the eigenvalues; they need not be imposed here.

## 4

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is the absolutely convergent power series

$$
\boxed{B(t)=e^{Lt}=\sum_{m=0}^\infty\frac{t^mL^m}{m!}.}
$$

It converges in any finite-dimensional [operator norm](../../../continuous-dual-space.md#operator-norm), since $\|L^m\|\le\|L\|^m$. Termwise differentiation gives $B'=LB$, $B(0)=I$, so the solution is $q(t)=B(t)q_0$. Also $e^{Lt}e^{-Lt}=I$, proving invertibility without requiring $L$ itself to be invertible.

The question's expansion in eigenvectors tacitly needs an eigenbasis: an invertible matrix alone need not be a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix). The exponential solution and the singular-value arguments remain valid without that assumption.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The relevant norm is the [operator norm](../../../continuous-dual-space.md#operator-norm) induced by the complex [Euclidean norm](../../../functional-analysis.md#euclidean-norm), also called the [matrix 2-norm](../../../continuous-dual-space.md#matrix-2-norm):

$$
\boxed{\|B\|_2=\max_{q\ne0}\frac{\|Bq\|_2}{\|q\|_2}=\max_{\|q\|_2=1}\|Bq\|_2.}
$$

The maximum exists because the unit sphere in finite dimensions is compact. It obeys $\|Bq\|_2\le\|B\|_2\|q\|_2$ and is the norm relevant to the specified perturbation energy. Other matrix norms do not in general give this gain.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

A [normal matrix](../../../linear-operator-theory.md#normal-matrix) admits [unitary diagonalization of a normal matrix](../../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix): $L=V\operatorname{diag}(\lambda_j)V^\dagger$ with orthonormal eigenvectors. Thus

$$
e^{Lt}=V\operatorname{diag}(e^{\lambda_jt})V^\dagger,\qquad
\|e^{Lt}q_0\|_2^2=\sum_j e^{2\operatorname{Re}\lambda_jt}|\phi_j|^2,\quad
\|q_0\|_2^2=\sum_j|\phi_j|^2.
$$

For $t\ge0$, the largest weight belongs to an eigenvalue with maximal real part. The weighted average is bounded by that weight and attains it on the corresponding eigenspace. Therefore the [optimal energy amplification of a linear system](../../../linear-operator-theory.md#optimal-energy-amplification-of-a-linear-system) is

$$
\boxed{G(t)=e^{2\operatorname{Re}\lambda_1t}\quad(t\ge0).}
$$

If the largest real part is repeated, any nonzero combination within that maximal eigenspace is optimal. For negative times the ordering reverses; the displayed formula concerns forward evolution.

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

The [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) of $B$ is $B=U\Sigma V^\dagger$, where $U,V$ are unitary and $\Sigma=\operatorname{diag}(\sigma_1,\ldots,\sigma_n)$, $\sigma_1\ge\cdots\ge\sigma_n>0$ since $B$ is invertible. Its [right singular vector](../../../linear-algebra.md#right-singular-vector) $v_j$ and [left singular vector](../../../linear-algebra.md#left-singular-vector) $u_j$ are the corresponding unit columns of $V$ and $U$, with

$$
\boxed{Bv_j=\sigma_ju_j,\qquad B^\dagger u_j=\sigma_jv_j.}
$$

Equivalently $B^\dagger Bv_j=\sigma_j^2v_j$ and $BB^\dagger u_j=\sigma_j^2u_j$. The positive numbers $\sigma_j$ are the [singular values](../../../linear-algebra.md#singular-value). Degenerate singular subspaces allow any orthonormal choice of paired vectors.

<h4 id="4/a/v">v</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/v/solution">Solution</h5>

↑ **Parent:** [V](#4/a/v)

For $q(t)=Bq_0$, the energy ratio is the [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) of the [Hermitian positive-definite matrix](../../../linear-algebra.md#hermitian-positive-definite-matrix) $B^\dagger B$:

$$
\frac{\|Bq_0\|_2^2}{\|q_0\|_2^2}=\frac{q_0^\dagger B^\dagger Bq_0}{q_0^\dagger q_0}.
$$

Expanding $q_0$ in the orthonormal [right singular vectors](../../../linear-algebra.md#right-singular-vector) makes this a weighted average of $\sigma_j^2$. Hence

$$
\boxed{G(t)=\|e^{Lt}\|_2^2=\sigma_1^2(t),\qquad q_0\propto v_1(t).}
$$

Any nonzero vector in the largest right-singular subspace is optimal if $\sigma_1$ is repeated. Its amplified state is proportional to the paired [left singular vector](../../../linear-algebra.md#left-singular-vector). For a [non-normal matrix](../../../linear-operator-theory.md#non-normal-matrix) $L$, this optimal initial direction need not be an eigenvector of $L$, explaining [transient growth from non-normal modes](../../../hydrodynamic-stability.md#transient-growth-from-non-normal-modes).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

A [normal mode](../../../wave-equation.md#normal-mode) $x\propto e^{-i\omega t}$ has eigenvalue $\lambda=-i\omega$ of $A$. Setting $d_\omega=\omega-\omega_1$, the characteristic equation is

$$
(-id_\omega)(-i(d_\omega+b))-ac=0,
\qquad d_\omega^2+bd_\omega+ac=0.
$$

Thus

$$
\omega=\omega_1-\frac b2\pm\sqrt{\frac{b^2}{4}-ac},\qquad
\boxed{\text{exponential modal instability}\ \Longleftrightarrow\ 4ac>b^2.}
$$

One branch then has positive imaginary frequency and hence positive exponential [growth rate](../../../wave-equation.md#growth-rate). If $4ac<b^2$, both frequencies are real and the distinct-eigenvalue system has bounded oscillatory motion. At equality there is no positive exponential growth rate, but a nontrivial [Jordan block](../../../linear-operator-theory.md#jordan-block) can cause algebraic growth, so exponential neutrality must not be confused with [Lyapunov stability](../../../dynamical-systems.md#lyapunov-stability). The parameter $d$ listed in the PDF does not appear in the printed matrix and has no effect on this calculation.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Put $q=10/Re>0$. The frequency formula becomes

$$
\omega_\pm=\omega_1-\frac q2\pm i\sqrt{q-\frac{q^2}{4}}.
$$

For large positive [Reynolds number](../../../fluid-mechanics.md#reynolds-number), $\sqrt{q-q^2/4}=\sqrt q[1-q/8+O(q^2)]$. Therefore

$$
\boxed{\omega_\pm=\omega_1\pm i\sqrt{\frac{10}{Re}}+O(Re^{-1}).}
$$

More precisely the real correction is $-5/Re$, and the next imaginary correction is $O(Re^{-3/2})$. The growing branch has a rate tending to zero as $Re\to\infty$, despite being unstable at every sufficiently large finite $Re$.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

For $q=10/Re$, the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
\boxed{\lambda_\pm=-i\omega_1+\frac{iq}{2}\pm\sqrt{q-\frac{q^2}{4}}.}
$$

For physical $Re>0$, this gives the following classification. If $Re>5/2$, then $0<q<4$ and one eigenvalue has positive real part: exponential instability. If $0<Re<5/2$, then $q>4$, both eigenvalues are distinct and imaginary, and solutions are bounded oscillatory combinations. At $Re=5/2$ there is a repeated imaginary eigenvalue $\lambda_0=-i\omega_1+2i$. The matrix $N=A-\lambda_0I=\begin{pmatrix}-2i&1\\4&2i\end{pmatrix}$ is nonzero and satisfies $N^2=0$, so $e^{At}=e^{\lambda_0t}(I+tN)$ has algebraically growing trajectories.

Thus **the exponential instability threshold is $Re>5/2$**, consistently with $4ac>b^2$, which here is $4q>q^2$. At the threshold the matrix is defective, and the eigenvector-basis assumption from part (a) cannot be used; the matrix-exponential and singular-value formulas still apply.

<h4 id="4/b/iv">iv</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/b/iv)

A [normal matrix](../../../linear-operator-theory.md#normal-matrix) satisfies $AA^\dagger=A^\dagger A$. Direct multiplication, with all parameters real, gives the [normality criterion for a two-mode shear model](../../../linear-operator-theory.md#normality-criterion-for-a-two-mode-shear-model):

$$
AA^\dagger-A^\dagger A=
\begin{pmatrix}a^2-c^2&-ib(a+c)\\ib(a+c)&c^2-a^2\end{pmatrix}.
$$

For $a=1$, $b=c=q=10/Re$, both $1-q^2=0$ and $q(1+q)=0$ are required. Their only common solution is $q=-1$. Hence

$$
\boxed{Re_N=-10\ \text{formally};\qquad\text{no normal case exists for }Re>0.}
$$

The original PDF really has these signs and $b=c=10/Re$. Thus parts (v) and (vi) have no physical positive-Reynolds-number case as printed. We give their algebraic continuation at $Re=-10$ below, without silently changing the matrix. The tempting value $Re=10$ makes the off-diagonal magnitudes equal but fails the off-diagonal commutator condition.

<h4 id="4/b/v">v</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/v/solution">Solution</h5>

↑ **Parent:** [V](#4/b/v)

At the formal value $Re=-10$, $q=-1$ and $A=-i\omega_1I+\begin{pmatrix}0&1\\-1&-i\end{pmatrix}$ is a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix). Put $r_\pm=(-1\pm\sqrt5)/2$. Its two eigenvalues and normalized [eigenvectors](../../../linear-operator-theory.md#eigenvector) are

$$
\lambda_\pm=-i\omega_1+ir_\pm,\qquad
\boxed{v_\pm=\frac{(1,ir_\pm)^T}{\sqrt{1+r_\pm^2}}.}
$$

Substitution uses $r_\pm^2+r_\pm-1=0$ and verifies $Av_\pm=\lambda_\pm v_\pm$. Their Hermitian inner product is

$$
v_+^\dagger v_-=
\frac{1+r_+r_-}{\sqrt{(1+r_+^2)(1+r_-^2)}}=0,
$$

since $r_+r_-=-1$. This provides the requested orthogonality in the formal continuation. There is no corresponding physical $Re_N>0$ for the printed system.

<h4 id="4/b/vi">vi</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#4/b/vi)

At the only algebraic normal value $Re=-10$, the generator is a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix), so its [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix). Both eigenvalues have zero real part; hence

$$
\boxed{G(t)=1\quad\text{and every nonzero }(x_1(0),x_2(0))\text{ is optimal}.}
$$

There is no distinguished initial amplitude ratio and no perturbation-energy growth. The relations $x_2(0)=ir_\pm x_1(0)$ select the individual orthogonal eigenmodes, but arbitrary nonzero combinations are equally optimal because all singular values are one. If $Re$ is restricted to its physical positive domain, this part has no applicable normal case at all. This resolves the inconsistency in the original printed parameters rather than assuming an unjustified optimal direction.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
