# Paper 54

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_54.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_54.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

In the vacuum exterior, the [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) gives $m'=0$, so $m(r)=M$. The remaining metric function obeys

$$
\Phi'(r)=\frac{M}{r(r-2M)}=\frac12\frac{d}{dr}\log\left(1-\frac{2M}{r}\right).
$$

Thus $e^{2\Phi}=C(1-2M/r)$. A constant rescaling of the time coordinate removes $C$; equivalently, [asymptotic flatness](../../../general-relativity.md#asymptotically-flat-spacetime) fixes $C=1$ when time is normalized at infinity. Consequently **the exterior is the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime)**:

$$
\boxed{ds^2=-\left(1-\frac{2M}{r}\right)dt^2+\left(1-\frac{2M}{r}\right)^{-1}dr^2+r^2d\Omega^2,\qquad r>R.}
$$

The [mass](../../../classical-mechanics.md#mass) $M=m(R)$ includes the full [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) interior. No equation of state beyond the surface enters this vacuum result.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

A [regular central expansion of the TOV equations](../../../general-relativity.md#regular-central-expansion-of-the-tov-equations) requires $m(0)=0$. Once $\rho_c$ is chosen, the [barotropic stellar equation of state](../../../thermodynamics.md#barotropic-stellar-equation-of-state) fixes $p_c=p(\rho_c)$. Smoothness at the centre forces the radial first derivatives of $p$ and $\rho$ to vanish. Expanding the [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) gives

$$
\begin{aligned}
m(r)&=\frac{4\pi}{3}\rho_c r^3+O(r^5),\\
p(r)&=p_c-2\pi(\rho_c+p_c)\left(\frac{\rho_c}{3}+p_c\right)r^2+O(r^4),\\
\Phi(r)&=\Phi_c+2\pi\left(\frac{\rho_c}{3}+p_c\right)r^2+O(r^4).
\end{aligned}
$$

Since $dp/d\rho>0$, the [equation of state](../../../thermodynamics.md#equation-of-state) is locally invertible, and these coefficients determine the corresponding [energy density](../../../statistical-physics.md#energy-density) expansion as well. Integrating the regular solution outward gives the surface at the first zero of the [pressure](../../../thermodynamics.md#pressure), when such a finite surface exists. The [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) uniqueness theorem then fixes the interior and its exterior [mass](../../../classical-mechanics.md#mass) from $\rho_c$.

The additive constant $\Phi_c$ is a time-coordinate normalization, not a second physical parameter. Matching to the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) with time normalized at infinity fixes it. Therefore **the regular stellar solutions, modulo time rescaling, have one physical parameter: $\rho_c$**. This statement uses a suitably smooth fixed [equation of state](../../../thermodynamics.md#equation-of-state) and refers to central densities for which the solution actually forms a regular star; not every central [energy density](../../../statistical-physics.md#energy-density) need give a finite-radius configuration.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The useful [high-density core bound from TOV compactness](../../../general-relativity.md#high-density-core-bound-from-tov-compactness) follows without choosing the unknown high-density [equation of state](../../../thermodynamics.md#equation-of-state). Let $a$ be the radius at which the decreasing [energy density](../../../statistical-physics.md#energy-density) first reaches $\rho_0$, and put $\mu=m(a)$, $p_0=p(\rho_0)$. The [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) gives $p'<0$ away from a nonempty centre; since $dp/d\rho>0$, [energy density](../../../statistical-physics.md#energy-density) decreases outward. Hence

$$
\mu=4\pi\int_0^a\rho(r)r^2\,dr\geq\frac{4\pi}{3}\rho_0a^3.
$$

For the local [stellar compactness](../../../general-relativity.md#stellar-compactness), if $z\geq0$, $1-z+\sqrt{1+z}\leq2$, since its derivative is $-1+(2\sqrt{1+z})^{-1}<0$. Applying the supplied compactness inequality at the core boundary therefore gives $\mu/a<4/9$. Combining the two bounds yields

$$
\boxed{a<\frac1{\sqrt{3\pi\rho_0}},\qquad\mu<\frac4{9\sqrt{3\pi\rho_0}}.}
$$

The pressure-dependent form further restricts the allowed core-boundary data:

$$
\frac{\mu}{a}<\frac29\left(1-6\pi a^2p_0+\sqrt{1+6\pi a^2p_0}\right).
$$

In particular, positivity of its right side gives $6\pi a^2p_0<3$, so $a^2<1/(2\pi p_0)$ when $p_0>0$. These restrictions depend only on known quantities, not on the [equation of state](../../../thermodynamics.md#equation-of-state) above $\rho_0$.

The intended stellar-mass argument now attaches the known low-density envelope to each admissible pair $(a,\mu)$ with [pressure](../../../thermodynamics.md#pressure) $p_0$. Its [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) involves only the known [equation of state](../../../thermodynamics.md#equation-of-state). For a physical low-density envelope with a uniformly bounded [mass](../../../classical-mechanics.md#mass) on this bounded set of core data, taking the supremum of the envelope-plus-core masses gives an upper [mass](../../../classical-mechanics.md#mass) limit independent of any high-density continuation. Stars with $\rho_c\leq\rho_0$ are also determined entirely by the known [equation of state](../../../thermodynamics.md#equation-of-state). **Unknown dense-core physics cannot evade the displayed core bounds.**

A qualification is necessary for a claim about the entire star: **the printed monotonicity assumptions alone do not guarantee a finite maximum total [mass](../../../classical-mechanics.md#mass) for an arbitrary known low-density [equation of state](../../../thermodynamics.md#equation-of-state)**. An explicit [low-density polytropic mass divergence](../../../stellar-structure.md#low-density-polytropic-mass-divergence) occurs for $p=K\rho^{5/4}$ with fixed $K>0$. In the low-density [Newtonian limit](../../../general-relativity.md#newtonian-limit), this is a [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) of index $n=4$, whose [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation) has a finite first zero. With $\rho=\rho_c\vartheta^4$ and $r=\ell\xi$, hydrostatic balance fixes

$$
\ell^2=\frac{5K}{4\pi}\rho_c^{-3/4},\qquad M=4\pi\rho_c\ell^3\mu_4\propto\rho_c^{-1/8},\qquad R\propto\rho_c^{-3/8},
$$

where $\mu_4>0$ is the dimensionless [Lane-Emden surface mass constant](../../../stellar-structure.md#lane-emden-surface-mass-constant). Thus $M\to\infty$ as $\rho_c\to0$, although $M/R\propto\rho_c^{1/4}\to0$. The first Lane-Emden zero is simple. The [continuous dependence of an ODE solution on parameters](../../../differential-equation.md#continuous-dependence-of-an-ode-solution-on-parameters) therefore preserves this finite surface for sufficiently small relativistic parameter. The relativistic correction is controlled by $p_c/\rho_c=K\rho_c^{1/4}\to0$, so the corresponding regular finite-radius [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) solutions have the same limiting scalings. They never sample $\rho>\rho_0$, and satisfy the local positivity and monotonicity assumptions in their nonvacuum interiors. This shows exactly why a suitable bounded-envelope hypothesis, or an appropriate restriction to physically stable stellar models, must accompany the intended total-mass conclusion. The compactness inequality supplies a bound on the unknown core, not a bound on the [mass](../../../classical-mechanics.md#mass) of every conceivable dilute envelope.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For the constant-density model, $m(r)=4\pi\rho r^3/3=Mr^3/R^3$. This is the incompressible [Interior Schwarzschild metric](../../../general-relativity.md#interior-schwarzschild-metric), replacing the earlier finite-slope [barotropic stellar equation of state](../../../thermodynamics.md#barotropic-stellar-equation-of-state). The [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) separates as

$$
\frac{dp}{(p+\rho)(p+\rho/3)}=-\frac{4\pi r\,dr}{1-8\pi\rho r^2/3}.
$$

On the left, partial fractions give

$$
\int\frac{dp}{(p+\rho)(p+\rho/3)}=\frac{3}{2\rho}\log\frac{p+\rho/3}{p+\rho}.
$$

On the right the antiderivative is $\tfrac3{4\rho}\log(1-8\pi\rho r^2/3)$. Applying the surface condition $p(R)=0$, and writing $s(r)=\sqrt{1-2Mr^2/R^3}$, $s_R=\sqrt{1-2M/R}$, gives

$$
\frac{p+\rho/3}{p+\rho}=\frac{s(r)}{3s_R}.
$$

Solving for the [pressure](../../../thermodynamics.md#pressure) recovers the [Interior Schwarzschild solution](../../../general-relativity.md#interior-schwarzschild-metric):

$$
p(r)=\rho\frac{s(r)-s_R}{3s_R-s(r)}.
$$

In particular the [central pressure of a constant-density relativistic star](../../../general-relativity.md#central-pressure-of-a-constant-density-relativistic-star) is

$$
\boxed{p_c=\rho\frac{1-\sqrt{1-2M/R}}{3\sqrt{1-2M/R}-1}.}
$$

The denominator must be positive for a regular positive-pressure centre, requiring $M/R<4/9$. As that limiting compactness is approached, the central [pressure](../../../thermodynamics.md#pressure) diverges, in agreement with [Buchdahl's theorem](../../../general-relativity.md#buchdahl-s-theorem).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For a [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) with nonnegative [energy density](../../../statistical-physics.md#energy-density) and [pressure](../../../thermodynamics.md#pressure), the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) is $p\leq\rho$. [Pressure](../../../thermodynamics.md#pressure) decreases outward, so it is enough to test the central [pressure](../../../thermodynamics.md#pressure). Put $s=\sqrt{1-2M/R}$; the regular [Interior Schwarzschild metric](../../../general-relativity.md#interior-schwarzschild-metric) requires $3s-1>0$. The [central pressure of a constant-density relativistic star](../../../general-relativity.md#central-pressure-of-a-constant-density-relativistic-star) gives

$$
\frac{p_c}{\rho}=\frac{1-s}{3s-1}\leq1\quad\Longleftrightarrow\quad1-s\leq3s-1\quad\Longleftrightarrow\quad s\geq\frac12.
$$

Therefore the [dominant-energy compactness bound for an incompressible star](../../../general-relativity.md#dominant-energy-compactness-bound-for-an-incompressible-star) is

$$
\boxed{\frac MR\leq\frac38.}
$$

Equality has $p_c=\rho$ and a finite central [pressure](../../../thermodynamics.md#pressure); it is allowed by the non-strict [dominant energy condition](../../../general-relativity.md#dominant-energy-condition). This is stronger than the regular-star [Buchdahl's theorem](../../../general-relativity.md#buchdahl-s-theorem) limit $M/R<4/9$.

## 2

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) is a smooth family of null geodesics filling a region without intersections there, with one tangent direction assigned smoothly at every point. Choose an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\lambda$ and tangent $U^a$, so $U^aU_a=0$ and $U^b\nabla_bU^a=0$. Choose a second null vector $N^a$ with $U\cdot N=-1$. The [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) is

$$
q_{ab}=g_{ab}+U_aN_b+N_aU_b.
$$

It annihilates $U,N$ and restricts to a positive-definite metric on the two-dimensional transverse screen. Project the [covariant derivative](../../../general-relativity.md#covariant-derivative) of the tangent to obtain the [optical tensor](../../../geodesic-congruence.md#optical-tensor)

$$
\widehat B_{ab}=q_a{}^cq_b{}^d\nabla_dU_c.
$$

Its decomposition defines the three optical quantities:

$$
\boxed{\theta=q^{ab}\widehat B_{ab},\qquad\widehat\omega_{ab}=\widehat B_{[ab]},\qquad\widehat\sigma_{ab}=\widehat B_{(ab)}-\frac12\theta q_{ab}.}
$$

The [null expansion](../../../geodesic-congruence.md#null-expansion) is the fractional rate of change of a transverse area, $\theta=A^{-1}dA/d\lambda$. The [null shear](../../../geodesic-congruence.md#null-shear) changes a beam's shape without changing its area to first order. The [null twist](../../../geodesic-congruence.md#null-twist) is its antisymmetric transverse deformation. The factor $1/2$ uses four spacetime dimensions.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

For an affinely parametrized [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence), put $B^a{}_b=\nabla_bU^a$. Differentiating along a ray and commuting [covariant derivatives](../../../general-relativity.md#covariant-derivative) gives

$$
U^c\nabla_c B^a{}_b=-B^a{}_cB^c{}_b+R^a{}_{dcb}U^dU^c,
$$

using $[\nabla_c,\nabla_b]V^a=R^a{}_{dcb}V^d$. The geodesic acceleration term vanishes. Since $U$ is null and affine, $B^a{}_bU^b=0$ and $U_aB^a{}_b=0$. Its trace is therefore the screen trace $\theta$, and the trace of its square equals that of the [optical tensor](../../../geodesic-congruence.md#optical-tensor) squared. Taking the trace, with $R_{db}=R^a{}_{dab}$, yields

$$
\frac{d\theta}{d\lambda}=-\widehat B_{ab}\widehat B^{ba}-R_{ab}U^aU^b.
$$

Now decompose the [optical tensor](../../../geodesic-congruence.md#optical-tensor) into [null expansion](../../../geodesic-congruence.md#null-expansion), [null shear](../../../geodesic-congruence.md#null-shear) and [null twist](../../../geodesic-congruence.md#null-twist). The symmetric trace-free part is orthogonal to the trace and to the antisymmetric part, while $\widehat\omega_{ab}\widehat\omega^{ba}=-\widehat\omega_{ab}\widehat\omega^{ab}$. Hence

$$
\widehat B_{ab}\widehat B^{ba}=\frac12\theta^2+\widehat\sigma_{ab}\widehat\sigma^{ab}-\widehat\omega_{ab}\widehat\omega^{ab}.
$$

Substitution proves the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation):

$$
\boxed{\frac{d\theta}{d\lambda}=-\frac12\theta^2-\widehat\sigma_{ab}\widehat\sigma^{ab}+\widehat\omega_{ab}\widehat\omega^{ab}-R_{ab}U^aU^b.}
$$

The squares use the positive-definite screen metric. Thus [null shear](../../../geodesic-congruence.md#null-shear) contributes to focusing, whereas nonzero [null twist](../../../geodesic-congruence.md#null-twist) has the opposite sign.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

In the two null coordinates the inverse metric has $g^{UV}=g^{VU}=-f^{-1}$ and $g^{UU}=g^{VV}=0$. Therefore

$$
\boxed{k^a=-(dU)^a=f^{-1}(\partial_V)^a,\qquad\ell^a=-(dV)^a=f^{-1}(\partial_U)^a.}
$$

Both tangents are null and future-directed, since $f>0$ and both coordinate directions are future-directed. To prove the [affine parameter](../../../riemannian-geometry.md#affine-parameter) property, use the [null-gradient affine-geodesic identity](../../../geodesic-congruence.md#null-gradient-affine-geodesic-identity). The one-form $k_a=-\nabla_aU$ is closed, so $\nabla_ak_b=\nabla_bk_a$. Consequently

$$
k^a\nabla_ak_b=k^a\nabla_bk_a=\frac12\nabla_b(k^ak_a)=0.
$$

The same argument applies to $\ell_a=-\nabla_aV$. Thus both vector fields satisfy the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) without a nonaffinity term, and generate affinely parametrized [null geodesic congruences](../../../geodesic-congruence.md#null-geodesic-congruence). The coordinate vectors alone need not be affine; the factors $f^{-1}$ are essential.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For the [spherical null expansions in double-null coordinates](../../../geodesic-congruence.md#spherical-null-expansions-in-double-null-coordinates), the cross-sectional area of a symmetry sphere is $A=4\pi r^2$. For the two affine [null geodesic congruences](../../../geodesic-congruence.md#null-geodesic-congruence), the definition of [null expansion](../../../geodesic-congruence.md#null-expansion) therefore gives

$$
\boxed{\theta_k=\frac{2r_{,V}}{fr},\qquad\theta_\ell=\frac{2r_{,U}}{fr}.}
$$

There is no extra derivative of $f$ in these formulas: the [null expansion](../../../geodesic-congruence.md#null-expansion) differentiates the transverse area, not the normalization of the tangent. Equivalently, the projected metric is $q_{AB}=r^2\gamma_{AB}$ and its [optical tensor](../../../geodesic-congruence.md#optical-tensor) is $(k(r)/r)q_{AB}$, or $(\ell(r)/r)q_{AB}$ for the other congruence. It is purely trace, so both [null shears](../../../geodesic-congruence.md#null-shear) vanish.

The [null twist](../../../geodesic-congruence.md#null-twist) vanishes because the covector tangents are gradients of $-U$ and $-V$, and hence their [exterior derivatives](../../../differential-form.md#exterior-derivative) vanish. Each congruence is orthogonal to a family of null hypersurfaces. This also identifies the [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) reason for zero [null twist](../../../geodesic-congruence.md#null-twist).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Use the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) for $\ell=f^{-1}\partial_U$. Its [null shear](../../../geodesic-congruence.md#null-shear) and [null twist](../../../geodesic-congruence.md#null-twist) vanish, and $R_{ab}\ell^a\ell^b=f^{-2}R_{UU}$. Substitution of $\theta_\ell=2r_{,U}/(fr)$ gives

$$
\frac2{fr}\partial_U(f^{-1}r_{,U})-\frac{2r_{,U}^2}{f^2r^2}=-\frac{2r_{,U}^2}{f^2r^2}-\frac{R_{UU}}{f^2}.
$$

The quadratic terms cancel. Thus the [double-null focusing identity](../../../geodesic-congruence.md#double-null-focusing-identity) is

$$
\boxed{\partial_U(f^{-1}r_{,U})=-\frac r{2f}R_{UU}=-\frac{4\pi r}{f}T_{UU}\leq0.}
$$

Here the last equality uses the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) in units $G=1$; terms proportional to the metric vanish in this null component. The inequality follows from the [null energy condition](../../../general-relativity.md#null-energy-condition).

For any point of the [future domain of dependence](../../../general-relativity.md#future-domain-of-dependence) $D^+(\Sigma)$, the past continuation of its $\ell$ generator must meet the [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) $\Sigma$: every past-inextendible causal curve from that point meets $\Sigma$. Along its future continuation, $U$ increases, and $f^{-1}r_{,U}$ is nonincreasing by the focusing identity. Its initial value is negative, so it stays negative. Since $f>0$, **$r_{,U}<0$ throughout the regular part of $D^+(\Sigma)$**. The argument is used only where the smooth double-null chart has $r>0$; it does not extend a congruence beyond a singular endpoint.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

A spherical [trapped surface](../../../general-relativity.md#trapped-surface) has both future [null expansions](../../../geodesic-congruence.md#null-expansion) negative. Thus the initial sphere has $r_{,U}<0$ and $r_{,V}<0$. The result of the previous part already gives $r_{,U}<0$ at every regular future sphere in $D^+(\Sigma)$.

Apply the same [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) to $k=f^{-1}\partial_V$. The exchanged-coordinate [double-null focusing identity](../../../geodesic-congruence.md#double-null-focusing-identity) is

$$
\partial_V(f^{-1}r_{,V})=-\frac r{2f}R_{VV}=-\frac{4\pi r}{f}T_{VV}\leq0.
$$

Along $U=U_0$, increasing $V$ is future-directed. Therefore

$$
f^{-1}r_{,V}(U_0,V_1)\leq f^{-1}r_{,V}(U_0,V_0)<0.
$$

Both [null expansions](../../../geodesic-congruence.md#null-expansion) remain negative, proving **[persistence of spherical trapping](../../../geodesic-congruence.md#persistence-of-spherical-trapping) along this future null direction**. As usual, the conclusion concerns every $V_1>V_0$ for which the sphere exists in the regular chart in $D^+(\Sigma)$; the inequality does not assert existence of such spheres beyond a focusing singularity.

## 3

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For the [Komar integral of a five-dimensional Reissner--Nordstrom metric](../../../general-relativity.md#komar-integral-of-a-five-dimensional-reissner-nordstrom-metric), use the one-form metrically dual to the stationary [Killing vector field](../../../general-relativity.md#killing-vector-field): $k^\flat=-f(r)dt$. Its [exterior derivative](../../../differential-form.md#exterior-derivative) is $dk^\flat=f'(r)dt\wedge dr$. The stated orientation gives volume form

$$
\epsilon=-r^3\sin^2\chi\sin\theta\,dt\wedge dr\wedge d\chi\wedge d\theta\wedge d\phi.
$$

Because the squared norm of $dt\wedge dr$ is $g^{tt}g^{rr}=-1$, the defining wedge identity for the [Hodge star operator](../../../differential-form.md#hodge-star-operator) gives

$$
\star(dt\wedge dr)=r^3\sin^2\chi\sin\theta\,d\chi\wedge d\theta\wedge d\phi.
$$

Thus the [Komar integral](../../../general-relativity.md#komar-charge) over the positively oriented angular three-sphere is

$$
\int_{S^3}\star dk^\flat=2\pi^2r^3f'(r),
$$

since the unit three-sphere has volume $2\pi^2$. Write $s=r_+^2+r_-^2$, $q=r_+^2r_-^2$. Then $f=1-s/r^2+q/r^4$ and $r^3f'=2s-4q/r^2$. With the normalization specified for the [Komar mass](../../../general-relativity.md#komar-mass),

$$
\boxed{M=\frac\pi4(r_+^2+r_-^2).}
$$

The orientation makes this positive. The problem's coefficient $1/(16\pi)$ must be retained: it is not the usual dimension-adjusted five-dimensional ADM-normalized Komar coefficient. With that conventional normalization the ADM [mass](../../../classical-mechanics.md#mass) would instead be $3\pi s/8$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For radial [null geodesics](../../../special-relativity.md#null-geodesic), the metric gives $dt/dr=\pm f^{-1}$ in the exterior. Define the [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate) by

$$
\boxed{r_\star(r)=\int^r\frac{dx}{f(x)}.}
$$

An outgoing future radial ray has $dt/dr=f^{-1}$, so $u=t-r_\star$ is constant; an ingoing ray has $dt/dr=-f^{-1}$, so $v=t+r_\star$ is constant. These describe the null trajectories independently of the choice of [affine parameter](../../../riemannian-geometry.md#affine-parameter).

For the [tortoise coordinate of a five-dimensional charged black hole](../../../general-relativity.md#tortoise-coordinate-of-a-five-dimensional-charged-black-hole), with $a=r_+$, $b=r_-$ and $\Delta=a^2-b^2$, partial fractions give

$$
\frac1{f(r)}=1+\frac{a^4}{\Delta(r^2-a^2)}-\frac{b^4}{\Delta(r^2-b^2)}.
$$

Thus a useful explicit [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate) is

$$
\boxed{r_\star=r+\frac{a^3}{2\Delta}\log\left|\frac{r-a}{r+a}\right|-\frac{b^3}{2\Delta}\log\left|\frac{r-b}{r+b}\right|+C.}
$$

The logarithms signal failure of the static coordinates at the horizons, rather than a curvature singularity there.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Since $v=t+r_\star$, $dt=dv-f^{-1}dr$. Substitution into the radial metric cancels the $dr^2/f$ terms. The [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates) give

$$
\boxed{ds^2=-f(r)dv^2+2\,dv\,dr+r^2d\Omega_3^2.}
$$

The radial block has [determinant](../../../linear-algebra.md#determinant) $-1$, even when $f=0$. Its coefficients are analytic for every $r>0$, so this form extends through $r=r_+$ and also through $r=r_-$ to $0<r<r_+$. Ordinary angular coordinate singularities are removed by angular charts on the three-sphere. The genuine endpoint $r=0$ is not included in this extension.

The field $n=-\partial_r$ is an ingoing null tangent. It is future-directed in the original exterior, since its inner product with the future stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) is $-1$, and it remains future-directed by continuation. This fixes the time orientation used in the next part.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For an [asymptotically flat spacetime](../../../general-relativity.md#asymptotically-flat-spacetime) with a chosen exterior component of [future null infinity](../../../general-relativity.md#future-null-infinity), the [black-hole region](../../../general-relativity.md#black-hole) is

$$
\boxed{\mathcal B=\mathcal M\setminus J^-(\mathscr I^+),}
$$

namely the events from which no future-directed [causal curve](../../../general-relativity.md#causal-curve) can reach that infinity. Here $\mathscr I^+$ is the infinity of the original $r>r_+$ exterior.

Let a future causal tangent in the [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates) have components $(\dot v,\dot r,\dot\Omega)$. Its inner product with the future null field $n=-\partial_r$ is $-\dot v$, so $\dot v\geq0$. The causal inequality is

$$
-f\dot v^2+2\dot v\dot r+r^2|\dot\Omega|^2\leq0.
$$

If $\dot v>0$, this implies

$$
\dot r\leq\frac f2\dot v-\frac{r^2|\dot\Omega|^2}{2\dot v}.
$$

In the band $r_-<r<r_+$, $f<0$, so $\dot r<0$. If $\dot v=0$, the causal inequality forces $\dot\Omega=0$, and future direction means the remaining radial tangent is a nonnegative multiple of $n$, again giving $\dot r\leq0$. This is [causal trapping between two spherical horizons](../../../general-relativity.md#causal-trapping-between-two-spherical-horizons): **$r$ is nonincreasing along every future causal curve in the between-horizon band**. No event there can escape outward. An event with $0<r\leq r_-$ would also have to cross this band outward to reach the original exterior, which is impossible. Thus all $0<r<r_+$ events in this extension lie in the [black-hole region](../../../general-relativity.md#black-hole).

Conversely, from any $r>r_+$ point, the outgoing radial null ray $u=\mathrm{constant}$ satisfies $dr/dv=f/2>0$. It reaches arbitrarily large $r$ and then the original [future null infinity](../../../general-relativity.md#future-null-infinity). Therefore **the exterior does not intersect the [black-hole region](../../../general-relativity.md#black-hole)**, and $r=r_+$ is its [event horizon](../../../general-relativity.md#event-horizon). This conclusion is relative to the selected asymptotic end; the maximal charged-black-hole extension can have other asymptotic ends.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

In the [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates), the stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) is $k=\partial_v$ with norm $k^2=-f$. The normal vector to a level set of $r$ is

$$
\nabla^ar=(\partial_v)^a+f(\partial_r)^a.
$$

At $r=r_+$ it equals $k^a$, which is null there. Thus this null hypersurface is a [Killing horizon](../../../general-relativity.md#killing-horizon) of $k$. Its [surface gravity](../../../general-relativity.md#surface-gravity) is fixed by $\nabla_a(k^2)=-2\kappa k_a$ on the horizon. Since $k_a=(dr)_a$ there and $\nabla_a(k^2)=-f'(r_+)(dr)_a$,

$$
\boxed{\kappa=\frac12f'(r_+)=\frac{r_+^2-r_-^2}{r_+^3}.}
$$

The positive sign follows from the future outer-horizon generator, normalized by the static time at infinity. It vanishes as the two radii approach the extremal limit.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

The inner horizon in the nonextreme [Reissner-Nordstrom spacetime](../../../general-relativity.md#reissner-nordstrom-spacetime) diagram is a [Cauchy horizon](../../../general-relativity.md#cauchy-horizon). Radiation from exterior perturbations can approach it at arbitrarily late advanced time and undergo unbounded blueshift. Here its positive blueshift scale is $\kappa_-=(r_+^2-r_-^2)/r_-^3$. The [inner-horizon blueshift coordinate](../../../general-relativity.md#inner-horizon-blueshift-coordinate) behaves as $V_-\propto-e^{-\kappa_-v}$, so

$$
T_{V_-V_-}=\left(\frac{dv}{dV_-}\right)^2T_{vv}\propto e^{2\kappa_-v}T_{vv}.
$$

Even a decaying power-law tail can therefore generate divergent local flux. With counterstreaming radiation, backreaction produces [mass inflation](../../../general-relativity.md#mass-inflation) and curvature growth, rather than the smooth inner horizon of the exact solution.

This supports the [strong cosmic censorship conjecture](../../../general-relativity.md#strong-cosmic-censorship-conjecture): a generically perturbed [maximal Cauchy development](../../../general-relativity.md#maximal-cauchy-development) is expected to lose the smooth extension across its [Cauchy horizon](../../../general-relativity.md#cauchy-horizon), restoring predictability in the appropriate regularity class. **The exact smooth inner horizon is unstable, not a robust failure of deterministic evolution.** Curvature divergence supports an obstruction to a $C^2$ metric extension; it does not by itself exclude every continuous metric extension. The regularity class is part of the conjecture, and the blueshift argument is evidence, not a general theorem proving it.

## 4

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Physical-process first law for a rotating black hole](../../../general-relativity.md#physical-process-first-law-for-a-rotating-black-hole), in four-dimensional [general relativity](../../../general-relativity.md) with $G=1$, is

$$
\boxed{\frac{\kappa}{8\pi}\delta A=\delta E-\Omega_H\delta J.}
$$

It applies to a small neutral matter influx into an initially stationary, nonextremal [black hole](../../../general-relativity.md#black-hole) that settles to another stationary state. The background [surface gravity](../../../general-relativity.md#surface-gravity) and angular velocity are $\kappa$ and $\Omega_H$, and $\delta E,\delta J$ are the [Killing energy](../../../general-relativity.md#killing-energy) and [angular momentum](../../../classical-mechanics.md#angular-momentum) delivered through the [event horizon](../../../general-relativity.md#event-horizon). Other conserved charges are held fixed. The perturbation must be small enough that its horizon generators do not develop caustics, and all equalities below are to first order.

Let $t^a$ be the stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) normalized at infinity, and $\psi^a$ the axial [Killing vector field](../../../general-relativity.md#killing-vector-field) with $2\pi$-periodic orbits. The horizon generator is $\xi^a=t^a+\Omega_H\psi^a$. Choose an affine tangent $k^a$ and parameter $\lambda$ with zero at the past stationary limiting section, so [affine horizon-generator scaling](../../../general-relativity.md#affine-horizon-generator-scaling) gives, on the background horizon

$$
\xi^a=\kappa\lambda k^a.
$$

The background [null expansion](../../../geodesic-congruence.md#null-expansion) and [null shear](../../../geodesic-congruence.md#null-shear) vanish, and [null twist](../../../geodesic-congruence.md#null-twist) vanishes for the hypersurface-orthogonal horizon generators. Linearizing the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) and using the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) gives

$$
\frac{d\,\delta\theta}{d\lambda}=-8\pi\delta T_{ab}k^ak^b.
$$

The quadratic [null expansion](../../../geodesic-congruence.md#null-expansion) and [null shear](../../../geodesic-congruence.md#null-shear) terms are second order. With background cross-sectional measure $dA_0$, the first-order area change is $\delta A=\int_{\mathcal H}\delta\theta\,d\lambda\,dA_0$. Multiplying the evolution equation by $\lambda$ and integrating by parts gives the [first-order horizon-area response to matter flux](../../../general-relativity.md#first-order-horizon-area-response-to-matter-flux)

$$
\delta A=8\pi\int_{\mathcal H}\lambda\,\delta T_{ab}k^ak^b\,d\lambda\,dA_0.
$$

The boundary term $[\lambda\delta\theta]$ vanishes: $\lambda=0$ at the past limiting section, and the final stationary boundary condition gives zero expansion in the settled future. Equivalently, assume a sufficiently localized influx with the required late-time decay.

The energy and angular-momentum fluxes have signs

$$
\delta E=\int_{\mathcal H}\delta T_{ab}t^ak^b\,d\lambda\,dA_0,\qquad\delta J=-\int_{\mathcal H}\delta T_{ab}\psi^ak^b\,d\lambda\,dA_0.
$$

These correspond to the particle conventions $E=-p\cdot t$ and $J=p\cdot\psi$. Their combination is

$$
\delta E-\Omega_H\delta J=\int_{\mathcal H}\delta T_{ab}\xi^ak^b\,d\lambda\,dA_0=\kappa\int_{\mathcal H}\lambda\delta T_{ab}k^ak^b\,d\lambda\,dA_0=\frac\kappa{8\pi}\delta A.
$$

This proves the requested [Physical-process first law of black-hole mechanics](../../../general-relativity.md#physical-process-first-law-of-black-hole-mechanics). For charged infall the corresponding law contains an additional horizon-potential term $\Phi_H\delta Q$; the energy-minus-angular-momentum version assumes that work term is absent.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Quantize the real massless [scalar field](../../../quantum-field-theory.md#scalar-field) using the normalized in-modes:

$$
\widehat\phi=\sum_j\left(a_jf_j+a_j^\dagger\bar f_j\right),\qquad[a_j,a_k^\dagger]=\delta_{jk},\qquad a_j|0_{\rm in}\rangle=0.
$$

Use the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) convention that is antilinear in its first argument. Mode normalization gives

$$
(f_j,f_k)=\delta_{jk},\qquad(\bar f_j,\bar f_k)=-\delta_{jk},\qquad(f_j,\bar f_k)=0.
$$

The out annihilation operator is $b_i=(p_i,\widehat\phi)$. Applying the [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation) and the negative norm of conjugate modes gives

$$
\boxed{b_i=\sum_j\left(\bar A_{ij}a_j-\bar B_{ij}a_j^\dagger\right).}
$$

Both the complex conjugation and the minus sign follow from the inner-product convention. These operators annihilate the [out-vacuum](../../../quantum-field-theory.md#out-vacuum), but need not annihilate the [in-vacuum](../../../quantum-field-theory.md#in-vacuum). The [particle number operator](../../../quantum-mechanics.md#number-operator) in out-mode $i$ is $N_i^{\rm out}=b_i^\dagger b_i$. In the [in-vacuum](../../../quantum-field-theory.md#in-vacuum), the only nonzero contraction is $\langle0_{\rm in}|a_ja_k^\dagger|0_{\rm in}\rangle=\delta_{jk}$, obtained from the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation). Thus

$$
\boxed{\langle0_{\rm in}|N_i^{\rm out}|0_{\rm in}\rangle=\sum_{j,k}B_{ij}\bar B_{ik}\delta_{jk}=\sum_j|B_{ij}|^2=(BB^\dagger)_{ii}.}
$$

This is [particle number from Bogoliubov coefficients](../../../quantum-field-theory.md#particle-number-from-bogoliubov-coefficients): mixing with negative-frequency in-modes produces out-particles even though no in-particles were present. For continuous mode labels the sum becomes an integral; normalized wave packets make an individual occupation number well-defined. No explicit collapse geometry or thermal spectrum is needed for this conclusion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
