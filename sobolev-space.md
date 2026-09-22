# Sobolev space

↑ **Parent:** [Functional analysis](functional-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sobolev_space)

For real $s$, the $L^2$-based Sobolev space $H^s(\mathbb R^n)$ consists of tempered distributions satisfying

$$
\lVert u\rVert_{H^s}^2
=\int_{\mathbb R^n}(1+|\xi|^2)^s|\widehat u(\xi)|^2\,d\xi<\infty.
$$

**Table of contents**

- [Zero-trace Sobolev space](#zero-trace-sobolev-space)
- [Near-identity Sobolev loop factorization](#near-identity-sobolev-loop-factorization)
- [Trace operator](#trace-operator)
  - [Sobolev trace theorem](#sobolev-trace-theorem)
    - [Multiplicative trace inequality on a bounded smooth domain](#multiplicative-trace-inequality-on-a-bounded-smooth-domain)
    - [W1p trace theorem on a half-space](#w1p-trace-theorem-on-a-half-space)
    - [Failure of an Lp hyperplane trace](#failure-of-an-lp-hyperplane-trace)
- [Sobolev interpolation inequality](#sobolev-interpolation-inequality)
- [Interior cone property](#interior-cone-property)
- [Clamped second-order Sobolev space](#clamped-second-order-sobolev-space)
  - [Clamped interval derivative norm bound](#clamped-interval-derivative-norm-bound)
  - [Weak formulation of a clamped fourth-order equation](#weak-formulation-of-a-clamped-fourth-order-equation)
  - [Clamped Hessian identity](#clamped-hessian-identity)
- [Homogeneous Sobolev space](#homogeneous-sobolev-space)
- [Gaussian Sobolev space](#gaussian-sobolev-space)
- [Sobolev norm](#sobolev-norm)
- [Sobolev multiplication by a smooth cutoff](#sobolev-multiplication-by-a-smooth-cutoff)
- [Sobolev duality](#sobolev-duality)
- [Sobolev fundamental theorem of calculus on lines](#sobolev-fundamental-theorem-of-calculus-on-lines)
  - [Sobolev slicing and planar continuity](#sobolev-slicing-and-planar-continuity)
- [Sobolev algebra](#sobolev-algebra)
  - [Tame Sobolev product estimate](#tame-sobolev-product-estimate)
- [Periodic Sobolev space](#periodic-sobolev-space)
- [Local Sobolev space](#local-sobolev-space)
- [First-order Sobolev space](#first-order-sobolev-space)
  - [Sobolev gradient vanishes on a zero set](#sobolev-gradient-vanishes-on-a-zero-set)
  - [Sobolev function with zero weak gradient](#sobolev-function-with-zero-weak-gradient)
  - [H1 space](#h1-space)
  - [Sobolev characterization by bounded difference quotients](#sobolev-characterization-by-bounded-difference-quotients)
  - [Zero-boundary Sobolev space](#zero-boundary-sobolev-space)
    - [No uniformly positive coefficient in a zero-boundary Sobolev space](#no-uniformly-positive-coefficient-in-a-zero-boundary-sobolev-space)
    - [Lipschitz truncation preserves zero-boundary Sobolev spaces](#lipschitz-truncation-preserves-zero-boundary-sobolev-spaces)
    - [Dirichlet inner product](#dirichlet-inner-product)
      - [Conformal invariance of the planar Dirichlet inner product](#conformal-invariance-of-the-planar-dirichlet-inner-product)
      - [Dirichlet energy space](#dirichlet-energy-space)
        - [Orthogonality of supported and harmonic Dirichlet functions](#orthogonality-of-supported-and-harmonic-dirichlet-functions)
  - [One-dimensional Sobolev representative](#one-dimensional-sobolev-representative)
    - [Interval Sobolev supremum estimate](#interval-sobolev-supremum-estimate)
  - [Density of smooth functions in a Sobolev space](#density-of-smooth-functions-in-a-sobolev-space)
  - [Zero extension of W01](#zero-extension-of-w01)
  - [Sobolev extension operator](#sobolev-extension-operator)
    - [Reflection extension from a half-space](#reflection-extension-from-a-half-space)
      - [Odd reflection](#odd-reflection)
  - [Absolutely continuous function](#absolutely-continuous-function)
    - [Dyadic slope-tail criterion for absolute continuity](#dyadic-slope-tail-criterion-for-absolute-continuity)
- [Sobolev space with a partial Dirichlet condition](#sobolev-space-with-a-partial-dirichlet-condition)
- [Affine Sobolev space](#affine-sobolev-space)
  - [Homogenization of Dirichlet boundary data](#homogenization-of-dirichlet-boundary-data)
- [Hardy operator](#hardy-operator)
  - [Hardy averaging inequality](#hardy-averaging-inequality)
    - [Hardy inequality on an interval](#hardy-inequality-on-an-interval)
- [Poincaré inequality](#poincare-inequality)
  - [Poincare inequality with a positive-measure zero set](#poincare-inequality-with-a-positive-measure-zero-set)
  - [Poincare inequality on an annulus](#poincare-inequality-on-an-annulus)
  - [Poincare-Wirtinger inequality](#poincare-wirtinger-inequality)
    - [Cube mean-gradient inequality](#cube-mean-gradient-inequality)
    - [Mean-zero Sobolev space](#mean-zero-sobolev-space)
  - [Poincare inequality with a partial Dirichlet boundary](#poincare-inequality-with-a-partial-dirichlet-boundary)
  - [Poincare inequality with a boundary trace](#poincare-inequality-with-a-boundary-trace)
  - [Weighted Poincare inequality](#weighted-poincare-inequality)
    - [Ground-state transform for a weighted Dirichlet energy](#ground-state-transform-for-a-weighted-dirichlet-energy)
- [Sobolev derivative estimate](#sobolev-derivative-estimate)
  - [Periodic elliptic estimate](#periodic-elliptic-estimate)
- [Massive Laplacian isomorphism on Sobolev spaces](#massive-laplacian-isomorphism-on-sobolev-spaces)
  - [Constant-drift massive elliptic estimate](#constant-drift-massive-elliptic-estimate)
- [Compactness from bounded support and an H2 bound](#compactness-from-bounded-support-and-an-h2-bound)
- [Regularity gain for one plus an even power of the Laplacian](#regularity-gain-for-one-plus-an-even-power-of-the-laplacian)
- [Sobolev embedding theorem](#sobolev-embedding-theorem)
  - [Morrey's inequality](#morrey-s-inequality)
  - [Differentiability almost everywhere of supercritical Sobolev functions](#differentiability-almost-everywhere-of-supercritical-sobolev-functions)
  - [Morrey inequality on a cube](#morrey-inequality-on-a-cube)
  - [Failure of first-order Sobolev embedding into Linfinity in two dimensions](#failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions)
  - [Sobolev inequality](#sobolev-inequality)
    - [Sobolev–Gallagher inequality](#sobolev-gallagher-inequality)
    - [H1 L3 interpolation inequality in three dimensions](#h1-l3-interpolation-inequality-in-three-dimensions)
    - [Hardy inequality in Euclidean space](#hardy-inequality-in-euclidean-space)
    - [Sobolev conjugate exponent](#sobolev-conjugate-exponent)
  - [Gagliardo-Nirenberg interpolation inequality](#gagliardo-nirenberg-interpolation-inequality)
  - [Rellich-Kondrachov theorem](#rellich-kondrachov-theorem)
    - [Failure of Rellich compactness on an unbounded domain](#failure-of-rellich-compactness-on-an-unbounded-domain)
    - [Rellich-Kondrashov compactness theorem for H01](#rellich-kondrashov-compactness-theorem-for-h01)
      - [Zero extension of H01](#zero-extension-of-h01)
      - [High-frequency control by a Sobolev derivative](#high-frequency-control-by-a-sobolev-derivative)
      - [Fourier proof of Rellich compactness](#fourier-proof-of-rellich-compactness)
      - [Weak lower semicontinuity of a bounded-domain Schrodinger energy](#weak-lower-semicontinuity-of-a-bounded-domain-schrodinger-energy)
        - [Constrained ground-state minimizer on a bounded domain](#constrained-ground-state-minimizer-on-a-bounded-domain)
      - [Local compactness plus uniform tail control](#local-compactness-plus-uniform-tail-control)
        - [Strong convergence from weak convergence and tightness](#strong-convergence-from-weak-convergence-and-tightness)
  - [Noncompactness of a Sobolev embedding by translation](#noncompactness-of-a-sobolev-embedding-by-translation)
    - [Loss of compactness at infinity](#loss-of-compactness-at-infinity)
    - [Vanishing Dirichlet energy by dilation on the line](#vanishing-dirichlet-energy-by-dilation-on-the-line)
  - [Hölder condition](#holder-condition)
    - [Hölder space](#holder-space)
      - [Hölder-Taylor remainder bound](#holder-taylor-remainder-bound)
        - [Wavelet coefficient decay for Hölder functions](#wavelet-coefficient-decay-for-holder-functions)
      - [Hölder norm](#holder-norm)
      - [Hölder seminorm](#holder-seminorm)
        - [Lower semicontinuity of a Hölder seminorm](#lower-semicontinuity-of-a-holder-seminorm)
      - [Hölder class](#holder-class)
      - [Hölder interpolation inequality](#holder-interpolation-inequality)
      - [Compact embedding of Hölder spaces](#compact-embedding-of-holder-spaces)
      - [Fourier proof of Hölder regularity from a Sobolev norm](#fourier-proof-of-holder-regularity-from-a-sobolev-norm)
    - [Hölder exponent](#holder-exponent)
    - [Hölder exponent greater than one forces constancy](#holder-exponent-greater-than-one-forces-constancy)
    - [Hölder continuity of a one-dimensional fractional kernel integral](#holder-continuity-of-a-one-dimensional-fractional-kernel-integral)
    - [Derivative criterion for Hölder continuity up to a boundary](#derivative-criterion-for-holder-continuity-up-to-a-boundary)
- [Ladyzhenskaya's inequality](#ladyzhenskaya-s-inequality)
  - [Ladyzhenskaya inequality in two dimensions](#ladyzhenskaya-inequality-in-two-dimensions)
- [Morrey-Campanato space](#morrey-campanato-space)
  - [Campanato space](#campanato-space)
    - [Campanato iteration lemma](#campanato-iteration-lemma)

## Zero-trace Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

The zero-trace first-order [Sobolev space](sobolev-space.md) is the closure of $C_c^\infty(\Omega)$ in the $H^1$ norm. On a bounded Lipschitz domain it is the kernel of the [Sobolev trace operator](#trace-operator). On an interval, its elements have absolutely continuous representatives with both endpoint values zero. The [Poincaré inequality](#poincare-inequality) makes the derivative norm equivalent to the full Sobolev norm. This is the natural form domain for an elliptic problem with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition).

## Near-identity Sobolev loop factorization

↑ **Parent:** [Sobolev space](sobolev-space.md)

For matrix-valued circle loops in $H^s$, $s>1/2$, use a submultiplicative algebra norm with contractive Fourier projections. If $\|X-I\|<1$, solve $Y_+=I+y_+$ by $y_+=-P_{>0}((X-I)(I+y_+))$, and solve $V_-=I+v_-$ by $v_-=-P_{<0}((I+v_-)(X-I))$. Both are contractions. Then $XY_+$ has only nonpositive modes, $V_-X$ has only nonnegative modes, and their compatible products equal a constant matrix. Invertibility of the Hardy compression $I+P_{\geq0}(X-I)$ makes that constant invertible. This yields the stated normalized factors; uniqueness follows because the two Fourier subalgebras intersect in constants.

## Trace operator

↑ **Parent:** [Sobolev space](sobolev-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trace_operator)

On a bounded [Lipschitz domain](real-analysis.md#lipschitz-domain), the [Sobolev trace operator](#trace-operator) is the continuous linear extension to $H^1(\Omega)$ of the boundary restriction of smooth functions. Continuity and density make this extension unique; its existence is the [Sobolev trace theorem](#sobolev-trace-theorem). The kernel prescribes a homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition). Vanishing [Sobolev trace](#trace-operator) on only part of the boundary instead gives the form domain for a [mixed boundary condition](differential-equation.md#mixed-boundary-condition), with the natural [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) on the remainder. On an assembly of congruent tiles, taking a [Sobolev trace](#trace-operator) commutes with a constant matrix acting on the tile restrictions. This lets a [transplantation theorem](riemannian-geometry.md#transplantation-theorem) be proved on [quadratic form](linear-algebra.md#quadratic-form) domains even when corner eigenfunctions have singular classical derivatives.

### Sobolev trace theorem

↑ **Parent:** [Trace operator](#trace-operator)

This theorem describes the continuous extension of the [Trace operator](#trace-operator). For $s>1/2$, restriction to the coordinate hyperplane extends uniquely to a bounded linear map

$$
\gamma:H^s(\mathbb R^n)\longrightarrow H^{s-1/2}(\mathbb R^{n-1}).
$$

In Fourier variables, Cauchy--Schwarz bounds the integral over the normal frequency because $(1+t^2)^{-s}$ is integrable exactly when $s>1/2$.

#### Multiplicative trace inequality on a bounded smooth domain

↑ **Parent:** [Sobolev trace theorem](#sobolev-trace-theorem)

On a bounded smooth domain, the [Sobolev trace theorem](#sobolev-trace-theorem) can be strengthened to

$$
\|Tu\|_{L^2(\partial U)}^2\leq C\bigl(\|u\|_{L^2(U)}^2+\|u\|_{L^2(U)}\|Du\|_{L^2(U)}\bigr)
\leq C'\|u\|_{L^2(U)}\|u\|_{H^1(U)}.
$$

For smooth $u$, extend the outward unit normal to a smooth vector field $X$ near the closure of $U$ with $X\cdot\nu=1$ on its boundary. The [divergence theorem](calculus.md#divergence-theorem) gives $\int_{\partial U}u^2=\int_U(\operatorname{div}X)u^2+2uX\cdot Du$, and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives the estimate. Density extends it to $H^1(U)$. A bound containing only the product $\|u\|_2\|Du\|_2$ is false for nonzero constant functions. Equivalently, for every $\varepsilon>0$, the [Young inequality](nonlinear-analysis.md#young-s-inequality-for-products) gives $\|Tu\|_2^2\leq\varepsilon\|Du\|_2^2+C_\varepsilon\|u\|_2^2$.

#### W1p trace theorem on a half-space

↑ **Parent:** [Sobolev trace theorem](#sobolev-trace-theorem)

For $1\leq p<\infty$, boundary restriction on smooth functions extends uniquely to a bounded linear map $T:W^{1,p}(\mathbb R_+^n)\to L^p(\mathbb R^{n-1})$. The estimate follows by applying the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) on normal line segments and then integrating over the boundary variables.

#### Failure of an Lp hyperplane trace

↑ **Parent:** [Sobolev trace theorem](#sobolev-trace-theorem)

For $1\leq p<\infty$, no bounded map from $L^p(\mathbb R^n)$ to $L^p(\mathbb R^{n-1})$ can agree with restriction on continuous functions. Indeed,

$$
u_k(x',x_n)=\phi(x')\psi(kx_n),\qquad \psi(0)=1,
$$

has a fixed nonzero trace while $\lVert u_k\rVert_p=k^{-1/p}\lVert\phi\rVert_p\lVert\psi\rVert_p\to0$.

## Sobolev interpolation inequality

↑ **Parent:** [Sobolev space](sobolev-space.md)

For $a<b$ and $0\leq\theta\leq1$, the displayed estimate holds on Euclidean space and a [torus](topology.md#torus) with the Fourier definition of the [Sobolev norm](#sobolev-norm). In the squared norm, write the weighted squared Fourier coefficient as the product of its weight-$a$ value to the power $1-\theta$ and its weight-$b$ value to the power $\theta$. [Holder inequality](functional-analysis.md#holder-inequality) then proves the estimate. On a [compact manifold](differential-geometry.md#compact-manifold), a finite coordinate cover and a [partition of unity](differential-geometry.md#partition-of-unity) give the same estimate up to a constant. [Young inequality](nonlinear-analysis.md#young-s-inequality-for-products) implies the useful absorption form $\|u\|_{H^{s+1}}\leq\varepsilon\|u\|_{H^{s+2}}+C_{s,\varepsilon}\|u\|_2$ for nonnegative $s$.

## Interior cone property

↑ **Parent:** [Sobolev space](sobolev-space.md)

A domain has the uniform interior cone property if fixed-height, fixed-opening cones can be placed inside the domain at its points, with an allowed orientation depending on the point. This geometric regularity permits the [Sobolev embedding theorem](#sobolev-embedding-theorem) and [Rellich-Kondrachov compactness theorem](#rellich-kondrachov-theorem). It is an interior condition, distinct from the [exterior cone condition](analysis.md#exterior-cone-condition) used in boundary regularity.

## Clamped second-order Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

This is the closure of the compactly supported [test functions](distribution-theory.md#test-function) $C_c^\infty(U)$ in the $H^2(U)$ [norm](functional-analysis.md#norm). On a smooth bounded domain it consists precisely of the $H^2$ functions with zero value and zero [normal derivative](differential-geometry.md#normal-derivative) traces. Tangential first derivatives then vanish as well. The [clamped Hessian identity](#clamped-hessian-identity) makes the [Laplacian](calculus.md#laplacian) [norm](functional-analysis.md#norm) equivalent to the full $H^2$ [norm](functional-analysis.md#norm) on this space, enabling a [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) treatment of the [clamped biharmonic problem](calculus.md#clamped-biharmonic-problem).

### Clamped interval derivative norm bound

↑ **Parent:** [Clamped second-order Sobolev space](#clamped-second-order-sobolev-space)

For $v\in H_0^2(-1,1)$, integrate its [weak derivative](distribution-theory.md#weak-derivative) from the left endpoint, where $v=v'=0$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|v'\|_2\leq2\|v''\|_2$ and $\|v\|_2\leq2\|v'\|_2$. Adding the three squared derivative norms gives the displayed bound. The constant is sufficient, rather than asserted sharp. Thus the second-derivative norm is equivalent to the full [Sobolev norm](#sobolev-norm) on this clamped space.

### Weak formulation of a clamped fourth-order equation

↑ **Parent:** [Clamped second-order Sobolev space](#clamped-second-order-sobolev-space)

For continuous real coefficients with $p>0$ and $q,r\geq0$ on a bounded interval, use the [clamped second-order Sobolev space](#clamped-second-order-sobolev-space) and the displayed [bilinear form](linear-algebra.md#bilinear-form). A forcing in $L^2$ defines $\ell(v)=\int fv$. The [weak solution](partial-differential-equation.md#weak-solution) satisfies $a(u,v)=\ell(v)$ for every clamped test vector. Compactly supported [test functions](distribution-theory.md#test-function) give $(pu'')''-(qu')'+ru=f$ as a [distribution](distribution-theory.md#distribution-mathematical-analysis); density extends that equation to the energy space. Continuous coefficients alone do not justify differentiating them classically. The [clamped interval derivative norm bound](#clamped-interval-derivative-norm-bound) gives coercivity, so [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) supplies a unique solution and the quadratic energy has that unique minimum.

### Clamped Hessian identity

↑ **Parent:** [Clamped second-order Sobolev space](#clamped-second-order-sobolev-space)

For $u\in H_0^2(U)$, $\sum_{i,j}\|\partial_{ij}u\|_2^2=\|\Delta u\|_2^2$. Two [integrations by parts](calculus.md#integration-by-parts) prove this for compactly supported [test functions](distribution-theory.md#test-function), and $H^2$ density extends it to the [clamped second-order Sobolev space](#clamped-second-order-sobolev-space). Together with the [Poincare-Wirtinger inequality](#poincare-wirtinger-inequality) applied to the mean-zero first derivatives and the zero-boundary [Poincaré inequality](#poincare-inequality), it controls the full $H^2$ [norm](functional-analysis.md#norm) by $\|\Delta u\|_2$. The boundary conditions are essential to this exact identity on bounded domains.

## Homogeneous Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

A homogeneous Sobolev space controls derivatives without an independent low-frequency [L2 norm](real-analysis.md#l2-norm): formally $\|f\|_{\dot H^s}^2=\int |\xi|^{2s}|\widehat f(\xi)|^2\,d\xi$, with the normalization chosen according to the [Fourier transform](analysis.md#fourier-transform). Completions or quotient conventions must be specified when polynomial ambiguities occur. In three dimensions $\dot H^1$ is represented by $L^6$ functions with [gradient](calculus.md#gradient) in $L^2$, and $\|f\|_6\leq C\|\nabla f\|_2$.

## Gaussian Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

The first Gaussian Sobolev space consists of functions and their weak first [derivatives](calculus.md#derivative) square-integrable for standard [Gaussian measure](stochastic-process.md#gaussian-measure). If $f=\sum c_nh_n$ in the normalized [Probabilists' Hermite polynomial](numerical-analysis.md#probabilists-hermite-polynomial) basis, [Gaussian integration by parts](probability-theory.md#stein-s-lemma-probability) gives $\langle f',h_{n-1}\rangle=\sqrt n c_n$. Thus [Parseval identity](fourier-analysis.md#parseval-identity) identifies it with $\sum(1+n)|c_n|^2<\infty$, and polynomial truncations converge in its norm. It is the form domain of the [Gaussian number operator](functional-analysis.md#gaussian-number-operator), with [Gaussian Dirichlet energy](functional-analysis.md#gaussian-dirichlet-energy) $\sum n|c_n|^2$.

## Sobolev norm

↑ **Parent:** [Sobolev space](sobolev-space.md)

For $1\leq p<\infty$, an inhomogeneous [Sobolev space](sobolev-space.md) [norm](functional-analysis.md#norm) is $\|u\|_{W^{k,p}(D)}=(\sum_{|\alpha|\leq k}\|D^\alpha u\|_{L^p(D)}^p)^{1/p}$, using [weak derivatives](distribution-theory.md#weak-derivative). In particular, $\|u\|_{H^1(D)}^2=\int_D(|u|^2+|\nabla u|^2)$. The [gradient](calculus.md#gradient) seminorm alone defines a different completion, the [Dirichlet energy space](#dirichlet-energy-space), unless a suitable [Poincaré inequality](#poincare-inequality) makes the two norms equivalent on the chosen zero-boundary space.

## Sobolev multiplication by a smooth cutoff

↑ **Parent:** [Sobolev space](sobolev-space.md)

Multiplication by a [test function](distribution-theory.md#test-function) is bounded on every real-index [Sobolev space](sobolev-space.md). Its [Fourier transform](analysis.md#fourier-transform) acts by convolution with a [Schwartz function](fourier-analysis.md#schwartz-function); frequency-weight estimates and [Young's convolution inequality](fourier-analysis.md#young-s-convolution-inequality) give the norm bound.

## Sobolev duality

↑ **Parent:** [Sobolev space](sobolev-space.md)

The continuous [dual space](linear-algebra.md#dual-space) of $H^s(\mathbb R^d)$ is $H^{-s}(\mathbb R^d)$ under the extension of the [L2 inner product](measure-theory.md#l2-inner-product). The [Fourier transform](analysis.md#fourier-transform) definition $\|f\|_{H^s}^2=\int(1+|\xi|^2)^s|\widehat f(\xi)|^2d\xi$ proves boundedness of the pairing by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), and the [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem) proves that every continuous functional has this form. Consequently a bounded [linear operator](vector-space.md#linear-operator) $K:H^r\to H^{r+a}$ has an [adjoint operator](hilbert-space.md#adjoint-operator), relative to this pairing, from $H^{-r-a}$ to $H^{-r}$. For an operator that smooths by two orders for every $r$, this yields $K^*:H^2\to H^4$ by taking $r=-4$.

## Sobolev fundamental theorem of calculus on lines

↑ **Parent:** [Sobolev space](sobolev-space.md)

If $u\in W^{1,p}(U)$, then after modification on a null set its restriction to almost every line parallel to a coordinate axis is absolutely continuous and satisfies

$$
u(x+he_i)-u(x)=\int_0^hD_i u(x+se_i)\,ds
$$

whenever the line segment lies in $U$.

### Sobolev slicing and planar continuity

↑ **Parent:** [Sobolev fundamental theorem of calculus on lines](#sobolev-fundamental-theorem-of-calculus-on-lines)

For $u\in W^{1,q}((0,1)^2)$ with $q>1$, almost every coordinate-line slice has an absolutely continuous representative and is [Hölder continuous](#holder-condition) with exponent $1-1/q$. Slice bounds need not be uniform. Global [Hölder continuity](#holder-condition) follows from [Morrey's inequality](#morrey-s-inequality) only when $q>2$, with exponent $1-2/q$; unbounded examples exist at and below $q=2$.

## Sobolev algebra

↑ **Parent:** [Sobolev space](sobolev-space.md)

On a sufficiently regular domain in $\mathbb R^n$, $H^s$ is a Banach algebra when $s>n/2$:

$$
\|uv\|_{H^s}\leq C\|u\|_{H^s}\|v\|_{H^s}.
$$

### Tame Sobolev product estimate

↑ **Parent:** [Sobolev algebra](#sobolev-algebra)

For an integer $k\geq0$ and sufficiently regular bounded functions, $\|fg\|_{H^k}\leq C_k(\|f\|_\infty\|g\|_{H^k}+\|g\|_\infty\|f\|_{H^k})$. The [Leibniz rule](calculus.md#leibniz-rule) and derivative interpolation give the estimate. In a differentiated [semilinear wave equation](wave-equation.md#semilinear-wave-equation), this separates a controlled low-order coefficient from an arbitrarily high [Sobolev norm](#sobolev-norm), allowing propagation of smoothness after a fixed base norm has been controlled.

## Periodic Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

The periodic Sobolev space $H^s(\mathbb T^d)$ consists of periodic distributions whose Fourier coefficients obey

$$
\sum_{n\in\mathbb Z^d}(1+|n|^2)^s|\widehat u_n|^2<\infty.
$$

In one dimension, $H^1(\mathbb T)$ embeds continuously into $L^\infty(\mathbb T)$ and is a Banach algebra.

## Local Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

A distribution $u$ on an open set $X$ belongs to $H^s_{\mathrm{loc}}(X)$ when $\chi u\in H^s(\mathbb R^n)$ for every test function $\chi\in C_c^\infty(X)$.

## First-order Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

For an open set $U\subseteq\mathbb R^n$ and $1\leq p\leq\infty$, the first-order Sobolev space is

$$
W^{1,p}(U)=\{u\in L^p(U):D_i u\in L^p(U)\text{ for }1\leq i\leq n\},
$$

where each $D_i u$ is a [weak derivative](distribution-theory.md#weak-derivative). Its standard norm is $\|u\|_{W^{1,p}}=\|u\|_p+\sum_i\|D_i u\|_p$.

### Sobolev gradient vanishes on a zero set

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

For a [Sobolev space](sobolev-space.md) function, almost every line parallel to a coordinate axis gives an absolutely continuous restriction. An absolutely continuous function has [derivative](calculus.md#derivative) zero [almost everywhere](measure-theory.md#almost-everywhere) on each of its level sets. Slicing and [Fubini's theorem](measure-theory.md#fubini-s-theorem) give the assertion in higher dimension. If $w\in W^{2,p}$, apply it to $w$ and then to each component of its [gradient](calculus.md#gradient) to get $D^2w=0$ [almost everywhere](measure-theory.md#almost-everywhere) on $\{w=0\}$. This supplies the contact differentiation used in [noncontact of ROF level boundaries](inverse-problem.md#noncontact-of-rof-level-boundaries).

### Sobolev function with zero weak gradient

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

On a connected open set, a [Sobolev space](sobolev-space.md) function with zero [weak gradient](distribution-theory.md#weak-gradient) is constant almost everywhere. Local [mollification](distribution-theory.md#mollification) gives constant smooth representatives on interior balls; overlaps and connectedness identify their constants. Without connectedness, the constant may differ between components. This explains the constant ambiguity in a [Neumann Poisson problem](partial-differential-equation.md#neumann-poisson-problem).

### H1 space

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

The H1 space is the [first-order Sobolev space](#first-order-sobolev-space) whose elements and first [weak derivatives](distribution-theory.md#weak-derivative) belong to [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). It is a [Hilbert space](hilbert-space.md) with inner product given by the sum of the [L2 inner products](measure-theory.md#l2-inner-product) of the functions and of their first [weak derivatives](distribution-theory.md#weak-derivative).

### Sobolev characterization by bounded difference quotients

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

For $f\in H^1(\mathbb R)$, its [difference quotient](calculus.md#difference-quotient) equals $D_hf=\int_0^1f'(\cdot+\theta h)\,d\theta$ in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). Thus $\|D_hf\|_2\leq\|f'\|_2$, and [translation of a function](function.md#translation-of-a-function) gives $D_hf\to f'$ in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). Conversely, bounded difference quotients have a weakly convergent subsequence as $h\to0$. Against a [test function](distribution-theory.md#test-function), $\int D_hf\,v\to-\int f v'$, so that weak limit is the [weak derivative](distribution-theory.md#weak-derivative) of $f$. It lies in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), which is precisely the [first-order Sobolev space](#first-order-sobolev-space) condition.

### Zero-boundary Sobolev space

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

The zero-boundary Sobolev space $H_0^1(U)$ is the closure of the [space of test functions](distribution-theory.md#space-of-test-functions) $C_c^\infty(U)$ in $H^1(U)$. Under standard regularity assumptions its elements have zero boundary trace.

#### No uniformly positive coefficient in a zero-boundary Sobolev space

↑ **Parent:** [Zero-boundary Sobolev space](#zero-boundary-sobolev-space)

On a nonempty bounded domain where the [Poincaré inequality](#poincare-inequality) holds, no $a\in H_0^1(\Omega)$ can satisfy $a\geq a_->0$ almost everywhere. For $g(s)=\min(\max(s,0),a_-)$, [Lipschitz truncation preserves zero-boundary Sobolev spaces](#lipschitz-truncation-preserves-zero-boundary-sobolev-spaces), so $g(a)\in H_0^1(\Omega)$. But $g(a)$ would be the nonzero constant $a_-$, whose zero gradient contradicts the [Poincaré inequality](#poincare-inequality). In a uniformly elliptic [divergence-form elliptic operator](elliptic-boundary-value-problem.md#divergence-form-elliptic-operator), the homogeneous boundary condition belongs to the unknown and test functions, not to a coefficient bounded below by a positive constant.

#### Lipschitz truncation preserves zero-boundary Sobolev spaces

↑ **Parent:** [Zero-boundary Sobolev space](#zero-boundary-sobolev-space)

If $v\in H_0^1(\Omega)$ and $g:\mathbb R\to\mathbb R$ is [Lipschitz continuous](real-analysis.md#lipschitz-continuity) with $g(0)=0$, then $g(v)\in H_0^1(\Omega)$. The Lipschitz version of the [Sobolev chain rule](distribution-theory.md#sobolev-chain-rule) controls its [weak derivatives](distribution-theory.md#weak-derivative), and its boundary trace is $g(0)=0$. Equivalently, approximate $v$ by compactly supported smooth functions, apply the derivative bound to their compositions, and pass weakly in $H^1$ and strongly in $L^2$. The closed linear space $H_0^1$ is weakly closed. This allows positive-part and bounded truncations in weak formulations without losing the [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition).

#### Dirichlet inner product

↑ **Parent:** [Zero-boundary Sobolev space](#zero-boundary-sobolev-space)

On a domain $U\subseteq\mathbb R^n$, a common normalization of the Dirichlet inner product is

$$
(f,g)_\nabla=\frac1{2\pi}\int_U\nabla f(x)\mathbin\cdot\nabla g(x)\,dx.
$$

The [Poincaré inequality](#poincare-inequality) makes its induced seminorm a norm on $H_0^1(U)$.

##### Conformal invariance of the planar Dirichlet inner product

↑ **Parent:** [Dirichlet inner product](#dirichlet-inner-product)

For a [conformal bijection](complex-analysis.md#biholomorphism) $f:D\to\widetilde D$ and [smooth](analysis.md#smooth-function) $u,v$ of [compact support](function.md#compact-support) on $\widetilde D$, $\boxed{(u\circ f,v\circ f)_{\nabla,D}=(u,v)_{\nabla,\widetilde D}}$. The [Jacobian matrix](calculus.md#jacobian-matrix) of $f$ is a rotation times $|f'|$. Consequently the [chain rule](calculus.md#chain-rule) introduces $|f'|^2$ into the [gradient](calculus.md#gradient) pairing, while the [change of variables formula](calculus.md#change-of-variables-formula) introduces precisely the same factor into area. They cancel. The identity extends by completion to the [Dirichlet energy spaces](#dirichlet-energy-space); it does not preserve the $L^2$ term of an inhomogeneous [Sobolev norm](#sobolev-norm).

##### Dirichlet energy space

↑ **Parent:** [Dirichlet inner product](#dirichlet-inner-product)

For planar [Gaussian free field](stochastic-process.md#gaussian-free-field) theory, this is the completion of real [test functions](distribution-theory.md#test-function) $C_c^\infty(D)$ in the norm induced by the [Dirichlet inner product](#dirichlet-inner-product), $(f,g)_\nabla=(2\pi)^{-1}\int_D\nabla f\cdot\nabla g$. On a general unbounded domain this convention must be distinguished from completion in the inhomogeneous $H^1$ norm. A [conformal map](geometry-and-topology.md#conformal-map) identifies its energy norm with that on the unit disc by conformal invariance.

###### Orthogonality of supported and harmonic Dirichlet functions

↑ **Parent:** [Dirichlet energy space](#dirichlet-energy-space)

Let $U\subseteq D$ be open. Regard $H_{\mathrm{supp}}=H_0^1(U)$ as functions on $D$ by [zero extension of H01](#zero-extension-of-h01), and let $H_{\mathrm{harm}}$ consist of the [weakly harmonic Sobolev functions](partial-differential-equation.md#weakly-harmonic-sobolev-function) on $U$ belonging to $H_0^1(D)$. For $h\in H_{\mathrm{harm}}$, the [Dirichlet inner product](#dirichlet-inner-product) $(h,\phi)_\nabla$ vanishes for each [test function](distribution-theory.md#test-function) supported in $U$. Approximate any $u\in H_{\mathrm{supp}}$ by those [test functions](distribution-theory.md#test-function) in the [gradient](calculus.md#gradient) [norm](functional-analysis.md#norm) and use the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). This gives $\boxed{(h,u)_\nabla=0}$. The proof also works with the inhomogeneous [zero-boundary Sobolev space](#zero-boundary-sobolev-space) convention, and with a homogeneous completion realized as weak functions.

### One-dimensional Sobolev representative

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

Every element of $W^{1,p}(a,b)$ for $1\leq p<\infty$ has an [absolutely continuous](#absolutely-continuous-function) representative. Its ordinary derivative exists [almost everywhere](measure-theory.md#almost-everywhere), equals its [weak derivative](distribution-theory.md#weak-derivative), and belongs to $L^p(a,b)$.

#### Interval Sobolev supremum estimate

↑ **Parent:** [One-dimensional Sobolev representative](#one-dimensional-sobolev-representative)

On $I=(-a,a)$, a [first-order Sobolev space](#first-order-sobolev-space) function has a continuous representative and obeys

$$
\|u\|_\infty\le(2a)^{-1/2}\|u\|_2+\sqrt{2a}\|u'\|_2\le\sqrt{(2a)^{-1}+2a}\,\|u\|_{H^1(I)}.
$$

Bound the average by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and average the identity $u(x)-u(y)=\int_y^xu'$. This also gives $[u]_{C^{0,1/2}}\le\|u'\|_2$. A unit constant with the standard [Sobolev norm](#sobolev-norm) cannot be asserted on arbitrary interval lengths: $u=1$ already disproves it when $2a<1$.

### Density of smooth functions in a Sobolev space

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

For every open set $U\subseteq\mathbb R^n$, smooth functions in $U$ are dense in $W^{1,p}(U)$ for $1\leq p<\infty$. Near a flat boundary, one may first translate the function into the domain and then apply a [mollifier](distribution-theory.md#mollifier).

### Zero extension of W01

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)

By the definition of $W_0^{1,p}(U)$ as the closure of $C_c^\infty(U)$, extending a function by zero outside $U$ gives a bounded map into $W^{1,p}(\mathbb R^n)$ and does not create a boundary distribution.

### Sobolev extension operator

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sobolev_extension_operator)

A Sobolev extension operator is a bounded linear map $E:W^{1,p}(U)\to W^{1,p}(\mathbb R^n)$ whose restriction to $U$ is the original function. For a half-space, reflection across the boundary gives such an operator.

#### Reflection extension from a half-space

↑ **Parent:** [Sobolev extension operator](#sobolev-extension-operator)

For $U=(0,\infty)\times\mathbb R^{n-1}$, the formula $Eu(x_1,x')=u(|x_1|,x')$ defines a bounded [Sobolev extension operator](#sobolev-extension-operator). Its weak normal derivative changes sign across the boundary, while its tangential weak derivatives are reflected unchanged.

##### Odd reflection

↑ **Parent:** [Reflection extension from a half-space](#reflection-extension-from-a-half-space)

The odd reflection of a function on a half-space is $Eu(x',x_n)=\operatorname{sgn}(x_n)u(x',|x_n|)$. When $u$ has zero trace on the boundary, this extension preserves the relevant weak regularity and often converts a homogeneous boundary problem into an interior problem.

### Absolutely continuous function

↑ **Parent:** [First-order Sobolev space](#first-order-sobolev-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absolutely_continuous_function)

A function $f:[a,b]\to\mathbb R$ is absolutely continuous exactly when there is a function $g\in L^1(a,b)$ such that

$$
f(x)=f(a)+\int_a^x g(s)\,ds.
$$

Then $f$ is [differentiable](analysis.md#differentiable-function) [almost everywhere](measure-theory.md#almost-everywhere) and $f'=g$ almost everywhere.

#### Dyadic slope-tail criterion for absolute continuity

↑ **Parent:** [Absolutely continuous function](#absolutely-continuous-function)

For a [continuous function](calculus.md#continuous-function) $f$ on $[0,1]$, let $G_n$ be its [dyadic slope martingale](martingale.md#dyadic-slope-martingale). Then $f$ is an [absolutely continuous function](#absolutely-continuous-function) if and only if

$$
\lim_{\lambda\to\infty}\sup_n\int_0^1|G_n(t)|\mathbf1_{\{|G_n(t)|\geq\lambda\}}dt=0.
$$

This is exactly [uniform integrability](convergence-of-random-variables.md#uniform-integrability). The [uniformly integrable martingale convergence theorem](martingale.md#uniformly-integrable-martingale-convergence-theorem) gives [convergence in L1](convergence-of-random-variables.md#convergence-in-l1) $G_n\to g$, while their integrated [linear interpolations](function.md#linear-interpolation) converge uniformly to $f$. Hence $f(x)=f(0)+\int_0^xg$. Conversely, if $f$ has density $g\in L^1$, its slopes are $\mathbb E[g\mid\mathcal F_n]$, and the [uniform integrability of conditional expectations](convergence-of-random-variables.md#uniform-integrability-of-conditional-expectations) proves the criterion. The dyadic tail [integral](calculus.md#integral) is also the sum of the absolute endpoint increments in cells whose slope is at least $\lambda$ in magnitude.

## Sobolev space with a partial Dirichlet condition

↑ **Parent:** [Sobolev space](sobolev-space.md)

For a boundary portion $\Gamma_D\subseteq\partial U$, the space

$$
V=\{v\in H^1(U):\operatorname{Tr}v|_{\Gamma_D}=0\}
$$

is the kernel of the restricted [trace map](#sobolev-trace-theorem), hence a [closed vector subspace](vector-space.md#closed-vector-subspace) of $H^1(U)$.

## Affine Sobolev space

↑ **Parent:** [Sobolev space](sobolev-space.md)

For prescribed boundary data $\varphi$, the affine Sobolev space

$$
\varphi+W_0^{1,p}(\Omega)
$$

consists of the $W^{1,p}$ functions whose [trace](#sobolev-trace-theorem) equals the trace of $\varphi$. It is the natural admissible set for a variational [Dirichlet problem](analysis.md#dirichlet-problem).

### Homogenization of Dirichlet boundary data

↑ **Parent:** [Affine Sobolev space](#affine-sobolev-space)

To solve a linear [Dirichlet problem](analysis.md#dirichlet-problem) with boundary value $g$, choose a sufficiently regular extension $G$ whose [trace](#sobolev-trace-theorem) is $g$ and write $v=w+G$. Then $w$ has zero trace, while moving the known term $LG$ to the right-hand side turns the equation $Lv=f$ into the homogeneous-boundary problem $Lw=f-LG$.

## Hardy operator

↑ **Parent:** [Sobolev space](sobolev-space.md)

The Hardy operator is the averaging operator

$$
Au(x)=\frac1x\int_0^xu(t)\,dt
$$

on functions over the positive half-line or an interval beginning at zero.

### Hardy averaging inequality

↑ **Parent:** [Hardy operator](#hardy-operator)

For $1<p<\infty$, the [Hardy operator](#hardy-operator) is bounded on $L^p(0,1)$ with operator norm at most $p/(p-1)$.

#### Hardy inequality on an interval

↑ **Parent:** [Hardy averaging inequality](#hardy-averaging-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hardy_inequality_on_an_interval)

If $u\in W^{1,p}(0,1)$ has zero [trace](#sobolev-trace-theorem) at zero, then

$$
\left\|\frac ux\right\|_{L^p(0,1)}
\leq\frac p{p-1}\|u'\|_{L^p(0,1)}.
$$

Indeed, the [one-dimensional Sobolev representative](#one-dimensional-sobolev-representative) satisfies $u(x)=\int_0^xu'(t)\,dt$, so the claim is the [Hardy averaging inequality](#hardy-averaging-inequality) applied to $u'$.

<h2 id="poincare-inequality">Poincaré inequality</h2>

↑ **Parent:** [Sobolev space](sobolev-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_inequality)

A Poincare inequality controls a function by its derivatives after the constant ambiguity has been removed. For example, on a bounded connected Lipschitz domain,

$$
\lVert u-u_U\rVert_{L^2(U)}\leq C\lVert\nabla u\rVert_{L^2(U)}.
$$

### Poincare inequality with a positive-measure zero set

↑ **Parent:** [Poincaré inequality](#poincare-inequality)

Suppose $u\in W^{1,2}(B_R)$ vanishes on a measurable subset of measure at least $\theta|B_R|$, with $\theta>0$. Writing $m$ for its mean, the zero set gives $\theta|B_R|m^2\leq\int_{B_R}|u-m|^2$. Thus $\int u^2\leq(1+\theta^{-1})\int|u-m|^2$, and the [Poincare-Wirtinger inequality](#poincare-wirtinger-inequality) supplies the displayed estimate. An elementary proof of that inequality on a ball bounds differences along line segments and splits the segment parameter at $1/2$, giving the valid explicit constant $C(n,\theta)=2^{n+1}(1+\theta^{-1})$. The change of scale from the unit ball multiplies the constant by $R^2$.

### Poincare inequality on an annulus

↑ **Parent:** [Poincaré inequality](#poincare-inequality)

For $n\geq2$, a round [annulus](topology.md#annulus-mathematics) $A_R=B_{2R}\setminus B_R$ is [connected](geometry-and-topology.md#connected-space) and obeys $\int_{A_R}|v-v_{A_R}|^2\leq C(n)R^2\int_{A_R}|\nabla v|^2$. Scaling reduces the claim to a fixed [annulus](topology.md#annulus-mathematics). In dimension one the [annulus](topology.md#annulus-mathematics) has two components, so the inequality fails with a single average; one needs a separate average on each component.

### Poincare-Wirtinger inequality

↑ **Parent:** [Poincaré inequality](#poincare-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincare-Wirtinger_inequality)

On a bounded connected Lipschitz domain $U$, every $u\in H^1(U)$ satisfies

$$
\|u-u_U\|_{L^2(U)}\leq C\|\nabla u\|_{L^2(U)},
\qquad
u_U=\frac1{|U|}\int_Uu.
$$

Equivalently, the gradient norm is equivalent to the $H^1$ norm on the [mean-zero Sobolev space](#mean-zero-sobolev-space).

#### Cube mean-gradient inequality

↑ **Parent:** [Poincare-Wirtinger inequality](#poincare-wirtinger-inequality)

For the cube $Q=(0,L)^n$ and $u\in H^1(Q)$,

$$
\|u\|_{L^2(Q)}^2
\leq |Q|u_Q^2+\frac n2L^2\|Du\|_{L^2(Q)}^2,
\qquad
u_Q=\frac1{|Q|}\int_Qu.
$$

This follows from the pairwise-difference identity

$$
\int_Q|u-u_Q|^2=\frac1{2|Q|}\int_Q\int_Q|u(x)-u(y)|^2\,dx\,dy
$$

and a coordinate-by-coordinate path from $x$ to $y$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds the squared sum of its $n$ increments by $n$ times the sum of their squares, while the one-dimensional [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) bounds each integrated increment by $L^{n+2}\|D_i u\|_2^2$. Division by $2|Q|=2L^n$ gives the stated constant.

#### Mean-zero Sobolev space

↑ **Parent:** [Poincare-Wirtinger inequality](#poincare-wirtinger-inequality)

The mean-zero Sobolev space is the closed subspace

$$
H^1_\dagger(U)=\left\{u\in H^1(U):\int_Uu=0\right\}.
$$

On a bounded connected Lipschitz domain, the [Poincare-Wirtinger inequality](#poincare-wirtinger-inequality) makes $\|\nabla u\|_2$ an equivalent Hilbert norm on this space.

### Poincare inequality with a partial Dirichlet boundary

↑ **Parent:** [Poincaré inequality](#poincare-inequality)

If $U$ is bounded and connected and a boundary portion $\Gamma_D$ has positive surface measure, then

$$
\lVert v\rVert_{L^2(U)}\leq C\lVert\nabla v\rVert_{L^2(U)}
$$

for every $v\in H^1(U)$ whose [trace](#sobolev-trace-theorem) vanishes on $\Gamma_D$. Otherwise a normalized counterexample sequence, the [Rellich-Kondrashov compactness theorem](#rellich-kondrashov-compactness-theorem-for-h01), and continuity of the trace would produce a nonzero constant with zero trace on $\Gamma_D$.

### Poincare inequality with a boundary trace

↑ **Parent:** [Poincaré inequality](#poincare-inequality)

On a bounded connected Lipschitz domain $U$,

$$
\|u\|_{L^2(U)}\leq C\left(\|Du\|_{L^2(U)}+\|\operatorname{Tr}u\|_{L^2(\partial U)}\right)
$$

for every $u\in H^1(U)$. If this failed, the [Rellich-Kondrachov compactness theorem](#rellich-kondrachov-theorem) would produce a normalized strong $L^2$ limit with zero [gradient](calculus.md#gradient), hence a [constant function](function.md#constant-function); continuity of the [Sobolev trace theorem](#sobolev-trace-theorem) would force that constant to vanish, contradicting its unit [norm](functional-analysis.md#norm).

### Weighted Poincare inequality

↑ **Parent:** [Poincaré inequality](#poincare-inequality)

For a [probability density function](continuous-probability-distribution.md#probability-density-function) $w$ on a domain, a weighted Poincare inequality has the form

$$
\int|h'|^2w\geq\lambda\int|h-\mathbb E_w h|^2w.
$$

The optimal $\lambda$ is the [spectral gap](linear-operator-theory.md#spectral-gap) of the associated weighted diffusion operator.

#### Ground-state transform for a weighted Dirichlet energy

↑ **Parent:** [Weighted Poincare inequality](#weighted-poincare-inequality)

For $w=e^{-\Phi}$ and $g=he^{-\Phi/2}$, [integration by parts](calculus.md#integration-by-parts) gives

$$
\int|h'|^2e^{-\Phi}
=\int|g'|^2+\int\left(\frac{|\Phi'|^2}{4}-\frac{\Phi''}{2}\right)|g|^2.
$$

This conjugates the weighted Dirichlet energy to a [Schrödinger operator](physics.md#schrodinger-operator) with effective potential $|\Phi'|^2/4-\Phi''/2$.

## Sobolev derivative estimate

↑ **Parent:** [Sobolev space](sobolev-space.md)

For every multi-index $\alpha$ and real $s$,

$$
\|D^\alpha u\|_{H^{s-|\alpha|}}
\leq\|u\|_{H^s}.
$$

This follows from the Fourier multiplier $(i\xi)^\alpha$.

### Periodic elliptic estimate

↑ **Parent:** [Sobolev derivative estimate](#sobolev-derivative-estimate)

If a periodic function $u$ has zero mean, its nonzero Fourier frequencies give

$$
\|u\|_{H^{s+2}}\leq C\|-\Delta u\|_{H^s}.
$$

Thus inversion of the Laplacian on mean-zero periodic functions gains two [Sobolev derivatives](sobolev-space.md).

## Massive Laplacian isomorphism on Sobolev spaces

↑ **Parent:** [Sobolev space](sobolev-space.md)

For every real $s$,

$$
-\Delta+1:H^{s+2}(\mathbb R^n)\to H^s(\mathbb R^n)
$$

is an isomorphism. Its inverse is the Fourier multiplier $(1+|\xi|^2)^{-1}$.

### Constant-drift massive elliptic estimate

↑ **Parent:** [Massive Laplacian isomorphism on Sobolev spaces](#massive-laplacian-isomorphism-on-sobolev-spaces)

For real $m\ne0$ and constant real $\alpha$, the Fourier symbol of $-\Delta-\alpha\cdot\nabla+m^2$ has modulus at least $|\xi|^2+m^2$. Its inverse therefore maps $L^2$ into $H^2$ with norm at most $\max(1,m^{-2})$, uniformly in the drift.

## Compactness from bounded support and an H2 bound

↑ **Parent:** [Sobolev space](sobolev-space.md)

A sequence bounded in $H^2(\mathbb R^n)$ whose members are supported in one bounded set has a subsequence converging strongly in $H^1(\mathbb R^n)$. Apply Rellich compactness simultaneously to the functions and their first derivatives.

## Regularity gain for one plus an even power of the Laplacian

↑ **Parent:** [Sobolev space](sobolev-space.md)

If $(\Delta^m+1)u=f$ distributionally on $\mathbb R^n$, $m$ is even, and $f\in H^r$, then

$$
\widehat u(\xi)=\frac{\widehat f(\xi)}{1+|\xi|^{2m}}
$$

and $u\in H^{r+2m}(\mathbb R^n)$.

## Sobolev embedding theorem

↑ **Parent:** [Sobolev space](sobolev-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sobolev_embedding_theorem)

If $s>d/2$, then $H^s(\mathbb R^d)$ embeds continuously into bounded continuous functions.

<h3 id="morrey-s-inequality">Morrey's inequality</h3>

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)

For $d<p<\infty$, every [Sobolev space](sobolev-space.md) element $u\in W^{1,p}(\mathbb R^d)$ has a [Hölder continuous function](#holder-condition) representative of exponent $1-d/p$, with the displayed bound. It also satisfies $\|u\|_\infty\leq C_{d,p}(\|u\|_p+\|\nabla u\|_p)$. Averaging the [fundamental theorem of calculus along a line segment](calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) over a ball gives

$$
|u(x)-u_{B(x,r)}|\leq C_d\int_{B(x,r)}\frac{|\nabla u(z)|}{|x-z|^{d-1}}\,dz.
$$

The [Holder inequality](functional-analysis.md#holder-inequality) bounds this by $C_{d,p}r^{1-d/p}\|\nabla u\|_p$, because $(d-1)p'<d$. To compare two ball averages, translate a ball along the segment between their centres and use the same [fundamental theorem of calculus along a line segment](calculus.md#fundamental-theorem-of-calculus-along-a-line-segment). These bounds give the displayed estimate. [Density of smooth functions in a Sobolev space](#density-of-smooth-functions-in-a-sobolev-space) supplies the representative for nonsmooth $u$. For $p=\infty$, the corresponding conclusion is [Lipschitz continuity](real-analysis.md#lipschitz-continuity).

### Differentiability almost everywhere of supercritical Sobolev functions

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)

For $p>n$, the [Hölder continuous function](#holder-condition) representative $u^*$ of $u\in W^{1,p}(\mathbb R^n)$ has a classical [Fréchet derivative](calculus.md#frechet-derivative) at almost every point, equal to its [weak derivative](distribution-theory.md#weak-derivative). At a point $x$ where the $p$-mean oscillation of $Du$ tends to zero, apply the [Morrey inequality on a cube](#morrey-inequality-on-a-cube) to $u^*(y)-u^*(x)-Du(x)\cdot(y-x)$. On a cube of side comparable to $|y-x|$, its oscillation is at most

$$
C|y-x|\left(\frac1{|Q_r(x)|}\int_{Q_r(x)}|Du(z)-Du(x)|^p dz\right)^{1/p}=o(|y-x|).
$$

The required points have full measure by the [Lebesgue differentiation theorem](measure-theory.md#lebesgue-differentiation-theorem).

### Morrey inequality on a cube

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)

For a cube $Q$ of side length $r$ in $\mathbb R^n$, $p>n$, and a [continuously differentiable function](calculus.md#continuously-differentiable-function) $v$, its average $v_Q=|Q|^{-1}\int_Qv$ satisfies

$$
|v(y)-v_Q|\leq C_{n,p}r^{1-n/p}\|Dv\|_{L^p(Q)}\qquad(y\in Q).
$$

Averaging the [fundamental theorem of calculus along a line segment](calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) from $y$ to $z\in Q$ and changing variables gives $|v(y)-v_Q|\leq C_n\int_Q|Dv(w)|\,|w-y|^{1-n}dw$. The [Holder inequality](functional-analysis.md#holder-inequality) applies because $(n-1)p'<n$, and the kernel norm is $O(r^{1-n/p})$. Approximation extends the estimate to the continuous representative of a [Sobolev space](sobolev-space.md) function. On $\mathbb R^n$ it yields a [Hölder continuous function](#holder-condition) of exponent $1-n/p$ representing every $W^{1,p}$ class.

### Failure of first-order Sobolev embedding into Linfinity in two dimensions

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)

On a two-dimensional domain containing the origin, a logarithmic singularity such as $u(r)=(\log(1/r))^\alpha$ with $0<\alpha<1/2$ belongs locally to $H^1$ but is unbounded. Thus the critical first-order [Sobolev space](sobolev-space.md) does not embed into $L^\infty$.

### Sobolev inequality

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sobolev_inequality)

A Sobolev inequality bounds a function in one $L^q$ norm by its weak derivatives in another $L^p$ norm. In three dimensions, the first-order case $\|u\|_{L^6}\leq C\|\nabla u\|_{L^2}$ is the endpoint estimate behind the continuous embedding $H^1\hookrightarrow L^6$.

<h4 id="sobolev-gallagher-inequality">Sobolev–Gallagher inequality</h4>

↑ **Parent:** [Sobolev inequality](#sobolev-inequality)

For a [continuously differentiable function](calculus.md#continuously-differentiable-function) $F$ on an interval $I=[t-\delta/2,t+\delta/2]$,

$$
|F(t)|^2\leq\frac1\delta\int_I|F(u)|^2\,du+\int_I|F(u)F\prime(u)|\,du.
$$

To prove it, average $|F(t)|^2-|F(u)|^2$ over $u\in I$ using the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus). On either half of $I$, the resulting derivative kernel has [absolute value](real-analysis.md#absolute-value) at most $1/2$. Since $|(|F|^2)\prime|\leq2|FF\prime|$, the displayed bound follows.

#### H1 L3 interpolation inequality in three dimensions

↑ **Parent:** [Sobolev inequality](#sobolev-inequality)

On a bounded three-dimensional domain, interpolation between $L^2$ and the [Sobolev inequality](#sobolev-inequality) $H^1\hookrightarrow L^6$ gives

$$
\|u\|_{L^3}\leq C\|u\|_{L^2}^{1/2}\|u\|_{H^1}^{1/2}.
$$

#### Hardy inequality in Euclidean space

↑ **Parent:** [Sobolev inequality](#sobolev-inequality)

This spatial form of [Hardy's inequality](real-analysis.md#hardy-s-inequality) controls a singular weight by [derivatives](calculus.md#derivative). For $d\geq3$ and $u\in H^1(\mathbb R^d)$,

$$
\int_{\mathbb R^d}\frac{|u(x)|^2}{|x|^2}\,dx
\leq\frac{4}{(d-2)^2}\int_{\mathbb R^d}|\nabla u(x)|^2\,dx.
$$

#### Sobolev conjugate exponent

↑ **Parent:** [Sobolev inequality](#sobolev-inequality)

For $1\leq p<n$, the Sobolev conjugate exponent $p^*$ is defined by

$$
\frac1{p^*}=\frac1p-\frac1n,
\qquad
p^*=\frac{np}{n-p}.
$$

The first-order [Sobolev inequality](#sobolev-inequality) maps one derivative in $L^p(\mathbb R^n)$ to the function in $L^{p^*}(\mathbb R^n)$.

### Gagliardo-Nirenberg interpolation inequality

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gagliardo-Nirenberg_interpolation_inequality)

The Gagliardo-Nirenberg interpolation inequalities bound an intermediate derivative norm by powers of a higher derivative norm and a lower norm. In two dimensions, one useful case is

$$
\|\nabla f\|_4^2\leq C\|\nabla f\|_2\|D^2f\|_2.
$$

### Rellich-Kondrachov theorem

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rellich–Kondrachov_theorem)

On a bounded Lipschitz domain $\Omega\subset\mathbb R^d$, the Sobolev embedding $W^{1,p}(\Omega)\hookrightarrow L^q(\Omega)$ is compact whenever $q$ lies strictly below the critical Sobolev exponent.

#### Failure of Rellich compactness on an unbounded domain

↑ **Parent:** [Rellich-Kondrachov theorem](#rellich-kondrachov-theorem)

Translations of one nonzero compactly supported smooth function have equal $W^{1,p}$ norms. On an unbounded domain they can have pairwise disjoint supports, so their mutual $L^p$ distances stay fixed and no subsequence converges in $L^p$.

#### Rellich-Kondrashov compactness theorem for H01

↑ **Parent:** [Rellich-Kondrachov theorem](#rellich-kondrachov-theorem)

This is the zero-boundary special case of the [Rellich-Kondrachov theorem](#rellich-kondrachov-theorem). For every bounded open $\Omega\subset\mathbb R^d$, the inclusion $H_0^1(\Omega)\hookrightarrow L^2(\Omega)$ is compact.

##### Zero extension of H01

↑ **Parent:** [Rellich-Kondrashov compactness theorem for H01](#rellich-kondrashov-compactness-theorem-for-h01)

By the definition of $H_0^1(\Omega)$ as the closure of compactly supported smooth functions, extension by zero maps it continuously into $H^1(\mathbb R^d)$ without creating a boundary distribution.

##### High-frequency control by a Sobolev derivative

↑ **Parent:** [Rellich-Kondrashov compactness theorem for H01](#rellich-kondrashov-compactness-theorem-for-h01)

For $u\in H^1(\mathbb R^d)$, Plancherel gives

$$
\int_{|\xi|>R}|\widehat u(\xi)|^2\,d\xi
\leq R^{-2}\lVert\nabla u\rVert_2^2.
$$

##### Fourier proof of Rellich compactness

↑ **Parent:** [Rellich-Kondrashov compactness theorem for H01](#rellich-kondrashov-compactness-theorem-for-h01)

Weak convergence on a bounded domain gives pointwise convergence of Fourier transforms and dominated convergence on bounded frequency balls. A uniform derivative bound controls the complementary high-frequency tails.

##### Weak lower semicontinuity of a bounded-domain Schrodinger energy

↑ **Parent:** [Rellich-Kondrashov compactness theorem for H01](#rellich-kondrashov-compactness-theorem-for-h01)

On bounded $\Omega$ with $V\in L^\infty(\Omega)$, weak convergence in $H_0^1(\Omega)$ makes the Dirichlet term lower semicontinuous and, by Rellich compactness, makes the potential term $\int Vu^2$ continuous. Thus

$$
E(u)=\int_\Omega(|Du|^2+Vu^2)
$$

is weakly lower semicontinuous.

###### Constrained ground-state minimizer on a bounded domain

↑ **Parent:** [Weak lower semicontinuity of a bounded-domain Schrodinger energy](#weak-lower-semicontinuity-of-a-bounded-domain-schrodinger-energy)

The infimum of $E(u)$ over $\lVert u\rVert_2=1$ is attained. A minimizing sequence is bounded in $H_0^1$ because $V$ is bounded below; weak compactness, Rellich strong $L^2$ convergence, and weak lower semicontinuity complete the direct-method argument.

##### Local compactness plus uniform tail control

↑ **Parent:** [Rellich-Kondrashov compactness theorem for H01](#rellich-kondrashov-compactness-theorem-for-h01)

Strong convergence on every bounded region combines with a tail estimate uniform in the sequence to give global strong convergence.

###### Strong convergence from weak convergence and tightness

↑ **Parent:** [Local compactness plus uniform tail control](#local-compactness-plus-uniform-tail-control)

If local compactness makes every subsequential local limit agree with the global weak limit and the $L^2$ mass is uniformly tight, weak convergence upgrades to strong convergence.

### Noncompactness of a Sobolev embedding by translation

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)

Translations of one compactly supported bump have equal Sobolev norms. Widely separated translates have disjoint supports and remain a fixed positive distance apart in $L^2$, obstructing compactness on an unbounded domain.

#### Loss of compactness at infinity

↑ **Parent:** [Noncompactness of a Sobolev embedding by translation](#noncompactness-of-a-sobolev-embedding-by-translation)

A bounded sequence can fail to have a strongly convergent subsequence because its mass escapes to infinity even when its local regularity is uniformly controlled.

#### Vanishing Dirichlet energy by dilation on the line

↑ **Parent:** [Noncompactness of a Sobolev embedding by translation](#noncompactness-of-a-sobolev-embedding-by-translation)

For $\phi\in H^1(\mathbb R)$ with $\lVert\phi\rVert_2=1$, the dilation

$$
u_R(x)=R^{-1/2}\phi(x/R)
$$

preserves the $L^2$ norm and satisfies $\lVert u_R'\rVert_2^2=R^{-2}\lVert\phi'\rVert_2^2$. Hence normalized functions on the line have Dirichlet-energy infimum zero, which no nonzero $L^2$ function attains.

<h3 id="holder-condition">Hölder condition</h3>

↑ **Parent:** [Sobolev embedding theorem](#sobolev-embedding-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hölder_condition)

A function is Hölder continuous with exponent $0<\alpha\leq1$ when $|f(x)-f(y)|\leq C|x-y|^\alpha$ for some constant $C$.

<h4 id="holder-space">Hölder space</h4>

↑ **Parent:** [Hölder condition](#holder-condition)

A [Hölder space](#holder-space) consists of functions satisfying a [Hölder condition](#holder-condition). A bounded function belongs to $C^{0,\alpha}(\mathbb R^n)$ when

$$
\sup_{x\ne y}\frac{|f(x)-f(y)|}{|x-y|^\alpha}<\infty.
$$

<h5 id="holder-taylor-remainder-bound">Hölder-Taylor remainder bound</h5>

↑ **Parent:** [Hölder space](#holder-space)

Write $\alpha=r+\beta$ with an [integer](number-theory.md#integer) $r\ge0$ and $0<\beta\le1$, using $r=\alpha-1$ at [integer](number-theory.md#integer) $\alpha$. For $f\in C^{r,\beta}$, subtract its degree-$r$ [Taylor polynomial](calculus.md#taylor-polynomial) at $x_0$. For $r\ge1$, the [integral](calculus.md#integral) [Taylor remainder](calculus.md#taylor-remainder) with $f^{(r)}(t)-f^{(r)}(x_0)$ is bounded using the [Hölder seminorm](#holder-seminorm); for $r=0$ this is exactly [Hölder continuity](#holder-condition). The resulting bound is the displayed estimate. At [integer](number-theory.md#integer) order, the convention is $C^{r,1}$; a $C^{r+1}$ [function](function.md) on a [compact](topology.md#compact-space) [closed interval](real-analysis.md#closed-real-interval) also obeys this estimate.

<h6 id="wavelet-coefficient-decay-for-holder-functions">Wavelet coefficient decay for Hölder functions</h6>

↑ **Parent:** [Hölder-Taylor remainder bound](#holder-taylor-remainder-bound)

Localized [wavelets](fourier-analysis.md#wavelet) of support diameter $O(2^{-j})$ and $L^1$ [norm](functional-analysis.md#norm) $O(2^{-j/2})$, with enough [vanishing moments](fourier-analysis.md#vanishing-moment), satisfy

$$
|\langle f,\psi_{j,n}\rangle|\le C\|f\|_{C^\alpha}2^{-j(\alpha+1/2)}.
$$

Subtract a [Taylor polynomial](calculus.md#taylor-polynomial) annihilated by the [wavelet](fourier-analysis.md#wavelet), apply the [Hölder-Taylor remainder bound](#holder-taylor-remainder-bound) on its [support of a function](function.md#support), and multiply by its $L^1$ [norm](functional-analysis.md#norm). The same argument applies to localized [boundary wavelets](fourier-analysis.md#boundary-wavelet) with the same cancellation; finitely many coarse [scaling functions](fourier-analysis.md#scaling-function) are handled separately.

<h5 id="holder-norm">Hölder norm</h5>

↑ **Parent:** [Hölder space](#holder-space)

The full norm is $|u|_{k,\alpha;U}=|u|_{k;U}+[D^k u]_{\alpha;U}$, combining the [derivative supremum norm](functional-analysis.md#derivative-supremum-norm) with the top-derivative [Hölder seminorm](#holder-seminorm). At order zero it is the sum of the [supremum norm](functional-analysis.md#supremum-norm) and the [Hölder seminorm](#holder-seminorm).

<h5 id="holder-seminorm">Hölder seminorm</h5>

↑ **Parent:** [Hölder space](#holder-space)

The Hölder seminorm of exponent $0<\alpha\leq1$ is

$$
[f]_{C^{0,\alpha}}=\sup_{x\ne y}\frac{|f(x)-f(y)|}{|x-y|^\alpha}.
$$

It measures [Hölder continuity](#holder-condition) without including the [supremum norm](functional-analysis.md#supremum-norm) of the function itself.

<h6 id="lower-semicontinuity-of-a-holder-seminorm">Lower semicontinuity of a Hölder seminorm</h6>

↑ **Parent:** [Hölder seminorm](#holder-seminorm)

If $f_j\to f$ uniformly and the [Hölder seminorms](#holder-seminorm) are uniformly bounded, each fixed difference quotient converges. Taking the supremum over point pairs gives $[f]_\mu\leq\liminf_j[f_j]_\mu$. The [supremum norms](functional-analysis.md#supremum-norm) converge, so the full [Hölder norm](#holder-norm) has the same [lower semicontinuity of a Hölder seminorm](#lower-semicontinuity-of-a-holder-seminorm).

<h5 id="holder-class">Hölder class</h5>

↑ **Parent:** [Hölder space](#holder-space)

A Hölder class bounds derivatives through order $\lceil\beta\rceil-1$ and requires the highest derivative to be Hölder continuous with exponent $\beta-\lceil\beta\rceil+1$ and constant $L$.

<h5 id="holder-interpolation-inequality">Hölder interpolation inequality</h5>

↑ **Parent:** [Hölder space](#holder-space)

On a ball of radius $R$, lower derivative norms of $u\in C^{l,\alpha}$ are bounded by an arbitrarily small multiple of the top Hölder seminorm plus a multiple of $\|u\|_{C^0}$. One endpoint form is

$$
R^l\|D^lu\|_0\leq\varepsilon R^{l+\alpha}[D^lu]_\alpha+C_\varepsilon\|u\|_0.
$$

<h5 id="compact-embedding-of-holder-spaces">Compact embedding of Hölder spaces</h5>

↑ **Parent:** [Hölder space](#holder-space)

On a bounded regular domain, a bounded subset of $C^{k,\alpha}$ is relatively compact in $C^{l,\beta}$ whenever $k+\alpha>l+\beta$. This is an [Arzelà-Ascoli theorem](topological-analysis.md#arzela-ascoli-theorem) argument applied successively to the derivatives.

<h5 id="fourier-proof-of-holder-regularity-from-a-sobolev-norm">Fourier proof of Hölder regularity from a Sobolev norm</h5>

↑ **Parent:** [Hölder space](#holder-space)

If $s>n/2+\alpha$ with $0<\alpha\leq1$, then Fourier inversion, $|e^{it}-1|\leq C_\alpha|t|^\alpha$, and Cauchy-Schwarz give

$$
\lVert u\rVert_{C^{0,\alpha}}
\leq C\lVert u\rVert_{H^s}.
$$

The weighted frequency integral converges precisely because $s-\alpha>n/2$.

<h4 id="holder-exponent">Hölder exponent</h4>

↑ **Parent:** [Hölder condition](#holder-condition)

The Hölder exponent in [Hölder continuity](#holder-condition) measures the power in the bound $|f(x)-f(y)|\leq C|x-y|^\alpha$. For $0<\alpha\leq1$, a larger exponent imposes stronger local regularity on bounded distance ranges. Exponent one is [Lipschitz continuity](real-analysis.md#lipschitz-continuity).

<h4 id="holder-exponent-greater-than-one-forces-constancy">Hölder exponent greater than one forces constancy</h4>

↑ **Parent:** [Hölder condition](#holder-condition)

If a real function on an interval obeys $|f(x)-f(y)|\leq C|x-y|^\alpha$ for finite $C$ and $\alpha>1$, its difference quotients tend to zero everywhere. The [mean value theorem](calculus.md#mean-value-theorem) makes it constant. Equivalently, divide a segment into $N$ pieces to obtain $|f(x)-f(y)|\leq C|x-y|^\alpha N^{1-\alpha}\to0$.

<h4 id="holder-continuity-of-a-one-dimensional-fractional-kernel-integral">Hölder continuity of a one-dimensional fractional kernel integral</h4>

↑ **Parent:** [Hölder condition](#holder-condition)

For $f\in L^2(0,1)$ and $0<\alpha<1/2$, the integral $g(x)=\int_0^1f(y)|x-y|^{-\alpha}\,dy$ is well defined for every real $x$. Scaling the squared kernel difference over the real line and using the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) give $|g(x+h)-g(x)|\leq C_\alpha\|f\|_2|h|^{1/2-\alpha}$.

<h4 id="derivative-criterion-for-holder-continuity-up-to-a-boundary">Derivative criterion for Hölder continuity up to a boundary</h4>

↑ **Parent:** [Hölder condition](#holder-condition)

If a holomorphic function on a half-rectangle satisfies $|f'(x+iy)|\leq Cy^{-1+\alpha}$ with $0<\alpha\leq1$, then it extends to an $\alpha$-Hölder continuous function on the closed half-rectangle. Integrate vertically to height $r=|z-w|$, horizontally at that height, and vertically back; each contribution is $O(r^\alpha)$.

<h2 id="ladyzhenskaya-s-inequality">Ladyzhenskaya's inequality</h2>

↑ **Parent:** [Sobolev space](sobolev-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ladyzhenskaya's_inequality)

[Ladyzhenskaya's inequality](#ladyzhenskaya-s-inequality) controls the [Lp norm](real-analysis.md#lp-norm) of a function by its [Lp norm](real-analysis.md#lp-norm) and the [Lp norm](real-analysis.md#lp-norm) of its [gradient](calculus.md#gradient): in dimension two, $\|u\|_4\leq C\|u\|_2^{1/2}\|\nabla u\|_2^{1/2}$; in dimension three the exponents are $1/4$ and $3/4$. These estimates hold for smooth compactly supported functions and extend using [density of smooth functions in a Sobolev space](#density-of-smooth-functions-in-a-sobolev-space).

### Ladyzhenskaya inequality in two dimensions

↑ **Parent:** [Ladyzhenskaya's inequality](#ladyzhenskaya-s-inequality)

This is the two-dimensional form of [Ladyzhenskaya's inequality](#ladyzhenskaya-s-inequality). For $u\in C_c^\infty(\mathbb R^2)$,

$$
\lVert u\rVert_4^4
\leq4\lVert u\rVert_2^2\lVert\nabla u\rVert_2^2.
$$

Apply the fundamental theorem of calculus to $|u|^2$ in each coordinate, multiply the resulting one-dimensional bounds, integrate, and use Cauchy--Schwarz.

## Morrey-Campanato space

↑ **Parent:** [Sobolev space](sobolev-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morrey–Campanato_space)

[Morrey-Campanato spaces](#morrey-campanato-space) control local integrals on balls by a power of their radius. The Morrey form uses $\sup_{x,r}r^{-\lambda}\int_{B_r(x)}|u|^p$; the [Campanato space](#campanato-space) uses $|u-u_{B_r(x)}|^p$ instead. Mean subtraction measures oscillation and relates this family to [Hölder spaces](#holder-space).

### Campanato space

↑ **Parent:** [Morrey-Campanato space](#morrey-campanato-space)

The Campanato seminorm measures mean oscillation by

$$
[f]_{\mathcal L^{p,\mu}(\Omega)}^p
=\sup_{x,r}r^{-\mu}\int_{\Omega\cap B_r(x)}|f-f_{\Omega\cap B_r(x)}|^p.
$$

On regular bounded domains, $\mathcal L^{p,n+p\alpha}=C^{0,\alpha}$ for $0<\alpha\leq1$, with equivalent norms.

#### Campanato iteration lemma

↑ **Parent:** [Campanato space](#campanato-space)

If a nondecreasing oscillation quantity satisfies

$$
\Phi(\rho)\leq A(\rho/R)^\gamma\Phi(R)+BR^\beta
$$

for $0<\rho\leq R$, with $\gamma>\beta$, then iteration gives $\Phi(\rho)\leq C(\rho/R)^\beta\Phi(R)+CB\rho^\beta$.

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (87)

- [Approximate gradient](inverse-problem.md#approximate-gradient)
- [Boundary trace of a function](differential-equation.md#boundary-trace-of-a-function)
- [Bounded-variation step outside W11](inverse-problem.md#bounded-variation-step-outside-w11)
- [Cauchy–Riemann operator](symplectic-geometry.md#cauchy-riemann-operator)
- [Elliptic boundary value problem](elliptic-boundary-value-problem.md)
- [Failure of first-order Sobolev embedding into Linfinity in two dimensions](#failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions)
- [Fixed-edge Euler-Lagrange equation for Mumford–Shah](computer-science.md#fixed-edge-euler-lagrange-equation-for-mumford-shah)
- [Fractional Dirichlet domain scale](partial-differential-equation.md#fractional-dirichlet-domain-scale)
- [Function space](functional-analysis.md#function-space)
- [Image signal](computer-science.md#image-signal)
- [Japanese bracket](analysis.md#japanese-bracket)
- [Lipschitz domain](real-analysis.md#lipschitz-domain)
- [Morrey inequality on a cube](#morrey-inequality-on-a-cube)
- [Morrey's inequality](#morrey-s-inequality)
- [Negative Sobolev regularity of a compactly supported distribution](distribution-theory.md#negative-sobolev-regularity-of-a-compactly-supported-distribution)
- [Orthogonalization of a transplantation matrix](riemannian-geometry.md#orthogonalization-of-a-transplantation-matrix)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-56.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-61.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#30b/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-12.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-12.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#31e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-68.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-66.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#3/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-67.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#4/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-9.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-9.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-9.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#16d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105.md#1/1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105.md#1/1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-107.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-107.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-107.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#1/3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-327.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-105.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-105.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#23i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-105.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#23g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341.md#section-a/4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#23f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#23f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-105.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-327.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-105.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-217.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-359.md#2/b/i/solution)
- [Periodic elliptic estimate](#periodic-elliptic-estimate)
- [Range of the Volterra integration operator](functional-analysis.md#range-of-the-volterra-integration-operator)
- [Riemann-Roch index for a real Cauchy-Riemann operator](symplectic-geometry.md#riemann-roch-index-for-a-real-cauchy-riemann-operator)
- [Smooth continuation criterion for semilinear wave equations](wave-equation.md#smooth-continuation-criterion-for-semilinear-wave-equations)
- [Sobolev domains of powers of an elliptic Dirichlet operator](distribution-theory.md#sobolev-domains-of-powers-of-an-elliptic-dirichlet-operator)
- [Sobolev function with zero weak gradient](#sobolev-function-with-zero-weak-gradient)
- [Sobolev gradient vanishes on a zero set](#sobolev-gradient-vanishes-on-a-zero-set)
- [Sobolev multiplication by a smooth cutoff](#sobolev-multiplication-by-a-smooth-cutoff)
- [Sobolev norm](#sobolev-norm)
- [Stokes operator](viscous-fluid-flow.md#stokes-operator)
- [White-noise likelihood for a square-integrable shift](stochastic-process.md#white-noise-likelihood-for-a-square-integrable-shift)
- [Zero-trace Sobolev space](#zero-trace-sobolev-space)
