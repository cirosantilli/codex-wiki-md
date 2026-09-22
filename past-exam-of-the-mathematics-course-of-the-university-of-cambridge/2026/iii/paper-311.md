# Paper 311

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20311.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20311.pdf)

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
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Because $U$ is a [null](../../../special-relativity.md#null-vector) tangent, metric compatibility gives

$$
U^aB_{ab}=U^a\nabla_bU_a
=\frac12\nabla_b(U^aU_a)=0.
$$

Because $U$ is tangent to an affinely parametrized [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence),

$$
B_{ab}U^b=U^b\nabla_bU_a=0
$$

by the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation). Thus $B$ has no component along $U$ in either index.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

With $U^2=N^2=0$ and $U\mathbin\cdot N=-1$, define the [screen-space projector](../../../geodesic-congruence.md#screen-space-projector)

$$
\boxed{P^a{}_b=\delta^a_b+U^aN_b+N^aU_b}.
$$

Direct contraction gives $P^a{}_bU^b=P^a{}_bN^b=0$, while a vector orthogonal to both $U$ and $N$ is unchanged. Moreover $P^a{}_cP^c{}_b=P^a{}_b$ and $P^a{}_a=2$, so its image is precisely the two-dimensional transverse space.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Decompose the [optical tensor](../../../geodesic-congruence.md#optical-tensor) on the two-dimensional screen space as

$$
\widehat B_{ab}
=\frac12\theta P_{ab}
+\widehat\sigma_{ab}
+\widehat\omega_{ab}.
$$

The [null expansion](../../../geodesic-congruence.md#null-expansion), [null shear](../../../geodesic-congruence.md#null-shear), and [null twist](../../../geodesic-congruence.md#null-twist) are respectively

$$
\boxed{\theta=P^{ab}\widehat B_{ab}},
\qquad
\boxed{\widehat\sigma_{ab}
=\widehat B_{(ab)}-\frac12\theta P_{ab}},
\qquad
\boxed{\widehat\omega_{ab}=\widehat B_{[ab]}}.
$$

The shear is symmetric and trace-free, while the twist is antisymmetric.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Differentiate $B_{ab}=\nabla_bU_a$ along an affinely parametrized generator. Commuting [covariant derivatives](../../../general-relativity.md#covariant-derivative) and using $\nabla_UU=0$ gives the optical evolution equation

$$
U^c\nabla_cB_{ab}
=-B_{ac}B^c{}_b-R_{acbd}U^cU^d.
$$

Taking its screen trace and using

$$
\widehat B_{ab}\widehat B^{ba}
=\frac12\theta^2
+\widehat\sigma_{ab}\widehat\sigma^{ab}
-\widehat\omega_{ab}\widehat\omega^{ab}
$$

produces the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation)

$$
\frac{d\theta}{d\lambda}
=-\frac12\theta^2
-\widehat\sigma_{ab}\widehat\sigma^{ab}
+\widehat\omega_{ab}\widehat\omega^{ab}
-R_{ab}U^aU^b.
$$

The generators lie in a [null hypersurface](../../../general-relativity.md#null-hypersurface), so they are hypersurface orthogonal. The [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) therefore gives $\widehat\omega_{ab}=0$, leaving

$$
\boxed{
\frac{d\theta}{d\lambda}
=-\frac12\theta^2
-\widehat\sigma_{ab}\widehat\sigma^{ab}
-R_{ab}U^aU^b}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Contracting the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) with the null tangent eliminates the trace term and gives

$$
R_{ab}U^aU^b=8\pi T_{ab}U^aU^b\geq0
$$

by the [null energy condition](../../../general-relativity.md#null-energy-condition). The screen metric is positive definite, so $\widehat\sigma_{ab}\widehat\sigma^{ab}\geq0$. The [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) consequently implies

$$
\frac{d\theta}{d\lambda}\leq-\frac12\theta^2.
$$

While $\theta<0$ this is equivalent to

$$
\frac{d}{d\lambda}\left(\frac1\theta\right)
\geq\frac12.
$$

If $	heta(\lambda_0)=\theta_0<0$, integration gives

$$
\frac1{\theta(\lambda)}
\geq\frac1{\theta_0}+\frac{\lambda-\lambda_0}{2}.
$$

The right-hand side reaches zero after affine distance $2/|\theta_0|$. A finite negative expansion cannot pass through this value, so $	heta\to-\infty$ no later than that point. This is the [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

Choose a coordinate sphere at late conformal time $\eta_0$ and comoving radius $r_0$. Its areal radius is $R=a(\eta)r$, so its area is $A=4\pi a^2r^2$. Future-directed radial null generators have $dr/d\eta=\pm1$. Up to a common positive normalization of their affine tangents, their expansions therefore have the signs of

$$
\frac1A\frac{dA}{d\eta}
=2\left(\frac{a'}a\pm\frac1r\right).
$$

The outgoing sign is positive because $a'>0$. The ingoing sign is also positive whenever

$$
r_0>\frac{a(\eta_0)}{a'(\eta_0)}.
$$

An arbitrarily large sphere exists because the spatial topology is $\mathbb R^3$. Both future null expansions are positive on such a sphere, so it is an [anti-trapped surface](../../../general-relativity.md#anti-trapped-surface).

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

Apply the time-reversed [Penrose singularity theorem](../../../general-relativity.md#penrose-singularity-theorem). The two past-directed null congruences orthogonal to the compact anti-trapped surface have negative expansion. The [null energy condition](../../../general-relativity.md#null-energy-condition), through the [Einstein field equations](../../../general-relativity.md#einstein-field-equations), supplies the null convergence condition, and the [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem) forces each generator to acquire a conjugate point within finite affine length if it can be extended that far.

If every past-directed null generator were complete, the boundary of the causal past of the surface would therefore be generated only for a bounded affine interval. Compactness of the initial surface and continuous dependence of geodesics on initial data would make that achronal boundary compact. A [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime) provides a [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) and a timelike flow projecting the boundary onto it. The standard Penrose argument then makes its image both open and closed, forcing the connected Cauchy hypersurface to be compact. This contradicts its stipulated topology $\mathbb R^3$.

Hence at least one past-directed null generator ends after finite affine parameter: the universe is [null-geodesically incomplete](../../../general-relativity.md#null-geodesic-completeness) to the past. Global hyperbolicity controls the causal boundary, the noncompact spatial topology supplies the contradiction, and the energy condition supplies focusing.

## 2

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The [Penrose diagram](../../../general-relativity.md#penrose-diagram) is the maximally extended Schwarzschild diagram modified by an ingoing null shell from the chosen $\mathcal I^-$. To its past the vacuum mass is $M$; to its future the exterior mass is $M+E$. Draw the shell as a $45^\circ$ ingoing line from the chosen $\mathcal I^-$, crossing the future [event horizon](../../../general-relativity.md#event-horizon) and ending on the future spacelike singularity. In that same exterior, label $i^-$ and $i^+$ at the lower and upper timelike corners, $i^0$ at the spatial corner, and $\mathcal I^-$ and $\mathcal I^+$ as the past and future null boundaries.

The crucial teleological feature is that the final $\mathcal H^+$, traced backward before the shell, lies outside the old $r=2M$ future horizon. It crosses the old past horizon $\mathcal H^-$ at the bifurcation two-sphere and continues into the white-hole region, ending on the past spacelike singularity. Thus the diagram must not draw the relevant $\mathcal H^+$ as beginning at the old bifurcation sphere.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

After the shell, spherical symmetry and stationarity put the horizon at $r=2(M+E)$. Before the shell, an outgoing radial null geodesic in the mass-$M$ region has $r$ linear in an affine parameter. The normalizations $r(0)=2M$ and $r(1)=2(M+E)$ therefore give

$$
r(\lambda)=2M+2E\lambda
\qquad(\lambda<1).
$$

The degenerate intrinsic metric of the horizon has no $d\lambda^2$ term, so

$$
\boxed{
ds^2_{\mathcal H^+}=
\begin{cases}
4(M+E\lambda)^2d\Omega^2,&\lambda<1,\\
4(M+E)^2d\Omega^2,&\lambda>1.
\end{cases}}
$$

The two expressions agree at the shell, $\lambda=1$.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

Tracing the generator backward through the mass-$M$ region gives $r=2(M+E\lambda)$. It reaches the past spacelike singularity when $r=0$, namely at

$$
\lambda=-\frac ME.
$$

The singular endpoint is not part of the spacetime, while the final stationary horizon extends indefinitely to the future. Hence

$$
\boxed{-\frac ME<\lambda<\infty}.
$$

In particular, negative $\lambda$ is physically necessary: that part of the relevant event horizon lies inside the old white-hole region before reaching the old bifurcation sphere at $\lambda=0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $k^a=(d/d\lambda)^a$ be an affine horizon generator, normalized so that the horizon Killing field is $\xi^a=\kappa\lambda k^a$. To first order in the small total injected energy, expansion and shear-squared terms are second order, and the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) on the horizon becomes

$$
\frac{d\theta}{d\lambda}=-8\pi T_{ab}k^ak^b.
$$

The flux of Killing energy through all the shells is

$$
\Delta M
=\int_{\mathcal H^+}T_{ab}\xi^ak^b\,d\lambda\,dA
=\kappa\int\lambda T_{ab}k^ak^b\,d\lambda\,dA.
$$

Substitute the linearized focusing equation and integrate by parts. Stationarity before and after the process makes the endpoint term $\lambda\theta$ vanish, while $dA/d\lambda=\theta A$ to first order. Therefore

$$
\Delta M
=\frac{\kappa}{8\pi}\int\theta\,d\lambda\,dA
=\frac{\kappa}{8\pi}\Delta A.
$$

Using the [Hawking temperature](../../../general-relativity.md#hawking-temperature) $T_H=\kappa/(2\pi)$ and [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy) $S_{BH}=A/4$ gives the [Physical-process first law of black-hole mechanics](../../../general-relativity.md#physical-process-first-law-of-black-hole-mechanics)

$$
\boxed{\Delta M=\frac{\kappa}{8\pi}\Delta A
=T_H\Delta S_{BH}}.
$$

The derivation is linear in the stress tensor, so separated shells simply contribute additively.

## 3

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The four independent [Killing vector fields](../../../general-relativity.md#killing-vector-field) are the stationary field $\partial_t$ and the three generators of spatial rotations on the two-spheres. In the Schwarzschild interior, $f(r)<0$, so

$$
g(\partial_t,\partial_t)=-f(r)>0.
$$

Every rotational Killing field is tangent to the positive-definite round-sphere metric. All four fields are tangent to a surface of constant $r$, whose induced metric

$$
(-f)dt^2+r^2d\Omega^2
$$

is positive definite. Consequently every nonzero linear combination of the Killing fields is spacelike wherever it does not vanish. A pure rotational Killing field can vanish on its rotation axis, but it is nowhere timelike.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Inside the horizon, $g^{ab}\nabla_ar\nabla_br=f<0$, so $\nabla r$ is timelike. The chosen black-hole time orientation declares $-\nabla r$ future directed; therefore every future-directed timelike vector $V$ has $V(r)<0$. Thus $r$ decreases strictly along every future-directed timelike curve.

Write $F=2M/r-1=-f>0$. Along such a curve,

$$
d\tau^2=\frac{dr^2}{F}-Fdt^2-r^2d\Omega^2
\leq\frac{dr^2}{F}.
$$

It cannot remain at any $r>0$ indefinitely, because $r$ is a time function and the displayed bound gives finite remaining proper time. From a starting radius $r_p<2M$,

$$
\tau\leq\int_0^{r_p}\frac{dr}{\sqrt{2M/r-1}}
<\int_0^{2M}\frac{dr}{\sqrt{2M/r-1}}.
$$

Putting $r=2M\sin^2\chi$ evaluates the last integral as $\pi M$. Hence every such curve reaches the $r=0$ curvature singularity with

$$
\boxed{\tau<\pi M}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The two future null directions are proportional to $k_+=(1,1)$ and $k_-=(1,-1)$. The [null energy condition](../../../general-relativity.md#null-energy-condition) requires

$$
T(k_+,k_+)=a+2b+c\geq0,
\qquad
T(k_-,k_-)=a-2b+c\geq0.
$$

Equivalently,

$$
\boxed{a+c\geq2|b|}.
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

In two dimensions every future causal vector is a nonnegative linear combination of $k_+$ and $k_-$. The [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) is therefore equivalent to nonnegativity of $T(k_+,k_+)$, $T(k_-,k_-)$, and the mixed pairing

$$
T(k_+,k_-)=a-c.
$$

Thus the necessary and sufficient conditions are

$$
\boxed{a+c\geq2|b|,
\qquad a\geq c}.
$$

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

A future unit timelike vector is proportional to $(1,v)$ with $|v|<1$. The measured energy density has the sign of

$$
q(v)=a+2bv+cv^2.
$$

Under the assumption $c>a$, the [weak energy condition](../../../general-relativity.md#weak-energy-condition) first requires $a=q(0)\geq0$, and hence $c>0$. The convex quadratic has its minimum at $v=-b/c$. Nonnegativity for every $|v|<1$ is then equivalent to

$$
a-\frac{b^2}{c}\geq0.
$$

Indeed this inequality implies $|b|/c\leq\sqrt{a/c}<1$, so the minimum lies inside the allowed interval. Therefore

$$
\boxed{a\geq0,
\qquad ac\geq b^2}
$$

is necessary and sufficient when $c>a$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Let $\Sigma_t$ be a [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) with induced metric $h_{ij}$, lapse $N$, shift $N^i$, and future unit normal $n^a$. For the normalization of the action in the question, the canonical momentum density is

$$
\Pi=2\sqrt h\,n^a\nabla_a\Phi
=\frac{2\sqrt h}{N}(\dot\Phi-N^i\partial_i\Phi).
$$

The equal-time [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) are

$$
[\widehat\Phi(t,\mathbf x),\widehat\Phi(t,\mathbf y)]=0,
\qquad
[\widehat\Pi(t,\mathbf x),\widehat\Pi(t,\mathbf y)]=0,
$$

and

$$
\boxed{[\widehat\Phi(t,\mathbf x),\widehat\Pi(t,\mathbf y)]
=i\delta^{(3)}(\mathbf x-\mathbf y)}.
$$

With the conventional extra factor $1/2$ in the action, $\Pi$ loses the factor two.

For complex classical solutions, the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) is

$$
(\phi_1,\phi_2)_{KG}
=i\int_{\Sigma_t}d\Sigma^a
(\phi_1^*\nabla_a\phi_2-\phi_2\nabla_a\phi_1^*).
$$

The integrand is a conserved current because both fields obey the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation). Applying the [divergence theorem](../../../calculus.md#divergence-theorem) between two Cauchy hypersurfaces shows that the value is independent of the foliation, provided there is no boundary flux.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

A [strictly stationary spacetime](../../../general-relativity.md#strictly-stationary-spacetime) has an everywhere timelike Killing field $K$. Choose a complete orthonormal set of [positive-frequency solutions](../../../quantum-field-theory.md#positive-frequency-solution) satisfying

$$
i\mathcal L_Ku_j=\omega_ju_j,
\qquad \omega_j>0,
$$

with positive [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product). Expand

$$
\widehat\Phi=\sum_j(a_ju_j+a_j^\dagger u_j^*)
$$

with the sum replaced by an integral for continuous labels. Equivalently, the coefficients are projections using the Klein-Gordon product: $a_j=(u_j,\widehat\Phi)_{KG}$ and $a_j^\dagger=-(u_j^*,\widehat\Phi)_{KG}$.

The stationary vacuum is uniquely selected, up to degeneracies and unitary changes of positive-frequency basis, by

$$
a_j|0\rangle=0
$$

for every $j$. Acting with the $a_j^\dagger$ constructs the [bosonic Fock space](../../../quantum-field-theory.md#bosonic-fock-space), the symmetric direct sum of all particle-number sectors.

In a nonstationary spacetime no preferred timelike Killing flow exists, so there is no canonical split into positive and negative frequencies. Different splits mix creation and annihilation operators by [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation) and lead to the [vacuum ambiguity in a nonstationary spacetime](../../../quantum-field-theory.md#vacuum-ambiguity-in-a-nonstationary-spacetime).

## 4

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

A black-hole metric is [stationary](../../../general-relativity.md#stationary-spacetime) when it admits a Killing field $K$ generating time translations and timelike near spatial infinity. It is [static](../../../general-relativity.md#static-spacetime) when $K$ is also hypersurface orthogonal,

$$
K_{[a}\nabla_bK_{c]}=0.
$$

In coordinates adapted to a static field, the metric coefficients are time independent and the time-space cross terms vanish.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

A [stationary axisymmetric spacetime](../../../general-relativity.md#stationary-axisymmetric-spacetime) additionally admits an axial Killing field $m$ with closed orbits. The two symmetry generators commute,

$$
[K,m]=0,
$$

and preserve the black-hole exterior and horizon. Coordinates adapted to them make the metric independent of both $t$ and $\phi$.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The [Kerr black hole](../../../general-relativity.md#kerr-black-hole) coefficients are independent of $t$ and $\phi$, so $\partial_t$ and $\partial_\phi$ are commuting Killing fields; the latter has closed circular orbits. Kerr is therefore stationary and axisymmetric.

Expanding the metric gives the nonzero cross component

$$
g_{t\phi}=-\frac{2Mar\sin^2\theta}{\Sigma}.
$$

For $a\ne0$ this cannot be removed throughout the exterior by a constant redefinition of $\phi$, and the asymptotically timelike stationary Killing field has nonzero twist. It is not hypersurface orthogonal, so Kerr is not static.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The stationary Killing field becomes null where

$$
g_{tt}=-\left(1-\frac{2Mr}{\Sigma}\right)=0.
$$

Solving $r^2-2Mr+a^2\cos^2\theta=0$ gives the stationary-limit surfaces

$$
r_E^\pm(\theta)=M\pm\sqrt{M^2-a^2\cos^2\theta}.
$$

The exterior [Kerr ergoregion](../../../general-relativity.md#kerr-ergoregion) is

$$
\boxed{r_+<r<r_E^+(\theta)},
\qquad
r_+=M+\sqrt{M^2-a^2}.
$$

The event horizon is the constant-radius surface $\Delta=0$, whereas the outer stationary limit lies outside it except at the poles, where the two meet.

Inside the ergoregion $\partial_t$ is spacelike, so future-directed particles can have negative conserved stationary Killing energy while still following causal trajectories. Sending such a particle through the horizon permits another particle to escape with increased positive energy. This is the [Penrose process](../../../general-relativity.md#penrose-process), which extracts the black hole's rotational energy.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

On the north-pole surface, $\theta=0$ and $d\theta=d\phi=0$, while $\Sigma=r^2+a^2$. Pulling back the [Boyer-Lindquist coordinates](../../../general-relativity.md#boyer-lindquist-coordinates) metric therefore gives

$$
\boxed{ds^2_{(2)}
=-\frac{\Delta}{r^2+a^2}dt^2
+\frac{r^2+a^2}{\Delta}dr^2}.
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Set $F(r)=\Delta/(r^2+a^2)$. The [Kerr polar tortoise coordinate](../../../general-relativity.md#kerr-polar-tortoise-coordinate) obeys

$$
\boxed{\frac{dr_*}{dr}=\frac1F
=\frac{r^2+a^2}{\Delta}}.
$$

Then $ds^2_{(2)}=F(-dt^2+dr_*^2)$. Introduce retarded time $u=t-r_*$, so $dt=du+dr_*$ and

$$
\boxed{ds^2_{(2)}=-F(r)du^2-2\,du\,dr}.
$$

The determinant of this metric is $-1$, including at $\Delta=0$. These outgoing Eddington-Finkelstein-type coordinates therefore extend analytically across the past event horizon into the white-hole region of Kerr.

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

At $r=0$ on the north pole,

$$
\Sigma=a^2,
\qquad
\Delta=a^2,
\qquad
F=1,
$$

so nothing singular occurs. The Kerr curvature singularity is the ring $\Sigma=0$, which requires both $r=0$ and $\theta=\pi/2$ and is absent from this polar surface. The analytic extension passes through $r=0$ into the negative-$r$ asymptotic region, giving the maximal coordinate range

$$
\boxed{-\infty<r<\infty}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

On a constant-$t$ asymptotically flat hypersurface, transform the large-$r$ spatial metric to asymptotically Cartesian coordinates. Its leading perturbation is

$$
h_{ij}=\delta_{ij}+q_{ij}+O(r^{-2}),
\qquad
q_{ij}=\frac{2M}{r}n_in_j
=\frac{2Mx_ix_j}{r^3}.
$$

The rotation parameter $a$ first affects the spatial metric at orders that vanish in the [Arnowitt-Deser-Misner energy](../../../general-relativity.md#arnowitt-deser-misner-energy) surface limit. Direct differentiation gives

$$
\partial_jq_{ij}=\frac{2M}{r^2}n_i,
\qquad
\partial_iq_{jj}=-\frac{2M}{r^2}n_i.
$$

Hence

$$
n^i(\partial_jh_{ij}-\partial_ih_{jj})
=\frac{4M}{r^2}+O(r^{-3}).
$$

Using $\int_{S_r^2}dA=4\pi r^2$ in the ADM surface integral yields

$$
\boxed{E_{ADM}
=\frac1{16\pi}(4\pi r^2)\frac{4M}{r^2}=M}.
$$

**Thus the Kerr parameter $M$ is its total mass in the rest frame.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
