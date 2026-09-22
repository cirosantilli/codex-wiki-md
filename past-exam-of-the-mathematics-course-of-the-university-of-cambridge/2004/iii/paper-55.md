# Paper 55

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper55.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper55.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [linear connection on a manifold](../../../fiber-bundle.md#affine-connection) is a rule $(X,Y)\mapsto\nabla_XY$ for differentiating [vector fields](../../../calculus.md#vector-field) which is additive, is $C^\infty$-linear in $X$, is real-linear in $Y$, and obeys $\nabla_X(fY)=X(f)Y+f\nabla_XY$. It extends to [covector fields](../../../differential-form.md#one-form) and arbitrary [tensor fields](../../../fiber-bundle.md#tensor-field) by the [Leibniz rule](../../../calculus.md#leibniz-rule) and compatibility with contraction. In coordinates,

$$
\nabla_aU^d=\partial_aU^d+\Gamma^d{}_{ac}U^c,\qquad
\nabla_a\omega_c=\partial_a\omega_c-\Gamma^d{}_{ac}\omega_d,\qquad
\nabla_af=\partial_af.
$$

This is the [covariant derivative](../../../general-relativity.md#covariant-derivative); the [affine connection](../../../fiber-bundle.md#affine-connection) terms correct the changes of the coordinate [basis](../../../vector-space.md#basis). A symmetric [affine connection](../../../fiber-bundle.md#affine-connection) has zero [torsion tensor](../../../fiber-bundle.md#torsion-tensor), $T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]=0$, or $\Gamma^c{}_{ab}=\Gamma^c{}_{ba}$ in a coordinate [basis](../../../vector-space.md#basis). Symmetry does not imply [metric compatibility](../../../fiber-bundle.md#metric-compatibility); no metric is required for this question.

Additivity of each [covariant derivative](../../../general-relativity.md#covariant-derivative) immediately gives additivity of $\Delta_{ab}$. Expanding the second derivative of a [tensor product](../../../linear-algebra.md#tensor-product) gives

$$
\begin{aligned}
\nabla_a\nabla_b(Q\otimes S)={}&(\nabla_a\nabla_bQ)\otimes S+(\nabla_bQ)\otimes\nabla_aS\\
&+(\nabla_aQ)\otimes\nabla_bS+Q\otimes\nabla_a\nabla_bS.
\end{aligned}
$$

Subtract the expression with $a,b$ exchanged. The two mixed terms cancel, proving that the [curvature commutator is a tensor derivation](../../../general-relativity.md#curvature-commutator-is-a-tensor-derivation):

$$
\boxed{\Delta_{ab}(Q\otimes S)=(\Delta_{ab}Q)\otimes S+Q\otimes\Delta_{ab}S.}
$$

For a scalar, $\nabla_a\nabla_bf=\partial_a\partial_bf-\Gamma^c{}_{ab}\partial_cf$. Commuting partial derivatives and using the symmetric [affine connection](../../../fiber-bundle.md#affine-connection) gives $\Delta_{ab}f=0$. Consequently $\Delta_{ab}(fU)=f\Delta_{ab}U$: the [commutator](../../../lie-algebra.md#commutator) is linear over smooth functions, not merely over constant scalars. Write $U=U^ce_c$ in a local [basis](../../../vector-space.md#basis). The [tensor](../../../linear-algebra.md#tensor)-product rule gives $\Delta_{ab}U=U^c\Delta_{ab}e_c$, showing that its value at a point depends only on $U$ at that point. Thus it defines the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) by

$$
\boxed{\Delta_{ab}U^d=R_{abc}{}^dU^c,\qquad
R_{abc}{}^d=\partial_a\Gamma^d{}_{bc}-\partial_b\Gamma^d{}_{ac}+\Gamma^d{}_{ae}\Gamma^e{}_{bc}-\Gamma^d{}_{be}\Gamma^e{}_{ac}.}
$$

The antisymmetrized second [covariant derivative](../../../general-relativity.md#covariant-derivative) is itself tensorial in the derivative indices, so this pointwise map transforms as a [tensor](../../../linear-algebra.md#tensor). The formula or the defining [commutator](../../../lie-algebra.md#commutator) gives $R_{abc}{}^d=-R_{bac}{}^d$, hence $R_{abc}{}^d=R_{[ab]c}{}^d$ with normalized antisymmetrization.

Apply the [commutator](../../../lie-algebra.md#commutator) to the scalar contraction $\omega_cU^c$. Its action vanishes, so

$$
0=(\Delta_{ab}\omega_c)U^c+\omega_cR_{abd}{}^cU^d.
$$

Since $U$ is arbitrary, $\Delta_{ab}\omega_c=-R_{abc}{}^d\omega_d$. Repeated use of the [tensor](../../../linear-algebra.md#tensor)-product rule gives one plus [curvature](../../../differential-geometry.md#curvature) action for an upper index and one minus action for each lower index. In particular,

$$
\boxed{\Delta_{ab}S^c{}_{de}=R_{abf}{}^cS^f{}_{de}-R_{abd}{}^fS^c{}_{fe}-R_{abe}{}^fS^c{}_{df}.}
$$

The type notation in the PDF means one contravariant and two covariant indices, not a fractional [tensor](../../../linear-algebra.md#tensor) order.

For the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity), put $\omega_c=\nabla_cf$ and $H_{bc}=\nabla_b\nabla_cf$. The [symmetric Hessian of a scalar field](../../../general-relativity.md#symmetric-hessian-of-a-scalar-field) satisfies $H_{bc}=H_{cb}$. Therefore the six third-derivative terms cancel in

$$
\Delta_{ab}\omega_c+\Delta_{bc}\omega_a+\Delta_{ca}\omega_b
=\nabla_aH_{bc}-\nabla_bH_{ac}+\nabla_bH_{ca}-\nabla_cH_{ba}+\nabla_cH_{ab}-\nabla_aH_{cb}=0.
$$

Substituting the covector [curvature](../../../differential-geometry.md#curvature) action gives $(R_{abc}{}^d+R_{bca}{}^d+R_{cab}{}^d)\nabla_df=0$. At a chosen point the [gradient](../../../calculus.md#gradient) of a smooth scalar can be any covector, so

$$
\boxed{R_{abc}{}^d+R_{bca}{}^d+R_{cab}{}^d=0,\qquad R_{[abc]}{}^d=0.}
$$

The second form follows from the already proved first-pair antisymmetry.

For the [second Bianchi identity](../../../general-relativity.md#second-bianchi-identity), the same third-derivative cancellation can be organized as an operator identity. On vector-valued components set $D_a=\partial_a+\Gamma_a$, with $(\Gamma_a)^e{}_d=\Gamma^e{}_{ad}$. Although a full second [covariant derivative](../../../general-relativity.md#covariant-derivative) includes a term $-\Gamma^f{}_{ab}D_f$ for its lower derivative index, that term cancels on antisymmetrization because the [affine connection](../../../fiber-bundle.md#affine-connection) is symmetric. Thus $[D_b,D_c]=\mathcal R_{bc}$, where $(\mathcal R_{bc})^e{}_d=R_{bcd}{}^e$ acts by multiplication. Expanding the three nested operator [commutators](../../../lie-algebra.md#commutator) makes all six triple products cancel:

$$
[D_a,[D_b,D_c]]+[D_b,[D_c,D_a]]+[D_c,[D_a,D_b]]=0.
$$

Equivalently, the cyclic sum of $\partial_a\mathcal R_{bc}+[\Gamma_a,\mathcal R_{bc}]$ vanishes. These are the [covariant derivative](../../../general-relativity.md#covariant-derivative) terms on the upper and last lower [curvature](../../../differential-geometry.md#curvature) indices. The two remaining lower indices add $-\Gamma^f{}_{ab}R_{fcd}{}^e-\Gamma^f{}_{ac}R_{bfd}{}^e$. In the cyclic sum these additions cancel in pairs, using $\Gamma^f{}_{ab}=\Gamma^f{}_{ba}$ and $R_{fcd}{}^e=-R_{cfd}{}^e$. Hence the [Bianchi identities from covariant derivative commutators](../../../general-relativity.md#bianchi-identities-from-covariant-derivative-commutators) give

$$
\boxed{\nabla_aR_{bcd}{}^e+\nabla_bR_{cad}{}^e+\nabla_cR_{abd}{}^e=0,\qquad\nabla_{[a}R_{bc]d}{}^e=0.}
$$

Both identities here apply to any torsion-free linear [affine connection](../../../fiber-bundle.md#affine-connection); the second derivation does not require choosing a metric [affine connection](../../../fiber-bundle.md#affine-connection).

## 2

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [strong equivalence principle](../../../general-relativity.md#strong-equivalence-principle) extends universality of free fall to bodies with appreciable gravitational binding energy and requires results of sufficiently local experiments, including gravitational experiments, in freely falling laboratories to be independent of their location and velocity. The [Einstein equivalence principle](../../../general-relativity.md#einstein-equivalence-principle) makes the corresponding statement for nongravitational experiments; the weak principle concerns test-body free fall without significant self-gravity. In a locally inertial frame the nongravitational laws take their special-relativistic form, while internal gravitational experiments retain the same local gravitational laws and coupling constants. They are not declared to have no gravity.

In a metric description, one may set $g_{ab}=\eta_{ab}$ and $\partial_cg_{ab}=0$ at a point by [Riemann normal coordinates](../../../general-relativity.md#normal-coordinates), so the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) vanishes there. This removes a locally uniform external gravitational acceleration, not the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor). Tidal effects between separated bodies, or accumulated over a finite-duration experiment, remain. The local limit must control both the laboratory's size and duration. Gravitationally self-bound bodies are included in the strong version, so it is stronger than equality of inertial and passive gravitational mass for ordinary test particles.

A heuristic field-equation argument supplements this principle with further assumptions: gravity is described only by a Lorentzian metric, matter couples universally to it, the [affine connection](../../../fiber-bundle.md#affine-connection) is Levi-Civita, and the leading local field equation is a symmetric covariant equation with at most second metric derivatives and is linear in those second derivatives. Matter obeys [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) $\nabla^aT_{ab}=0$. [Curvature](../../../differential-geometry.md#curvature) therefore supplies the natural candidates $R_{ab}$ and $Rg_{ab}$, with a constant multiple of $g_{ab}$ also allowed. Write the candidate as $R_{ab}+cRg_{ab}+\Lambda g_{ab}=\kappa T_{ab}$. The [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) and [metric compatibility](../../../fiber-bundle.md#metric-compatibility) give

$$
\nabla^aR_{ab}=\frac12\nabla_bR,\qquad
\nabla^a(R_{ab}+cRg_{ab})=(\tfrac12+c)\nabla_bR.
$$

To permit varying [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) consistently with matter conservation, take $c=-1/2$. This gives the [Einstein tensor](../../../general-relativity.md#einstein-tensor) $G_{ab}=R_{ab}-g_{ab}R/2$ and

$$
G_{ab}+\Lambda g_{ab}=\kappa T_{ab}.
$$

The [cosmological constant](../../../cosmology.md#cosmological-constant) is constant so that its divergence vanishes. These assumptions motivate the usual Einstein equation; the equivalence principle alone does not exclude theories with extra fields or higher [curvature](../../../differential-geometry.md#curvature) terms.

The sign and normalization are fixed by the supplied Newtonian limit. Use signature $(+---)$, the [curvature](../../../differential-geometry.md#curvature) [commutator](../../../lie-algebra.md#commutator) convention of Q1, and the Ricci contraction

$$
R_{ab}=R_{acb}{}^c.
$$

This is the contraction for which $R_{00}\simeq-\nabla^2\varphi$ in the question. In four dimensions, tracing the candidate equation gives $-R+4\Lambda=\kappa T$, and substituting back gives

$$
R_{ab}=\kappa\left(T_{ab}-\frac12g_{ab}T\right)+\Lambda g_{ab}.
$$

For slowly moving pressureless matter, $T_{00}\simeq\rho$, $T\simeq\rho$ and $g_{00}\simeq1$. On local scales where the cosmological term is negligible, $R_{00}\simeq\kappa\rho/2$. Compare this with $R_{00}\simeq-\nabla^2\varphi$ and the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) $\nabla^2\varphi=4\pi G\rho$. The [Newtonian normalization of the Einstein field equations](../../../general-relativity.md#newtonian-normalization-of-the-einstein-field-equations) is therefore

$$
\boxed{\kappa=-8\pi G,\qquad G_{ab}+\Lambda g_{ab}=-8\pi G T_{ab}.}
$$

Units with light speed one are used, as in the paper; for conventional physical stress-energy units the coupling is $-8\pi G/c^4$. If the opposite Ricci/[curvature](../../../differential-geometry.md#curvature) sign convention is adopted, the displayed geometric coupling sign changes accordingly. With the cosmological term retained in the same weak-field calculation, the Newtonian equation becomes $\nabla^2\varphi=4\pi G\rho-\Lambda$, consistent with this sign choice.

## 3

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use units $c=1$, signature $(+---)$, and the weak-field metric $g_{ab}=\eta_{ab}+h_{ab}$. Define the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation) by $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$, with $h=\eta^{ab}h_{ab}$. In the [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity), $\partial^a\bar h_{ab}=0$, the sign convention of Q2 gives

$$
G^{(1)}_{ab}=\frac12\Box\bar h_{ab},\qquad
\Box\bar h_{ab}=-16\pi G T_{ab}.
$$

For completeness, the linearized [Ricci tensor](../../../general-relativity.md#ricci-tensor) in this convention is

$$
R^{(1)}_{ab}=\frac12\left(\Box h_{ab}+\partial_a\partial_bh-\partial_c\partial_ah^c{}_b-\partial_c\partial_bh^c{}_a\right).
$$

Substituting the Lorenz condition $\partial_ch^c{}_b=\partial_bh/2$ and trace reversing gives the stated [Einstein tensor](../../../general-relativity.md#einstein-tensor). For a stationary source, $\Box=-\nabla^2$, so $\nabla^2\bar h_{ab}=16\pi G T_{ab}$.

Keep the monopole terms of order $\epsilon=GM/R$ and the leading term linear in the rotation rate. Since $\Omega R=O(\epsilon^{1/2})$, the latter metric term is of order $\epsilon\Omega R=O(\epsilon^{3/2})$ on the shell. Thus it would disappear from a strictly order-$\epsilon$ truncation; the requested approximation must retain the leading rotation correction as well. Terms $T_{ij}=\rho v_iv_j$ generate metric corrections of order $\epsilon(\Omega R)^2=O(\epsilon^2)$ and are neglected. Corrections to four-velocity normalization and the supporting shell stresses affect the omitted higher orders. To retained order,

$$
T_{00}=\rho,\qquad T_{0i}=-\rho v_i,\qquad
\mathbf v=\boldsymbol\Omega\times\mathbf x,\quad\boldsymbol\Omega=\Omega\widehat{\mathbf z}.
$$

The minus sign in $T_{0i}$ comes from lowering its spatial index; using $T^{0i}$ in its place would reverse the dragging direction.

The scalar Poisson solution regular at the centre and vanishing at spatial infinity is $\bar h_{00}=-4GM/r$ outside the shell and $\bar h_{00}=-4GM/R=-4\epsilon$ inside. Continuity and the derivative jump $\bar h_{00}'(R^+)-\bar h_{00}'(R^-)=4GM/R^2$ verify the density $M\delta(r-R)/(4\pi R^2)$. Also $\bar h_{ij}=0$ at this order. Undoing trace reversal gives

$$
h_{00}=\frac12\bar h_{00}=-2\epsilon,\qquad h_{ij}=\frac12\delta_{ij}\bar h_{00}=-2\epsilon\delta_{ij}.
$$

Comparing with the scalar parts of the interior line element yields **$A=-\epsilon$ and $C=\epsilon$**.

For the mass-current contribution write

$$
\bar h_{0i}=F(r)(\widehat{\mathbf z}\times\widehat{\mathbf r})_i.
$$

Each nonzero angular component is a degree-one [spherical harmonic](../../../analysis.md#spherical-harmonic). The supplied [Laplacian](../../../calculus.md#laplacian) eigenvalue therefore gives

$$
F''+\frac2rF'-\frac2{r^2}F=-\frac{4GM\Omega}{R}\delta(r-R).
$$

Away from the shell, the two radial solutions are $r$ and $r^{-2}$. Regularity at $r=0$ and decay at infinity select $F_{\rm in}=ar$ and $F_{\rm out}=b/r^2$. Continuity at $R$ requires $b=aR^3$, and integrating the [differential equation](../../../differential-equation.md) across the shell gives

$$
F'(R^+)-F'(R^-)=-3a=-\frac{4GM\Omega}{R}.
$$

Thus $a=4GM\Omega/(3R)=\omega$, with $F_{\rm in}=\omega r$. Trace reversal leaves mixed components unchanged, so $h_{0i}=\omega(\widehat{\mathbf z}\times\mathbf x)_i=\omega(-y,x,0)_i$. The paper writes $g_{0i}=-B_i$, giving the [frame dragging inside a slowly rotating spherical shell](../../../general-relativity.md#frame-dragging-inside-a-slowly-rotating-spherical-shell)

$$
\boxed{-A=C=\epsilon,\qquad\mathbf B=\omega(y,-x,0),\qquad\omega=\frac{4\epsilon\Omega}{3}.}
$$

This dipole matching is valid throughout $r<R$; it does not assume the observation point is very close to the centre. The stationary current is divergence-free, so this solution also satisfies the Lorenz gauge. The exterior result is $h_{0i}=2G(\mathbf J\times\mathbf x)_i/r^3$, where the thin shell has $\mathbf J=(2/3)MR^2\boldsymbol\Omega$, providing a check on the coefficient.

To identify the freely falling frames inside, let $\mathcal R_z(\theta)$ be the ordinary spatial rotation by angle $\theta$. Define the [inertial coordinates inside a slowly rotating spherical shell](../../../general-relativity.md#inertial-coordinates-inside-a-slowly-rotating-spherical-shell) by

$$
T=(1-\epsilon)t,\qquad\mathbf X=(1+\epsilon)\mathcal R_z(-\omega t)\mathbf x.
$$

Differentiating and dropping $\epsilon^2$, products beyond the retained rotation order, and $\omega^2$ gives

$$
dT^2-d\mathbf X^2=(1-2\epsilon)dt^2-(1+2\epsilon)d\mathbf x^2+2(\boldsymbol\omega\times\mathbf x)\cdot d\mathbf x\,dt,
$$

which is precisely the interior metric. Thus the retained interior [curvature](../../../differential-geometry.md#curvature) is zero, despite its nontrivial relation to the nonrotating coordinates anchored at infinity. [Timelike geodesics](../../../general-relativity.md#timelike-geodesic) in these local inertial coordinates are straight lines $\mathbf X=\mathbf X_0+\mathbf V T$, with $|\mathbf V|<1$. In the original coordinates this is

$$
\mathbf x(t)=\frac1{1+\epsilon}\mathcal R_z(\omega t)\{\mathbf X_0+(1-\epsilon)\mathbf Vt\},
$$

understood to the same perturbative order. Their coordinate equation is $d^2\mathbf x/dt^2=2\boldsymbol\omega\times d\mathbf x/dt$ to first rotation order. There is no interior Newtonian acceleration from the constant potential; the velocity-dependent term is the apparent Coriolis term relative to the locally dragged inertial axes.

A freely transported [gyroscope](../../../classical-mechanics.md#gyroscope) at rest in the interior to the retained order has constant spatial direction in the $\mathbf X$ frame, hence its direction in the original axes obeys $d\mathbf S/dt=\boldsymbol\omega\times\mathbf S$. **Local inertial axes precess in the same sense as the shell, at $\omega=(4\epsilon/3)\Omega$ relative to distant nonrotating axes.** This is the interior [Lense-Thirring precession](../../../general-relativity.md#lense-thirring-precession). For a weak shell the dragging is only a small fraction of its [angular velocity](../../../classical-mechanics.md#angular-velocity), not perfect corotation. It is compatible with the equivalence principle: rotation relative to distant axes is a comparison between frames, and local flatness at the retained order does not make that comparison vanish. Quadratic rotation terms, which would include centrifugal effects and additional [curvature](../../../differential-geometry.md#curvature), are outside the requested leading approximation.

## 4

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Both metrics have [curvature](../../../differential-geometry.md#curvature) radius one and signature $(+-)$. Their global topology must be specified as well as their local metric. The usual [two-dimensional de Sitter spacetime](../../../general-relativity.md#two-dimensional-de-sitter-spacetime) is the hyperboloid $(X^0)^2-(X^1)^2-(X^2)^2=-1$ in three-dimensional [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), parametrized by

$$
X^0=\sinh t,\qquad X^1=\cosh t\cos\chi,\qquad X^2=\cosh t\sin\chi.
$$

Thus **$t\in\mathbb R$ and $\chi$ is periodic modulo $2\pi$**, for example $0\leq\chi<2\pi$. Spatial slices are circles. Unwrapping $\chi$ instead gives the [universal cover](../../../algebraic-topology.md#universal-cover), not the usual closed spatial model.

The ordinary [two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#two-dimensional-anti-de-sitter-spacetime) hyperboloid is $(X^0)^2+(X^1)^2-(X^2)^2=1$ in ambient signature $(++-)$, with

$$
X^0=\cosh r\cos t,\qquad X^1=\cosh r\sin t,\qquad X^2=\sinh r.
$$

On this quadric **$r\in\mathbb R$ and $t$ is periodic modulo $2\pi$**. The closed time circles are timelike, so it contains [closed timelike curves](../../../general-relativity.md#closed-timelike-curve). The usual physically causal [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) model is its [universal cover](../../../algebraic-topology.md#universal-cover), for which **$r,t\in\mathbb R$**, with time no longer identified. The signed radial coordinate has two spatial ends; restricting to $r\geq0$ would retain only half of this global model. The metric by itself cannot distinguish periodic time from the cover. The [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) is $+2$ for [de Sitter](../../../general-relativity.md#de-sitter-spacetime) and $-2$ for [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) in the Ricci convention of Q2. Both are maximally symmetric and have no [curvature](../../../differential-geometry.md#curvature) singularity; these toy two-dimensional metrics illustrate causal geometry rather than the ordinary four-dimensional matter field equations.

For the [conformal cylinder of two-dimensional de Sitter spacetime](../../../general-relativity.md#conformal-cylinder-of-two-dimensional-de-sitter-spacetime), introduce

$$
\eta=\arctan(\sinh t),\qquad d\eta=\operatorname{sech}t\,dt,\qquad
\cosh t=\sec\eta.
$$

Then

$$
\boxed{ds^2=\sec^2\eta\,(d\eta^2-d\chi^2),\qquad-\pi/2<\eta<\pi/2,\quad\chi\sim\chi+2\pi.}
$$

The [conformal boundaries](../../../geometry-and-topology.md#conformal-boundary) $\eta=\pm\pi/2$ are spacelike circles, representing past and future infinity. [Null geodesics](../../../special-relativity.md#null-geodesic) are straight lines $\chi=\chi_0\pm(\eta-\eta_0)$, with the periodic spatial identification. The finite total conformal-time interval explains the [cosmological horizons](../../../general-relativity.md#cosmological-horizon): light cannot complete a full trip around the circle during the entire history.

For the [conformal strip of two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#conformal-strip-of-two-dimensional-anti-de-sitter-spacetime), use

$$
\psi=\arctan(\sinh r),\qquad dr=\sec\psi\,d\psi,\qquad\cosh r=\sec\psi,
$$

so on the [universal cover](../../../algebraic-topology.md#universal-cover)

$$
\boxed{ds^2=\sec^2\psi\,(dt^2-d\psi^2),\qquad-\pi/2<\psi<\pi/2,\quad t\in\mathbb R.}
$$

Its two [conformal boundaries](../../../geometry-and-topology.md#conformal-boundary) at $\psi=\pm\pi/2$ are timelike. Null rays are $t\pm\psi=\text{constant}$, and the strip extends for arbitrarily long coordinate time. The distances in these conformal diagrams are not physical lengths: a [conformal boundary](../../../geometry-and-topology.md#conformal-boundary) may be reached in finite coordinate time while lying infinitely far away in physical [affine parameter](../../../riemannian-geometry.md#affine-parameter).

<a id="4/image-conformal-cylinder-and-observer-horizons-of-two-dimensional-de-sitter-spacetime-compared-with-the-timelike-boundaries-and-geodesics-of-the-ads-universal-cover"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-55-conformal-structure.png)

**[Figure 1](#4/image-conformal-cylinder-and-observer-horizons-of-two-dimensional-de-sitter-spacetime-compared-with-the-timelike-boundaries-and-geodesics-of-the-ads-universal-cover). Conformal cylinder and observer horizons of two-dimensional de Sitter spacetime, compared with the timelike boundaries and geodesics of the AdS universal cover**.

The sides of the [de Sitter](../../../general-relativity.md#de-sitter-spacetime) diagram are identified; its top and bottom are spacelike infinities. The [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) diagram shows a finite window of an infinite time strip, with no identification of top and bottom. Null rays have slope one in both diagrams. The blue curves are [timelike geodesics](../../../general-relativity.md#timelike-geodesic), while the colored [de Sitter](../../../general-relativity.md#de-sitter-spacetime) lines bound the central observer's causal domains.

The [geodesics of two-dimensional de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-de-sitter-spacetime) can be derived directly. Let an overdot denote an [affine parameter](../../../riemannian-geometry.md#affine-parameter) normalized so that the tangent norm is $\kappa=1,0,-1$ for timelike, null and [spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic). The cyclic coordinate $\chi$ gives conserved $p=\cosh^2t\,\dot\chi$, and normalization gives

$$
\dot t^2-\frac{p^2}{\cosh^2t}=\kappa.
$$

Writing $y=\sinh t$ reduces this to $\dot y^2=p^2+\kappa(1+y^2)$. For a future-directed [timelike geodesic](../../../general-relativity.md#timelike-geodesic),

$$
y=\sqrt{1+p^2}\sinh(\tau-\tau_0),\qquad
\chi(t)=\chi_0+\arcsin\left(\frac{p\tanh t}{\sqrt{1+p^2}}\right).
$$

The spatially comoving curves $p=0$ are [geodesics](../../../riemannian-geometry.md#geodesic), and every [timelike geodesic](../../../general-relativity.md#timelike-geodesic) extends through all $t\in\mathbb R$, with infinite [proper time](../../../special-relativity.md#proper-time) in both directions. Initially comoving nearby observers have physical separation proportional to $\cosh t$, displaying [de Sitter](../../../general-relativity.md#de-sitter-spacetime)'s tidal defocusing. Relative separation can initially decrease for other initial velocities; not every pair is monotonically separating.

For a nontrivial [null geodesic](../../../special-relativity.md#null-geodesic), $p\ne0$ and $\sinh t=\pm|p|\lambda+\text{constant}$. Hence the conformal infinities at $t\to\pm\infty$ occur at infinite [affine parameter](../../../riemannian-geometry.md#affine-parameter), despite their finite values of $\eta$. For a [spacelike geodesic](../../../riemannian-geometry.md#spacelike-geodesic), $|p|\geq1$ and $y=\sqrt{p^2-1}\sin(s-s_0)$. Over a full affine-length period $2\pi$, integrating $\dot\chi=p/[1+(p^2-1)\sin^2(s-s_0)]$ gives a change $2\pi\operatorname{sgn}p$. Thus the [spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic) close on the usual cylinder. The special case $|p|=1$ is the equatorial circle $t=0$. These closed spacelike curves do not threaten causality.

The [geodesics of two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-anti-de-sitter-spacetime) instead conserve $E=\cosh^2r\,\dot t$. Their norm equation gives

$$
\dot r^2=\frac{E^2}{\cosh^2r}-\kappa,\qquad
\left(\frac{d}{ds}\sinh r\right)^2=E^2-\kappa(1+\sinh^2r).
$$

A future [timelike geodesic](../../../general-relativity.md#timelike-geodesic) has $E\geq1$ and

$$
\boxed{\sinh r=\sqrt{E^2-1}\sin(\tau-\tau_0).}
$$

Its turning points are $r=\pm\operatorname{arcosh}E$. [Timelike geodesics](../../../general-relativity.md#timelike-geodesic) oscillate rather than escaping to the spatial boundary. For $E=1$, the central curve $r=0$ is [geodesic](../../../riemannian-geometry.md#geodesic). Integrating $\dot t=E/[1+(E^2-1)\sin^2(\tau-\tau_0)]$ shows that a full proper-time period $2\pi$ advances coordinate time by $2\pi$. They close on the periodically identified hyperboloid but remain complete nonclosed curves on the [universal cover](../../../algebraic-topology.md#universal-cover). [Geodesics](../../../riemannian-geometry.md#geodesic) leaving $r=0,t=0$ reconverge at $r=0,t=\pi$ after [proper time](../../../special-relativity.md#proper-time) $\pi$, illustrating [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) tidal focusing. A static observer at nonzero fixed $r$ is accelerated, not one of these oscillating free trajectories.

For [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) [null geodesics](../../../special-relativity.md#null-geodesic), $\sinh r=\pm E\lambda+\text{constant}$ and $t\mp\psi=\text{constant}$. They approach either timelike [conformal boundary](../../../geometry-and-topology.md#conformal-boundary) at infinite [affine parameter](../../../riemannian-geometry.md#affine-parameter), while the coordinate-time travel from the centre is only $\pi/2$. A [spacelike geodesic](../../../riemannian-geometry.md#spacelike-geodesic) has $\sinh r=\sqrt{E^2+1}\sinh(s-s_0)$ and connects the two spatial ends with infinite affine length. Both global models are geodesically complete. Reflecting a signal at the [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) [conformal boundary](../../../geometry-and-topology.md#conformal-boundary) is a choice of boundary condition for fields; it is not an automatic continuation of a [geodesic](../../../riemannian-geometry.md#geodesic) at a finite affine endpoint.

For the complete [de Sitter](../../../general-relativity.md#de-sitter-spacetime) observer at $\chi=0$, let $d(\chi,0)\in[0,\pi]$ be the shortest angular distance. An event at $(\eta,\chi)$ can send a signal reaching the observer at a finite future time exactly when

$$
d(\chi,0)<\pi/2-\eta.
$$

It can receive a signal sent by the observer at a finite past time exactly when $d(\chi,0)<\eta+\pi/2$. Equality gives the future and past [observer horizons in two-dimensional de Sitter spacetime](../../../general-relativity.md#observer-horizons-in-two-dimensional-de-sitter-spacetime); their null branches are respectively $\chi=\pm(\pi/2-\eta)$ and $\chi=\pm(\eta+\pi/2)$ on the displayed cylinder. Their intersection is the central static patch, $d(\chi,0)+|\eta|<\pi/2$. All complete [timelike geodesic](../../../general-relativity.md#timelike-geodesic) observers have analogous horizons by [de Sitter](../../../general-relativity.md#de-sitter-spacetime) symmetry. These are observer-dependent [cosmological horizons](../../../general-relativity.md#cosmological-horizon), not singularities of the global coordinates or Cauchy horizons.

In contrast, the complete central [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) observer can exchange signals with every event at finite $r$: the conformal distance $|\psi|$ is finite and the observer exists for all $t\in\mathbb R$. Its static Killing vector has squared norm $\cosh^2r>0$ everywhere. Thus **global [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) on its cover has no cosmological event horizon for this observer**, although other restricted patches or accelerated observers can have horizons.

The causal predictability distinction is also important. Global [de Sitter](../../../general-relativity.md#de-sitter-spacetime) is [globally hyperbolic](../../../general-relativity.md#globally-hyperbolic-spacetime): constant-$t$ circles are [Cauchy surfaces](../../../general-relativity.md#cauchy-surface). A causal curve is monotone in $t$ and satisfies $|d\chi/dt|\leq\operatorname{sech}t$; if it ended at finite $t$, compactness of the spatial circle would allow an endpoint and extension. Hence an inextendible causal curve crosses every such slice once. [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) on the cover has no closed timelike curves, but it is not globally hyperbolic. For two central events at $t=-T$ and $t=T$, with $T>\pi/2$, their causal diamond contains events at $t=0$ and arbitrarily large $r$, so it is not compact. Initial data alone do not determine field evolution without conditions at the timelike [conformal boundaries](../../../geometry-and-topology.md#conformal-boundary). **[de Sitter](../../../general-relativity.md#de-sitter-spacetime) has spacelike conformal infinities and cosmological observer horizons; covered [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) has timelike conformal infinities and requires boundary data.** The distinction between the [AdS](../../../general-relativity.md#anti-de-sitter-spacetime) quadric and its [universal cover](../../../algebraic-topology.md#universal-cover) is also explained in [David Tong's general relativity lectures](https://www.damtp.cam.ac.uk/user/tong/gr/grhtml/S4.html).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
