# Calculus of variations

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Calculus_of_variations)

Calculus of variations finds [stationary points](#stationary-point) of [functionals](#functional), often among [functions](function.md) or [regular curves](differential-geometry.md#regular-curve).

**Table of contents**

- [Quadratic minor null Lagrangian](#quadratic-minor-null-lagrangian)
- [Brachistochrone problem](#brachistochrone-problem)
- [Travel-time minimization with speed proportional to squared radius](#travel-time-minimization-with-speed-proportional-to-squared-radius)
- [Gamma-convergence](#gamma-convergence)
- [Variational problem](#variational-problem)
- [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)
  - [Weak lower semicontinuity of convex gradient energies](#weak-lower-semicontinuity-of-convex-gradient-energies)
  - [Symmetric elliptic Dirichlet energy with a nonpositive potential](#symmetric-elliptic-dirichlet-energy-with-a-nonpositive-potential)
  - [Screened sine-Gordon energy](#screened-sine-gordon-energy)
    - [Failure of the source-size bound for the screened sine-Gordon equation](#failure-of-the-source-size-bound-for-the-screened-sine-gordon-equation)
  - [Minimizing sequence](#minimizing-sequence)
  - [Bounded slope condition](#bounded-slope-condition)
  - [Comparison principle for convex variational integrals](#comparison-principle-for-convex-variational-integrals)
- [Functional](#functional)
  - [Quadratic functional](#quadratic-functional)
  - [Epigraph](#epigraph)
  - [Functional derivative](#functional-derivative)
    - [Functional chain rule](#functional-chain-rule)
  - [Energy functional](#energy-functional)
    - [Critical point of an energy functional](#critical-point-of-an-energy-functional)
    - [p-energy](#p-energy)
  - [Lagrangian](#lagrangian)
    - [Lagrangian function in constrained optimization](#lagrangian-function-in-constrained-optimization)
  - [Variation](#variation)
    - [First variation](#first-variation)
      - [Fundamental lemma of the calculus of variations](#fundamental-lemma-of-the-calculus-of-variations)
- [Stationary point](#stationary-point)
- [Dirichlet principle](#dirichlet-principle)
  - [Sharp radial Dirichlet energy inequality](#sharp-radial-dirichlet-energy-inequality)
- [Optical ray in cylindrical coordinates](#optical-ray-in-cylindrical-coordinates)
  - [Helical extremal](#helical-extremal)
- [Noether theorem](#noether-theorem)
  - [Noether second theorem](#noether-second-theorem)
    - [Noether identity for abelian scalar gauge symmetry](#noether-identity-for-abelian-scalar-gauge-symmetry)
  - [Noether conserved quantity for a mechanical point symmetry](#noether-conserved-quantity-for-a-mechanical-point-symmetry)
- [Second variation](#second-variation)
  - [Jacobi equation](#jacobi-equation)
  - [Conjugate point](#conjugate-point)
    - [Multiplicity of a conjugate point](#multiplicity-of-a-conjugate-point)
    - [Nonpositive sectional curvature excludes conjugate points](#nonpositive-sectional-curvature-excludes-conjugate-points)
  - [Wirtinger inequality](#wirtinger-inequality)
    - [Periodic Wirtinger inequality](#periodic-wirtinger-inequality)

## Quadratic minor null Lagrangian

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For constant $K$, this quadratic combination of two-by-two gradient minors is a [divergence](calculus.md#divergence). Indeed,

$$
K_{k\gamma}\epsilon_{\alpha\beta\gamma}\epsilon_{ijk}\overline{u_{i,\alpha}}u_{j,\beta}=\partial_\alpha\left(K_{k\gamma}\epsilon_{\alpha\beta\gamma}\epsilon_{ijk}\overline{u_i}u_{j,\beta}\right),
$$

because the term containing $u_{j,\beta\alpha}$ vanishes by antisymmetry of the [Levi-Civita symbol](calculus.md#levi-civita-symbol). Its volume integral vanishes for homogeneous displacement boundary data. It also vanishes pointwise on [rank-one matrices](vector-space.md#rank-one-matrix), since $\nu_\alpha\nu_\beta$ is symmetric. Consequently one can strengthen an elastic energy density by such a term without changing fixed-boundary incremental energies or [acoustic tensors](continuum-mechanics.md#acoustic-tensor).

## Brachistochrone problem

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

The brachistochrone problem asks for the curve along which a particle released from rest reaches a specified target fastest under a uniform gravitational field, without friction. With downward depth $u$, conservation of energy gives speed $\sqrt{2gu}$ and travel time $\int\sqrt{(1+u'^2)/(2gu)}\,dx$. The [Beltrami identity](analysis.md#beltrami-identity) makes $u(1+u'^2)$ constant, leading to a [cycloid](topology.md#cycloid). If only the horizontal endpoint coordinate $x_0>0$ is fixed, the [natural boundary conditions for a free endpoint](analysis.md#natural-boundary-conditions-for-a-free-endpoint) select the half arch ending at its deepest point, with depth $2x_0/\pi$ and minimum time $\sqrt{\pi x_0/g}$.

## Travel-time minimization with speed proportional to squared radius

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For speed $v=kr^2$ in the punctured plane, the travel-time element is $ds/(kr^2)$. Under the [inversion in a circle](group-theory.md#inversion-in-a-circle) with radial coordinate $u=1/r$, this becomes $k^{-1}\sqrt{du^2+u^2d\theta^2}$, the [arc length](riemannian-geometry.md#arc-length) in [Euclidean space](functional-analysis.md#euclidean-norm) divided by $k$. Thus a shortest travel-time route corresponds to a straight [line segment](mathematical-optimization.md#line-segment) in the inverted plane, whenever that segment avoids the origin and lies in the allowed region. Between $(a,0)$ and $(0,a)$ the inverted segment has equation $u(\cos\theta+\sin\theta)=1/a$. The route is $r=a(\cos\theta+\sin\theta)$, and its minimum travel time is $\sqrt2/(ka)$. The [triangle inequality](topological-analysis.md#triangle-inequality) for [arc length](riemannian-geometry.md#arc-length) proves global minimality.

## Gamma-convergence

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

A sequence of functionals Gamma-converges in a specified [topology](topology.md) when every convergent $u_n\to u$ satisfies $F(u)\le\liminf_nF_n(u_n)$, and each $u$ has a recovery sequence $u_n\to u$ with $F_n(u_n)\to F(u)$. With appropriate compactness of energy sublevels, limits of approximate global [minimizers](analysis.md#global-minimizer) minimize $F$, and the minimum values converge. This is suited to variational approximation such as the [Ambrosio–Tortorelli approximation](computer-science.md#ambrosio-tortorelli-approximation); it does not describe arbitrary local minima.

## Variational problem

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

A variational problem seeks a stationary point or minimizer of a [functional](#functional) on a specified [function space](functional-analysis.md#function-space). For a symmetric [coercive bilinear form](linear-algebra.md#coercive-bilinear-form) $a$ and bounded [linear functional](linear-algebra.md#linear-functional) $\ell$ on a real [Hilbert space](hilbert-space.md), minimizing $J(v)=a(v,v)/2-\ell(v)$ is equivalent to the [weak formulation](partial-differential-equation.md#weak-formulation) $a(u,v)=\ell(v)$ for every test vector. The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) gives a unique solution, and $J(u+w)-J(u)=a(w,w)/2$ proves unique minimization. Specifying the admissible space and its boundary constraints is part of the problem.

## Direct method in the calculus of variations

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_method_in_the_calculus_of_variations)

The direct method takes a minimizing sequence, extracts a subsequence using compactness, and uses lower semicontinuity to show that its limit attains the infimum.

### Weak lower semicontinuity of convex gradient energies

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

Suppose the domain has finite measure and $F\in C^1$ is convex, with $|F(p)|\leq C(1+|p|^2)$ and $|DF(p)|\leq C(1+|p|)$. The supporting inequality $F(p)\geq F(q)+DF(q)\cdot(p-q)$, integrated with $q=Du$, gives $\int F(Du_k)\geq\int F(Du)+\int DF(Du)\cdot(Du_k-Du)$. The last term tends to zero by weak convergence of the gradients and the fixed $L^2$ test field $DF(Du)$. This proves weak lower semicontinuity without requiring pointwise convergence of gradients.

### Symmetric elliptic Dirichlet energy with a nonpositive potential

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For a bounded domain, bounded symmetric uniformly elliptic $A$, $q\leq0$, and $f\in L^2$, minimizing $J$ on $\psi+H_0^1$ solves $\operatorname{div}(A\nabla u)+qu=f$. The nonnegative quadratic terms are weakly lower semicontinuous, and [Poincaré inequality](sobolev-space.md#poincare-inequality) makes the gradient norm coercive on the zero-boundary part. The first variation gives the weak equation with the forcing sign displayed above. If $q$ is positive, coercivity may fail at a Dirichlet eigenvalue; orthogonality to the homogeneous kernel is then needed for solvability.

### Screened sine-Gordon energy

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For real $f\in L^2(\mathbb R^3)$, this [energy functional](#energy-functional) on $H^1(\mathbb R^3)$ is coercive and attains its minimum by the [direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations). The nonnegative potential term is weakly lower semicontinuous by [local Sobolev compactness gives lower semicontinuity of a nonnegative integral](functional-analysis.md#local-sobolev-compactness-gives-lower-semicontinuity-of-a-nonnegative-integral). Its [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) is $-\Delta u+u+\sin u=f$ in the [weak solution](partial-differential-equation.md#weak-solution) sense. The extra linear restoring term screens the [Sine-Gordon equation](integrable-systems.md#sine-gordon-equation) nonlinearity. The scalar potential $V(s)=s^2/2+1-\cos s$ is convex because $V''(s)=1+\cos s\geq0$; hence any weak critical point is a minimizer. The [elliptic regularity](distribution-theory.md#elliptic-regularity) estimate for $-\Delta+1$, together with $|\sin u|\leq|u|$, gives $u\in H^2$. The [Sobolev inequality](sobolev-space.md#sobolev-inequality) then puts $u$ in $W^{1,6}$, so [Morrey's inequality](sobolev-space.md#morrey-s-inequality) and [uniformly continuous integrable functions vanish at infinity](topological-analysis.md#uniformly-continuous-integrable-functions-vanish-at-infinity) give a continuous representative tending to zero.

#### Failure of the source-size bound for the screened sine-Gordon equation

↑ **Parent:** [Screened sine-Gordon energy](#screened-sine-gordon-energy)

Take $a=3\pi/2$, $L=10$ and $u(x)=a\exp(-|x|^2/L^2)$ on $\mathbb R^3$. Set $f=-\Delta u+u+\sin u$. Both functions are smooth and belong to [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), and $u\in H^1$. The strictly increasing reaction $h(s)=s+\sin s$ has $0\leq h(u)\leq h(a)=a-1$, while

$$
|\Delta u|=\frac{a}{L^2}|4q-6|e^{-q}\leq\frac{6a}{L^2},\qquad q=|x|^2/L^2.
$$

Consequently $\|f\|_\infty\leq a-1+6a/L^2<a=\|u\|_\infty$. This $u$ is a minimizer of the [screened sine-Gordon energy](#screened-sine-gordon-energy): it solves the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) and that energy is convex. Thus even the minimizing and smooth hypotheses do not justify the stronger source-size bound. The appropriate general estimate is [maximum bound for a monotone reaction term](elliptic-boundary-value-problem.md#maximum-bound-for-a-monotone-reaction-term).

### Minimizing sequence

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

A [minimizing sequence](#minimizing-sequence) satisfies $E(u_n)\to\inf E$. [Coercivity](real-analysis.md#coercive-function) bounds an appropriate [sublevel set](calculus.md#sublevel-set), [Compactness](topology.md#compact-space) supplies a [convergent subsequence](real-analysis.md#convergent-subsequence), and [sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity) turns its limit into a [global minimizer](analysis.md#global-minimizer).

### Bounded slope condition

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

Boundary data $g$ satisfy the bounded slope condition with constant $K$ when every boundary point admits affine lower and upper supporting functions of Lipschitz constant at most $K$. Comparison with these barriers gives a global Lipschitz bound for convex variational problems.

### Comparison principle for convex variational integrals

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For suitable convex integral functionals, ordered boundary values of two minimizers imply the same ordering in the domain. Affine minimizers can therefore serve as upper and lower barriers.

## Functional

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functional_(mathematics))

A functional is a [function](function.md) whose inputs are themselves functions, curves, or other elements of a function space.

### Quadratic functional

↑ **Parent:** [Functional](#functional)

A quadratic functional on a real vector space combines a [quadratic form](linear-algebra.md#quadratic-form) $B(v,v)$, a [linear functional](linear-algebra.md#linear-functional) $\ell(v)$ and a constant. If $B$ is a symmetric [bounded bilinear form](linear-algebra.md#bounded-bilinear-form), its [first variation](#first-variation) is $DI(v)[w]=2B(v,w)-2\ell(w)$. For a strictly positive $B$, an existing stationary point is the unique minimizer by the [quadratic variational principle for a symmetric positive operator](hilbert-space.md#quadratic-variational-principle-for-a-symmetric-positive-operator).

### Epigraph

↑ **Parent:** [Functional](#functional)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Epigraph_(mathematics))

The [epigraph](#epigraph) is $\{(u,t):E(u)\leq t\}$. It is a [convex set](mathematical-optimization.md#convex-set) exactly when $E$ is a [convex function](real-analysis.md#convex-function), and is a [sequentially closed set](topology.md#sequentially-closed-set) in the [product topology](geometry-and-topology.md#product-topology) exactly when $E$ is [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity).

### Functional derivative

↑ **Parent:** [Functional](#functional)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functional_derivative)

The functional derivative is defined by the first variation

$$
F[\phi+\epsilon h]-F[\phi]
=\epsilon\int\frac{\delta F}{\delta\phi(x)}h(x),dx+o(\epsilon).
$$

#### Functional chain rule

↑ **Parent:** [Functional derivative](#functional-derivative)

Along a differentiable path of fields $\phi(x,t)$, a differentiable functional obeys

$$
\frac{d}{dt}F[\phi(t)]
=\int dx\,
\frac{\delta F}{\delta\phi(x)}\,
\partial_t\phi(x,t).
$$

Integrating in time expresses the functional change as the line integral of its functional derivative along the path.

### Energy functional

↑ **Parent:** [Functional](#functional)

An energy functional assigns an integral energy to a function. Minimization of a suitable energy is the basis of the [Dirichlet principle](#dirichlet-principle). For the modified Helmholtz equation, a natural example is

$$
E[u]=\int_V\left(|\nabla u|^2+m^2u^2\right)dV.
$$

#### Critical point of an energy functional

↑ **Parent:** [Energy functional](#energy-functional)

A field configuration is critical for an [energy functional](#energy-functional) $E$ if its [first variation](#first-variation) vanishes for every admissible infinitesimal field variation. For $E[\phi]=\int(\tfrac12|\nabla\phi|^2+U(\phi))$, integration by parts against compactly supported variations gives $\delta E=\int(-\Delta\phi+U'(\phi))\delta\phi$, so [stationary field configurations](#critical-point-of-an-energy-functional) satisfy the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) $\Delta\phi=U'(\phi)$. A constrained target instead allows only tangent variations, changing that field equation. Criticality is stationarity, not necessarily energetic stability or a local minimum.

#### p-energy

↑ **Parent:** [Energy functional](#energy-functional)

The p-energy of a Sobolev function is

$$
E_p[u]=\frac1p\int_\Omega|Du|^p\,dx.
$$

Its stationary points under fixed boundary data are weak solutions of the [p-Laplacian equation](partial-differential-equation.md#p-laplacian).

### Lagrangian

↑ **Parent:** [Functional](#functional)

A Lagrangian is a function or density whose stationary integral encodes an extremization problem. In [Lagrangian mechanics](classical-mechanics.md#lagrangian-mechanics) its action gives the equations of motion; in geometry it describes geodesics and minimal surfaces.

In [Lagrangian](quantum-field-theory.md#lagrangian-field-theory), the action integrates such a density over spacetime.

#### Lagrangian function in constrained optimization

↑ **Parent:** [Lagrangian](#lagrangian)

For an objective $f(x)$ with equality constraints $g_i(x)=0$, the Lagrangian function is

$$
L(x,\lambda)=f(x)+\sum_i\lambda_i g_i(x).
$$

### Variation

↑ **Parent:** [Functional](#functional)

A variation of a function $y$ is a one-parameter family $y+\varepsilon\eta$, where $\eta$ satisfies the required [boundary conditions](differential-equation.md#boundary-condition).

#### First variation

↑ **Parent:** [Variation](#variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_variation)

The first variation of a [functional](#functional) $L$ at $y$ in the direction $\eta$ is

$$
\delta L[y;\eta]
=\left.\frac d{d\varepsilon}L[y+\varepsilon\eta]\right|_{\varepsilon=0}.
$$

##### Fundamental lemma of the calculus of variations

↑ **Parent:** [First variation](#first-variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_lemma_of_the_calculus_of_variations)

If a continuous function $f$ satisfies

$$
\int_a^b f(x)\eta(x)\,dx=0
$$

for every smooth compactly supported test function $\eta$, then $f=0$ on $(a,b)$.

## Stationary point

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stationary_point)

A point is stationary for a [differentiable function](analysis.md#differentiable-function) or [functional](#functional) when its first [derivative](calculus.md#derivative) or [first variation](#first-variation) vanishes in every admissible direction.

## Dirichlet principle

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_principle)

Among functions with fixed boundary values, the solution of $\nabla\cdot(\kappa\nabla\phi)=0$ with $\kappa>0$ uniquely minimizes the weighted energy

$$
\int\kappa|\nabla\phi|^2.
$$

### Sharp radial Dirichlet energy inequality

↑ **Parent:** [Dirichlet principle](#dirichlet-principle)

For $g(1)=1$ and finite displayed energy, the angular mode $g(r)\cos\theta$ has [Dirichlet energy](differential-geometry.md#dirichlet-energy) equal to $\pi$ times that integral. The [harmonic function](partial-differential-equation.md#harmonic-function) $r\cos\theta$ minimizes the energy with the same boundary data by the [Dirichlet principle](#dirichlet-principle), giving the bound. Finite energy forces $g(r)\to0$ as $r\to0$: Cauchy–Schwarz bounds changes of $g^2$ by twice the product of the two energy tails, so $g^2$ has a limit, and a nonzero limit would make $\int g^2/r$ divergent. Consequently completing the square gives the exact identity $\int_0^1[rg'^2+g^2/r]=1+\int_0^1r(g'-g/r)^2$. Equality occurs exactly for $g(r)=r$. This identity also covers finite-energy functions whose polar expression is not classically smooth at the centre.

## Optical ray in cylindrical coordinates

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Optical_ray_in_cylindrical_coordinates)

Fermat-type optical paths in cylindrical coordinates extremize refractive index times Euclidean arclength.

### Helical extremal

↑ **Parent:** [Optical ray in cylindrical coordinates](#optical-ray-in-cylindrical-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helical_extremal)

A helical extremal has constant radius and a polar angle linear in axial position.

## Noether theorem

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noether_theorem)

Noether’s theorem associates a conserved quantity to each continuous variational symmetry.

### Noether second theorem

↑ **Parent:** [Noether theorem](#noether-theorem)

Suppose an action is invariant under a local transformation $\delta\Phi_a=R_a\alpha+R_a^\mu\partial_\mu\alpha$ for every compactly supported function $\alpha$. Variation and integration by parts give the off-shell identity

$$
\sum_a\left(\mathcal E_aR_a-\partial_\mu(\mathcal E_aR_a^\mu)\right)\equiv0.
$$

Thus arbitrary local symmetry parameters imply dependencies among the field equations. In [gauge theory](quantum-field-theory.md#gauge-theory), these identities accompany constraints rather than independent physical charges for each function. This complements the conserved-current statement of [Noether theorem](#noether-theorem).

#### Noether identity for abelian scalar gauge symmetry

↑ **Parent:** [Noether second theorem](#noether-second-theorem)

For $\delta A_\mu=\partial_\mu\alpha$, $\delta\phi=-ie\alpha\phi$ and $\delta\phi^*=ie\alpha\phi^*$, [Noether second theorem](#noether-second-theorem) gives

$$
-\partial_\mu\mathcal E_A^\mu-ie\phi\mathcal E_\phi+ie\phi^*\mathcal E_{\phi^*}\equiv0.
$$

This holds without imposing the field equations. On the matter equations it becomes a divergence identity for the electromagnetic equation, expressing compatibility with charge conservation. The Hamiltonian description carries the corresponding [Gauss law constraint in gauge theory](relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory).

### Noether conserved quantity for a mechanical point symmetry

↑ **Parent:** [Noether theorem](#noether-theorem)

If a time-independent [Lagrangian](#lagrangian) $L(q,\dot q)$ is invariant under a one-parameter point transformation with infinitesimal generator $\xi_i=\partial_sQ_i|_{s=0}$, then every Euler-Lagrange trajectory conserves

$$
J=\sum_i\frac{\partial L}{\partial\dot q_i}\xi_i.
$$

## Second variation

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_variation)

The second variation is the quadratic term in a functional's expansion along $u+\varepsilon\eta$; positivity on admissible variations is a local-minimum test.

### Jacobi equation

↑ **Parent:** [Second variation](#second-variation)

The Jacobi equation is the linearization of an [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) about a stationary path. Its solutions describe infinitesimal one-parameter families of stationary paths.

### Conjugate point

↑ **Parent:** [Second variation](#second-variation)

A conjugate point marks a nonzero endpoint-vanishing Jacobi variation and the loss of positive definiteness of the second variation.

For the energy functional of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), this variational condition yields [conjugate points along a geodesic](riemannian-geometry.md#conjugate-points).

#### Multiplicity of a conjugate point

↑ **Parent:** [Conjugate point](#conjugate-point)

Along a nonconstant affinely parametrized [geodesic](riemannian-geometry.md#geodesic), the multiplicity of a [conjugate point](#conjugate-point) at positive time $t_0$ is the dimension of the space of [Jacobi fields](general-relativity.md#jacobi-field) vanishing at both endpoints. The tangential component of such a [Jacobi field](general-relativity.md#jacobi-field) is affine and vanishes at both endpoints, hence is zero. Uniqueness for the [Jacobi field](general-relativity.md#jacobi-field) equation embeds this space into the $(n-1)$-dimensional normal space by $J\mapsto D_tJ(0)$. Thus its dimension is at most $n-1$.

#### Nonpositive sectional curvature excludes conjugate points

↑ **Parent:** [Conjugate point](#conjugate-point)

For a [Jacobi field](general-relativity.md#jacobi-field) along a [geodesic](riemannian-geometry.md#geodesic) with nonpositive [sectional curvature](second-fundamental-form.md#sectional-curvature), the curvature convention with positive round-sphere curvature gives

$$
(|J|^2)''=2|D_tJ|^2-2\langle R(J,\dot\gamma)\dot\gamma,J\rangle\ge0.
$$

Thus $|J|^2$ is nonnegative and convex. If it vanishes at both ends of a segment, convexity forces it to vanish everywhere. No nonzero [Jacobi field](general-relativity.md#jacobi-field) can vanish at both ends, so the segment has no [conjugate points](riemannian-geometry.md#conjugate-points). Only curvature of planes containing the [geodesic](riemannian-geometry.md#geodesic) tangent is needed, and completeness is unnecessary.

### Wirtinger inequality

↑ **Parent:** [Second variation](#second-variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wirtinger_inequality)

For $f(0)=f(T)=0$,

$$
\int_0^T|f'|^2dt\geq\frac{\pi^2}{T^2}\int_0^T|f|^2dt,
$$

with equality for a multiple of $\sin(\pi t/T)$.

#### Periodic Wirtinger inequality

↑ **Parent:** [Wirtinger inequality](#wirtinger-inequality)

If a continuously differentiable $L$-periodic function $f$ has mean zero, then

$$
\int_0^L f(s)^2\,ds
\leq\frac{L^2}{4\pi^2}\int_0^L f'(s)^2\,ds.
$$

Equality holds exactly for $f(s)=A\cos(2\pi s/L)+B\sin(2\pi s/L)$.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4.md#16b/solution)
