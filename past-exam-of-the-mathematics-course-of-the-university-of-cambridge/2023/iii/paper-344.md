# Paper 344

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_344.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_344.pdf)

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
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
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

## 1

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Because $\phi$ is a conserved composition density, an infinitesimal material displacement $\mathbf r\mapsto\mathbf r+\mathbf u$ changes it at fixed position by

$$
\delta\phi=-\nabla\mathbin\cdot(\phi\mathbf u)
=-\mathbf u\mathbin\cdot\nabla\phi-\phi\nabla\mathbin\cdot\mathbf u.
$$

The second term is essential when the deformation is compressible. By the definition of the [chemical potential](../../../thermodynamics.md#chemical-potential), and taking $\mathbf u$ to vanish on the boundary,

$$
\delta F=\int\mu\,\delta\phi\,d\mathbf r
=-\int\mu\nabla\mathbin\cdot(\phi\mathbf u)d\mathbf r
=\int\phi\nabla_j\mu\,u_jd\mathbf r.
$$

The same free-energy change written in terms of the [stress tensor](../../../continuum-mechanics.md#stress) is

$$
\delta F=\int\Sigma_{ij}\nabla_i u_jd\mathbf r
=-\int(\nabla_i\Sigma_{ij})u_jd\mathbf r.
$$

Since $\mathbf u$ is arbitrary,

$$
\boxed{\nabla_i\Sigma_{ij}=-\phi\nabla_j\mu.}
$$

This is the [Korteweg force](../../../critical-phenomenon.md#korteweg-force) density of a diffuse-interface mixture.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Functional differentiation gives

$$
\mu=f'(\phi)-\kappa\nabla^2\phi.
$$

For $\Pi=\mu\phi-\mathbb F$ and $\Sigma_{ij}=-\Pi\delta_{ij}-\kappa(\nabla_i\phi)(\nabla_j\phi)$,

$$
\begin{aligned}
\nabla_i\Sigma_{ij}
={}&-\nabla_j(\mu\phi-\mathbb F)
-\kappa\nabla_i[(\nabla_i\phi)(\nabla_j\phi)]\\
={}&-\phi\nabla_j\mu
+[f'(\phi)-\mu-\kappa\nabla^2\phi]\nabla_j\phi.
\end{aligned}
$$

The bracket vanishes by the expression for $\mu$, while the two mixed second-derivative terms cancel. Therefore

$$
\boxed{\nabla_i\Sigma_{ij}=-\phi\nabla_j\mu.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Equilibrium minimizes $F$ at fixed total composition $\int\phi$, so a [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) gives $\delta F/\delta\phi=\mu_0$, independent of position. In the two homogeneous phases,

$$
f'(\pm\phi_B)=a(\pm\phi_B)+b(\pm\phi_B)^3=0,
\qquad \phi_B=\sqrt{-a/b}.
$$

The symmetric coexistence pair therefore has $\mu_0=0$. For a planar profile depending only on the normal coordinate $x$,

$$
0=\mu=a\phi+b\phi^3-\kappa\phi'',
$$

or

$$
\boxed{\kappa\phi''=a\phi+b\phi^3,
\qquad \phi(\pm\infty)=\pm\phi_B}
$$

up to reversal of the two phases.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put $\phi=\phi_Bg(u)$, $u=(x-x_0)/\xi_0$, and $\xi_0^2=-2\kappa/a$. Since $b\phi_B^2=-a$, the interface equation reduces to

$$
g''=2g(g^2-1).
$$

Multiplication by $g'$ and use of $g(\pm\infty)=\pm1$, $g'(\pm\infty)=0$ gives the first integral

$$
(g')^2=(1-g^2)^2.
$$

For the increasing profile, $g'=1-g^2$, so $\operatorname{artanh}g=u$ after shifting $x_0$. Hence the [phi-four diffuse interface](../../../critical-phenomenon.md#phi-four-diffuse-interface) is

$$
\boxed{\phi(x)=\pm\phi_B\tanh\left(\frac{x-x_0}{\xi_0}\right).}
$$

The sign chooses the orientation and the translation zero mode $x_0$ sets the interface position.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Far from a planar interface, the equilibrium profile equals a bulk minimum and contributes the uniform density $f(\phi_B)$. The localized transition layer contributes an additional free energy proportional to its area $A$, because translation invariance makes the excess per unit area independent of position. By the definition of [surface tension](../../../fluid-mechanics.md#surface-tension) as interfacial excess free energy per area,

$$
\boxed{\sigma A=F[\phi_E]-Vf(\phi_B).}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

For a profile depending only on $x$, equation (2) gives $\Sigma_{yy}=-\Pi$ and $\Sigma_{xx}=-\Pi-\kappa(\phi')^2$. Thus

$$
\Sigma_{yy}-\Sigma_{xx}=\kappa(\phi')^2.
$$

For $\phi_E=\phi_B\tanh[(x-x_0)/\xi_0]$,

$$
\phi_E'=\frac{\phi_B}{\xi_0}\operatorname{sech}^2\left(\frac{x-x_0}{\xi_0}\right).
$$

Changing variable to $u=(x-x_0)/\xi_0$ yields

$$
\sigma=\frac{\kappa\phi_B^2}{\xi_0}
\int_{-\infty}^{\infty}\operatorname{sech}^4u\,du
=\frac{4\kappa\phi_B^2}{3\xi_0}.
$$

Using $\phi_B^2=-a/b$ and $\xi_0^2=-2\kappa/a$ gives the positive [interfacial tension of a phi-four diffuse interface](../../../critical-phenomenon.md#interfacial-tension-of-a-phi-four-diffuse-interface)

$$
\boxed{\sigma=\sqrt{\frac{-8a^3\kappa}{9b^2}}.}
$$

## 2

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [polar liquid crystal](../../../critical-phenomenon.md#polar-liquid-crystal) distinguishes the two ends of each constituent. Its orientational order is described by a vector $\mathbf p$, and $\mathbf p$ and $-\mathbf p$ represent different states. A [nematic liquid crystal](../../../critical-phenomenon.md#nematic-liquid-crystal) has head-tail symmetry, so its director obeys $\mathbf n\sim-\mathbf n$. Its lowest-rank faithful [nematic order parameter](../../../critical-phenomenon.md#nematic-order-parameter) is the symmetric traceless tensor

$$
Q_{ij}=S\left(n_in_j-\frac13\delta_{ij}\right),
$$

which is unchanged by $\mathbf n\mapsto-\mathbf n$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Fourier transform](../../../analysis.md#fourier-transform) sends each spatial derivative to $iq_i$, so at Gaussian level

$$
\boxed{G(q)=a+\kappa q^2+\gamma q^4.}
$$

For $\kappa<0<\gamma$, minimizing over $s=q^2\geq0$ gives

$$
s_0=-\frac\kappa{2\gamma},
\qquad
\boxed{q_0=\sqrt{-\frac\kappa{2\gamma}}.}
$$

The minimum kernel is $G(q_0)=a-\kappa^2/(4\gamma)$. Gaussian fluctuations first diverge when this vanishes, so the [nonzero-wavevector soft-mode sphere](../../../critical-phenomenon.md#nonzero-wavevector-soft-mode-sphere) becomes unstable at

$$
\boxed{a_c=\frac{\kappa^2}{4\gamma}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For candidate (i), $\mathbf p=p_0\widehat{\mathbf p}\cos q_0x$. Since $G(q_0)=\widehat a:=a-a_c$, $\langle\cos^2q_0x\rangle=1/2$, and $\langle\cos^4q_0x\rangle=3/8$, its mean-field free-energy density is

$$
\boxed{\frac FV=\frac{\widehat a}{4}p_0^2+\frac{3b}{32}p_0^4.}
$$

For $\widehat a<0$, stationarity gives

$$
p_0^2=-\frac{4\widehat a}{3b},
$$

and substitution yields

$$
\boxed{\frac{F_{(i)}}V=-\frac{\widehat a^2}{6b}.}
$$

For $\widehat a\geq0$, the minimum is $p_0=0$. The amplitude therefore vanishes continuously as $p_0\propto(a_c-a)^{1/2}$ on approaching $a_c$ from below, which is a continuous [mean-field transition](../../../critical-phenomenon.md#mean-field-approximation).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For candidate (ii), $|\mathbf p|=p_0$ everywhere and each component has wavevector magnitude $q_0$. The quadratic density is therefore $\widehat a p_0^2/2$, while the quartic density is $bp_0^4/4$ without trigonometric averaging:

$$
\frac{F_{(ii)}}V=\frac{\widehat a}{2}p_0^2+\frac b4p_0^4.
$$

For $\widehat a<0$,

$$
p_0^2=-\frac{\widehat a}{b},
\qquad
\boxed{\frac{F_{(ii)}}V=-\frac{\widehat a^2}{4b}.}
$$

Since $(-1/4)/(-1/6)=3/2$, the helical structure's free energy is $50\%$ more negative than that of candidate (i).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Every term in the free energy contracts the vector components with the [Euclidean inner product](../../../linear-algebra.md#inner-product): it depends only on $|\mathbf p|^2$, $|\mathbf p|^4$, $(\nabla_i p_j)(\nabla_i p_j)$, and $|\nabla^2\mathbf p|^2$. A constant $\mathcal R\in SO(3)$ preserves all these contractions and commutes with spatial differentiation. Therefore

$$
F[\mathcal R\mathbf p]=F[\mathbf p],
$$

so every constant rotation of candidate (ii) has the same free energy. The orientation of the rotation plane of the [polar helical smectic](../../../critical-phenomenon.md#polar-helical-smectic) is thus continuously degenerate.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Let $\mathbf e_1,\mathbf e_2$ span the rotating plane and let $\mathbf n=\mathbf e_1\times\mathbf e_2$ be its normal. For modulation along $\widehat{\mathbf x}$,

$$
\mathbf p=p_0(\mathbf e_1\cos q_0x+\mathbf e_2\sin q_0x),
$$

and period averaging gives

$$
\left\langle|\nabla\mathbin\cdot\mathbf p|^2\right\rangle
=\frac{q_0^2p_0^2}{2}
[(\mathbf e_1\mathbin\cdot\widehat{\mathbf x})^2
+(\mathbf e_2\mathbin\cdot\widehat{\mathbf x})^2]
=\frac{q_0^2p_0^2}{2}[1-(\mathbf n\mathbin\cdot\widehat{\mathbf x})^2].
$$

For $\lambda>0$, this is minimized by $\mathbf n\parallel\widehat{\mathbf x}$, so the rotation plane is perpendicular to the modulation direction and the helix is transverse. For $\lambda<0$, it is minimized energetically by maximizing the bracket: $\mathbf n\perp\widehat{\mathbf x}$, so the modulation direction lies in the rotation plane. Thus either sign lifts the full rotational degeneracy, leaving only the rotations consistent with its selected relative orientation. A sufficiently small negative $\lambda$ does not overcome the stabilizing higher-gradient terms.

## 3

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) gives a pressure excess $2\sigma/R$ inside a spherical droplet. Near coexistence, the common chemical-potential shift is $\mu\simeq\alpha\delta$, where $\alpha=f''(\phi_B)$, while changing phase changes the composition by approximately $2\phi_B$. Balancing the capillary pressure against this thermodynamic shift gives the [Gibbs--Thomson relation](../../../fluid-mechanics.md#gibbs-thomson-relation)

$$
2\phi_B\alpha\delta\simeq\frac{2\sigma}{R}.
$$

Hence the compositions immediately outside and inside are

$$
\phi(R^+)=-\phi_B+\delta(R),
\qquad
\phi(R^-)=+\phi_B+\delta(R),
$$

with

$$
\boxed{\delta(R)=\frac{\sigma}{\alpha\phi_BR}\propto\frac\sigma R.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

In the exterior write $\phi=-\phi_B+\widetilde\phi$. Linearization at the bulk minimum gives

$$
\mu=\frac{\delta F}{\delta\phi}
\simeq\alpha\widetilde\phi-\kappa\nabla^2\widetilde\phi.
$$

For a large droplet, variations occur on scale $R$ much larger than the interfacial [correlation length](../../../critical-phenomenon.md#correlation-length), so the second term is smaller by $O(\kappa/(\alpha R^2))$ and $\mu\simeq\alpha\widetilde\phi$. The [conserved order-parameter dynamics](../../../critical-phenomenon.md#conserved-order-parameter-dynamics) then becomes

$$
\partial_t\widetilde\phi\simeq\alpha M\nabla^2\widetilde\phi.
$$

Diffusion relaxes the exterior profile much faster than the droplet radius changes. In this quasistatic limit $\partial_t\widetilde\phi\simeq0$, and therefore

$$
\boxed{\nabla^2\widetilde\phi=0\qquad(r>R).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The spherically symmetric [Laplace equation](../../../partial-differential-equation.md#laplace-equation) with $\widetilde\phi(R)=\delta(R)$ and $\widetilde\phi(\infty)=\varepsilon$ has solution

$$
\widetilde\phi(r)=\varepsilon+[\delta(R)-\varepsilon]\frac Rr.
$$

Thus

$$
J_r(R^+)=-M\partial_r\mu|_{R^+}
=-\frac{\alpha M}{R}[\varepsilon-\delta(R)].
$$

Conservation at the moving interface, whose composition jump is $2\phi_B$, gives $2\phi_B\dot R=-J_r(R^+)$ and hence

$$
\boxed{\dot R=\frac{\alpha M}{2\phi_BR}[\varepsilon-\delta(R)].}
$$

Since $\delta(R)=C/R$, the right side is proportional to $\varepsilon/R-C/R^2$. It is negative for $R<R^*$, zero at $R^*=C/\varepsilon$, positive for $R>R^*$, and approaches zero from above for large $R$. Thus $R^*$ is the unstable [critical nucleus](../../../thermodynamics.md#critical-nucleus): smaller droplets dissolve, while larger droplets grow.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Using $\delta(R)=\sigma/(\alpha\phi_BR)$, the growth law is

$$
\dot R=\frac{\alpha M\varepsilon}{2\phi_BR}
-\frac{M\sigma}{2\phi_B^2R^2}.
$$

For

$$
F(R)=4\pi\sigma R^2-\frac{4\pi}{3}\Delta R^3,
\qquad
\Delta=2\phi_B\alpha\varepsilon,
$$

one has $F'=8\pi\sigma R-4\pi\Delta R^2$. Therefore, with $\mathcal M(R)=M/(16\pi\phi_B^2R^3)$,

$$
\boxed{\dot R=-\mathcal M(R)\frac{dF}{dR}.}
$$

The first term in $F$ is the positive surface cost and the second is the negative bulk free-energy gain of converting a metastable volume. The nonzero stationary radius and barrier are the [classical nucleation theory](../../../thermodynamics.md#classical-nucleation-theory) values

$$
\boxed{R^*=\frac{2\sigma}{\Delta}
=\frac{\sigma}{\phi_B\alpha\varepsilon},
\qquad
F^*=F(R^*)=\frac{16\pi\sigma^3}{3\Delta^2}.}
$$

Since $F''(R^*)=-8\pi\sigma<0$, this stationary point is a maximum.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Thermal molecular motion causes the coarse droplet radius to fluctuate as well as drift down $F(R)$, so its effective equation must be an [overdamped Langevin dynamics](../../../stochastic-calculus.md#overdamped-langevin-dynamics). With $\langle\Lambda(t)\Lambda(t')\rangle=\delta(t-t')$, detailed balance with equilibrium density proportional to $e^{-F/(k_BT)}$ imposes the [Fluctuation-dissipation theorem](../../../quantum-field-theory.md#fluctuation-dissipation-theorem). The [Model A fluctuation-dissipation relation](../../../critical-phenomenon.md#model-a-fluctuation-dissipation-relation) gives

$$
\boxed{A=\sqrt{2k_BT\,\overline{\mathcal M}}.}
$$

The factor of mobility ensures that the diffusion in $R$ and the dissipative drift have the same equilibrium Gibbs distribution.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

A subcritical droplet must make a rare thermal fluctuation from the metastable basin over the free-energy barrier $F^*$. Its probability carries the [Boltzmann factor](../../../statistical-physics.md#boltzmann-factor) $e^{-F^*/(k_BT)}$, so the nucleation rate has the [Arrhenius form](../../../thermodynamics.md#arrhenius-nucleation-time)

$$
\Gamma\sim\Gamma_0e^{-F^*/(k_BT)}.
$$

For a volume containing order one candidate subcritical droplet, the waiting time for a supercritical droplet and subsequent macroscopic growth is therefore

$$
\boxed{\tau\sim\tau_0e^{F^*/(k_BT)},}
$$

up to an algebraic kinetic prefactor. This is the [Arrhenius nucleation time](../../../thermodynamics.md#arrhenius-nucleation-time).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
