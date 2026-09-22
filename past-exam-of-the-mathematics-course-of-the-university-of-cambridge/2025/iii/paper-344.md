# Paper 344

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_344.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_344.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
  - [e](#1/e)
    - [i](#1/e/i)
      - [Solution](#1/e/i/solution)
    - [ii](#1/e/ii)
      - [Solution](#1/e/ii/solution)
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
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)

## 1

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [binary fluid mixture](../../../critical-phenomenon.md#binary-fluid-mixture), the [compositional order parameter](../../../critical-phenomenon.md#compositional-order-parameter) $\phi(\mathbf r)$ may be taken as the local concentration difference between the two species. In a closed system

$$
\int_V\phi(\mathbf r),d\mathbf r
$$

is fixed by the total amount of each species. This is the sense in which $\phi$ is conserved; locally it changes through a current and obeys a continuity equation.

For a symmetric mixture, the [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) free energy is

$$
F[\phi]=\int_V\left[\frac a2\phi^2+\frac b4\phi^4+\frac{\kappa_1}{2}|\nabla\phi|^2\right]d\mathbf r,
\qquad b,\kappa_1>0.
$$

A term $h\int_V\phi,d\mathbf r$ is constant on the allowed configurations and therefore changes neither equilibrium probabilities nor the dynamics. Equivalently, it merely shifts the [chemical potential](../../../thermodynamics.md#chemical-potential) by a spatial constant, whose gradient vanishes.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The coupling $\frac c2\int\phi p^2$ is linear in $\phi$, but its coefficient $p^2(\mathbf r)$ is generally position dependent and dynamical. It therefore cannot be reduced to a constant times the conserved integral of $\phi$; it changes both the local chemical potential of the mixture and the tendency of the [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) to order.

Interchanging the labels of the two species sends $\phi\mapsto-\phi$ while leaving the even terms in $\phi$ unchanged. It sends $c\mapsto-c$, so one may choose $c>0$ without loss of generality.

The isotropic disordered system is invariant under spatial inversion, which sends the [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) $p\mapsto-p$ while leaving the scalar composition $\phi$ unchanged. A term $\phi p$ is odd under this symmetry and is forbidden; in more than one dimension it also fails to be a rotational scalar. Finally, if no higher even powers are retained, $b<0$ or $B<0$ makes the free energy unbounded below as the corresponding field grows. Thermodynamic stability therefore requires $b,B>0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At fixed uniform $\phi$, the nonconserved variable $p$ can relax freely, so [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) minimizes

$$
f(\phi,p)=\frac a2\phi^2+\frac b4\phi^4+\frac{A+c\phi}{2}p^2+\frac B4p^4
$$

with respect to $p$. The stationary solutions obey

$$
p\left(A+c\phi+Bp^2\right)=0.
$$

Thus $p=0$ when $A+c\phi\geq0$, while $p^2=-(A+c\phi)/B$ when $A+c\phi<0$. Substitution gives

$$
f(\phi)=\frac a2\phi^2+\frac b4\phi^4-\frac{(A+c\phi)^2}{4B}\,	heta(-A-c\phi).
$$

Writing this in the requested form yields

$$
\boxed{\phi_o=-\frac Ac},
\qquad
\boxed{C=\frac{c^2}{2B}},
$$

because $A+c\phi=c(\phi-\phi_o)$. The value $\phi_o$ is the composition at which the coefficient of $p^2$ changes sign, so it is the mean-field threshold for polar ordering.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

With $\phi_o=0$,

$$
f(\phi)=
\begin{cases}
\frac12(a-C)\phi^2+\frac b4\phi^4,&\phi<0,\\
\frac a2\phi^2+\frac b4\phi^4,&\phi>0.
\end{cases}
$$

For $C<a$, both branches are locally convex at the origin. At

$$
\boxed{C_c=a}
$$

the negative-side curvature vanishes; for $C>a$ the interval near $0^-$ has $f''=a-C+3b\phi^2<0$, so a homogeneous composition there is unstable and the equilibrium free energy is its convex envelope. The sketch therefore has an ordinary upward quartic on the positive side and, beyond $C_c$, a negative-curvature shoulder and a minimum on the negative side.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

The two [binodal](../../../critical-phenomenon.md#binodal) compositions $\phi_1<0<\phi_2$ are the contact points of the [common-tangent construction](../../../critical-phenomenon.md#common-tangent-construction). Equivalently, they solve

$$
f'(\phi_1)=f'(\phi_2)=\mu,
\qquad
f(\phi_1)-\mu\phi_1=f(\phi_2)-\mu\phi_2.
$$

The first equality is equality of [chemical potential](../../../thermodynamics.md#chemical-potential); the second is equality of [pressure](../../../thermodynamics.md#pressure). Here

$$
(a-C)\phi_1+b\phi_1^3=a\phi_2+b\phi_2^3
$$

together with the intercept equation determines the two densities. As $C\downarrow a$, both contact points approach zero continuously with scale $|\phi_{1,2}|\propto\sqrt{C-a}$, so this mean-field onset of phase separation is continuous.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/i">i</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/i/solution">Solution</h5>

↑ **Parent:** [I](#1/e/i)

When $b=\kappa_1=0$, stationarity in $\phi$ gives

$$
\frac{\delta F}{\delta\phi}=a\phi+\frac c2p^2=0,
\qquad
\phi=-\frac{c}{2a}p^2.
$$

Substituting this value, or completing the square in the Gaussian integral over $\phi$, gives

$$
F[p]=\int\left[\frac A2p^2+\frac{\widetilde B}{4}p^4+\frac\kappa2|\nabla p|^2\right]d\mathbf r,
\qquad
\boxed{\widetilde B=B-\frac{c^2}{2a}}.
$$

When $A>0$ and the quartic term is negligible, each Fourier mode is Gaussian with the [Ornstein--Zernike correlation function](../../../critical-phenomenon.md#ornstein-zernike-correlation-function)

$$
\boxed{S_p(q)=\frac{k_BT}{A+\kappa q^2}}
$$

up to the chosen Fourier normalization. Its correlation length is $\xi_p=\sqrt{\kappa/A}$.

<h4 id="1/e/ii">ii</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/e/ii)

The eliminated field obeys $\phi=-cp^2/(2a)$, so its connected [correlation function](../../../critical-phenomenon.md#correlation-function) is

$$
C_\phi(r)=\frac{c^2}{4a^2}\left[\langle p^2(0)p^2(r)\rangle-\langle p^2\rangle^2\right].
$$

For the zero-mean Gaussian field of part (i), [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) gives

$$
\boxed{C_\phi(r)=\frac{c^2}{2a^2}C_p(r)^2}.
$$

It is therefore nonnegative and has the square of the Ornstein--Zernike spatial form. In particular, if $C_p(r)$ has exponential factor $e^{-r/\xi_p}$, then $C_\phi(r)$ has $e^{-2r/\xi_p}$ and correlation length $\xi_p/2$, with the algebraic prefactor also squared.

## 2

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Take

$$
F[\phi]=\int\left[\frac a2\phi^2+\frac b4\phi^4+\frac\kappa2|\nabla\phi|^2\right]d\mathbf r.
$$

Its variational chemical potential is

$$
\mu=\frac{\delta F}{\delta\phi}=a\phi+b\phi^3-\kappa\nabla^2\phi.
$$

Conservation gives $\dot\phi=-\nabla\mathbin{\cdot}\mathbf J$. Assuming an isotropic constant mobility $M>0$, local linear irreversible thermodynamics gives $\mathbf J=-M\nabla\mu$. Hence the noiseless [conserved order-parameter dynamics](../../../critical-phenomenon.md#conserved-order-parameter-dynamics) is

$$
\boxed{\dot\phi=-\nabla\mathbin{\cdot}\mathbf J},
\qquad
\boxed{\mathbf J=-M\nabla(a\phi+b\phi^3-\kappa\nabla^2\phi)}.
$$

It decreases the free energy because $\dot F=-\int M|\nabla\mu|^2d\mathbf r\leq0$ under closed or no-flux boundary conditions.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $a<0$ and $b>0$, planar coexistence occurs at $\phi=\pm\phi_B$ with $\phi_B=\sqrt{-a/b}$. Put $\alpha=f''(\phi_B)=a+3b\phi_B^2=-2a>0$. A common small shift $\delta$ gives equal chemical potentials to first order,

$$
\mu(\pm\phi_B+\delta)=\alpha\delta+O(\delta^2).
$$

The thermodynamic pressure is $P=\phi\mu-f$. Its difference between the positive interior and negative exterior is therefore

$$
P_+-P_-=2\phi_B\alpha\delta+O(\delta^2).
$$

For a sphere the [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) gives $P_+-P_-=2\sigma/R$. Consequently the [Gibbs--Thomson relation](../../../fluid-mechanics.md#gibbs-thomson-relation) is

$$
\boxed{\delta=\frac{\sigma}{\alpha\phi_BR}=\frac\lambda R},
\qquad
\boxed{\lambda=\frac{\sigma}{\alpha\phi_B}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The curved interface requires exterior composition $-\phi_B+\delta$, but the far field supplies only $-\phi_B$. Material therefore diffuses away from the droplet, which evaporates. Write $\phi=-\phi_B+g$ outside. Linearization gives $\mu=\alpha g$, and the quasistatic condition $\dot\phi=M\nabla^2\mu\simeq0$ gives

$$
\nabla^2g=0,
\qquad
g(R)=\delta,
\qquad
g(\infty)=0.
$$

Spherical symmetry yields $g(r)=\delta R/r$. Taking the normal outward from the droplet,

$$
J_n=-M\partial_r\mu=-M\alpha\partial_rg,
\qquad
J_n(R)=\frac{M\alpha\delta}{R}>0.
$$

The interface converts positive-phase material into negative-phase material. Integrating the continuity equation through the moving interface gives the Stefan condition

$$
v_n[\phi]=-J_n,
$$

where $[\phi]=2\phi_B$, and hence

$$
\boxed{v_n=-\frac{J_n}{2\phi_B}<0}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For $h=\eta\sin(qx)$, the linearized mean curvature is

$$
K=(\partial_x^2+\partial_y^2)h=-q^2\eta\sin(qx).
$$

The boundary value in the upper phase is therefore

$$
g(x,0)=\frac{\sigma q^2\eta}{2\alpha\phi_B}\sin(qx).
$$

The decaying harmonic extension into $z>0$ is

$$
g(x,z)=\frac{\sigma q^2\eta}{2\alpha\phi_B}e^{-|q|z}\sin(qx).
$$

With the normal directed into the upper half-space,

$$
\boxed{J_n(x,0^+)=-M\alpha\partial_zg(x,0^+)=\frac{M\sigma|q|^3}{2\phi_B}\eta\sin(qx)}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Using only this upper-phase flux in $\dot h=v_n=-J_n/(2\phi_B)$ gives

$$
\dot\eta=-\nu|q|^3\eta,
\qquad
\boxed{\nu=\frac{M\sigma}{4\phi_B^2}>0}.
$$

Positive [surface tension](../../../fluid-mechanics.md#surface-tension) raises the chemical potential at a crest, drives material away from it, and therefore smooths the interface, which fixes the negative sign of the decay rate.

The dynamics is nonlocal because the conserved composition must diffuse through the bulk. Solving Laplace's equation maps a boundary Fourier amplitude to its normal derivative by multiplication by $|q|$. Combining this Dirichlet-to-Neumann factor with the curvature factor $q^2$ produces the nonanalytic $|q|^3$ rate described by [diffusion-limited relaxation of an interface](../../../fluid-mechanics.md#diffusion-limited-relaxation-of-an-interface).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Both coexisting phases transport the conserved order parameter. The calculation above included only the harmonic field and normal current in the upper half-space. The lower half-space contributes an equal flux into the interface for equal mobilities and symmetric phases. The total interface speed is therefore twice the one-sided result, so the correct coefficient is

$$
\boxed{\nu_{\rm full}=\frac{M\sigma}{2\phi_B^2}}.
$$

## 3

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The antisymmetric velocity-gradient tensor $\boldsymbol\Omega$ is the local angular velocity of a rigid-body rotation. Under such a rotation a material vector must rotate at exactly the same angular velocity, independently of its molecular constitution. The coefficient of $\boldsymbol\Omega\mathbin{\cdot}\mathbf p$ is therefore fixed to one by rotational covariance, also called material objectivity. In contrast, the symmetric strain-rate tensor $\mathbf D$ deforms rather than merely rotates the material, so its flow-alignment coefficient $\xi$ is material dependent.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

During a small incompressible displacement $u_i=v_i\Delta t$, pure advection changes the polar field by

$$
\delta p_i=-u_k\nabla_kp_i-\Omega_{ij}[u]p_j+\xi D_{ij}[u]p_j.
$$

The free-energy change is $\delta F=\int h_i\delta p_i,d\mathbf r$, where $h_i=\delta F/\delta p_i$. Integrating the translational term by parts and separating the antisymmetric and symmetric parts of $\nabla_i u_j$ identifies the [order-parameter stress](../../../critical-phenomenon.md#order-parameter-stress). Up to an arbitrary isotropic pressure, its three contributions obey

$$
\boxed{\nabla_i\Sigma_{ij}^{(1)}=-p_i\nabla_jh_i},
$$



$$
\boxed{\Sigma_{ij}^{(2)}=\frac12(p_ih_j-p_jh_i)},
\qquad
\boxed{\Sigma_{ij}^{(3)}=\frac\xi2(p_ih_j+p_jh_i)}.
$$

The first term is the distortion or Ericksen force density, the second transfers antisymmetric rotational torque, and the third is the symmetric [flow alignment of a polar order parameter](../../../critical-phenomenon.md#flow-alignment-of-a-polar-order-parameter) contribution.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

For a uniform field, $\mathbf v\mathbin{\cdot}\nabla\mathbf p=0$, and the stated flow has $\boldsymbol\Omega=0$ and

$$
\mathbf D\mathbin{\cdot}\mathbf p=\gamma(p_x,-p_y/2,-p_z/2).
$$

The equation $D\mathbf p/Dt=-\Gamma\mathbf h$ becomes

$$
\partial_t\mathbf p=-\Gamma\left[\mathbf h-\frac{\xi\gamma}{\Gamma}(p_x,-p_y/2,-p_z/2)\right].
$$

Thus

$$
\boxed{\widetilde{\mathbf h}=\mathbf h+\alpha(p_x,-p_y/2,-p_z/2)},
\qquad
\boxed{\alpha=-\frac{\xi\gamma}{\Gamma}}.
$$

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The shifted molecular field is the gradient of

$$
\boxed{\mathbb F_{\rm mod}=\frac12(a+\alpha)p_x^2+\frac12\left(a-\frac\alpha2\right)(p_y^2+p_z^2)+\frac b4(p_x^2+p_y^2+p_z^2)^2}.
$$

Thus $A=\operatorname{diag}(a+\alpha,a-\alpha/2,a-\alpha/2)$.

If $\alpha<0$, the $x$ mode softens first at

$$
\boxed{a_c=-\alpha},
\qquad
\boxed{\mathbf p=(\pm\sqrt{(-a-\alpha)/b},0,0)}quad(a<a_c).
$$

The extensional flow already selects the $x$ axis, and ordering chooses one of its two polar directions. The transition is continuous and spontaneously breaks the remaining inversion symmetry $p_x\mapsto-p_x$.

If $\alpha>0$, the degenerate transverse modes soften first at

$$
\boxed{a_c=\frac\alpha2},
\qquad
\boxed{p_x=0,quad p_y^2+p_z^2=\frac{\alpha/2-a}{b}}quad(a<a_c).
$$

This transition is also continuous. The flow preserves rotations about the $x$ axis, while the ordered vector chooses an azimuthal direction in the $yz$ plane and spontaneously breaks that $SO(2)$ symmetry.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

For $\alpha<0$, choose one ordered state $\mathbf p=(p,0,0)$ with $p^2=(-a-\alpha)/b$. Stationarity gives $\widetilde{\mathbf h}=0$, hence

$$
\mathbf h=-\alpha(p,0,0).
$$

Uniformity makes $\nabla_i\Sigma_{ij}^{(1)}=0$, so its spatially constant part can be absorbed into the pressure. Since $\mathbf h$ is parallel to $\mathbf p$, the antisymmetric term $\Sigma^{(2)}$ vanishes. The symmetric term is

$$
\boxed{\Sigma_{ij}^p=-\xi\alpha p^2\,\delta_{ix}\delta_{jx}}
$$

up to isotropic pressure. Using $\alpha=-\xi\gamma/\Gamma$, its only deviatoric component is $\Sigma_{xx}^p=(\xi^2\gamma/\Gamma)p^2$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
