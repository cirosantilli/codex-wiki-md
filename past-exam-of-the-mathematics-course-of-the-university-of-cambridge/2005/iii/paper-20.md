# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper20.pdf)

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

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The central problem of [spectral geometry](../../../riemannian-geometry.md#spectral-geometry) is how much of a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is determined by the [eigenvalues](../../../linear-operator-theory.md#eigenvalue), with [multiplicities](../../../polynomial.md#multiplicity-mathematics), of its [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator). For a membrane with fixed [boundary](../../../topology.md#boundary-of-a-set), the squared vibration frequencies are proportional to the [Dirichlet eigenvalues](../../../analysis.md#dirichlet-eigenvalue). Kac's [1966 paper](https://www.math.ucdavis.edu/~saito/courses/ACHA.READ.F03/kac-drum.pdf) brought this inverse problem into focus: the full sequence of frequencies might encode a domain's shape, but recovering a few geometric quantities is much weaker than recovering an [isometry](../../../riemannian-geometry.md#isometry) class.

The first major line of development extracts geometric information from spectral sums. On a smooth [closed](../../../topology.md#closed-set) $d$-dimensional [manifold](../../../topology.md#topological-manifold), the [heat trace](../../../riemannian-geometry.md#heat-trace) has the short-time expansion

$$
Z(t)=\sum_j e^{-t\lambda_j}\sim(4\pi t)^{-d/2}\left(\operatorname{Vol}(M)+\frac t6\int_M R\,dV+\cdots\right),
$$

where $\lambda_j$ are the nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $P=-\Delta$ and $R$ is [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). The coefficients are [heat invariants](../../../diffusion-equation.md#heat-invariants), formed by integrating local curvature expressions. They recover dimension, [Riemannian volume](../../../differential-geometry.md#riemannian-volume) and total [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). For smooth planar domains with the [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition),

$$
Z(t)=\frac{\operatorname{Area}(\Omega)}{4\pi t}-\frac{\operatorname{Length}(\partial\Omega)}{8\sqrt{\pi t}}+O(1).
$$

Thus [area](../../../differential-geometry.md#surface-area) and [boundary](../../../topology.md#boundary-of-a-set) length are audible. The constant term also contains topological information through [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem), with corner corrections when the [boundary](../../../topology.md#boundary-of-a-set) is polygonal. The [Weyl law](../../../riemannian-geometry.md#weyl-law) is the corresponding leading eigenvalue-counting result. Neither the leading term nor the whole list of local heat coefficients automatically reconstructs global geometry.

In the 1970s, the [wave trace](../../../riemannian-geometry.md#wave-trace) introduced a complementary link with global [closed geodesics](../../../riemannian-geometry.md#closed-geodesic). The [distribution](../../../distribution-theory.md#distribution-mathematical-analysis)

$$
W(t)=\sum_j e^{it\sqrt{\lambda_j}}
$$

is spectral, while its singularities are governed by periodic [geodesic](../../../riemannian-geometry.md#geodesic) motion. The [1975 Duistermaat-Guillemin work](https://link.springer.com/article/10.1007/BF01405172) made this relationship precise. Its [trace](../../../linear-algebra.md#matrix-trace) formula places singularities at [geodesic](../../../riemannian-geometry.md#geodesic) lengths and computes their coefficients under suitable clean or nondegenerate hypotheses. When a coefficient is nonzero, the corresponding length is audible. Possible cancellation must be addressed before identifying the entire [length spectrum](../../../geometry-and-topology.md#length-spectrum) with the singular support. This approach led to [spectral rigidity](../../../riemannian-geometry.md#spectral-rigidity) questions, rather than just the recovery of integral curvature quantities.

The second main line constructs counterexamples to metric determination. A precedent was the [1964 flat-torus example](https://doi.org/10.1073/pnas.51.4.542): different sixteen-dimensional [Euclidean lattices](../../../fourier-analysis.md#euclidean-lattice) could give the same [Laplacian eigenvalues](../../../partial-differential-equation.md#laplacian-eigenvalue). Subsequent lattice constructions lowered the dimension; [Conway and Sloane's 1992 work](https://academic.oup.com/imrn/article-abstract/1992/4/93/660616) exhibited four-dimensional [Euclidean lattices](../../../fourier-analysis.md#euclidean-lattice) with matching [lattice theta series](../../../modular-function.md#theta-series-of-a-euclidean-lattice). For a [flat torus](../../../second-fundamental-form.md#flat-torus) $\mathbb R^d/\Lambda$, the spectrum is the multiset $4\pi^2|\xi|^2$ for $\xi\in\Lambda^*$, so equality of [lattice theta series](../../../modular-function.md#theta-series-of-a-euclidean-lattice) of the [dual lattices](../../../fourier-analysis.md#dual-lattice) gives [isospectrality](../../../riemannian-geometry.md#isospectral-manifolds) even when the [Euclidean lattices](../../../fourier-analysis.md#euclidean-lattice) are not related by an [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation).

A systematic geometric construction arrived with the [Sunada theorem in 1985](https://annals.math.princeton.edu/1985/121-1/p04). For a common Riemannian cover with finite [isometry](../../../riemannian-geometry.md#isometry) [group](../../../group.md) $T$, [almost conjugate subgroups](../../../representation-theory.md#gassmann-equivalence) have the same number of invariant vectors in each [Laplacian](../../../calculus.md#laplacian) [eigenspace](../../../linear-operator-theory.md#eigenspace). Their freely acting quotients are therefore [isospectral manifolds](../../../riemannian-geometry.md#isospectral-manifolds). This reduces an analytic equality to a finite-group representation identity. It produces many examples on surfaces and in higher dimensions, but nonconjugacy of the [subgroups](../../../group.md#subgroup) must be supplemented by an argument excluding extra quotient [isometries](../../../riemannian-geometry.md#isometry). [Transplantation theorem](../../../riemannian-geometry.md#transplantation-theorem) provides an explicit version: piecewise [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) are recombined by a fixed invertible linear transformation that respects the gluing and [boundary conditions](../../../differential-equation.md#boundary-condition).

The planar problem itself was answered negatively by [Gordon, Webb and Wolpert in 1992](https://arxiv.org/abs/math/9207215): noncongruent simply connected polygonal plane domains have equal Dirichlet spectra. This is stronger than counterexamples among abstract [manifolds](../../../topology.md#topological-manifold) or [flat tori](../../../second-fundamental-form.md#flat-torus), since these are genuine two-dimensional planar membranes. It does not settle every restricted version, such as asking for two domains within a specified smooth or convex class.

By the 1990s, [isospectrality](../../../riemannian-geometry.md#isospectral-manifolds) was also known to coexist with continuous metric variation and changes in local geometry. For example, [a 1997 construction](https://arxiv.org/abs/dg-ga/9710004) gives continuous isospectral families on products of spheres and [tori](../../../topology.md#torus) whose members need not be locally [isometric](../../../riemannian-geometry.md#isometry); in some examples the maximum [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) changes. Conversely, rigidity and [compactness](../../../topology.md#compact-space) results show that an isospectral class is not unrestricted. The [1988 surface compactness theorem](https://doi.org/10.1016/0022-1236(88)90071-7) makes fixed-spectrum sets of [closed](../../../topology.md#closed-set) orientable surface metrics [compact](../../../topology.md#compact-space) modulo [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism). [Compactness](../../../topology.md#compact-space) does not mean there is only one metric, or even finitely many metrics. By 2005, the subject therefore combined local [heat invariants](../../../diffusion-equation.md#heat-invariants), global [geodesic](../../../riemannian-geometry.md#geodesic) information, group-theoretic constructions, explicit [transplantation](../../../riemannian-geometry.md#transplantation-theorem) and geometric rigidity. **The spectrum determines substantial geometry, while generally failing to determine the full metric.**

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [smooth function](../../../analysis.md#smooth-function) $f$ and the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) $\nabla$, the [Riemannian Hessian](../../../riemannian-geometry.md#riemannian-hessian) is the covariant two-tensor

$$
\operatorname{Hess}_g f(X,Y)=(\nabla_Xdf)(Y)=X(Yf)-df(\nabla_XY).
$$

The connection rules show that this is linear over [smooth functions](../../../analysis.md#smooth-function) in both vector-field arguments, so it is a [tensor](../../../linear-algebra.md#tensor). Torsion-freeness gives its symmetry:

$$
\operatorname{Hess}_g f(X,Y)-\operatorname{Hess}_g f(Y,X)
=[X,Y]f-df(\nabla_XY-\nabla_YX)=0.
$$

Its [metric trace](../../../linear-algebra.md#metric-trace) defines the paper's [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator), $\Delta=\operatorname{div}_g\operatorname{grad}_g$; its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) on a [closed manifold](../../../differential-geometry.md#closed-manifold) are nonpositive. We use $P=-\Delta$ when listing nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) or writing $e^{-tP}$.

At $p$, choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $e_1,\ldots,e_d$ of the [tangent space](../../../differential-geometry.md#tangent-space) and unit-speed [geodesics](../../../riemannian-geometry.md#geodesic) $\gamma_i(t)=\exp_p(te_i)$. Differentiating twice along a curve gives

$$
\frac{d^2}{dt^2}f(\gamma_i(t))
=\operatorname{Hess}_g f(\dot\gamma_i,\dot\gamma_i)+df(\nabla_{\dot\gamma_i}\dot\gamma_i).
$$

The covariant acceleration vanishes on a [geodesic](../../../riemannian-geometry.md#geodesic). Taking the [trace](../../../linear-algebra.md#matrix-trace) at $t=0$ proves the [geodesic trace formula for the Laplace-Beltrami operator](../../../differential-geometry.md#geodesic-trace-formula-for-the-laplace-beltrami-operator):

$$
\boxed{\Delta f(p)=\sum_{i=1}^d(f\circ\gamma_i)''(0)
=\lim_{h\to0}\frac{\sum_{i=1}^d[f(\exp_p(he_i))+f(\exp_p(-he_i))-2f(p)]}{h^2}.}
$$

The last equality is Taylor's formula along the [geodesics](../../../riemannian-geometry.md#geodesic), and expresses the [Laplacian](../../../calculus.md#laplacian) entirely through nearby function values.

For stabilization, let $X_1,X_2$ be the assumed isospectral nonisometric four-dimensional [tori](../../../topology.md#torus), and let $k=n-4>0$. Take the same small [flat torus](../../../second-fundamental-form.md#flat-torus) $F_\varepsilon=\mathbb R^k/\varepsilon\mathbb Z^k$ as an extra factor. On a [Riemannian product](../../../riemannian-geometry.md#riemannian-product),

$$
P_{X_i\times F_\varepsilon}=P_{X_i}\otimes I+I\otimes P_{F_\varepsilon}.
$$

If $\phi_j$ and $\psi_\ell$ are [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_j$ and $\mu_\ell$, then $\phi_j\psi_\ell$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda_j+\mu_\ell$. Products of [orthonormal eigenbases](../../../linear-operator-theory.md#orthonormal-eigenbasis) are complete in the product $L^2$ space, so this lists all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) with [multiplicities](../../../polynomial.md#multiplicity-mathematics), including coincidences between different sums. Consequently the two products are isospectral.

One must also prove that multiplying by a common factor has not accidentally made the two [manifolds](../../../topology.md#topological-manifold) [isometric](../../../riemannian-geometry.md#isometry). Choose

$$
0<\varepsilon<\delta<\min\{\operatorname{inj}(X_1),\operatorname{inj}(X_2)\}.
$$

The injectivity radii are positive because the factors are [compact](../../../topology.md#compact-space). A [closed](../../../topology.md#closed-set) product [geodesic](../../../riemannian-geometry.md#geodesic) of length less than $\delta$ projects to a [closed geodesic](../../../riemannian-geometry.md#closed-geodesic) of length less than $\delta$ in $X_i$. Such a projected [geodesic](../../../riemannian-geometry.md#geodesic) must be constant: otherwise its initial vector over one period would be a nonzero vector of norm below the [injectivity radius](../../../riemannian-geometry.md#injectivity-radius) mapping back to its starting point under the [exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry). Thus all sufficiently short [closed geodesics](../../../riemannian-geometry.md#closed-geodesic) lie in the $F_\varepsilon$ directions. Conversely the $k$ coordinate circles, of length $\varepsilon$, pass through every point and span those directions.

It follows that the [smooth distribution](../../../differential-geometry.md#distribution-differential-geometry) tangent to the small flat-torus factor is characterized intrinsically by the span of tangent vectors to [closed geodesics](../../../riemannian-geometry.md#closed-geodesic) of length below $\delta$. A hypothetical product [isometry](../../../riemannian-geometry.md#isometry) would preserve this [smooth distribution](../../../differential-geometry.md#distribution-differential-geometry) and its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). The latter has leaves $X_i\times\{q\}$; the [isometry](../../../riemannian-geometry.md#isometry) and its inverse take whole leaves to whole leaves, thereby giving an [isometry](../../../riemannian-geometry.md#isometry) $X_1\cong X_2$, a contradiction. This proves [isospectral stabilization by a small flat torus](../../../riemannian-geometry.md#isospectral-stabilization-by-a-small-flat-torus):

$$
\boxed{X_1\times F_\varepsilon\text{ and }X_2\times F_\varepsilon\text{ are isospectral nonisometric }n\text{-tori for every }n>4.}
$$

This argument works even without assuming that the original four-dimensional [torus](../../../topology.md#torus) metrics are flat.

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Work on a [closed](../../../topology.md#closed-set) [compact](../../../topology.md#compact-space) smooth [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) $M$ without [boundary](../../../topology.md#boundary-of-a-set), as in the usual discrete spectral setting here. Use the paper's $\Delta=\operatorname{tr}_g\operatorname{Hess}_g$, and put $P=-\Delta$. The [Riemannian heat kernel](../../../diffusion-equation.md#riemannian-heat-kernel) $H(t,x,y)$ is the smooth kernel, for $t>0$, representing the solution of

$$
\partial_tu=\Delta u,\qquad u(0,\cdot)=f,\qquad
u(t,x)=\int_M H(t,x,y)f(y)\,dV(y).
$$

Thus $(\partial_t-\Delta_x)H=0$ and its distributional initial value in $x$ is the [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function) at $y$. The [heat trace](../../../riemannian-geometry.md#heat-trace) is

$$
Z_M(t)=\int_M H(t,x,x)\,dV(x)=\operatorname{Tr}(e^{-tP}).
$$

The [heat invariants](../../../diffusion-equation.md#heat-invariants) are the coefficients $a_r(M)$ in the short-time [heat trace](../../../riemannian-geometry.md#heat-trace) expansion specified below.

To derive its spectral form, take an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) $P\phi_j=\lambda_j\phi_j$, with $0=\lambda_0\le\lambda_1\le\cdots$, repeating [eigenvalues](../../../linear-operator-theory.md#eigenvalue) according to [multiplicity](../../../polynomial.md#multiplicity-mathematics). For the initial datum $\phi_j$, the function $e^{-t\lambda_j}\phi_j$ solves the [heat equation](../../../diffusion-equation.md#heat-equation). Uniqueness identifies it with the heat-kernel solution. Expanding arbitrary initial data in this basis therefore gives the [spectral expansion of the Riemannian heat kernel](../../../diffusion-equation.md#spectral-expansion-of-the-riemannian-heat-kernel):

$$
H(t,x,y)=\sum_{j=0}^\infty e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}.
$$

Standard elliptic estimates and [eigenvalue](../../../linear-operator-theory.md#eigenvalue) growth imply smooth convergence for $t$ bounded away from zero: polynomial bounds on derivatives of [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) are dominated by the exponential factors. On the diagonal all summands are nonnegative, so [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) also justifies integration without needing an interchange of conditionally convergent terms. Since each [eigenfunction](../../../linear-operator-theory.md#eigenfunction) has unit $L^2$ norm,

$$
\boxed{Z_M(t)=\sum_{j=0}^\infty e^{-t\lambda_j}.}
$$

Equivalently, if the paper's [Laplacian eigenvalues](../../../partial-differential-equation.md#laplacian-eigenvalue) are written $\nu_j=-\lambda_j$, the formula is $\sum_j e^{t\nu_j}$; a growing exponential is not the [heat semigroup](../../../diffusion-equation.md#heat-semigroup).

Here are the needed [heat kernel expansion](../../../diffusion-equation.md#heat-kernel-expansion) facts, stated without proof. On a [closed](../../../topology.md#closed-set) $d$-dimensional smooth [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold),

$$
H(t,x,x)\sim(4\pi t)^{-d/2}\sum_{r=0}^\infty u_r(x)t^r,\qquad u_0(x)=1,
$$

with the diagonal remainder uniform in $x$ after any finite truncation. The coefficients are smooth local geometric quantities; $u_1=R/6$. [Compactness](../../../topology.md#compact-space) therefore allows integration term by term:

$$
Z_M(t)\sim(4\pi t)^{-d/2}\sum_{r=0}^\infty a_r(M)t^r,
\qquad a_r(M)=\int_Mu_r(x)\,dV(x),\qquad a_0(M)=\operatorname{Vol}(M)>0.
$$

These integrated coefficients are the [heat invariants](../../../diffusion-equation.md#heat-invariants). The uniform leading remainder in particular gives $Z_M(t)=(4\pi t)^{-d/2}(\operatorname{Vol}(M)+O(t))$.

[Isospectral manifolds](../../../riemannian-geometry.md#isospectral-manifolds) have identical [heat traces](../../../riemannian-geometry.md#heat-trace) by the derived spectral formula. If their dimensions were $d<e$, multiplying the common [trace](../../../linear-algebra.md#matrix-trace) by $t^{d/2}$ would give a finite positive limit on the $d$-dimensional [manifold](../../../topology.md#topological-manifold) but divergence on the $e$-dimensional one. Thus the dimensions are equal, and equality of the leading coefficient gives equal [Riemannian volume](../../../differential-geometry.md#riemannian-volume). Explicitly,

$$
\boxed{d=2\lim_{t\downarrow0}\frac{\log Z_M(t)}{\log(1/t)},\qquad
\operatorname{Vol}(M)=\lim_{t\downarrow0}(4\pi t)^{d/2}Z_M(t).}
$$

The absence of a [boundary](../../../topology.md#boundary-of-a-set) fixes this particular integer-power expansion. With a [boundary](../../../topology.md#boundary-of-a-set) one must first specify [boundary conditions](../../../differential-equation.md#boundary-condition) and include the appropriate half-integer [boundary](../../../topology.md#boundary-of-a-set) terms; the leading dimension-and-volume conclusion remains valid in the usual [compact](../../../topology.md#compact-space) smooth setting.

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $p:N\to M=U\backslash N$ be a finite normal Riemannian covering, so $U$ acts freely by deck [isometries](../../../riemannian-geometry.md#isometry). With $x,y$ any lifts of $\bar x,\bar y$, the [heat kernel on a finite isometric quotient](../../../diffusion-equation.md#heat-kernel-on-a-finite-isometric-quotient) satisfies

$$
\boxed{H_M(t,\bar x,\bar y)=\sum_{u\in U}H_N(t,x,uy).}
$$

There is no factor $1/|U|$ in this kernel formula. Simultaneous invariance of $H_N$ under [isometries](../../../riemannian-geometry.md#isometry) proves independence of the lifts, by reindexing $U$. Each term solves the lifted [heat equation](../../../diffusion-equation.md#heat-equation). If $F_U$ is a [fundamental domain](../../../group-theory.md#fundamental-domain) and $f$ a function on $M$, the integral of the right side against $f(\bar y)$ over $F_U$ equals

$$
\int_NH_N(t,x,y)f(p(y))\,dV(y),
$$

because the translates $uF_U$ tile $N$ up to sets of measure zero. This converges to $f(p(x))$ as $t\downarrow0$, proving the initial condition. Uniqueness of the [heat equation](../../../diffusion-equation.md#heat-equation) solution on the [closed manifold](../../../differential-geometry.md#closed-manifold) gives the formula. For a noncompact finite cover, use the minimal [heat kernels](../../../diffusion-equation.md#heat-kernel), or compatible Friedrichs heat realizations. The normalized pullback $f\mapsto |U|^{-1/2}f\circ p$ is unitary onto the deck-invariant $L^2$ subspace and preserves the [Dirichlet energy](../../../differential-geometry.md#dirichlet-energy), so it intertwines the [heat semigroups](../../../diffusion-equation.md#heat-semigroup) and yields the same kernel formula. No uniqueness of unrestricted noncompact heat-equation solutions is needed.

Set $I_t(g)=\int_N H_N(t,x,gx)\,dV(x)$ for an [isometry](../../../riemannian-geometry.md#isometry) $g$. Diagonal integration and the covering degree give

$$
\boxed{Z_{U\backslash N}(t)=\frac1{|U|}\sum_{u\in U}I_t(u).}
$$

Unlike the kernel formula, the [trace](../../../linear-algebra.md#matrix-trace) formula has an averaging factor: integration of a quotient function over $N$ is $|U|$ times integration over $U\backslash N$.

Suppose now $U\le T$, with $T$ any larger [group](../../../group.md) of [isometries](../../../riemannian-geometry.md#isometry) of the [closed manifold](../../../differential-geometry.md#closed-manifold) $N$. Change variables $x=hy$ and use simultaneous heat-kernel invariance to obtain

$$
I_t(hgh^{-1})=\int_NH_N(t,hy,hgy)\,dV(y)=I_t(g).
$$

Thus $I_t$ is a [class function](../../../representation-theory.md#class-function), and the [Sunada orbital heat-trace formula](../../../riemannian-geometry.md#sunada-orbital-heat-trace-formula) can be grouped by [conjugacy classes](../../../group-theory.md#conjugacy-class) $C$ of $T$:

$$
\boxed{Z_{U\backslash N}(t)=\sum_{C\subseteq T}\frac{|U\cap C|}{|U|}I_t(c_C),\qquad c_C\in C.}
$$

Only classes meeting the finite [subgroup](../../../group.md#subgroup) $U$ contribute, so this class sum is finite even if the larger [isometry](../../../riemannian-geometry.md#isometry) [group](../../../group.md) $T$ is infinite.

For finite $T$, [Gassmann equivalence](../../../representation-theory.md#gassmann-equivalence) means $|U_1\cap C|=|U_2\cap C|$ for every [conjugacy class](../../../group-theory.md#conjugacy-class). Summing these counts gives $|U_1|=|U_2|$, so the displayed formula gives identical [heat traces](../../../riemannian-geometry.md#heat-trace). Their spectra, with [multiplicities](../../../polynomial.md#multiplicity-mathematics), agree: as $t\to\infty$, the constant limit identifies the [multiplicity](../../../polynomial.md#multiplicity-mathematics) of zero; after subtracting it, the slowest-decaying exponential identifies the least positive [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and its [multiplicity](../../../polynomial.md#multiplicity-mathematics). Repeating determines every subsequent [eigenvalue](../../../linear-operator-theory.md#eigenvalue). This proves the [Sunada theorem](../../../riemannian-geometry.md#sunada-theorem) in the stated covering situation.

There is an important convention when the [universal cover](../../../algebraic-topology.md#universal-cover) $N$ has an infinite deck [group](../../../group.md) $T$. For [compact](../../../topology.md#compact-space) quotient [manifolds](../../../topology.md#topological-manifold), the [subgroups](../../../group.md#subgroup) must have finite index; the appropriate generalized Gassmann condition is equality of the characters of the finite coset [permutation representations](../../../representation-theory.md#permutation-representation), not equality of possibly infinite cardinalities of conjugacy-class intersections. Let $K$ be the intersection of the two [subgroup](../../../group.md#subgroup) cores. Each core is the kernel of the corresponding finite coset action, so $K$ is normal and of finite index in $T$, and $K\subseteq U_1\cap U_2$. The [manifold](../../../topology.md#topological-manifold) $X=K\backslash N$ is then a [compact](../../../topology.md#compact-space) finite normal cover of $M_0$. The [finite group](../../../group.md#finite-group) $G=T/K$ acts on $X$, and $H_i=U_i/K$ have equal coset [permutation characters](../../../representation-theory.md#permutation-character) in $G$. For a [finite group](../../../group.md#finite-group), the fixed-coset count is

$$
\chi_{G/H_i}(g)=\frac{|C_G(g)|}{|H_i|}\,|H_i\cap[g]|.
$$

Equality at the identity gives equal [subgroup](../../../group.md#subgroup) orders, and then equality for all $g$ gives almost-conjugacy. Applying the proved finite theorem to $H_i\backslash X=U_i\backslash N$ establishes [isospectrality](../../../riemannian-geometry.md#isospectral-manifolds) also in this finite-index interpretation. It avoids taking the divergent [heat trace](../../../riemannian-geometry.md#heat-trace) of a noncompact [universal cover](../../../algebraic-topology.md#universal-cover).

To realize a [finitely presented group](../../../geometric-group-theory.md#finitely-presented-group) $T=\langle a_1,\ldots,a_r\mid R_1,\ldots,R_s\rangle$, begin with the [closed](../../../topology.md#closed-set) smooth four-manifold $B=\#_{j=1}^r(S^1\times S^3)$, whose [fundamental group](../../../algebraic-topology.md#fundamental-group) is free on the $a_j$. Represent the relator words by disjoint smoothly embedded circles; general position permits this in dimension four, including separating self-intersections of representatives. Their oriented normal rank-three bundles are trivial, so perform framed surgeries replacing $S^1\times D^3$ by $D^2\times S^2$. Removing the circles' tubular neighborhoods leaves the [fundamental group](../../../algebraic-topology.md#fundamental-group) unchanged, by codimension-three general position. The [Seifert-van Kampen theorem](../../../algebraic-topology.md#seifert-van-kampen-theorem) shows that each replacement kills exactly the normal closure of its relator. The resulting [closed](../../../topology.md#closed-set) smooth $M_0$ has $\pi_1(M_0)\cong T$. This gives a concrete [closed-manifold realization of a finitely presented fundamental group](../../../algebraic-topology.md#closed-manifold-realization-of-a-finitely-presented-fundamental-group). Equip it with any smooth [Riemannian metric](../../../differential-geometry.md#riemannian-metric) and lift that metric to the universal and intermediate covers; all [covering maps](../../../algebraic-topology.md#covering-space) become [local isometries](../../../differential-geometry.md#local-isometry).

To ensure nonisometry, one must choose nonconjugate [subgroups](../../../group.md#subgroup). If $U_1=U_2$, or they are conjugate, the quotients are [isometric](../../../riemannian-geometry.md#isometry) for every lifted metric, so [Gassmann equivalence](../../../representation-theory.md#gassmann-equivalence) alone cannot imply nonisometry. For nonconjugate [subgroups](../../../group.md#subgroup), choose the base metric to have no nonidentity [local isometry](../../../differential-geometry.md#local-isometry) between open sets, using the [Sunada local isometry lemma](../../../differential-geometry.md#sunada-local-isometry-lemma) in dimension at least two. If $F:M_1\to M_2$ were an [isometry](../../../riemannian-geometry.md#isometry), a local inverse of the first covering followed by $F$ and the second covering would be a [local isometry](../../../differential-geometry.md#local-isometry) of $M_0$, hence the identity. Thus the [covering maps](../../../algebraic-topology.md#covering-space) satisfy $p_2F=p_1$ everywhere. Classification of connected covers then forces $U_1,U_2$ to be conjugate in $\pi_1(M_0)=T$, a contradiction. Therefore **nonconjugate almost-conjugate [subgroups](../../../group.md#subgroup) and a locally rigid base metric give isospectral nonisometric quotients**.

## 5

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use an oriented [geodesic](../../../riemannian-geometry.md#geodesic) hyperbolic $2s$-gon $D$ with paired edges of equal length. Identify each pair by a length-preserving map reversing the [boundary](../../../topology.md#boundary-of-a-set) directions, to make an oriented base surface $M_0$ with possibly singular vertices. Assign to the $s$ edge pairs generators $A_1,\ldots,A_s$ of $T$, with inverse labels for reversed crossings. For each $g\in T$, take a copy $D_g$ and glue its positively labelled edge of type $k$ to the corresponding mate in $D_{gA_k}$. The generators make the glued surface $M$ connected. Left multiplication $D_g\mapsto D_{hg}$ commutes with these right-labelled gluings and gives the $T$ action with quotient $M_0$.

Existence for an arbitrary finite [group](../../../group.md) can even be arranged with no cone singularities. If $T$ has $d$ generators, take $h\ge\max\{2,d\}$ and a regular [hyperbolic polygon](../../../geometry-and-topology.md#hyperbolic-polygon) with $4h$ edges, all angles $\pi/(2h)$, paired with side word $\prod_{i=1}^h a_ib_ia_i^{-1}b_i^{-1}$. Its vertices form one cycle of angle $2\pi$, giving a smooth base of [genus](../../../topology.md#genus-of-a-surface) $h$. Label the $a_i$ by the generators of $T$, padded by identities, and every $b_i$ by the identity. The single vertex word is $\prod_i[A_i,1]=1$, so every lifted vertex also has angle $2\pi$. The resulting connected ordinary [normal covering map](../../../algebraic-topology.md#normal-covering-map) has degree $|T|$ and deck [group](../../../group.md) $T$.

This is the [paired-polygon construction of finite surface covers](../../../geometry-and-topology.md#paired-polygon-construction-of-finite-surface-covers). Interior and open-edge points are regular hyperbolic points; possible singularities occur only at vertices. When the base has cone points, the map is an [orbifold](../../../geometry-and-topology.md#orbifold) covering and may be branched as a map between the underlying topological surfaces. It should not be called an unbranched [manifold](../../../topology.md#topological-manifold) covering at those branch points.

A [vertex cycle of a paired polygon](../../../geometry-and-topology.md#vertex-cycle-of-a-paired-polygon) is the collection of vertices identified to one point on $M_0$. Let $r$ be the number of cycles, $\theta_j$ the sum of the polygon angles in cycle $j$, and $C_j\in T$ the gluing word recorded on going around it. If $q_j=|C_j|$ is the order of that element, a lift closes after $q_j$ turns. It has angle $q_j\theta_j$, and there are $|T|/q_j$ such lifted vertices. The base and lifted cone orders, when they are integer [orbifold](../../../geometry-and-topology.md#orbifold) orders, are

$$
\boxed{m_j=\frac{2\pi}{\theta_j},\qquad \widetilde m_j=\frac{2\pi}{q_j\theta_j}=\frac{m_j}{q_j}.}
$$

An [orbifold](../../../geometry-and-topology.md#orbifold) homomorphism requires $q_j\mid m_j$. The lifted point is smooth exactly when $q_j\theta_j=2\pi$, equivalently $q_j=m_j$ in that case. For arbitrary cone metrics the angle formulas remain valid even when an angle does not correspond to an integer [orbifold](../../../geometry-and-topology.md#orbifold) order.

Counting faces, edges and vertices gives the [Euler characteristic of a paired-polygon surface cover](../../../geometry-and-topology.md#euler-characteristic-of-a-paired-polygon-surface-cover):

$$
\boxed{\chi(M_0)=1-s+r,\qquad \chi(M)=|T|\left(1-s+\sum_{j=1}^r\frac1{q_j}\right).}
$$

These are ordinary topological Euler characteristics, rather than [orbifold](../../../geometry-and-topology.md#orbifold) Euler characteristics. If the lifted surface is smooth, the equivalent [orbifold](../../../geometry-and-topology.md#orbifold) formula is

$$
\chi(M)=|T|\chi_{\rm orb}(M_0),\qquad
\chi_{\rm orb}(M_0)=\chi(M_0)-\sum_j\left(1-\frac1{m_j}\right).
$$

For a [closed](../../../topology.md#closed-set) oriented smooth surface, $\chi=2-2g$ defines its [genus](../../../topology.md#genus-of-a-surface). These formulas also follow from the [Riemann-Hurwitz formula](../../../complex-analysis.md#riemann-hurwitz-formula) by subtracting the ramification deficits $|T|-|T|/q_j$ over each base vertex.

For $U\le T$, the quotient map $M\to M_1=U\backslash M$ is an ordinary normal covering if and only if $U$ acts freely. All possible point stabilizers in this construction are conjugates of $\langle C_j\rangle$, so the concrete necessary and sufficient condition is

$$
\boxed{U\cap g\langle C_j\rangle g^{-1}=\{1\}\quad\text{for every }j\text{ and every }g\in T.}
$$

This is the [freeness criterion for a subgroup of a polygon-cover deck group](../../../geometry-and-topology.md#freeness-criterion-for-a-subgroup-of-a-polygon-cover-deck-group). Under it the deck [group](../../../group.md) is $U$, the degree is $|U|$, and

$$
\boxed{\chi(M_1)=\frac{\chi(M)}{|U|}.}
$$

There is no requirement $U\triangleleft T$ for this map. That different condition characterizes normality of the intermediate cover $M_1\to M_0$. If fixed points are retained and one instead speaks of an [orbifold](../../../geometry-and-topology.md#orbifold) covering, the quotient is regular as an [orbifold](../../../geometry-and-topology.md#orbifold) cover, but ordinary [Euler characteristic](../../../homology.md#euler-characteristic) need not divide by $|U|$; [orbifold Euler characteristic](../../../geometry-and-topology.md#orbifold-euler-characteristic) does.

For the low-genus examples take

$$
T=\operatorname{GL}(3,\mathbb F_2)=\operatorname{PSL}(3,2),\qquad |T|=(8-1)(8-2)(8-4)=168.
$$

Let $U_1$ be a nonzero-vector stabilizer and $U_2$ a plane stabilizer. Their actions have seven points, so $|U_1|=|U_2|=24$ and $[T:U_i]=7$. They are [almost conjugate subgroups](../../../representation-theory.md#gassmann-equivalence): the numbers of fixed nonzero vectors for a matrix $A$ and its dual action $A^{-T}$ are both $2^{\dim\ker(A-I)}-1$. Thus the two coset [permutation characters](../../../representation-theory.md#permutation-character) agree, which is equivalent to [Gassmann equivalence](../../../representation-theory.md#gassmann-equivalence). They are not conjugate: a point stabilizer has a common fixed nonzero vector, whereas a plane stabilizer fixes no nonzero vector globally. In particular, since $7\nmid24$, neither [subgroup](../../../group.md#subgroup) contains any nonidentity element of a cyclic [subgroup](../../../group.md#subgroup) of order seven. All cone monodromies of exact order seven therefore act freely on the intermediate covers.

For [genus](../../../topology.md#genus-of-a-surface) three, start with a [hyperbolic triangle](../../../geometry-and-topology.md#hyperbolic-triangle) whose three angles are $\pi/7$ and double it across one edge. The resulting quadrilateral $D$ has angles

$$
\boxed{\pi/7,\ 2\pi/7,\ \pi/7,\ 2\pi/7.}
$$

The side pairings produce three base vertex cycles, each of total angle $2\pi/7$, and an underlying sphere. Choose generators $A,B$ with $|A|=|B|=|AB|=7$; the three vertex words are $A,B,(AB)^{-1}$. Hence $s=2$, $r=3$ and all $q_j=7$. The full cover is smooth, and

$$
\chi(M)=168\left(-1+\frac37\right)=-96,\qquad
\chi(U_i\backslash M)=-96/24=-4,\qquad\boxed{g_i=3.}
$$

The [hyperbolic polygon area](../../../geometry-and-topology.md#hyperbolic-polygon-area) of $D$ is $8\pi/7$, so the seven-sheeted surfaces have [area](../../../differential-geometry.md#surface-area) $8\pi$, agreeing with Gauss-Bonnet. Their equal spectra follow from the Sunada theorem. For complete numerical generator data, one possible pair is

$$
A=\begin{pmatrix}0&0&1\\0&1&1\\1&1&0\end{pmatrix},\qquad
B=\begin{pmatrix}0&0&1\\1&0&0\\0&1&1\end{pmatrix}
\quad\text{over }\mathbb F_2.
$$

These generate all of $T$ and have the required orders. This construction establishes the requested [isospectrality](../../../riemannian-geometry.md#isospectral-manifolds); it does not establish nonisometry. In the constant-curvature triangle example a lifted reflection can identify the point and plane covers, as in [reflection intertwining of triangle-cover coset actions](../../../riemannian-geometry.md#reflection-intertwining-of-triangle-cover-coset-actions). Breaking that symmetry with a generic metric gives nonisometric genus-three surfaces, but then the metric need not have constant curvature. Those are distinct assertions.

For [genus](../../../topology.md#genus-of-a-surface) four, use the [cone-torus construction of genus-four Sunada surfaces](../../../riemannian-geometry.md#cone-torus-construction-of-genus-four-sunada-surfaces). Take a regular hyperbolic quadrilateral with four angles

$$
\boxed{\pi/14,\ \pi/14,\ \pi/14,\ \pi/14}
$$

and pair opposite sides in the usual [torus](../../../topology.md#torus) pattern $a,b,a^{-1},b^{-1}$. All four vertices belong to one cycle, whose total angle is $2\pi/7$; the underlying base is a [torus](../../../topology.md#torus) with one [cone point](../../../differential-geometry.md#cone-point). Choose $A,B$ of order four generating $T$, with commutator $[A,B]$ of order seven. For example,

$$
A=\begin{pmatrix}0&0&1\\0&1&0\\1&1&0\end{pmatrix},\qquad
B=\begin{pmatrix}0&0&1\\0&1&1\\1&0&0\end{pmatrix},\qquad
|A|=|B|=4,\quad |[A,B]|=7.
$$

Only the commutator is a cone monodromy, so the order-four side labels do not create cone points of order four. Here $s=2$, $r=1$, $q_1=7$, giving

$$
\chi(M)=168\left(-1+\frac17\right)=-144,\qquad
\chi(U_i\backslash M)=-144/24=-6,\qquad\boxed{g_i=4.}
$$

The quadrilateral has [area](../../../differential-geometry.md#surface-area) $12\pi/7$, and each seven-sheeted smooth quotient has [area](../../../differential-geometry.md#surface-area) $12\pi$. Again the order-seven cone stabilizer meets neither $U_i$ nontrivially, so the metrics are smooth and the Sunada theorem gives identical spectra. The required [group](../../../group.md) and [subgroup](../../../group.md#subgroup) orders are therefore **168 and 24 in both constructions**; the genus-three side-generator orders are **7 and 7**, and the displayed genus-four side-generator orders are **4 and 4**, with cone-word order **7** in both cases.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
