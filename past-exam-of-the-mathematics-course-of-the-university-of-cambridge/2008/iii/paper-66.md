# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper66.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

| [Spacetime](../../../special-relativity.md#spacetime) | [Extendible](../../../special-relativity.md#extendible-spacetime) | [Geodesically complete](../../../riemannian-geometry.md#geodesic-completeness) | [Globally hyperbolic](../../../general-relativity.md#globally-hyperbolic-spacetime) | [Asymptotically simple](../../../general-relativity.md#asymptotic-simplicity) |
| --- | --- | --- | --- | --- |
| [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime), exterior $r>2M$ | Yes | No | Yes | No |
| [Kruskal spacetime](../../../general-relativity.md#kruskal-spacetime) | No | No | Yes | No |
| Maximal analytic extension of extremal [Reissner-Nordstrom spacetime](../../../general-relativity.md#reissner-nordstrom-spacetime) | No | No | No | No |
| [Rindler spacetime](../../../special-relativity.md#rindler-wedge) | Yes | No | Yes | No |
| [Einstein static universe](../../../general-relativity.md#einstein-static-universe) | No | Yes | Yes | No |

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Use [geometrized units](../../../general-relativity.md#geometrized-units) $G=c=1$. For a stationary [asymptotically flat spacetime](../../../general-relativity.md#asymptotically-flat-spacetime), normalize the timelike [Killing vector field](../../../general-relativity.md#killing-vector-field) $\xi$ to have squared norm $-1$ at infinity. The [Komar mass](../../../general-relativity.md#komar-mass) is

$$
M_K=-\frac1{8\pi}\lim_{S\to\infty}\int_S\nabla^a\xi^b\,dS_{ab}.
$$

Here the oriented binormal is chosen so that an ordinary positive-mass static solution gives a positive integral. Equivalently, on a static slice with lapse $N=\sqrt{-\xi^2}$ and outward spatial unit normal $s^i$,

$$
M_K=\frac1{4\pi}\lim_{S\to\infty}\int_Ss^iD_iN\,dA.
$$

This second expression fixes the orientation unambiguously and is convenient for the [Majumdar–Papapetrou solution](../../../general-relativity.md#majumdar-papapetrou-solution).

The spatial metric is $\gamma_{ij}=H^2\delta_{ij}$ and $N=H^{-1}$. On a large coordinate sphere, $s^i=H^{-1}\widehat r^i$ and $dA=H^2r^2d\Omega$. Thus

$$
s^iD_iN\,dA=-\frac{r^2}{H}\partial_rH\,d\Omega,\qquad M_K=-\frac1{4\pi}\lim_{r\to\infty}\int_{S^2}\frac{r^2\partial_rH}{H}\,d\Omega.
$$

The original PDF has the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) in each source denominator, which is missing in the TeX aid. With that norm, the [harmonic function](../../../partial-differential-equation.md#harmonic-function) has asymptotics

$$
H=1+\frac{\sum_iM_i}{r}+O(r^{-2}),\qquad\partial_rH=-\frac{\sum_iM_i}{r^2}+O(r^{-3}).
$$

Therefore

$$
\boxed{M_K=\sum_{i=1}^NM_i.}
$$

If $M_i$ are retained as length parameters while $G$ is restored, the physical mass is $\sum_iM_i/G$. This is the charge at infinity. A [Komar integral](../../../general-relativity.md#komar-charge) is not generally surface-independent here, since [Einstein-Maxwell theory](../../../general-relativity.md#einstein-maxwell-theory) has the electromagnetic [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) between the surfaces; in particular it should not be confused with a sum of vacuum horizon [Komar charges](../../../general-relativity.md#komar-charge).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Take the first centre at the origin. If some listed centres coincide, first combine their poles; let $M$ be the total residue at the origin, so $M=M_1$ when the centres are distinct. The contributions from centres away from the origin are real analytic there. Their constant term is

$$
\boxed{h=1+\sum_{\mathbf x_j\ne0}\frac{M_j}{|\mathbf x_j|},\qquad H=\frac Mr+h+rF(r,\theta,\phi),}
$$

where $F$ is analytic in $r$ and in local angular charts. This follows by substituting $\mathbf x=r\mathbf n(\theta,\phi)$ in the ordinary [Taylor expansions](../../../calculus.md#taylor-expansion) of the regular contributions. The constant $h$ is independent of angle, which makes the hinted coordinate differential integrable.

Put $A=M+hr$, $Q=rH=A+r^2F$, and define

$$
v=t+h^2r+2hM\log r-\frac{M^2}{r},\qquad dv=dt+\left(h+\frac Mr\right)^2dr
$$

initially for $r>0$. Substitution into the metric gives

$$
ds^2=-\frac{r^2}{Q^2}dv^2+2\frac{A^2}{Q^2}dv\,dr+\frac{Q^4-A^4}{r^2Q^2}dr^2+Q^2d\Omega_2^2.
$$

The apparently singular radial coefficient is actually

$$
\frac{Q^4-A^4}{r^2Q^2}=F\frac{(Q+A)(Q^2+A^2)}{Q^2},
$$

since $Q-A=r^2F$. All coefficients therefore extend analytically to negative and positive $r$ near zero, with $Q(0)=M>0$. At the horizon $g_{vv}=0$, $g_{vr}=1$, $g_{rr}=4MF(0,\theta,\phi)$ and the angular metric is $M^2d\Omega_2^2$. The $v,r$ determinant is $-1$ both before and at the extension, so the metric remains nondegenerate and Lorentzian. Angular coordinate singularities are handled by ordinary sphere charts. This explicitly constructs the [analytic extension of a Majumdar–Papapetrou horizon](../../../general-relativity.md#analytic-extension-of-a-majumdar-papapetrou-horizon).

Inverting the radial block gives $g^{rr}=r^2/Q^2$, which vanishes at $r=0$. Thus the hypersurface is null. Its normal agrees there with the metric dual of $\xi=\partial_v$: $\xi_a\,dx^a=dr$ on the horizon. The metric is independent of $v$, so $\xi$ is a [Killing vector field](../../../general-relativity.md#killing-vector-field) and the null hypersurface is a [Killing horizon](../../../general-relativity.md#killing-horizon).

The [surface gravity](../../../general-relativity.md#surface-gravity) obeys $\nabla_a(\xi^2)=-2\kappa\xi_a$ on a [Killing horizon](../../../general-relativity.md#killing-horizon). Here $\xi^2=-r^2/Q^2$ has a double zero and its entire differential vanishes at $r=0$, while $\xi_a$ is the nonzero normal. Consequently

$$
\boxed{\kappa=0.}
$$

The horizon is degenerate. Its cross-sectional area is $4\pi M^2$, independent of the centres away from the origin. The essential cancellation would fail with an arbitrary constant in place of the displayed regular part $h$.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $x^a(\lambda,s)$ be a smooth family of affinely parametrized [null geodesics](../../../special-relativity.md#null-geodesic). The tangent is $U=\partial x/\partial\lambda$, and the [deviation vector](../../../riemannian-geometry.md#deviation-vector) is $Z=\partial x/\partial s$, comparing nearby rays at the same [affine parameter](../../../riemannian-geometry.md#affine-parameter). The two parameter derivatives commute, so

$$
\boxed{[U,Z]=0,\qquad\nabla_UZ=\nabla_ZU.}
$$

Thus the separation vector is Lie-transported along the [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence); it is not required to be parallel-transported. Differentiating once more gives the [geodesic deviation](../../../general-relativity.md#geodesic-deviation) equation. With curvature convention $[\nabla_c,\nabla_d]V^a=R^a{}_{bcd}V^b$,

$$
\nabla_U\nabla_UZ^a=R^a{}_{bcd}U^bU^cZ^d.
$$

For optical measurements one uses transverse deviations with $U\cdot Z=0$ and identifies longitudinal additions proportional to $U$. The scalar $U\cdot Z$ is constant along affine null rays by the displayed transport relation, so an initially transverse deviation remains transverse.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose an auxiliary [null vector](../../../special-relativity.md#null-vector) $N$ with $U\cdot N=-1$, parallel-transported along each affine ray. The [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) and its induced positive metric are

$$
\boxed{P^a{}_b=\delta^a_b+U^aN_b+N^aU_b,\qquad P_{ab}=g_{ab}+U_aN_b+N_aU_b.}
$$

They annihilate $U,N$, obey $P^2=P$, and have trace two in four [spacetime](../../../special-relativity.md#spacetime) dimensions. Since both $U$ and $N$ are parallel along $U$, $\nabla_UP=0$. Equivalently, the screen represents the two-dimensional quotient $U^\perp/\operatorname{span}(U)$.

Define the [optical matrix of a null congruence](../../../geodesic-congruence.md#optical-matrix-of-a-null-congruence) by

$$
\widehat B_{ab}=P_a{}^cP_b{}^d\nabla_dU_c.
$$

For a transverse deviation, its screen projection $\zeta=PZ$ satisfies $\nabla_U\zeta^a=\widehat B^a{}_b\zeta^b$. Decompose the [matrix](../../../vector-space.md#matrix) as

$$
\boxed{\widehat B_{ab}=\frac12\theta P_{ab}+\widehat\sigma_{ab}+\widehat\omega_{ab},\quad\theta=P^{ab}\widehat B_{ab},\quad\widehat\sigma_{ab}=\widehat B_{(ab)}-\frac12\theta P_{ab},\quad\widehat\omega_{ab}=\widehat B_{[ab]}.}
$$

These are the [null expansion](../../../geodesic-congruence.md#null-expansion), [null shear](../../../geodesic-congruence.md#null-shear) and [null twist](../../../geodesic-congruence.md#null-twist). [Null expansion](../../../geodesic-congruence.md#null-expansion) gives the fractional change of a small transverse area, $\theta=d\log(dA)/d\lambda$. [Null shear](../../../geodesic-congruence.md#null-shear) is symmetric trace-free distortion; [null twist](../../../geodesic-congruence.md#null-twist) is the antisymmetric rotation part. This [null expansion](../../../geodesic-congruence.md#null-expansion) convention uses the full trace, not half the trace. The auxiliary screen fixes representatives, while the transverse optical content is intrinsic to the [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence).

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

First let $B_{ab}=\nabla_bU_a$ without projection. Commute derivatives on this [covector](../../../linear-algebra.md#covector) and use affine [geodesic](../../../riemannian-geometry.md#geodesic) motion:

$$
U^c\nabla_cB_{ab}=\nabla_b(U^c\nabla_cU_a)-(\nabla_bU^c)(\nabla_cU_a)-U^cU^dR_{dacb}=-B_{ac}B^c{}_b-R_{cadb}U^cU^d.
$$

The last equality relabels the two contracted null-vector indices. Nullness and affine parametrization give $U^aB_{ab}=0$ and $B_{ab}U^b=0$. Therefore inserting $P$ into the contracted middle index changes no screen-projected quadratic term. Since $\nabla_UP=0$, screen projection proves the [Sachs optical equations](../../../geodesic-congruence.md#sachs-optical-equations)

$$
\boxed{U\cdot\nabla\widehat B_{ab}=-\widehat B_{ac}\widehat B^c{}_b-\mathcal R_{ab},\qquad\mathcal R_{ab}=P_a{}^eP_b{}^fR_{cedf}U^cU^d.}
$$

The optical tidal [matrix](../../../vector-space.md#matrix) $\mathcal R_{ab}$ is symmetric by the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor)'s pair symmetries. Raising one screen index gives the corresponding equation for $\widehat B^a{}_b$.

In terms of the defined optical scalars, the equation is explicitly

$$
\begin{aligned}
U\cdot\nabla\widehat B_{ab}={}&-\frac{\theta^2}{4}P_{ab}-\theta(\widehat\sigma_{ab}+\widehat\omega_{ab})\\
&-\widehat\sigma_{ac}\widehat\sigma^c{}_b-\widehat\omega_{ac}\widehat\omega^c{}_b\\
&-\widehat\sigma_{ac}\widehat\omega^c{}_b-\widehat\omega_{ac}\widehat\sigma^c{}_b-\mathcal R_{ab}.
\end{aligned}
$$

This [matrix](../../../vector-space.md#matrix) identity contains the [null expansion](../../../geodesic-congruence.md#null-expansion), [null shear](../../../geodesic-congruence.md#null-shear) and [null twist](../../../geodesic-congruence.md#null-twist) evolution equations as its trace, symmetric trace-free part and antisymmetric part.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Take the screen trace of the [optical matrix of a null congruence](../../../geodesic-congruence.md#optical-matrix-of-a-null-congruence) equation. The cross-contractions of symmetric [null shear](../../../geodesic-congruence.md#null-shear) with antisymmetric [null twist](../../../geodesic-congruence.md#null-twist) vanish, and

$$
\operatorname{tr}(\widehat B^2)=\frac12\theta^2+\widehat\sigma_{ab}\widehat\sigma^{ab}-\widehat\omega_{ab}\widehat\omega^{ab}.
$$

The minus sign in the [null twist](../../../geodesic-congruence.md#null-twist) contribution follows from tracing the square of an [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix). The tidal trace is $P^{ef}R_{cedf}U^cU^d=R_{cd}U^cU^d$: the additional null terms in $P^{ef}$ vanish by curvature antisymmetry. Thus the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) is

$$
\boxed{U\cdot\nabla\theta=-\frac12\theta^2-\widehat\sigma_{ab}\widehat\sigma^{ab}+\widehat\omega_{ab}\widehat\omega^{ab}-R_{ab}U^aU^b.}
$$

In particular, [null shear](../../../geodesic-congruence.md#null-shear) focuses the [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) while [null twist](../../../geodesic-congruence.md#null-twist) enters with the opposite sign. With vanishing [null twist](../../../geodesic-congruence.md#null-twist) and the [null energy condition](../../../general-relativity.md#null-energy-condition), the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) imply $U\cdot\nabla\theta\le-\theta^2/2$. These signs and the factor $1/2$ depend on using the full-trace [null expansion](../../../geodesic-congruence.md#null-expansion) in a two-dimensional screen.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Choose a parallel-transported [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the screen. In that basis a symmetric trace-free [null shear](../../../geodesic-congruence.md#null-shear) and antisymmetric [null twist](../../../geodesic-congruence.md#null-twist) have forms

$$
\widehat\sigma=\begin{pmatrix}s&t\\t&-s\end{pmatrix},\qquad\widehat\omega=\begin{pmatrix}0&w\\-w&0\end{pmatrix}.
$$

Direct multiplication gives

$$
\widehat\sigma^2=(s^2+t^2)I,\qquad\widehat\omega^2=-w^2I,\qquad\widehat\sigma\widehat\omega+\widehat\omega\widehat\sigma=0.
$$

Hence

$$
\widehat B^2=\left(\frac{\theta^2}{4}+s^2+t^2-w^2\right)I+\theta(\widehat\sigma+\widehat\omega).
$$

Since the tidal [matrix](../../../vector-space.md#matrix) is symmetric, the antisymmetric part of the [Sachs optical equations](../../../geodesic-congruence.md#sachs-optical-equations) immediately gives

$$
\boxed{U\cdot\nabla\widehat\omega_{ab}=-\theta\widehat\omega_{ab}.}
$$

Thus an initially [null twist](../../../geodesic-congruence.md#null-twist)-free [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) remains [null twist](../../../geodesic-congruence.md#null-twist)-free while its optical description is regular.

To obtain the trace-free symmetric source, use the original PDF's [Weyl tensor](../../../general-relativity.md#weyl-tensor) formula, with antisymmetrization brackets carrying weight $1/2$. The TeX aid has lost indices and brackets. The correct curvature decomposition is

$$
R_{cedf}=C_{cedf}+g_{c[d}R_{f]e}-g_{e[d}R_{f]c}-\frac R3g_{c[d}g_{f]e}.
$$

Contract with $U^cU^d$ and project $e,f$ onto the screen. Terms containing $U^2$ or a remaining screen-projected $U$ vanish. The only Ricci term left is

$$
\mathcal R_{ab}=P_a{}^eP_b{}^fC_{cedf}U^cU^d+\frac12P_{ab}R_{cd}U^cU^d.
$$

The Weyl term has zero screen trace, by its trace-free property and antisymmetry. Consequently the trace-free symmetric part of the optical equation is the [null-shear propagation equation](../../../geodesic-congruence.md#null-shear-propagation-equation)

$$
\boxed{U\cdot\nabla\widehat\sigma_{ab}=-\theta\widehat\sigma_{ab}-P_a{}^eP_b{}^fC_{cedf}U^cU^d.}
$$

The two-dimensional [matrix](../../../vector-space.md#matrix) identities are essential: in a higher-dimensional screen the [null shear](../../../geodesic-congruence.md#null-shear) square can have a trace-free part and the [null shear](../../../geodesic-congruence.md#null-shear)–[null twist](../../../geodesic-congruence.md#null-twist) [anticommutator](../../../vector-space.md#anticommutator) need not vanish. Choosing the parallel-transported auxiliary [null vector](../../../special-relativity.md#null-vector) makes these tensor transport formulae hold without extra moving-screen terms.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use [geometrized units](../../../general-relativity.md#geometrized-units) $G=c=1$. The [Physical-process first law of black-hole mechanics](../../../general-relativity.md#physical-process-first-law-of-black-hole-mechanics) concerns a small perturbation of a rotating [black hole](../../../general-relativity.md#black-hole) in an initially [stationary spacetime](../../../general-relativity.md#stationary-spacetime) by infalling matter, followed by relaxation to another [stationary spacetime](../../../general-relativity.md#stationary-spacetime). For an uncharged [black hole](../../../general-relativity.md#black-hole), or neutral accretion with charge held fixed, its first-order statement is

$$
\boxed{\delta E-\Omega_H\delta J=\frac{\kappa}{8\pi}\delta A.}
$$

Here $\kappa>0$ is the background [surface gravity](../../../general-relativity.md#surface-gravity), $\Omega_H$ is the background [horizon angular velocity](../../../general-relativity.md#horizon-angular-velocity), and $\delta A$ is the change in [event horizon](../../../general-relativity.md#event-horizon) area. The [energy](../../../classical-mechanics.md#energy) $\delta E$ and [angular momentum](../../../classical-mechanics.md#angular-momentum) $\delta J$ are the fluxes carried into the [event horizon](../../../general-relativity.md#event-horizon); when these account for the changes of the [black hole](../../../general-relativity.md#black-hole), they equal $\delta M$ and its change of [angular momentum](../../../classical-mechanics.md#angular-momentum). The result is a linearized law, not an exact identity for a finite violent accretion event. The perturbation must be small enough that focusing does not produce new caustics or invalidate the expansion about the existing generators.

Let $k^a$ be the stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) normalized at infinity, $m^a$ the axial [Killing vector field](../../../general-relativity.md#killing-vector-field) with $2\pi$-periodic orbits, and

$$
\chi^a=k^a+\Omega_Hm^a.
$$

On the background [Killing horizon](../../../general-relativity.md#killing-horizon), $\chi^a$ is its future-directed null generator and satisfies $\chi^b\nabla_b\chi^a=\kappa\chi^a$. Choose a parameter $v$ with $\chi=\partial_v$. The [null expansion](../../../geodesic-congruence.md#null-expansion) in this parameter is $\theta=\partial_v\log dA$. The generator is not affinely parametrized; if $\ell=\partial_\lambda$ is affine, then $\chi=\kappa\lambda\ell$ after an appropriate choice of affine origin, with $\lambda\propto e^{\kappa v}$. Rescaling the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) gives

$$
\frac{d\theta}{dv}=\kappa\theta-\frac12\theta^2-\widehat\sigma_{ab}\widehat\sigma^{ab}-R_{ab}\chi^a\chi^b.
$$

The [null twist](../../../geodesic-congruence.md#null-twist) vanishes because the generators are normal to the [event horizon](../../../general-relativity.md#event-horizon). By the [Einstein field equations](../../../general-relativity.md#einstein-field-equations), $R_{ab}\chi^a\chi^b=8\pi T_{ab}\chi^a\chi^b$. Background [null expansion](../../../geodesic-congruence.md#null-expansion) and [null shear](../../../geodesic-congruence.md#null-shear) vanish on a [Killing horizon](../../../general-relativity.md#killing-horizon) of the background [stationary spacetime](../../../general-relativity.md#stationary-spacetime). Thus $\theta$ and $\widehat\sigma$ are first order, their squares are second order, and the linearized equation is

$$
\frac{d\theta}{dv}-\kappa\theta=-8\pi\delta T_{ab}\chi^a\chi^b.
$$

The final [stationary spacetime](../../../general-relativity.md#stationary-spacetime) supplies the boundary condition $\theta\to0$ in the future. Explicitly,

$$
\theta(v)=8\pi\int_v^\infty e^{\kappa(v-v')}\delta T_{ab}\chi^a\chi^b(v')\,dv'.
$$

This future boundary condition reflects the global definition of the [event horizon](../../../general-relativity.md#event-horizon). For localized infall, $\theta$ also tends to zero in the remote past. Integrating the linearized equation along the generators, and then over a background cross-section with area element $dA_0$, gives

$$
\kappa\delta A=8\pi\int_{\mathcal H}\delta T_{ab}\chi^a\chi^b\,dv\,dA_0,
\qquad
\delta A=\int_{\mathcal H}\theta\,dv\,dA_0.
$$

Using the background area element introduces only second-order corrections.

With orientations chosen so that future infalling positive [energy](../../../classical-mechanics.md#energy) has positive flux, the conserved [Killing energy](../../../general-relativity.md#killing-energy) and axial [angular momentum](../../../classical-mechanics.md#angular-momentum) give

$$
\delta E=\int_{\mathcal H}\delta T_{ab}k^a\chi^b\,dv\,dA_0,
\qquad
\delta J=-\int_{\mathcal H}\delta T_{ab}m^a\chi^b\,dv\,dA_0.
$$

Consequently $\delta E-\Omega_H\delta J=\int_{\mathcal H}\delta T_{ab}\chi^a\chi^b\,dv\,dA_0$, proving the displayed [Physical-process first law of black-hole mechanics](../../../general-relativity.md#physical-process-first-law-of-black-hole-mechanics). Restoring $G$ replaces $8\pi$ by $8\pi G$. The [null energy condition](../../../general-relativity.md#null-energy-condition) makes the integral nonnegative and therefore implies area increase in this regime; that condition is needed for the sign conclusion, not for the linearized flux identity itself. Charged infall would require the additional electrostatic work term, and an extremal background needs separate treatment because the proof uses $\kappa>0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $p^a$ be the future-directed causal [four-momentum](../../../special-relativity.md#four-momentum) of the fragment captured by the [Kerr black hole](../../../general-relativity.md#kerr-black-hole). In signature $(-+++)$ its conserved [Killing energy](../../../general-relativity.md#killing-energy) and axial [angular momentum](../../../classical-mechanics.md#angular-momentum) are

$$
E=-p_ak^a,\qquad L=p_am^a.
$$

The future-directed null generator of the [Killing horizon](../../../general-relativity.md#killing-horizon) is $\chi^a=k^a+\Omega_Hm^a$, where $\Omega_H$ is the [Kerr horizon angular velocity](../../../general-relativity.md#kerr-horizon-angular-velocity). At a crossing of the future [event horizon](../../../general-relativity.md#event-horizon), the scalar product of a future-directed causal vector with a future-directed [null vector](../../../special-relativity.md#null-vector) is nonpositive. For example, in a local orthonormal frame, $\chi=\alpha(1,\mathbf n)$ with $|\mathbf n|=1$ and $\alpha>0$, while $p^0\ge|\mathbf p|$; hence $p\cdot\chi=\alpha(-p^0+\mathbf p\cdot\mathbf n)\le0$. Therefore

$$
\boxed{E-\Omega_HL=-p\cdot\chi\ge0,\qquad E\ge\Omega_HL.}
$$

This is a local causal restriction, so it applies also to an extremal [Kerr black hole](../../../general-relativity.md#kerr-black-hole). A massive fragment crossing a regular future [event horizon](../../../general-relativity.md#event-horizon) has a strict inequality; equality is the reversible limiting case, with causal [four-momentum](../../../special-relativity.md#four-momentum) approaching the generator direction.

The [Penrose process](../../../general-relativity.md#penrose-process) exploits the fact that $k^a$ becomes spacelike in the [Kerr ergoregion](../../../general-relativity.md#kerr-ergoregion), allowing future-directed fragments with negative [Killing energy](../../../general-relativity.md#killing-energy). For a positive choice of [Kerr horizon angular velocity](../../../general-relativity.md#kerr-horizon-angular-velocity), a captured negative-[energy](../../../classical-mechanics.md#energy) fragment must have sufficiently negative [angular momentum](../../../classical-mechanics.md#angular-momentum) to satisfy the inequality. Conservation of [energy](../../../classical-mechanics.md#energy) in the splitting then gives $E_{\mathrm{escape}}=E_{\mathrm{initial}}-E_{\mathrm{capture}}>E_{\mathrm{initial}}$: the escaping fragment extracts rotational [energy](../../../classical-mechanics.md#energy) and the captured fragment reduces the [black hole](../../../general-relativity.md#black-hole)'s mass and [angular momentum](../../../classical-mechanics.md#angular-momentum).

For the independent thermodynamic argument, take a subextremal [Kerr black hole](../../../general-relativity.md#kerr-black-hole) and a small capture process covered by the [Physical-process first law of black-hole mechanics](../../../general-relativity.md#physical-process-first-law-of-black-hole-mechanics). To first order, $\delta M=E$, $\delta J=L$, so

$$
E-\Omega_HL=\frac{\kappa}{8\pi}\delta A.
$$

The [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics), under its classical [null energy condition](../../../general-relativity.md#null-energy-condition) and regularity hypotheses, gives $\delta A\ge0$; since $\kappa>0$, this reproduces $E\ge\Omega_HL$. The ideal reversible limit has $\delta A\to0$. One should not infer a general finite-capture equality for an extremal [black hole](../../../general-relativity.md#black-hole) by simply substituting $\kappa=0$: the linearized nonextremal process proof and its differentiability assumptions must first be controlled. The causal proof already establishes the required inequality there without this issue.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

[Hawking radiation](../../../general-relativity.md#hawking-radiation) is a prediction of [quantum field theory in curved spacetime](../../../quantum-field-theory.md#quantum-field-theory-in-curved-spacetime), not of classical collapse alone. Consider a free massless [Klein-Gordon field](../../../quantum-field-theory.md#klein-gordon-field) in the [collapse vacuum for Hawking radiation](../../../general-relativity.md#collapse-vacuum-for-hawking-radiation): initially no incoming particles from [past null infinity](../../../general-relativity.md#past-null-infinity), with the short-distance state regular for freely falling observers through the forming [event horizon](../../../general-relativity.md#event-horizon). At late times use the approximately fixed exterior [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime); neglect backreaction during the observation interval. First set $G=c=\hbar=k_B=1$.

The exterior metric has $f(r)=1-2M/r$. Introduce the [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate) and outgoing and ingoing null coordinates,

$$
r_*=r+2M\log\left(\frac r{2M}-1\right),\qquad u=t-r_*,\qquad v=t+r_*.
$$

The [surface gravity](../../../general-relativity.md#surface-gravity) is $\kappa=1/(4M)$. The logarithm in $r_*$ makes a late escaping ray spend a long exterior coordinate time close to the [event horizon](../../../general-relativity.md#event-horizon). One of the regular outgoing [Kruskal–Szekeres coordinates](../../../general-relativity.md#kruskal-szekeres-coordinates) is proportional to $-e^{-\kappa u}$. Smooth propagation backwards through the collapsing body relates this regular coordinate to the incoming coordinate on [past null infinity](../../../general-relativity.md#past-null-infinity). If $v_H$ labels the last ray able to escape, the late-time [Hawking exponential ray map](../../../general-relativity.md#hawking-exponential-ray-map) is consequently

$$
\boxed{v_H-v=C e^{-\kappa u},\qquad
u(v)=-\frac1\kappa\log\left(\frac{v_H-v}{C}\right),\quad C>0.}
$$

Here the symbol $u(v)$ is the outgoing retarded time evaluated on the ray; the first equation is the leading asymptotic relation, with subleading corrections that vanish at late times. The constant $C$ depends on collapse history, whereas the exponential rate is determined by the final [surface gravity](../../../general-relativity.md#surface-gravity). The relation follows from a nondegenerate [Killing horizon](../../../general-relativity.md#killing-horizon); a linear ray map would not have the same effect.

An outgoing positive-frequency mode at [future null infinity](../../../general-relativity.md#future-null-infinity) behaves as $p_\omega\sim e^{-i\omega u}/\sqrt{4\pi\omega}$, where $\omega>0$ is measured with respect to the asymptotic stationary time. In the near-horizon [geometric optics](../../../optics.md#geometrical-optics) approximation its backward-propagated form on [past null infinity](../../../general-relativity.md#past-null-infinity) is

$$
p_\omega(v)\sim\frac{1}{\sqrt{4\pi\omega}}\,
\Theta(v_H-v)\left(\frac{v_H-v}{C}\right)^{i\omega/\kappa}.
$$

This is not purely positive frequency in $v$. Its decomposition into incoming positive-frequency modes $f_{\omega'}\sim e^{-i\omega'v}/\sqrt{4\pi\omega'}$ and their complex conjugates is a [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation):

$$
p_\omega=\int_0^\infty\left(\alpha_{\omega\omega'}f_{\omega'}+\beta_{\omega\omega'}f_{\omega'}^*\right)d\omega'.
$$

The coefficients follow from the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product), or equivalently from the [Fourier transform](../../../analysis.md#fourier-transform) with the indicated flux normalization. Writing $y=v_H-v$ and $a=\omega/\kappa$, the two Fourier integrals, after a convergence regulator, are

$$
I_\pm=\int_0^\infty y^{ia}e^{-(\epsilon\pm i\omega')y}\,dy
=\Gamma(1+ia)(\epsilon\pm i\omega')^{-1-ia},\qquad\epsilon>0.
$$

The equality is the defining integral of the [Gamma function](../../../complex-analysis.md#gamma-function), continued to these arguments from the right half-plane. Up to phases of unit modulus, $\alpha$ is $\sqrt{\omega'/\omega}\,I_+/(2\pi)$ and $\beta$ is $\sqrt{\omega'/\omega}\,I_-/(2\pi)$. Taking $\epsilon\downarrow0$ on the principal branches, the arguments of $\epsilon\pm i\omega'$ tend to $\pm\pi/2$. Thus $|I_+|\propto e^{\pi a/2}$ and $|I_-|\propto e^{-\pi a/2}$, giving the [thermal ratio of Hawking Bogoliubov coefficients](../../../general-relativity.md#thermal-ratio-of-hawking-bogoliubov-coefficients)

$$
\boxed{\frac{|\beta_{\omega\omega'}|^2}{|\alpha_{\omega\omega'}|^2}=e^{-2\pi\omega/\kappa}.}
$$

In particular, using $|\Gamma(1+ia)|^2=\pi a/\sinh(\pi a)$,

$$
|\beta_{\omega\omega'}|^2=\frac{1}{2\pi\kappa\omega'}\frac{1}{e^{2\pi\omega/\kappa}-1}.
$$

The collapse-dependent phases and $C$ disappear from the ratio. The [canonical identities for a bosonic Bogoliubov transformation](../../../quantum-field-theory.md#canonical-identities-for-a-bosonic-bogoliubov-transformation) state that the positive-frequency norm minus the negative-frequency norm is one for a normalized outgoing mode. Combining that identity with the thermal ratio yields the late-time mean occupation

$$
\boxed{\langle N_\omega\rangle=\frac{1}{e^{2\pi\omega/\kappa}-1},\qquad
T_H=\frac{\kappa}{2\pi}=\frac{1}{8\pi M}.}
$$

These are the [Bose-Einstein distribution](../../../statistical-physics.md#bose-einstein-distribution) and the [Hawking temperature](../../../general-relativity.md#hawking-temperature). Strictly, monochromatic modes have delta-function normalization, and $\int d\omega'\,|\beta_{\omega\omega'}|^2$ contains the infinite-duration divergence $\int d\omega'/\omega'$. Normalized [wave packets](../../../wave-equation.md#wave-packet) with a finite frequency band and a finite retarded-time window remove this artifact. For sufficiently late packets the occupation is the frequency average of the displayed thermal factor, tending to it for a narrow band. Fermionic fields instead give the corresponding denominator $e^{2\pi\omega/\kappa}+1$ because their canonical normalization uses anticommutators.

Four-dimensional propagation adds an important qualification to the word thermal. Separation of the massless [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) into [spherical harmonics](../../../analysis.md#spherical-harmonic) gives an exterior radial scattering potential

$$
V_\ell(r)=f(r)\left(\frac{\ell(\ell+1)}{r^2}+\frac{2M}{r^3}\right).
$$

Only a fraction $\Gamma_\ell(\omega)$ of the outgoing mode is transmitted to [future null infinity](../../../general-relativity.md#future-null-infinity); this is the [greybody factor](../../../general-relativity.md#greybody-factor). The scalar particle flux there is

$$
\boxed{\frac{dN}{du\,d\omega}=\frac{1}{2\pi}\sum_{\ell=0}^\infty
(2\ell+1)\frac{\Gamma_\ell(\omega)}{e^{8\pi M\omega}-1}.}
$$

The factor $2\ell+1$ counts the angular modes, and multiplication by $\omega$ gives the spectral [energy](../../../classical-mechanics.md#energy) flux. An observer at infinity therefore receives an outgoing thermal population filtered by curvature scattering, rather than an exact unfiltered blackbody spectrum. In physical units, for mass $M_{\mathrm{phys}}$,

$$
\boxed{T_H=\frac{\hbar c^3}{8\pi G k_BM_{\mathrm{phys}}}.}
$$

There is no incoming thermal bath in the [collapse vacuum for Hawking radiation](../../../general-relativity.md#collapse-vacuum-for-hawking-radiation). The outgoing flux has positive [Killing energy](../../../general-relativity.md#killing-energy); its counterpart inside the [event horizon](../../../general-relativity.md#event-horizon) can carry negative [Killing energy](../../../general-relativity.md#killing-energy). Including the expectation value of the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) in the gravitational evolution allows the mass to decrease. The fixed-background derivation describes the slowly evolving semiclassical regime and does not determine the endpoint of evaporation. Quantum expectation values need not satisfy the classical [null energy condition](../../../general-relativity.md#null-energy-condition), so this loss of area is not a contradiction of the classical [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics). The essential late-time universality is the combination of a regular initial quantum state and the exponential redshift at the newly formed [event horizon](../../../general-relativity.md#event-horizon).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
