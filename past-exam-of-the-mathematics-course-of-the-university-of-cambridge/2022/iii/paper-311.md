# Paper 311

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_311.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_311.pdf)

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
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [i](#2/e/i)
      - [Solution](#2/e/i/solution)
    - [ii](#2/e/ii)
      - [Solution](#2/e/ii/solution)
    - [iii](#2/e/iii)
      - [Solution](#2/e/iii/solution)
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
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Outside the star, $p=\rho=0$. The first [Tolman–Oppenheimer–Volkoff equation](../../../general-relativity.md#tolman-oppenheimer-volkoff-equation) gives $m(r)=M$, and the second gives

$$
\Phi'(r)=\frac{M}{r(r-2M)}
=\frac12\frac d{dr}\log\left(1-\frac{2M}{r}\right).
$$

Asymptotic flatness fixes the integration constant, so $e^{2\Phi}=1-2M/r$. The exterior line element is therefore the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) with mass $M=m(R)$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Regularity at the center requires $m(0)=0$ and a finite central density $\rho_c$. The [equation of state](../../../thermodynamics.md#equation-of-state) fixes $p_c=p(\rho_c)$, and the regular central series begins

$$
m(r)=\frac{4\pi}{3}\rho_c r^3+O(r^5),
\qquad
p(r)=p_c+O(r^2).
$$

For each admissible $\rho_c$, ordinary-differential-equation uniqueness determines $m,p,\rho$ outward until the first zero of $p$, which defines $R$. The remaining additive constant in $\Phi$ is fixed by matching to the exterior Schwarzschild time coordinate. Thus smooth stars form a one-parameter family labelled uniquely by $\rho_c$.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Let $r_0$ be where the outward-decreasing density first reaches $\rho_0$ and set $p_0=p(\rho_0)$. The quoted compactness inequality at $r_0$ bounds $m_0/r_0$ using only $p_0r_0^2$. Its right side must be positive. Writing $x=6\pi p_0r_0^2$, positivity of $1-x+\sqrt{1+x}$ implies $x<3$, hence

$$
r_0^2<\frac1{2\pi p_0},
\qquad
m_0<\frac49r_0.
$$

Both the radius and mass of the unknown high-density core are therefore bounded using only the known pressure $p_0$. From $(r_0,m_0,p_0)$ outward, the known low-density equation of state uniquely determines the envelope and adds only a bounded mass before $p$ reaches zero. Maximizing over the resulting bounded set of admissible initial data gives a finite maximum stellar mass independent of the equation of state above $\rho_0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For constant density,

$$
m(r)=\frac{4\pi\rho_0r^3}{3}=M\frac{r^3}{R^3},
\qquad M=\frac{4\pi\rho_0R^3}{3}.
$$

Substitution in the pressure equation makes it separable. Integrating from $r$ to the surface, where $p(R)=0$, gives the [Interior Schwarzschild solution](../../../general-relativity.md#interior-schwarzschild-metric)

$$
\boxed{
p(r)=\rho_0
\frac{\sqrt{1-2Mr^2/R^3}-\sqrt{1-2M/R}}
{3\sqrt{1-2M/R}-\sqrt{1-2Mr^2/R^3}}}.
$$

Direct differentiation verifies the TOV equation and the surface boundary condition.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Set $C=M/R$ and $s=\sqrt{1-2C}$. At the center,

$$
\frac{p_c}{\rho_0}=\frac{1-s}{3s-1}.
$$

The barotropic bound $p_c\leq\omega\rho_0$ implies

$$
1-s\leq\omega(3s-1),
\qquad
s\geq\frac{1+\omega}{1+3\omega}.
$$

Therefore

$$
\boxed{\frac MR\leq
\frac12\left[1-\left(\frac{1+\omega}{1+3\omega}\right)^2\right]
=\frac{2\omega(1+2\omega)}{(1+3\omega)^2}}.
$$

As $\omega\to\infty$, this approaches $4/9$, the limiting value in [Buchdahl's theorem](../../../general-relativity.md#buchdahl-s-theorem). Constant-density stars with increasingly large allowed central pressure can therefore approach the Buchdahl bound arbitrarily closely.

## 2

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Every metric coefficient and the gauge potential are independent of $t$. Therefore

$$
\mathcal L_{\partial_t}g=0,
$$

so $K=\partial_t$ is a [Killing vector field](../../../general-relativity.md#killing-vector-field).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Define the ingoing coordinate

$$
v=t+r_*,
\qquad
\frac{dr_*}{dr}=\frac1{f(r)}.
$$

Then $dt=dv-dr/f$ and

$$
\boxed{ds^2=-f(r)dv^2+2\,dv\,dr+r^2d\Omega_{d-2}^2}.
$$

This is the higher-dimensional analogue of [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates). Its metric and inverse are regular at $r=r_+$, including when the zero is degenerate. A gauge transformation removes the singular radial term in the transformed potential, leaving the regular representative $A=-Q r^{-(d-3)}dv$. These expressions analytically extend the spacetime through the future outer horizon.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The normal to $r=r_+$ is $dr$, whose squared norm is $g^{rr}=f(r_+)=0$, so the surface is a [null hypersurface](../../../general-relativity.md#null-hypersurface). In ingoing coordinates $K=\partial_v$, and on the horizon

$$
K_a=g_{av}=(0,1,0,\ldots)=\nabla_ar.
$$

Thus $K$ is both tangent and normal there, making the surface a [Killing horizon](../../../general-relativity.md#killing-horizon). For a static metric of this form, the [surface gravity](../../../general-relativity.md#surface-gravity) is $\kappa=f'(r_+)/2$. With $n=d-3$,

$$
\boxed{\kappa=\frac{d-3}{2r_+}
\left[1-\left(\frac{r_-}{r_+}\right)^{d-3}\right]}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Curvature invariants and the electromagnetic invariant diverge at $r=0$, so it is a genuine [curvature singularity](../../../general-relativity.md#curvature-singularity), not a coordinate singularity. The causal structures are the higher-dimensional analogues of the familiar four-dimensional diagrams:

- for $r_-=0$, there is one nondegenerate horizon and a spacelike singularity, giving the Schwarzschild Penrose diagram;
- for $0<r_-<r_+$, the outer event horizon and inner [Cauchy horizon](../../../general-relativity.md#cauchy-horizon) enclose a region ending at a timelike singularity, with the maximally extended Reissner-Nordström chain of blocks;
- for $r_-=r_+$, the horizon is degenerate with $\kappa=0$, the singularity remains timelike, and the extremal throat has infinite spatial length.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/i">i</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/i/solution">Solution</h5>

↑ **Parent:** [I](#2/e/i)

Differentiate $E=-mK_aU^a+q\Phi$ along the worldline. The symmetric contraction $U^aU^b\nabla_aK_b$ vanishes by the [Killing equation](../../../general-relativity.md#killing-equation). Using the [Lorentz force](../../../electromagnetism.md#lorentz-force) and $K^aF_{ab}=\nabla_b\Phi$, the remaining force term cancels $qU^a\nabla_a\Phi$. Hence

$$
\boxed{U^a\nabla_aE=0}.
$$

<h4 id="2/e/ii">ii</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/e/ii)

For the displayed gauge field,

$$
i_KF=d\Phi,
\qquad
\Phi=\frac{Q}{r^{d-3}},
$$

which already vanishes at infinity. A static future-directed particle has $U=K/\sqrt f$, so

$$
E(r)=m\sqrt{f(r)}+\frac{qQ}{r^{d-3}}.
$$

If $qQ<0$, the first term tends to zero at $r_+$ while the second remains negative. Lowering the particle sufficiently close to the horizon therefore produces $E<0$. Dropping it into the hole reduces the black-hole mass by $|E|$, while the external agent receives the corresponding positive work: this is charged-particle [black-hole energy extraction](../../../general-relativity.md#black-hole-energy-extraction).

<h4 id="2/e/iii">iii</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/e/iii)

In the reversible limit the particle is released arbitrarily close to the horizon, so

$$
dM=\Phi_H\,dQ=\frac{Q}{r_+^{d-3}}\,dQ.
$$

Holding $r_+$ fixed and using $Q^2=r_+^{d-3}r_-^{d-3}$,

$$
M=\frac12\left(r_+^{d-3}+\frac{Q^2}{r_+^{d-3}}\right).
$$

Discharging to $Q=0$ therefore extracts at most

$$
\boxed{E_{\rm ext}^{\rm max}
=M-\frac12r_+^{d-3}
=\frac{Q^2}{2r_+^{d-3}}
=\frac12r_-^{d-3}}.
$$

[Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem) forbids the horizon area, and hence $r_+$, from decreasing. The smallest possible final neutral mass is consequently $r_+^{d-3}/2$, giving exactly the same upper bound.

## 3

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Because $t_a=\nabla_at$ is a gradient, $\nabla_at_b=\nabla_bt_a$. Therefore

$$
t^b\nabla_bt_a=t^b\nabla_at_b
=\frac12\nabla_a(t^bt_b)=0.
$$

**Thus $t^a$ is an affinely parametrized [timelike geodesic vector field](../../../geodesic-congruence.md#timelike-geodesic-vector-field), and because $t$ is constant on $S$, it emanates orthogonally from $S$.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

With $c=-\nabla_at^a$, commute covariant derivatives and use the geodesic equation:

$$
\begin{aligned}
t^b\nabla_bc
&=-t^b\nabla_b\nabla_at^a\\
&=R_{ab}t^at^b+(\nabla_at_b)(\nabla^at^b).
\end{aligned}
$$

This is the hypersurface-orthogonal [Raychaudhuri equation](../../../cosmology.md#friedmann-acceleration-equation) written in terms of positive convergence rather than expansion.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [strong energy condition](../../../general-relativity.md#strong-energy-condition) and Einstein's equation imply $R_{ab}t^at^b\geq0$. Since the congruence is hypersurface orthogonal, its vorticity vanishes. The tensor in the hint is the trace-free spatial shear, so

$$
S_{ab}S^{ab}
=(\nabla_at_b)(\nabla^at^b)-\frac13(\nabla_at^a)^2\geq0.
$$

Because $\nabla_at^a=-c$, part b gives

$$
\boxed{t^a\nabla_ac\geq\frac13c^2}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $\tau$ be proper time along a geodesic. While $c$ is finite and positive,

$$
\frac d{d\tau}\left(\frac1c\right)
=-\frac1{c^2}\frac{dc}{d\tau}\leq-\frac13.
$$

Thus

$$
\frac1{c(\tau)}\leq\frac1{c_0}-\frac\tau3.
$$

The right side reaches zero at $\tau=3/c_0$, so the convergence must diverge no later than that proper time.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Suppose instead that every future-directed normal timelike geodesic were complete. Choose a point more than $3/c_0$ proper time to the future of $S$. Global hyperbolicity supplies a longest timelike curve from $S$ to that point; it is a geodesic orthogonal to $S$ and has no focal point before its endpoint. But part d makes the convergence of every such normal congruence diverge within proper time $3/c_0$. Nearby geodesics then intersect, producing a [focal point](../../../geodesic-congruence.md#focal-point-of-a-hypersurface) after which the geodesic cannot maximize proper time. This contradiction proves that at least one timelike geodesic has finite maximal proper time, so $(M,g)$ has [timelike geodesic incompleteness](../../../geodesic-congruence.md#timelike-geodesic-incompleteness).

## 4

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The four [laws of black-hole mechanics](../../../general-relativity.md#laws-of-black-hole-mechanics) closely parallel thermodynamics. The zeroth law says that the [surface gravity](../../../general-relativity.md#surface-gravity) $\kappa$ is constant over a stationary Killing horizon. The first law is

$$
\delta M=\frac{\kappa}{8\pi G}\delta A
+\Omega_H\delta J+\Phi_H\delta Q.
$$

The second law is [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem), $\delta A\geq0$ under the [null energy condition](../../../general-relativity.md#null-energy-condition), and the [third law of black-hole mechanics](../../../general-relativity.md#third-law-of-black-hole-mechanics) says that a regular extremal horizon with $\kappa=0$ cannot be reached by a finite physical process. These match constancy of temperature in equilibrium, $dE=T\,dS+$ work terms, entropy increase, and unattainability of zero temperature.

Quantum field theory makes the analogy literal. A stationary horizon emits at the [Hawking temperature](../../../general-relativity.md#hawking-temperature)

$$
T_H=\frac{\hbar\kappa}{2\pi k_Bc}.
$$

Comparing $T_HdS$ with the area term in the first law gives the [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy)

$$
\boxed{S_{\rm BH}=\frac{k_Bc^3A}{4G\hbar}}.
$$

For a Schwarzschild black hole, $\kappa=c^4/(4GM)$ and $T_H=\hbar c^3/(8\pi GMk_B)$.

To see why particles are produced, quantize a real scalar field using the conserved [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product). In the asymptotically Minkowski past choose positive-frequency modes $u_i^{\rm in}$ and write

$$
\widehat\Phi=\sum_i(a_i^{\rm in}u_i^{\rm in}
+a_i^{{\rm in}\dagger}u_i^{{\rm in}*}).
$$

The asymptotically Minkowski future supplies another positive-frequency basis $u_j^{\rm out}$ and operators $a_j^{\rm out}$. In a nonstationary middle region there is no preferred timelike Killing vector and therefore no invariant positive-frequency split: the notion of particle is observer- and basis-dependent. The two mode bases are related by a [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation),

$$
u_j^{\rm out}=\sum_i(\alpha_{ji}u_i^{\rm in}
+\beta_{ji}u_i^{{\rm in}*}),
$$

so the corresponding operators mix annihilation and creation operators. The in-vacuum then contains

$$
\langle0_{\rm in}|N_j^{\rm out}|0_{\rm in}\rangle
=\sum_i|\beta_{ji}|^2
$$

out-particles whenever $\beta\ne0$.

For a black hole formed by collapse, late outgoing modes traced backwards toward the event horizon undergo an exponentially large blueshift. This produces a universal Bogoliubov mixing with

$$
\langle N_\omega\rangle
=\frac1{e^{2\pi\omega/\kappa}-1},
$$

the Planck distribution at $T_H$. Greybody scattering outside the horizon modifies the flux reaching infinity but not its characteristic temperature.

Hawking radiation gives a black hole negative heat capacity: it heats up as it loses mass and can evaporate in finite time. The [generalized second law](../../../general-relativity.md#generalized-second-law) assigns entropy $S_{\rm BH}$ to the hole and states that this plus exterior entropy does not decrease. The enormous area entropy suggests microscopic horizon degrees of freedom. If semiclassical evaporation ends with only thermal radiation, an initially pure state appears to become mixed, producing the [black hole information paradox](../../../general-relativity.md#black-hole-information-paradox). Resolving the endpoint, information recovery, and the microscopic origin of the area law are central constraints on quantum gravity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
