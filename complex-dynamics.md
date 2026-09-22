# Complex dynamics

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_dynamics)

Complex dynamics studies iteration of holomorphic and rational maps, especially the division of the Riemann sphere into stable Fatou behavior and chaotic Julia behavior.

**Table of contents**

- [Holomorphic conjugacy](#holomorphic-conjugacy)
  - [Möbius conjugacy](#mobius-conjugacy)
- [Completely invariant set of a rational map](#completely-invariant-set-of-a-rational-map)
- [Periodic point](#periodic-point)
  - [Cycle of a holomorphic map](#cycle-of-a-holomorphic-map)
  - [Repelling periodic point](#repelling-periodic-point)
  - [Attracting periodic point](#attracting-periodic-point)
    - [Superattracting periodic point](#superattracting-periodic-point)
- [Mandelbrot set](#mandelbrot-set)
  - [Period-two bulb of the Mandelbrot set](#period-two-bulb-of-the-mandelbrot-set)
  - [Main cardioid of the Mandelbrot set](#main-cardioid-of-the-mandelbrot-set)
- [Normal family](#normal-family)
  - [Pointwise anchoring of a holomorphic normal family](#pointwise-anchoring-of-a-holomorphic-normal-family)
  - [Normality is a local property](#normality-is-a-local-property)
  - [Normal-family proof of angular boundary convergence](#normal-family-proof-of-angular-boundary-convergence)
  - [Montel's theorem](#montel-s-theorem)
- [Fatou set](#fatou-set)
  - [Fatou component](#fatou-component)
    - [Herman ring](#herman-ring)
    - [Siegel disc](#siegel-disc)
    - [Fatou component containing an entire fiber is completely invariant](#fatou-component-containing-an-entire-fiber-is-completely-invariant)
  - [Fixed Fatou component classification](#fixed-fatou-component-classification)
    - [Attracting fixed point attracts a critical point](#attracting-fixed-point-attracts-a-critical-point)
    - [Postcritical set](#postcritical-set)
    - [Parabolic basin](#parabolic-basin)
      - [Parabolic disk for z minus z squared](#parabolic-disk-for-z-minus-z-squared)
    - [No-wandering-domain theorem](#no-wandering-domain-theorem)
- [Julia set](#julia-set)
  - [Commuting rational maps of degree at least two have the same Julia set](#commuting-rational-maps-of-degree-at-least-two-have-the-same-julia-set)
  - [Filled Julia set](#filled-julia-set)
  - [Completely invariant closed set of a rational map](#completely-invariant-closed-set-of-a-rational-map)
  - [Julia set has no isolated points](#julia-set-has-no-isolated-points)
  - [Rational map with Julia set equal to the Riemann sphere](#rational-map-with-julia-set-equal-to-the-riemann-sphere)
  - [Chebyshev polynomial Julia set](#chebyshev-polynomial-julia-set)
- [Böttcher's equation](#bottcher-s-equation)
  - [Böttcher theorem](#bottcher-theorem)
    - [Böttcher coordinate](#bottcher-coordinate)
      - [Escape-rate Green function of a polynomial](#escape-rate-green-function-of-a-polynomial)
        - [Connected Julia set criterion for a polynomial](#connected-julia-set-criterion-for-a-polynomial)
      - [Mandelbrot set connectedness from the parameter Böttcher coordinate](#mandelbrot-set-connectedness-from-the-parameter-bottcher-coordinate)
- [Holomorphic fixed-point index](#holomorphic-fixed-point-index)
  - [Multiplier relation for three distinct fixed points of a quadratic rational map](#multiplier-relation-for-three-distinct-fixed-points-of-a-quadratic-rational-map)
- [Parabolic cycle](#parabolic-cycle)
- [Hyperbolic component](#hyperbolic-component)
  - [Parabolic periods in the quadratic family](#parabolic-periods-in-the-quadratic-family)

## Holomorphic conjugacy

↑ **Parent:** [Complex dynamics](complex-dynamics.md)

Holomorphic maps $R$ and $S$ are holomorphically conjugate if a biholomorphic coordinate change $h$ satisfies $h\circ R=S\circ h$. Iterating gives $h\circ R^n=S^n\circ h$, so periodic points and their exact periods correspond. Differentiating at a periodic point gives equality of return multipliers, since the nonzero derivative of $h$ cancels. Locally uniform convergence and normality transfer through the coordinate change, so it also transports [Fatou sets](#fatou-set) and [Julia sets](#julia-set). Between entire Riemann spheres the biholomorphic change is a [Möbius transformation](group-theory.md#mobius-transformation); an affine change is sufficient for many polynomial normalizations.

<h3 id="mobius-conjugacy">Möbius conjugacy</h3>

↑ **Parent:** [Holomorphic conjugacy](#holomorphic-conjugacy)

Two rational sphere maps are Möbius conjugate if $S=h\circ R\circ h^{-1}$ for a [Möbius transformation](group-theory.md#mobius-transformation) $h$. This is precisely global [holomorphic conjugacy](#holomorphic-conjugacy) between Riemann-sphere self-maps. It preserves degree, [local degrees of a holomorphic map](complex-analysis.md#local-degree-of-a-holomorphic-map), exact periods and return [periodic-orbit multipliers](dynamical-systems.md#multiplier-of-a-periodic-orbit-of-an-iteration), and transports the [Fatou set](#fatou-set) and [Julia set](#julia-set) by $h$. Since a Möbius map and its inverse are Lipschitz on the [compact](topology.md#compact-space) sphere, this last assertion follows directly from [equicontinuity](topological-analysis.md#equicontinuity) of the iterate families. An affine [holomorphic conjugacy](#holomorphic-conjugacy) is the special case where $h$ fixes infinity.

## Completely invariant set of a rational map

↑ **Parent:** [Complex dynamics](complex-dynamics.md)

A subset $E$ is completely invariant for a rational map if $R(E)=E=R^{-1}(E)$. This asserts invariance in both directions, including every preimage, rather than just invariance of one chosen inverse branch. For a nonconstant sphere map, the two inclusions $R(E)\subseteq E$ and $R^{-1}(E)\subseteq E$ already imply the equalities, because the map is surjective. The [Fatou set](#fatou-set) and [Julia set](#julia-set) are completely invariant. A [Fatou component](#fatou-component) need not itself be completely invariant even though the union of all components is.

## Periodic point

↑ **Parent:** [Complex dynamics](complex-dynamics.md)

A point $p$ is periodic for an iterated map $R$ if $R^n(p)=p$ for some positive integer $n$. Its exact period is the least such $n$, and the distinct points $p,R(p),\ldots,R^{n-1}(p)$ form its periodic orbit. For a holomorphic map its [periodic-orbit multiplier](dynamical-systems.md#multiplier-of-a-periodic-orbit-of-an-iteration) is $(R^n)'(p)$, computed in a local coordinate; at infinity use a reciprocal coordinate. The chain rule makes this the cyclic product of derivatives along the orbit, so it is the same at every point of that orbit.

### Cycle of a holomorphic map

↑ **Parent:** [Periodic point](#periodic-point)

An exact $n$-cycle consists of $n$ distinct points $w_0,\ldots,w_{n-1}$ with $R(w_j)=w_{j+1}$, indices read modulo $n$. Every point has exact period $n$. The return multiplier is $\prod_{j=0}^{n-1}R'(w_j)$, computed in local charts if necessary; cyclically changing the starting point leaves it unchanged. Thus an attracting, superattracting or repelling return is of the same type at every point of the cycle. If a period-$n$ root coincides with a lower-period point at a parameter limit, multiplicity in the equation $R^n(z)=z$ need not represent distinct points of an exact cycle.

### Repelling periodic point

↑ **Parent:** [Periodic point](#periodic-point)

A holomorphic periodic point is repelling when its return multiplier has modulus greater than one. It belongs to the [Julia set](#julia-set): if the iterates were normal near it, a subsequence of the return iterates, all fixing the point, would converge locally uniformly in the spherical metric. Near their fixed finite value the limit lies in a finite coordinate chart, so Cauchy's derivative estimate would bound their derivatives at the point. Those derivatives are the successive powers of the multiplier and are unbounded. The same argument in a reciprocal coordinate handles infinity.

### Attracting periodic point

↑ **Parent:** [Periodic point](#periodic-point)

A holomorphic periodic point is attracting when its return multiplier has modulus strictly less than one. For the return map $G=R^n$, choose a local coordinate at the fixed point and a number $q$ strictly between $|G'(p)|$ and one. Taylor expansion gives $|G(z)-p|\leq q|z-p|$ on a sufficiently small disc. It maps that disc into itself, and successive returns converge uniformly to $p$ there. Composing with the finitely many intervening maps gives locally uniform convergence to the periodic orbit and places its basin in the [Fatou set](#fatou-set).

#### Superattracting periodic point

↑ **Parent:** [Attracting periodic point](#attracting-periodic-point)

A holomorphic periodic point is superattracting if its return multiplier is zero. The return map then has local expansion $G(p+u)=p+a u^e+O(u^{e+1})$ with $e\geq2$. This implies a strict contraction on a sufficiently small disc and rapid convergence of returns. Infinity is superattracting for every polynomial of degree at least two: the reciprocal-coordinate return has a zero of order equal to the polynomial degree.

## Mandelbrot set

↑ **Parent:** [Complex dynamics](complex-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mandelbrot_set)

For $f_c(z)=z^2+c$, the Mandelbrot set is $\mathcal M=\{c:\{f_c^n(0)\}_{n\geq0}\text{ is bounded}\}$. Thus it records the nonescaping finite critical orbit. The [connected Julia set criterion for a polynomial](#connected-julia-set-criterion-for-a-polynomial) says that the corresponding [filled Julia set](#filled-julia-set) is connected exactly for these quadratic parameters. Parameters with an attracting fixed point form the main cardioid: its multiplier $\lambda$ gives the fixed point $\lambda/2$ and parameter $c=\lambda/2-\lambda^2/4$, with $|\lambda|<1$. Its boundary has a cusp at $c=1/4$. There the critical orbit increases along the real interval to the parabolic fixed point $1/2$, so the cusp belongs to the set. The real section extends from $-2$ to $1/4$; the familiar period-two bulb is attached at $-3/4$.

### Period-two bulb of the Mandelbrot set

↑ **Parent:** [Mandelbrot set](#mandelbrot-set)

The period-two bulb is the open disc $|c+1|<1/4$ of quadratic parameters with an attracting exact two-cycle. The points in that cycle are roots of $z^2+z+c+1$, whose product is $c+1$. Its multiplier is therefore $4(c+1)$, giving precisely the disc inequality. At $c=-3/4$ the two roots merge into the fixed point $-1/2$, whose original multiplier is minus one; the second iterate has multiplier one and a triple fixed-point root. This boundary point is the attachment to the [main cardioid](#main-cardioid-of-the-mandelbrot-set).

### Main cardioid of the Mandelbrot set

↑ **Parent:** [Mandelbrot set](#mandelbrot-set)

The main cardioid consists of quadratic parameters with an attracting fixed point. If that fixed point has multiplier $\lambda$, then it is $\lambda/2$ and $c=\lambda/2-\lambda^2/4$, $|\lambda|<1$. The map is injective on the open unit disc: equality of two parameter values forces either equal multipliers or their sum to be two, impossible for distinct interior multipliers. Its boundary is the cardioid obtained from $\lambda=e^{it}$. At $\lambda=1$ the parameter derivative vanishes, giving the cusp $c=1/4$. Parameters just to the real right of that cusp have monotonically escaping critical orbits, while the cusp's critical orbit tends to $1/2$, so it is on the [Mandelbrot set](#mandelbrot-set) boundary.

## Normal family

↑ **Parent:** [Complex dynamics](complex-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_family)

A family of holomorphic or meromorphic maps is normal when every sequence has a subsequence converging locally uniformly in the spherical metric, possibly to infinity.

### Pointwise anchoring of a holomorphic normal family

↑ **Parent:** [Normal family](#normal-family)

For a holomorphic [normal family](#normal-family), limits are holomorphic or identically infinity. A uniform bound at one interior point excludes infinity on its [connected](geometry-and-topology.md#connected-space) domain. Every sequence therefore has a finite locally uniform subsequential limit. The [Cauchy integral formula](analysis.md#cauchy-integral-formula) makes the [derivatives](calculus.md#derivative) converge locally uniformly too, so the [derivative](calculus.md#derivative) family is normal. Without the point bound this can fail: $n(1+z^2/2)$ tends uniformly to infinity on the unit disk, whereas its [derivatives](calculus.md#derivative) $nz$ are not normal at zero.

### Normality is a local property

↑ **Parent:** [Normal family](#normal-family)

Choose a countable cover by [connected](geometry-and-topology.md#connected-space) disks on which a family is normal. From any sequence extract successive subsequences converging on each disk and use the diagonal sequence. The limits agree on overlaps; a finite holomorphic limit and infinity cannot agree on a nonempty overlap. Connectedness therefore gives one global type of limit, and finite [compact](topology.md#compact-space) subcovers give [locally uniform convergence](real-analysis.md#locally-uniform-convergence). This proves normality of the family on the whole domain from normality near every point.

### Normal-family proof of angular boundary convergence

↑ **Parent:** [Normal family](#normal-family)

If a bounded [holomorphic function](complex-analysis.md#holomorphic-function) $g$ on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) has $g(iy)\to\ell$ as $y\downarrow0$, the rescaled functions $g(z/n)$ form a [normal family](#normal-family). Every subsequential limit equals $\ell$ on the imaginary axis, hence everywhere by the [identity theorem for holomorphic functions](complex-analysis.md#identity-theorem). The entire sequence converges locally uniformly to $\ell$. For a nontangential sequence $z_j=x_j+iy_j\to0$, put $n_j=\lfloor1/y_j\rfloor$; then $n_jz_j$ remains in a fixed compact subset of the half-plane. This gives $g(z_j)\to\ell$. The bounded example $e^{-i/z}$ shows that unrestricted boundary convergence can fail.

// Destination: analysis.bigb

<h3 id="montel-s-theorem">Montel's theorem</h3>

↑ **Parent:** [Normal family](#normal-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Montel's_theorem)

A family of meromorphic functions on a domain that omits three fixed points of the Riemann sphere is normal. For holomorphic functions with values in the complex plane, omitting two fixed values suffices.

## Fatou set

↑ **Parent:** [Complex dynamics](complex-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fatou_set)

The Fatou set of a rational map is the largest open subset of the Riemann sphere on which its iterates form a [normal family](#normal-family). Its complement is the [Julia set](#julia-set).

### Fatou component

↑ **Parent:** [Fatou set](#fatou-set)

A Fatou component is a connected component of the [Fatou set](#fatou-set) of a rational map. It is open. A rational map sends each Fatou component onto another one: complete invariance of the Fatou set puts it inside the inverse image of the target component; its maximal connectedness makes it one full inverse-image component. Restricting the globally proper sphere map to such a component is proper, since the inverse image of a compact subset intersected with the component is closed in a compact set. Its image is both open and closed in the connected target component, hence the whole target. A component is periodic if some iterate returns it to itself.

#### Herman ring

↑ **Parent:** [Fatou component](#fatou-component)

A Herman ring is a doubly connected periodic [Fatou component](#fatou-component) on which the first-return map is holomorphically conjugate to an irrational rotation of an annulus $r<|w|<1$. Compactness of the circle of rotation factors proves normality of the return iterates, and the finitely many intervening iterates preserve normality. It is the annular rotation-domain counterpart of a [Siegel disc](#siegel-disc).

#### Siegel disc

↑ **Parent:** [Fatou component](#fatou-component)

A Siegel disc is a simply connected periodic [Fatou component](#fatou-component) on which the first-return map is holomorphically conjugate to an irrational rotation of the unit disc: $h\circ R^p\circ h^{-1}(w)=e^{2\pi i\theta}w$, with $\theta\notin\mathbb Q$. Its return iterates are normal because any sequence of rotation factors has a convergent subsequence in the unit circle, giving locally uniform limits after conjugation. The iterates generally do not converge to a constant. This is a rotation domain, illustrating stability without attraction.

#### Fatou component containing an entire fiber is completely invariant

↑ **Parent:** [Fatou component](#fatou-component)

Suppose a [Fatou component](#fatou-component) $U$ satisfies $R(U)\subseteq U$, and some $a\in U$ has $R^{-1}(a)\subseteq U$. Every connected component of $R^{-1}(U)$ maps properly and surjectively to $U$: properness follows by intersecting compact preimages with the relatively closed component; openness and closedness then give surjectivity. Such a component must meet the entire fiber over $a$, which lies in $U$. Since $U$ is itself one inverse-image component, there can be no other. Hence $R^{-1}(U)=U$ and $R(U)=U$, proving complete invariance.

### Fixed Fatou component classification

↑ **Parent:** [Fatou set](#fatou-set)

A periodic Fatou component of a rational map is an immediate attracting basin, an immediate parabolic basin, a Siegel disc, or a Herman ring. Attracting and parabolic basins capture critical orbits, while the boundaries of rotation domains lie in the closure of the postcritical set.

#### Attracting fixed point attracts a critical point

↑ **Parent:** [Fixed Fatou component classification](#fixed-fatou-component-classification)

Every immediate basin of an attracting fixed point of a rational map contains a critical point. Otherwise the map on the basin would be an unbranched covering; lifting it to the unit disc would give an automorphism fixing a point, contradicting strict contraction at the attracting fixed point.

#### Postcritical set

↑ **Parent:** [Fixed Fatou component classification](#fixed-fatou-component-classification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Postcritical_set)

The postcritical set is the closure of the union of the forward orbits of all critical values.

#### Parabolic basin

↑ **Parent:** [Fixed Fatou component classification](#fixed-fatou-component-classification)

A parabolic basin consists of [Fatou components](#fatou-component) whose iterates approach a parabolic periodic orbit.

A parabolic basin consists of points whose iterates converge to a parabolic cycle along a specified attracting direction. Each connected basin component lies in the Fatou set, and its boundary lies in the Julia set.

##### Parabolic disk for z minus z squared

↑ **Parent:** [Parabolic basin](#parabolic-basin)

For $P(z)=z-z^2$, the disc $\Delta=\{|z-1/2|<1/2\}$ corresponds under $w=1/z$ to $\Re w>1$. The transformed map is $T(w)=w+1+1/(w-1)$, so $\Re T(w)>\Re w+1$. Thus $P(\Delta)\subseteq\Delta$ and $|P^n(z)|<1/(n+1)$ there. The [Fatou component](#fatou-component) $U$ containing the disc has $P^n\to0$ locally uniformly by normality and the identity theorem. It is forward invariant. The point $1/4$ in the disc has the entire fiber $\{1/2\}$, so the [Fatou component containing an entire fiber is completely invariant](#fatou-component-containing-an-entire-fiber-is-completely-invariant) criterion gives $P^{-1}(U)=U$. Zero itself is a Julia point: a normal subsequential limit near zero would be zero by the disc limit, but every iterate has derivative one at zero, contradicting derivative convergence.

#### No-wandering-domain theorem

↑ **Parent:** [Fixed Fatou component classification](#fixed-fatou-component-classification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/No-wandering-domain_theorem)

Every Fatou component of a rational map of degree at least two is eventually periodic. Thus the periodic-component classification accounts for the entire Fatou set.

## Julia set

↑ **Parent:** [Complex dynamics](complex-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Julia_set)

The Julia set is the complement of the [Fatou set](#fatou-set). It is nonempty, closed, completely invariant, and perfect for every rational map of degree at least two.

### Commuting rational maps of degree at least two have the same Julia set

↑ **Parent:** [Julia set](#julia-set)

Let $R,S$ commute. On an open set where $\{R^n\}$ is equicontinuous, so is $\{S\circ R^n\}$, by the [rational map is Lipschitz in the chordal metric](complex-analysis.md#rational-map-is-lipschitz-in-the-chordal-metric) bound. Since this equals $\{R^n\circ S\}$, equicontinuity descends through the open map $S$: near $S(x)$ every nearby value has a preimage near $x$, and the corresponding estimates hold for all $n$. Thus $S(F(R))\subseteq F(R)$. A degree-at-least-two Julia set contains at least three points, all omitted by the iterates of $S$ on $F(R)$. The three-value [Montel theorem](#montel-s-theorem) gives $F(R)\subseteq F(S)$. Exchanging the maps proves equality of their Fatou and Julia sets. The degree hypothesis excludes Möbius examples with only one Julia point.

### Filled Julia set

↑ **Parent:** [Julia set](#julia-set)

For a polynomial $P$ of degree at least two, the filled Julia set $K(P)$ consists of the points with bounded forward orbit. Choose an escape radius $B$ so that $|P(z)|>2|z|$ for $|z|>B$. Then $K(P)=\bigcap_{n\geq0}(P^n)^{-1}(\{|z|\leq B\})$ is compact, and its complement is the basin of infinity. On the interior all iterates are bounded by $B$, so they form a [normal family](#normal-family); on the complement they converge locally uniformly to infinity. At a boundary point, normality would give a subsequential limit equal to infinity on an open escaping part and hence identically infinity, contradicting the uniform bound at a nearby point of $K(P)$. Therefore $\partial K(P)=J(P)$.

### Completely invariant closed set of a rational map

↑ **Parent:** [Julia set](#julia-set)

If a closed set $E$ satisfies $f^{-1}(E)=E$ for a rational map of degree at least two, then either $E$ has at most two points and lies in the [Fatou set](#fatou-set), or $J(f)\subseteq E$. The complement omits every point of $E$, so [Montel theorem](#montel-s-theorem) proves normality when $|E|\geq3$.

### Julia set has no isolated points

↑ **Parent:** [Julia set](#julia-set)

The accumulation-point set of $J(f)$ is closed and completely invariant. Applying the classification of completely invariant closed sets shows that it equals $J(f)$; hence the Julia set is perfect.

### Rational map with Julia set equal to the Riemann sphere

↑ **Parent:** [Julia set](#julia-set)

For every $d\geq2$, choose a $d$th root of unity $r\ne1$ with $d|1-r|>1$, put $a=1-r$, and set

$$
f(z)=1-\frac a{z^d}.
$$

Its only critical points are $0$ and infinity, and both land on the repelling fixed point $r$. The postcritically finite map has no possible Fatou component, so its Julia set is the whole sphere.

### Chebyshev polynomial Julia set

↑ **Parent:** [Julia set](#julia-set)

The degree-$d$ Chebyshev polynomial has Julia set the interval $[-1,1]$ after the standard normalization. Its Fatou set is the connected complement of that interval in the Riemann sphere, so it has exactly one Fatou component.

<h2 id="bottcher-s-equation">Böttcher's equation</h2>

↑ **Parent:** [Complex dynamics](complex-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Böttcher's_equation)

[Böttcher's equation](#bottcher-s-equation) asks for a holomorphic coordinate conjugating a map with a superattracting fixed point to a monomial. If $f(z)=az^m+O(z^{m+1})$ with $m\geq2$ and $a\ne0$, a normalized local solution has $\phi(z)=bz+O(z^2)$ with $b^{m-1}=a$. The [Böttcher theorem](#bottcher-theorem) asserts the existence and uniqueness of this local coordinate after choosing $b$.

<h3 id="bottcher-theorem">Böttcher theorem</h3>

↑ **Parent:** [Böttcher's equation](#bottcher-s-equation)

Near a superattracting fixed point, a holomorphic map is conformally conjugate to its leading monomial.

<h4 id="bottcher-coordinate">Böttcher coordinate</h4>

↑ **Parent:** [Böttcher theorem](#bottcher-theorem)

For a degree-$d$ polynomial $f(z)=a_dz^d+\cdots$, the Böttcher coordinate near infinity satisfies

$$
\phi_f(f(z))=\phi_f(z)^d,
\qquad
\phi_f(z)\sim a_d^{1/(d-1)}z.
$$

Its modulus extends naturally throughout the basin of infinity.

##### Escape-rate Green function of a polynomial

↑ **Parent:** [Böttcher coordinate](#bottcher-coordinate)

The escape-rate Green function is

$$
G_f(z)=\lim_{n\to\infty}d^{-n}\log^+|f^n(z)|.
$$

It vanishes on the filled Julia set, is positive and harmonic on the basin of infinity, satisfies $G_f\circ f=dG_f$, and equals $\log|\phi_f|$ near infinity and by continuation throughout the basin.

###### Connected Julia set criterion for a polynomial

↑ **Parent:** [Escape-rate Green function of a polynomial](#escape-rate-green-function-of-a-polynomial)

The Julia set of a polynomial is connected exactly when every finite critical point belongs to the filled Julia set. In this case the Böttcher coordinate extends conformally over the entire basin of infinity; an escaping critical point is precisely an obstruction to that continuation.

<h5 id="mandelbrot-set-connectedness-from-the-parameter-bottcher-coordinate">Mandelbrot set connectedness from the parameter Böttcher coordinate</h5>

↑ **Parent:** [Böttcher coordinate](#bottcher-coordinate)

For $f_c(z)=z^2+c$ outside the Mandelbrot set, evaluate the dynamical Böttcher coordinate at the critical value:

$$
\Phi(c)=\phi_c(c).
$$

This parameter Böttcher map is a conformal isomorphism from the complement of the Mandelbrot set to the exterior unit disc, proving that the Mandelbrot set is full and connected.

## Holomorphic fixed-point index

↑ **Parent:** [Complex dynamics](complex-dynamics.md)

The holomorphic fixed-point index is

$$
\iota(f,z_0)=\operatorname*{Res}_{z=z_0}\frac1{z-f(z)}.
$$

At a simple fixed point of multiplier $\lambda\ne1$, it equals $1/(1-\lambda)$. The indices of all fixed points of a rational map, counted appropriately, sum to one.

### Multiplier relation for three distinct fixed points of a quadratic rational map

↑ **Parent:** [Holomorphic fixed-point index](#holomorphic-fixed-point-index)

If a quadratic rational map has three distinct fixed points with multipliers $\lambda_0,\lambda_1,\lambda_2$, then $\lambda_i\lambda_j\ne1$ for $i\ne j$. Otherwise the two corresponding indices already sum to one, contradicting the nonzero third index.

## Parabolic cycle

↑ **Parent:** [Complex dynamics](complex-dynamics.md)

A parabolic cycle is a special kind of [periodic point](#periodic-point) orbit.

A parabolic cycle is a periodic orbit whose multiplier is a root of unity; an iterate then has multiplier one and attracting petals.

## Hyperbolic component

↑ **Parent:** [Complex dynamics](complex-dynamics.md)

For quadratic-polynomial parameter space, these are open components of the interior of the [Mandelbrot set](#mandelbrot-set) with an attracting periodic orbit.

A hyperbolic component in a parameter space consists of maps with a specified attracting cycle. Its multiplier gives a holomorphic coordinate on the component in the quadratic family, and root-of-unity boundary multipliers give parabolic parameters.

### Parabolic periods in the quadratic family

↑ **Parent:** [Hyperbolic component](#hyperbolic-component)

For every prime $p$, the polynomial $f_c^p(0)$ has a nonzero root, giving a superattracting cycle of exact period $p$. Moving in its hyperbolic component to a boundary point with cycle multiplier $-1$ gives a parabolic cycle of exact period $p$. Thus the set of parabolic periods in the quadratic family is infinite.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
