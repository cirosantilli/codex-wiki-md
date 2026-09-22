# Paper 86

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper86.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper86.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $f$ be [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on a neighborhood of the closure of a bounded region with piecewise smooth positively oriented boundary, with no boundary zeros and with $f$ not identically zero. The [argument principle](../../../complex-analysis.md#argument-principle) states

$$
\boxed{\frac1{2\pi i}\int_{\partial G}\frac{f'(z)}{f(z)}\,dz=\sum_{a\in G:f(a)=0}m_a,}
$$

where $m_a$ is the zero [multiplicity](../../../polynomial.md#multiplicity-mathematics). More generally a closed contour avoiding the zeros gives $\sum_a m_a\operatorname{Ind}(\Gamma,a)$, and the integral is the [winding number](../../../complex-analysis.md#winding-number) of $f\circ\Gamma$ about zero.

To prove it, factor near a zero $a$ as $f(z)=(z-a)^{m_a}h(z)$ with $h(a)\ne0$. Then $f'/f=m_a/(z-a)+h'/h$. Remove small disjoint circles about the finitely many zeros in the region. On the remainder $f'/f$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point), so the [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) reduces the boundary integral to the sum of the small-circle integrals. Each is $2\pi i m_a$ because $h'/h$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on its small disc. This proves the formula. Along a contour, the imaginary part of $d\log f$ is the change in a continuous argument, giving the winding interpretation and the indexed version.

Now choose a closed disc $\overline{D(z_0,r)}\subset\Omega$ on which $z_0$ is the only zero of the nonconstant limit $f$. Its boundary has $\min|f|>0$. [Local uniform convergence](../../../real-analysis.md#locally-uniform-convergence) gives $\max|f_n-f|<\min|f|$ there for all sufficiently large $n$. The contour functions $f+t(f_n-f)$, $0\le t\le1$, have no boundary zero. Their [winding numbers](../../../complex-analysis.md#winding-number) are constant under this homotopy, so the [argument principle](../../../complex-analysis.md#argument-principle) shows that $f_n$ has exactly the same positive number $m$ of zeros, counted with [multiplicity](../../../polynomial.md#multiplicity-mathematics), inside the disc. This is the [Rouche theorem](../../../complex-analysis.md#rouche-s-theorem) argument, here derived from the contour count.

Choose a zero $z_n$ in that disc. For every $0<\epsilon<r$, the compact annulus $\epsilon\le|z-z_0|\le r$ contains no zero of $f$, so [uniform convergence](../../../real-analysis.md#uniform-convergence) makes $f_n$ nonzero on it eventually. Therefore all of the chosen zeros eventually lie within $\epsilon$ of $z_0$. Consequently

$$
\boxed{f_n(z_n)=0,\qquad z_n\longrightarrow z_0.}
$$

The maps $f_n$ are eventually not identically zero, since they converge at any fixed point where $f$ is nonzero; thus their zero counts above are legitimate.

A double zero need not persist as a double zero. On the [unit disc](../../../topology.md#unit-disc) take $f(z)=z^2$, $f_n(z)=z^2+1/n$. Its zeros $\pm i/\sqrt n$ converge to zero but are simple, while $f_n'$ vanishes only at zero and $f_n(0)=1/n\ne0$. Hence **the additional simultaneous [derivative](../../../calculus.md#derivative) condition cannot always be imposed**. [Local uniform convergence](../../../real-analysis.md#locally-uniform-convergence) preserves total nearby [multiplicity](../../../polynomial.md#multiplicity-mathematics), not its concentration at a single point.

## 2

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the curvature-minus-one normalization of the [hyperbolic metric](../../../geometry-and-topology.md#hyperbolic-metric):

$$
\boxed{ds_{\mathbb D}=\lambda(z)|dz|,\qquad\lambda(z)=\frac2{1-|z|^2}.}
$$

The associated distance is $d(z,w)=2\operatorname{artanh}|(z-w)/(1-\overline wz)|$. A connected [Riemann surface](../../../complex-analysis.md#riemann-surfaces) has its complete canonical [Poincare metric on a Riemann surface](../../../geometry-and-topology.md#poincare-metric-on-a-riemann-surface) precisely when its [universal cover](../../../algebraic-topology.md#universal-cover) is conformally the [unit disc](../../../topology.md#unit-disc). By the [uniformization theorem](../../../complex-analysis.md#uniformization-theorem), the other [simply connected](../../../algebraic-topology.md#simply-connected-space) covering types are the complex plane and [Riemann sphere](../../../complex-analysis.md#riemann-sphere). Disc automorphisms preserve $\lambda(z)|dz|$, as direct differentiation of $(z-a)/(1-\overline az)$ shows; therefore the metric descends through the deck group. This is the uniformization notion of hyperbolicity, not the different potential-theoretic Green-function classification.

First prove the needed [Schwarz lemma](../../../analysis.md#schwarz-lemma). If $F:\mathbb D\to\mathbb D$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) and $F(0)=0$, then $F(z)/z$ extends holomorphically at zero. On $|z|=r<1$ its modulus is at most $1/r$. The [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) and $r\uparrow1$ give $|F(z)|\le|z|$ and $|F'(0)|\le1$.

Write $\psi_a(z)=(z-a)/(1-\overline az)$. Conjugating $f$ by the source and target disc automorphisms, $\psi_{f(a)}\circ f\circ\psi_a^{-1}$ fixes zero. Applying the [derivative](../../../calculus.md#derivative) bound gives

$$
\boxed{\frac{|f'(a)|}{1-|f(a)|^2}\le\frac1{1-|a|^2},\qquad f^*ds_{\mathbb D}\le ds_{\mathbb D}.}
$$

Integrate along any piecewise smooth path and then take the infimum of lengths: $d(f(z),f(w))\le d(z,w)$. This proves the [Schwarz-Pick theorem](../../../analysis.md#schwarz-pick-theorem). Contraction means nonexpansion, not a uniform Lipschitz constant strictly smaller than one; automorphisms preserve all distances.

If both $R$ and $S$ have disc universal covers, lift $g\circ\pi_R$ to $\widetilde g:\mathbb D\to\mathbb D$ through $\pi_S$. The disc is [simply connected](../../../algebraic-topology.md#simply-connected-space), so the lift exists, and it is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) because the [covering maps](../../../algebraic-topology.md#covering-space) are local [biholomorphisms](../../../complex-analysis.md#biholomorphism). Both [covering maps](../../../algebraic-topology.md#covering-space) are local hyperbolic isometries. The disc contraction therefore descends to $g^*ds_S\le ds_R$ and, by the path-length argument, $d_S(g(p),g(q))\le d_R(p,q)$. If only $S$ is known to have a [hyperbolic metric](../../../geometry-and-topology.md#hyperbolic-metric), a nonconstant $g$ forces $R$ to have one too: otherwise lift from the plane or sphere [universal cover](../../../algebraic-topology.md#universal-cover) of $R$ to the disc cover of $S$. A bounded entire function is constant by the [Liouville theorem](../../../complex-analysis.md#liouville-theorem), and a [holomorphic map](../../../complex-analysis.md#holomorphic-map) from the compact sphere into the disc is constant by the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle). Thus **a nonconstant map into a hyperbolic surface is distance-nonincreasing between the canonical hyperbolic metrics; a nonhyperbolic source admits only constant such maps**.

For the prescribed point, [Schwarz-Pick theorem](../../../analysis.md#schwarz-pick-theorem) gives $|\psi_{w_0}(f(z))|\le|\psi_{z_0}(z)|$. Therefore

$$
h(z)=\frac{\psi_{w_0}(f(z))}{\psi_{z_0}(z)}
$$

is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) after filling the [removable singularity](../../../isolated-singularity.md#removable-singularity) at $z_0$, and $|h|\le1$. Inverting the target automorphism proves

$$
\boxed{f(z)=\frac{(z-z_0)h(z)+w_0(1-\overline z_0z)}{\overline w_0(z-z_0)h(z)+(1-\overline z_0z)},\qquad\sup_{\mathbb D}|h|\le1.}
$$

Conversely every [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) $h$ with this bound gives an admissible disc map: $|\psi_{z_0}(z)h(z)|<1$, its inverse target automorphism remains in the disc, and the denominator cannot vanish.

Fix $z$ and put $r=|\psi_{z_0}(z)|<1$. The possible intermediate values fill $|v|\le r$, since constant choices $h\equiv c$, $|c|\le1$, attain them all. Thus the [one-point value region of a holomorphic disc map](../../../analysis.md#one-point-value-region-of-a-holomorphic-disc-map) is $|\psi_{w_0}(w)|\le r$. Completing the square in $|w-w_0|^2\le r^2|1-\overline w_0w|^2$ gives its Euclidean centre and radius:

$$
\boxed{C=\frac{(1-r^2)w_0}{1-r^2|w_0|^2},\qquad s=\frac{r(1-|w_0|^2)}{1-r^2|w_0|^2}.}
$$

This closed disc lies strictly inside the [unit disc](../../../topology.md#unit-disc) because $r<1$. For $z=z_0$ it degenerates to the single point $w_0$. Its boundary is attainable by unimodular constant $h$; requiring $f$ to map into the open disc does not remove that boundary.

## 3

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a nonconstant [meromorphic](../../../isolated-singularity.md#meromorphic-function) map, write $T_f(R)=m(R,f)+N(R;\infty)$ in the usual normalization, where $m=(2\pi)^{-1}\int\log^+|f(Re^{i\theta})|\,d\theta$. Let $N(R;a)$ count $a$-points with their local degrees, and let $\overline N(R;a)$ count each distinct point once, using the same integrated logarithmic weights. At infinity the local degree is the [pole](../../../isolated-singularity.md#pole) order. The [Nevanlinna deficiency](../../../isolated-singularity.md#nevanlinna-deficiency) and [Nevanlinna ramification index](../../../isolated-singularity.md#nevanlinna-ramification-index) are

$$
\boxed{\delta_f(a)=1-\limsup_{R\to\infty}\frac{N(R;a)}{T_f(R)},\qquad
\theta_f(a)=\liminf_{R\to\infty}\frac{N(R;a)-\overline N(R;a)}{T_f(R)}.}
$$

The latter is an asymptotic excess-multiplicity index, not the integer local ramification degree. The [Nevanlinna first main theorem](../../../isolated-singularity.md#nevanlinna-first-main-theorem) gives $N(R;a)\le T_f(R)+O(1)$ and identifies deficiency with the lower limiting normalized proximity. The target $a$ ranges over the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), not just the real line.

The exponential is entire and has no [poles](../../../isolated-singularity.md#pole). Consequently

$$
T_e(R)=\frac1{2\pi}\int_0^{2\pi}\max(0,R\cos\theta)\,d\theta
=\boxed{\frac R\pi}.
$$

Thus $c=1/\pi$ in this normalization.

To obtain the rational-composition growth, represent the nonconstant degree-$d$ sphere map by relatively prime homogeneous [polynomials](../../../polynomial.md) $(P,Q)$ of degree $d$. Their joint norm on the unit sphere in $\mathbb C^2$ has a positive minimum and finite maximum: simultaneous vanishing would contradict relative primeness on the projective line. Homogeneity therefore gives constants $0<A\le B<\infty$ with

$$
A\|(w,s)\|^d\le\|(P(w,s),Q(w,s))\|\le B\|(w,s)\|^d.
$$

Apply this to the entire nonvanishing lift $(e^z,1)$. The logarithmic joint norm differs from $d\log\|(e^z,1)\|$ by a bounded function. Its circular mean minus the value at zero is the spherical characteristic. It differs from the ordinary characteristic by $O(1)$: [Jensen's formula](../../../complex-analysis.md#jensen-s-formula) applied to the entire denominator counts its zeros, while

$$
0\le\tfrac12\log(1+x^2)-\log^+x\le\tfrac12\log2
$$

controls the proximity replacement. If the denominator vanishes at zero, factor its zero and use its leading coefficient in [Jensen's formula](../../../complex-analysis.md#jensen-s-formula); the discrepancy is still a basepoint-dependent constant. This proves the [rational composition law for the Nevanlinna characteristic](../../../isolated-singularity.md#rational-composition-law-for-the-nevanlinna-characteristic) here and gives

$$
\boxed{T_{U\circ e}(R)=\frac d\pi R+O(1)\sim\frac d\pi R.}
$$

If $U$ is constant, $d=0$ and its characteristic is bounded instead.

For a simultaneous nonzero deficiency and ramification example choose

$$
f(z)=e^z(e^z-1)^2,
$$

a degree-three [polynomial](../../../polynomial.md) composed with the exponential. Its characteristic is $3R/\pi+O(1)$. Its only zeros are $2\pi i n$, $n\in\mathbb Z$, all of [multiplicity](../../../polynomial.md#multiplicity-mathematics) two. The number of distinct such points in a large disc is $R/\pi+O(1)$, so integration of their count gives

$$
\overline N(R;0)=R/\pi+O(\log R),\qquad N(R;0)=2R/\pi+O(\log R).
$$

The origin contribution is handled by its usual logarithmic counting term. Therefore

$$
\boxed{\delta_f(0)=\tfrac13,\qquad\theta_f(0)=\tfrac13.}
$$

This is [simultaneous deficiency and ramification for an exponential polynomial](../../../isolated-singularity.md#simultaneous-deficiency-and-ramification-for-an-exponential-polynomial): the missing exponential value contributes a deficit, while the attained value is attained with double [multiplicity](../../../polynomial.md#multiplicity-mathematics).

## 4

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [growth order of a meromorphic function](../../../isolated-singularity.md#growth-order-of-a-meromorphic-function) is

$$
\rho(f)=\limsup_{R\to\infty}\frac{\log^+T_f(R)}{\log R}.
$$

The order of the integrated count is defined analogously using $\log^+N(R;a)$, with an identically zero count assigned order zero. Constants have function order zero. These are growth orders, not local zero or [pole](../../../isolated-singularity.md#pole) orders. For nonconstant $f$, the first main theorem gives $\rho(N(\cdot;a))\le\rho(f)$ for every target.

Use the truncated [Nevanlinna second main theorem](../../../isolated-singularity.md#nevanlinna-second-main-theorem) in the following standard form: for distinct fixed targets $a_1,\ldots,a_q$,

$$
(q-2)T_f(R)\le\sum_{j=1}^q\overline N(R;a_j)+S_f(R),\qquad
S_f=O(\log^+T_f+\log R),
$$

outside an exceptional set of radii of finite linear measure. For finite order the error is $O(\log R)$; replacing each truncated count by its full count preserves the inequality.

Suppose $0<\rho(f)<\infty$ and three targets have counting orders below $\rho(f)$. Choose $\mu$ strictly between the maximum of their three orders and $\rho(f)$. Each full count is at most $R^\mu$ eventually. The theorem with $q=3$ then gives $T_f(R)\le C R^\mu$ for sufficiently large radii outside the exceptional set. Its tail measure is eventually less than one, so every interval $[R,R+1]$ contains a nonexceptional radius $R'$. Monotonicity of the characteristic yields $T_f(R)\le T_f(R')\le C(R+1)^\mu$ for all large $R$. This contradicts its order. If $\rho(f)=0$, all the counting orders are already zero. Hence the [counting-order exceptions for a finite-order meromorphic function](../../../isolated-singularity.md#counting-order-exceptions-for-a-finite-order-meromorphic-function) satisfy

$$
\boxed{\rho(N(\cdot;a))=\rho(f)\quad\text{apart from at most two targets}.}
$$

The exponential has order one but omits both zero and infinity, so those two counts are zero; this realizes two exceptions.

For a [Möbius map](../../../group-theory.md#mobius-transformation) $U(w)=(aw+b)/(cw+d)$ with $ad-bc\ne0$, translation and multiplication by a nonzero constant change $T$ by $O(1)$, as follows directly from the proximity inequalities and unchanged [pole](../../../isolated-singularity.md#pole) multiplicities. The first main theorem also gives $T(1/h)=T(h)+O(1)$. If $c=0$, $U$ is affine. If $c\ne0$, write $U(w)=a/c+K/(cw+d)$ with $K\ne0$ and use these three elementary operations. Thus $T_{U\circ f}=T_f+O(1)$, proving

$$
\boxed{\rho(U\circ f)=\rho(f).}
$$

For the sum, a [pole](../../../isolated-singularity.md#pole) of $f_1+f_2$ has order no larger than the sum of the two [pole](../../../isolated-singularity.md#pole) orders, and

$$
\log^+|f_1+f_2|\le\log2+\log^+|f_1|+\log^+|f_2|.
$$

Therefore $T_{f_1+f_2}\le T_{f_1}+T_{f_2}+O(1)$ and

$$
\boxed{\rho(f_1+f_2)\le\max(\rho(f_1),\rho(f_2)).}
$$

If $\rho(f_1)>\rho(f_2)$, apply the same inequality to $f_1=(f_1+f_2)-f_2$. It forces $\rho(f_1)\le\max(\rho(f_1+f_2),\rho(f_2))$, hence the sum's order equals $\rho(f_1)$. The reversed case is identical. This reasoning also handles an infinite larger order. For equal orders cancellation can be strict: $f_1=e^z$, $f_2=-e^z$ both have order one, but their sum is zero of order zero.

## 5

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

If $\phi$ is identically zero there are no exceptions. Otherwise choose $x_0$ with $\phi(x_0)>0$ and put $I_+=\{x\ge x_0:\phi'(x)>\phi(x)^2\}$. Monotonicity implies $\phi(x)>0$ thereafter. On this set, $1<\phi'/\phi^2$, whence

$$
|I_+|\le\int_{I_+}\frac{\phi'}{\phi^2}\,dx\le\int_{x_0}^\infty\frac{\phi'}{\phi^2}\,dx
=\frac1{\phi(x_0)}-\lim_{X\to\infty}\frac1{\phi(X)}\le\frac1{\phi(x_0)}.
$$

Adding the finite initial interval $[0,x_0]$ proves

$$
\boxed{\phi'(x)\le\phi(x)^2\quad\text{outside a set of finite measure}.}
$$

This [derivative growth outside a finite-measure set](../../../isolated-singularity.md#derivative-growth-outside-a-finite-measure-set) controls exceptional radii in Nevanlinna estimates. For example let $T_s$ be the smooth spherical characteristic and $A(r)=rT_s'(r)$ its increasing area-counting function. Apply the lemma to $T_s+1$ and $A+1$: outside the union of two finite-measure sets,

$$
A(r)\le r(T_s(r)+1)^2,\qquad A'(r)\le(A(r)+1)^2.
$$

Their logarithms are consequently $O(\log r+\log(T_s+1))$. Such [derivative](../../../calculus.md#derivative)/area bounds in estimates from the [Poisson-Jensen formula](../../../complex-analysis.md#poisson-jensen-formula) give the [Nevanlinna logarithmic derivative lemma](../../../isolated-singularity.md#nevanlinna-logarithmic-derivative-lemma), $m(r,f'/f)=O(\log^+T_f+\log r)$ outside a finite-length set. The second main theorem uses that estimate as its error term. The elementary growth lemma controls that error and its exceptional set; it is not itself a substitute for the analytic estimates.

We use the truncated second main theorem stated in the preceding solution, together with the fact that a transcendental [meromorphic function](../../../isolated-singularity.md#meromorphic-function) has $T_f(r)/\log r\to\infty$. Here is a justification of the latter fact. If there are infinitely many [poles](../../../isolated-singularity.md#pole), fixing any arbitrarily large finite [pole](../../../isolated-singularity.md#pole) count gives $N(r;\infty)\ge A\log r-O_A(1)$. If there are only finitely many [poles](../../../isolated-singularity.md#pole), multiply by a [polynomial](../../../polynomial.md) $p$ removing them to obtain a transcendental entire function $h=pf$. Its [Taylor series](../../../calculus.md#taylor-series) has nonzero coefficients of arbitrarily high degrees $n$. Cauchy's coefficient estimate gives $\log M_h(r/2)\ge n\log r-O_n(1)$; the [subharmonic function](../../../partial-differential-equation.md#subharmonic-function) Poisson estimate gives $\log M_h(r/2)\le3m(r,h)$. Since $T_h\le T_f+O(\log r)$, letting $n$ be arbitrarily large proves the claimed ratio limit. Thus the second-theorem error is $o(T_f)$ along large nonexceptional radii.

Let $N_{\rm simple}(r;a)$ count just the simple $a$-points. A multiple $a$-point of degree $m\ge2$ contributes one to the truncated count and at least two to the full count; a simple point contributes one to each. Hence, with the same positive logarithmic weights for large radii,

$$
\overline N(r;a)\le\tfrac12N(r;a)+\tfrac12N_{\rm simple}(r;a).
$$

If each of the five values had only finitely many simple preimages, each simple counting function would be $O(\log r)$. Summing and using the first main theorem would give $\sum_{j=1}^5\overline N(r;a_j)\le(5/2)T_f+O(\log r)$. But the second theorem requires $3T_f\le\sum\overline N+o(T_f)$, a contradiction. This proves the stronger result [five values force infinitely many simple preimages](../../../isolated-singularity.md#five-values-force-infinitely-many-simple-preimages):

$$
\boxed{\text{At least one of the five values has infinitely many simple preimages.}}
$$

In particular **more than one simple zero is necessary**, but **more than one target with simple zeros is not necessary**.

For the last distinction, take a nonsingular [Weierstrass elliptic function](../../../complex-analysis.md#weierstrass-elliptic-function) scaled so that $\wp'^2=4\wp(\wp-1)(\wp+1)$; it has branch values $-1,0,1,\infty$. These are the [four totally ramified Weierstrass values](../../../complex-analysis.md#four-totally-ramified-weierstrass-values): finite branch preimages have local degree two, and all [poles](../../../isolated-singularity.md#pole) are double. Set

$$
f(z)=\frac1{\wp(z)-2},\qquad
\{a_1,\ldots,a_5\}=\{-\tfrac13,-\tfrac12,-1,0,1\}.
$$

The first four targets are the images of those branch values under the [Möbius transformation](../../../group-theory.md#mobius-transformation). Their preimages remain double; at a lattice [pole](../../../isolated-singularity.md#pole), for example, $f(z)\sim(z-z_*)^2$. The last target corresponds to $\wp=3$, where $\wp'^2=96\ne0$, so every such preimage is simple. The degree-two torus map attains that regular value, and periodicity produces infinitely many preimages in the plane. This nonconstant [elliptic function](../../../complex-analysis.md#elliptic-function) is transcendental because it has infinitely many [poles](../../../isolated-singularity.md#pole). Exactly one of the five selected finite targets therefore has simple preimages.

## 6

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

There are two necessary qualifications to the printed formula. **Critical points satisfy $g'=0$, not $g'=1$.** At a point with $g'=1$, the local degree is one and the printed summand is zero. In addition, $\log\|g'(0)\|$ is finite only when $g'(0)\ne0$; constant maps and origin-critical maps need separate treatment.

These are genuine issues even for otherwise ordinary disc maps. The map $g(z)=(z-1/2)^2/4$ maps the [unit disc](../../../topology.md#unit-disc) into itself and has $g'(0)\ne0$. Its [derivative](../../../calculus.md#derivative) never equals one in the disc, so the printed count is zero, but it has a [ramification point](../../../complex-analysis.md#ramification-point-of-a-holomorphic-map) at $1/2$ of [multiplicity](../../../polynomial.md#multiplicity-mathematics) one. For $R>1/2$ the correct identity has the additional term $\log(2R)$, proving that the displayed identity with the literal printed count is false. Also $g(z)=z^2$ shows the undefined basepoint logarithm in an origin-critical example.

Prove the intended identity first for a nonconstant map with $g'(0)\ne0$. Let $H(z)=2|g'(z)|/(1-|g(z)|^2)$ be its [hyperbolic derivative density](../../../geometry-and-topology.md#hyperbolic-derivative-density) and $u=\log H$. Away from [derivative](../../../calculus.md#derivative) zeros, $\log|g'|$ is harmonic, and direct differentiation gives

$$
\Delta[-\log(1-|g|^2)]=\frac{4|g'|^2}{(1-|g|^2)^2}=H^2.
$$

At a zero $a$ of $g'$ of [multiplicity](../../../polynomial.md#multiplicity-mathematics) $m_a$, factor $g'=(z-a)^{m_a}h$ with $h(a)\ne0$. Its logarithm contains $m_a\log|z-a|$, whose distributional [Laplacian](../../../calculus.md#laplacian) is $2\pi m_a\delta_a$. Thus

$$
\Delta u=H^2+2\pi\sum_{g'(a)=0}m_a\delta_a.
$$

The local map degree is $m_a+1$, so this is the required excess-degree weighting.

For a smooth function, differentiating its circular mean and applying the [divergence theorem](../../../calculus.md#divergence-theorem) gives $\overline u'(r)=(2\pi r)^{-1}\int_{|z|<r}\Delta u\,dA$. Integrating in $r$ gives the logarithmic Green-Jensen formula. Factoring the isolated logarithmic singularities extends it to the present $u$:

$$
\frac1{2\pi}\int_0^{2\pi}u(Re^{i\theta})\,d\theta-u(0)
=\frac1{2\pi}\int_{|z|<R}\log\frac R{|z|}\,\Delta u\,dA.
$$

Substitution yields the [critical-point Jensen identity for the hyperbolic derivative](../../../geometry-and-topology.md#critical-point-jensen-identity-for-the-hyperbolic-derivative)

$$
\boxed{T_{\mathbb D}(R)+N_{\rm crit}(R)=\frac1{2\pi}\int_0^{2\pi}\log H(Re^{i\theta})\,d\theta-\log H(0),}
$$

where $N_{\rm crit}=\sum_{|a|<R:g'(a)=0}m_a\log(R/|a|)$. This is the requested formula with the critical-point typo corrected. Initially choose a circle containing no [ramification point](../../../complex-analysis.md#ramification-point-of-a-holomorphic-map) on its boundary; continuity and integrability of logarithmic boundary singularities extend the result to the remaining radii.

By [Schwarz-Pick theorem](../../../analysis.md#schwarz-pick-theorem), $H(z)\le2/(1-|z|^2)$. Therefore

$$
T_{\mathbb D}(R)+N_{\rm crit}(R)\le\log\frac2{1-R^2}-\log H(0).
$$

The normalized [hyperbolic distance](../../../geometry-and-topology.md#hyperbolic-distance) is $\rho(R)=\log((1+R)/(1-R))$, and

$$
\log\frac2{1-R^2}=\rho(R)+\log2-2\log(1+R)\le\rho(R)+\log2.
$$

Consequently

$$
\boxed{T_{\mathbb D}(R)+N_{\rm crit}(R)\le\rho(R)+\log\frac2{H(0)}.}
$$

One can take $C_1=1$ and $C_2=\log(2/H(0))\ge0$. Since the corrected count is nonnegative in the noncritical-basepoint case, this also proves the growth bound for $T_{\mathbb D}$ with the literal printed, identically zero count, though not its false identity.

For completeness, if $g'$ vanishes to order $m\ge1$ at zero, put $c=\lim_{z\to0}H(z)/|z|^m>0$ and

$$
N_{\rm crit}^{\rm reg}(R)=m\log R+\sum_{0<|a|<R:g'(a)=0}m_a\log(R/|a|).
$$

Apply the same formula to $\log H-m\log|z|$, which is regular at zero. It gives

$$
\boxed{T_{\mathbb D}(R)+N_{\rm crit}^{\rm reg}(R)=\langle\log H\rangle_R-\log c\le\rho(R)+\log(2/c).}
$$

The origin contribution is a regularized Jensen term, not the undefined $\log(R/0)$. If one instead omits the origin term, the upper bound gains $-m\log R$; this is bounded for $R\ge1/2$, while the characteristic and off-origin count are bounded on any smaller compact disc. Thus a bound $C_1\rho+C_2$ still holds for that nonnegative-count convention after enlarging $C_2$. For a constant map $H=0$ and $T_{\mathbb D}=0$, so its characteristic growth bound is trivial; the logarithmic identity and a finite critical-divisor count are not defined. These qualifications resolve all maps allowed by the original opening sentence without asserting an undefined equality.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
