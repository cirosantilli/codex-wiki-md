# Distribution theory

↑ **Parent:** [Analysis](analysis.md)

Distribution theory extends functions to continuous linear functionals on test functions, allowing generalized derivatives and point sources.

**Table of contents**

- [Distribution (mathematical analysis)](#distribution-mathematical-analysis)
  - [Tensor product of distributions](#tensor-product-of-distributions)
  - [Regular distribution](#regular-distribution)
  - [Order of a distribution](#order-of-a-distribution)
    - [Distribution of unbounded order](#distribution-of-unbounded-order)
    - [Order-zero distribution](#order-zero-distribution)
  - [Hadamard finite-part integral](#hadamard-finite-part-integral)
    - [Finite-part inverse-absolute-value distribution](#finite-part-inverse-absolute-value-distribution)
    - [Hadamard finite-part reciprocal-power distribution](#hadamard-finite-part-reciprocal-power-distribution)
  - [Weak convergence of distributions](#weak-convergence-of-distributions)
    - [Oscillating point-mass defect](#oscillating-point-mass-defect)
      - [Radial quadratic oscillation defect in two dimensions](#radial-quadratic-oscillation-defect-in-two-dimensions)
  - [Translation of a distribution](#translation-of-a-distribution)
    - [Differentiability of distribution translations](#differentiability-of-distribution-translations)
    - [Translation invariance and vanishing distributional derivative](#translation-invariance-and-vanishing-distributional-derivative)
- [Space of smooth functions](#space-of-smooth-functions)
  - [Compactly supported distribution space](#compactly-supported-distribution-space)
- [Test function](#test-function)
  - [Cutoff function](#cutoff-function)
  - [Space of test functions](#space-of-test-functions)
    - [Test-function inductive limit topology](#test-function-inductive-limit-topology)
    - [Density of test functions in distributions](#density-of-test-functions-in-distributions)
  - [Locally integrable function](#locally-integrable-function)
- [Distributional identity](#distributional-identity)
- [Dirac delta function](#dirac-delta-function)
  - [Folded sine approximation to a Dirac delta](#folded-sine-approximation-to-a-dirac-delta)
  - [Surface delta distribution](#surface-delta-distribution)
    - [Spherical surface measure convolution](#spherical-surface-measure-convolution)
    - [Level-set normalization of a surface delta](#level-set-normalization-of-a-surface-delta)
  - [Fourier representation of the Dirac delta function](#fourier-representation-of-the-dirac-delta-function)
    - [Delta derivatives from polynomial oscillatory amplitudes](#delta-derivatives-from-polynomial-oscillatory-amplitudes)
  - [Distributional derivative of the Heaviside step function](#distributional-derivative-of-the-heaviside-step-function)
    - [Distributional jump formula for a Heaviside product](#distributional-jump-formula-for-a-heaviside-product)
  - [Dirac delta scaling](#dirac-delta-scaling)
  - [Derivative of the Dirac delta](#derivative-of-the-dirac-delta)
- [Multi-index notation](#multi-index-notation)
- [Distributional derivative](#distributional-derivative)
  - [Distributional derivative of the logarithmic modulus](#distributional-derivative-of-the-logarithmic-modulus)
  - [A distribution with zero derivative is constant](#a-distribution-with-zero-derivative-is-constant)
  - [Weak derivative](#weak-derivative)
    - [Bounded isolated-point removability for weak first derivatives](#bounded-isolated-point-removability-for-weak-first-derivatives)
    - [Locality of weak differentiability](#locality-of-weak-differentiability)
    - [Weak gradient](#weak-gradient)
    - [Sobolev chain rule](#sobolev-chain-rule)
      - [Gradient of a Sobolev function vanishes on a level set](#gradient-of-a-sobolev-function-vanishes-on-a-level-set)
- [Multiplication of a distribution by a smooth function](#multiplication-of-a-distribution-by-a-smooth-function)
  - [Distribution annihilated by a function with simple zeros](#distribution-annihilated-by-a-function-with-simple-zeros)
    - [Kernel of multiplication by a coordinate](#kernel-of-multiplication-by-a-coordinate)
  - [Dirac delta multiplication identity](#dirac-delta-multiplication-identity)
  - [Principal-value reciprocal distribution](#principal-value-reciprocal-distribution)
- [Dilation of a distribution](#dilation-of-a-distribution)
  - [Support law for distributional dilation](#support-law-for-distributional-dilation)
  - [Homogeneous distribution](#homogeneous-distribution)
    - [Fourier transform of a homogeneous distribution](#fourier-transform-of-a-homogeneous-distribution)
      - [Fourier transform of a reciprocal positive quadratic form](#fourier-transform-of-a-reciprocal-positive-quadratic-form)
        - [Accretive complex quadratic reciprocal Fourier transform](#accretive-complex-quadratic-reciprocal-fourier-transform)
- [Riesz potential](#riesz-potential)
  - [Riesz kernel](#riesz-kernel)
  - [Hedberg inequality](#hedberg-inequality)
- [Mollifier](#mollifier)
  - [Mollification](#mollification)
  - [Mollification of a divergence-forcing equation](#mollification-of-a-divergence-forcing-equation)
- [Support of a distribution](#support-of-a-distribution)
  - [Compactly supported distribution](#compactly-supported-distribution)
    - [Negative Sobolev regularity of a compactly supported distribution](#negative-sobolev-regularity-of-a-compactly-supported-distribution)
    - [Fourier transform of a compactly supported distribution](#fourier-transform-of-a-compactly-supported-distribution)
      - [Shrinking-cutoff exponential-type estimate](#shrinking-cutoff-exponential-type-estimate)
      - [Fourier decay in a bounded complex strip](#fourier-decay-in-a-bounded-complex-strip)
    - [Structure theorem for compactly supported distributions](#structure-theorem-for-compactly-supported-distributions)
      - [Compact continuous-derivative representation of a distribution](#compact-continuous-derivative-representation-of-a-distribution)
      - [Bessel potential](#bessel-potential)
- [Fundamental solution of a linear differential operator](#fundamental-solution-of-a-linear-differential-operator)
  - [Malgrange–Ehrenpreis theorem](#malgrange-ehrenpreis-theorem)
    - [Hörmander staircase](#hormander-staircase)
      - [Finite-height polynomial root avoidance](#finite-height-polynomial-root-avoidance)
  - [Retarded fundamental solution](#retarded-fundamental-solution)
    - [Retarded fundamental solution of a constant-coefficient ordinary differential operator](#retarded-fundamental-solution-of-a-constant-coefficient-ordinary-differential-operator)
- [Elliptic differential operator](#elliptic-differential-operator)
  - [Elliptic system of differential equations](#elliptic-system-of-differential-equations)
  - [Odd-order obstruction for scalar elliptic operators in at least three dimensions](#odd-order-obstruction-for-scalar-elliptic-operators-in-at-least-three-dimensions)
  - [High-frequency lower bound for an elliptic polynomial](#high-frequency-lower-bound-for-an-elliptic-polynomial)
  - [Elliptic regularity](#elliptic-regularity)
    - [Interior second-derivative estimate for the Poisson equation](#interior-second-derivative-estimate-for-the-poisson-equation)
    - [Elliptic regularity bootstrap with smooth lower-order coefficients](#elliptic-regularity-bootstrap-with-smooth-lower-order-coefficients)
    - [Divergence-forcing interior H1 estimate](#divergence-forcing-interior-h1-estimate)
    - [Interior gradient estimate near a zero Dirichlet side](#interior-gradient-estimate-near-a-zero-dirichlet-side)
    - [Second-derivative estimate at a flat Dirichlet boundary](#second-derivative-estimate-at-a-flat-dirichlet-boundary)
    - [Cutoff bootstrap for local elliptic regularity](#cutoff-bootstrap-for-local-elliptic-regularity)
    - [Spectral characterization of elliptic Dirichlet domains](#spectral-characterization-of-elliptic-dirichlet-domains)
    - [Sobolev domains of powers of an elliptic Dirichlet operator](#sobolev-domains-of-powers-of-an-elliptic-dirichlet-operator)
    - [Boundary elliptic regularity for the shifted Dirichlet Laplacian](#boundary-elliptic-regularity-for-the-shifted-dirichlet-laplacian)
    - [Dirichlet Poisson regularity theorem](#dirichlet-poisson-regularity-theorem)
  - [Parametrix](#parametrix)
    - [High-frequency reciprocal parametrix kernel](#high-frequency-reciprocal-parametrix-kernel)
  - [Symbol class](#symbol-class)
    - [Symbol calculus](#symbol-calculus)
- [Oscillatory integral](#oscillatory-integral)
  - [Abel regularization of an oscillatory integral](#abel-regularization-of-an-oscillatory-integral)
  - [Cutoff independence of an oscillatory integral](#cutoff-independence-of-an-oscillatory-integral)
  - [Symbol order reduction by a phase integration operator](#symbol-order-reduction-by-a-phase-integration-operator)
  - [Finite order of an oscillatory integral distribution](#finite-order-of-an-oscillatory-integral-distribution)
  - [Amplitude of an oscillatory integral](#amplitude-of-an-oscillatory-integral)
    - [Conic support of an oscillatory amplitude](#conic-support-of-an-oscillatory-amplitude)
      - [Stationary-direction bound for singular support](#stationary-direction-bound-for-singular-support)
        - [Slice-support obstruction for oscillatory singularities](#slice-support-obstruction-for-oscillatory-singularities)
        - [Ordinary amplitude support can miss a singular-support limit](#ordinary-amplitude-support-can-miss-a-singular-support-limit)
  - [Phase function](#phase-function)
- [Singular support](#singular-support)
- [Paley–Wiener theorem](#paley-wiener-theorem)
  - [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem)
    - [Fourier independence from disjoint distribution supports](#fourier-independence-from-disjoint-distribution-supports)
    - [Polynomial division preservation of exponential type](#polynomial-division-preservation-of-exponential-type)
    - [Contour-shift proof of the Paley–Wiener–Schwartz theorem](#contour-shift-proof-of-the-paley-wiener-schwartz-theorem)
      - [Mollifier regularization for contour recovery of support](#mollifier-regularization-for-contour-recovery-of-support)
- [Hypoelliptic operator](#hypoelliptic-operator)
  - [Derivative-ratio Sobolev gain for a polynomial operator](#derivative-ratio-sobolev-gain-for-a-polynomial-operator)

## Distribution (mathematical analysis)

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Distribution_(mathematical_analysis))

A distribution on an open set $U$ is a continuous linear functional on the [space of test functions](#space-of-test-functions) $\mathcal D(U)=C_c^\infty(U)$.

### Tensor product of distributions

↑ **Parent:** [Distribution (mathematical analysis)](#distribution-mathematical-analysis)

For [distributions](#distribution-mathematical-analysis) $u$ on $\mathbb R^m$ and $v$ on $\mathbb R^n$, their tensor product acts on a joint [test function](#test-function) by $\langle u\otimes v,\Phi\rangle=\langle u_x,\langle v_y,\Phi(x,y)\rangle\rangle$. The inner function is smooth with [compact support](function.md#compact-support) in the projection of $\operatorname{supp}\Phi$, and finite [order of a distribution](#order-of-a-distribution) estimates prove continuity. Reversing the pairings gives the same value: finite sums of product kernels are dense in the required smooth seminorms, and the two orders agree on product kernels. Its support is contained in the Cartesian product of the two supports. This provides a rigorous replacement for formal integration in separate [distribution](#distribution-mathematical-analysis) variables.

### Regular distribution

↑ **Parent:** [Distribution (mathematical analysis)](#distribution-mathematical-analysis)

A [locally integrable function](#locally-integrable-function) $f$ defines a [distribution](#distribution-mathematical-analysis) by $\langle u_f,\varphi\rangle=\int f\varphi$. The pairing is bilinear if distributions are taken complex-linear. This identifies ordinary functions with a subset of [distributions](#distribution-mathematical-analysis) without claiming that every distribution is a function.

### Order of a distribution

↑ **Parent:** [Distribution (mathematical analysis)](#distribution-mathematical-analysis)

The order of a distribution on a compact set is the least nonnegative integer $m$ for which its action is bounded by a constant times the sup norms of test-function derivatives through order $m$.

#### Distribution of unbounded order

↑ **Parent:** [Order of a distribution](#order-of-a-distribution)

A [distribution](#distribution-mathematical-analysis) can have finite [order of a distribution](#order-of-a-distribution) on every [compact set](topology.md#compact-space) without having one order bound valid on the whole domain. For example, the locally finite sum $\sum_{j\geq1}\partial^j\delta_j$ on the real line has orders growing without bound near the integers.

#### Order-zero distribution

↑ **Parent:** [Order of a distribution](#order-of-a-distribution)

An order-zero distribution is locally bounded by the sup norm of its test function. Such distributions are precisely the distributions represented locally by signed or complex [Radon measures](measure-theory.md#radon-measure).

### Hadamard finite-part integral

↑ **Parent:** [Distribution (mathematical analysis)](#distribution-mathematical-analysis)

A Hadamard finite-part integral subtracts the divergent terms of a truncated integral and retains its finite limit. It defines distributions such as the extension of $1/x$ obtained by differentiating $\log x_+$.

#### Finite-part inverse-absolute-value distribution

↑ **Parent:** [Hadamard finite-part integral](#hadamard-finite-part-integral)

Subtract a [test function](#test-function)'s value at zero before integrating $1/|k|$ near zero, and retain the ordinary tail integral. This defines an even [tempered distribution](fourier-analysis.md#tempered-distribution). Changing the subtraction cutoff adds a multiple of the [Dirac delta distribution](#dirac-delta-function). Multiplication by $k$ gives $\operatorname{sgn}k$.

#### Hadamard finite-part reciprocal-power distribution

↑ **Parent:** [Hadamard finite-part integral](#hadamard-finite-part-integral)

For $m\geq2$, the symmetric [Hadamard finite-part integral](#hadamard-finite-part-integral) defining $\Lambda_m$ subtracts the [Taylor polynomial](calculus.md#taylor-polynomial) through degree $m-2$ from a [test function](#test-function) before division by $x^m$. It has finite [order of a distribution](#order-of-a-distribution) and satisfies

$$
\Lambda_m=\frac{(-1)^{m-1}}{(m-1)!}\left(\frac d{dx}\right)^m\log|x|.
$$

The lower-order subtraction terms are integrable at infinity, while the remaining odd $1/x$ singularity cancels under symmetric truncation.

### Weak convergence of distributions

↑ **Parent:** [Distribution (mathematical analysis)](#distribution-mathematical-analysis)

A sequence of distributions $u_j$ converges weakly to $u$ when $\langle u_j,\varphi\rangle\to\langle u,\varphi\rangle$ for every [test function](#test-function) $\varphi$.

#### Oscillating point-mass defect

↑ **Parent:** [Weak convergence of distributions](#weak-convergence-of-distributions)

A sequence can converge as [distributions](#distribution-mathematical-analysis) off one point while retaining a nonconvergent multiple of a [Dirac delta function](#dirac-delta-function) at that point. If $u_j=v+c_j\delta_p+o_{\mathcal D'}(1)$ with $c_j$ nonconvergent, restriction to the punctured domain tends to $v$, but a test nonzero at $p$ detects the obstruction to global convergence.

##### Radial quadratic oscillation defect in two dimensions

↑ **Parent:** [Oscillating point-mass defect](#oscillating-point-mass-defect)

For $a>0$, polar-coordinate reduction and [integration by parts](calculus.md#integration-by-parts) give $m\sin(m||x|^2-a|)=2\delta(|x|^2-a)-\pi\cos(ma)\delta_0+o_{\mathcal D'}(1)$ in two dimensions. The circle term comes from the cusp in the folded phase, while the origin term is a radial endpoint contribution. A punctured-domain limit therefore need not extend across the quadratic critical point.

### Translation of a distribution

↑ **Parent:** [Distribution (mathematical analysis)](#distribution-mathematical-analysis)

If $\tau_hf(x)=f(x-h)$ for functions, its extension to distributions is defined by

$$
\langle\tau_hu,\varphi\rangle=\langle u,\varphi(\mathord\cdot+h)\rangle.
$$

#### Differentiability of distribution translations

↑ **Parent:** [Translation of a distribution](#translation-of-a-distribution)

With [translation of a distribution](#translation-of-a-distribution) defined by $\langle\tau_hu,\varphi\rangle=\langle u,\varphi(\mathord\cdot+h)\rangle$, differentiation of the [test function](#test-function) gives $\frac d{dh}\tau_hu=-\tau_hu'$ in [weak convergence of distributions](#weak-convergence-of-distributions). The [Taylor theorem](calculus.md#taylor-theorem) shows convergence in the [space of test functions](#space-of-test-functions), including a common [compact support](function.md#compact-support). Thus $(\tau_{-h}u-u)/h\to u'$; fixing the translation convention prevents a sign error.

#### Translation invariance and vanishing distributional derivative

↑ **Parent:** [Translation of a distribution](#translation-of-a-distribution)

A distribution is invariant under every translation parallel to the $i$th coordinate axis exactly when its $i$th [distributional derivative](#distributional-derivative) vanishes. Differentiate the translated pairing for one direction; integrate that derivative in the translation parameter for the converse.

## Space of smooth functions

↑ **Parent:** [Distribution theory](distribution-theory.md)

For an [open set](topology.md#open-set) $X\subseteq\mathbb R^n$, the space $\mathcal E(X)=C^\infty(X)$ carries the [Fréchet topology](topological-vector-space.md#frechet-space) in which $f_j\to f$ exactly when every derivative converges uniformly on every [compact set](topology.md#compact-space) contained in $X$.

### Compactly supported distribution space

↑ **Parent:** [Space of smooth functions](#space-of-smooth-functions)

The [continuous dual](continuous-dual-space.md) $\mathcal E'(X)$ of $\mathcal E(X)$ is the space of [compactly supported distributions](#compactly-supported-distribution) on $X$. Its weak topology is pointwise convergence on $\mathcal E(X)$.

## Test function

↑ **Parent:** [Distribution theory](distribution-theory.md)

A test function is a smooth function with [compact support](function.md#compact-support). Weak and distributional equations are identities obtained by integrating against every test function.

### Cutoff function

↑ **Parent:** [Test function](#test-function)

A cutoff function is a smooth function that equals one on a chosen inner set and vanishes outside a slightly larger set. On concentric balls $B_r\subset B_R$, it can be chosen with $|D\eta|\leq C/(R-r)$.

### Space of test functions

↑ **Parent:** [Test function](#test-function)

The space of test functions is $\mathcal D(U)=C_c^\infty(U)$. A sequence converges in $\mathcal D(U)$ when all its supports eventually lie in one compact subset of $U$ and every derivative converges uniformly there.

#### Test-function inductive limit topology

↑ **Parent:** [Space of test functions](#space-of-test-functions)

The [space of test functions](#space-of-test-functions) has the locally convex inductive-limit topology of the spaces of [smooth functions](analysis.md#smooth-function) supported in a fixed [compact set](topology.md#compact-space) $K$. Each $\mathcal D_K$ uses [seminorms](topological-vector-space.md#seminorm) $p_m(\varphi)=\max_{|\alpha|\leq m}\|\partial^\alpha\varphi\|_\infty$. Sequential convergence means a common [compact support](function.md#compact-support) and [uniform convergence](real-analysis.md#uniform-convergence) of every derivative. A [linear functional](linear-algebra.md#linear-functional) on this space is a [distribution](#distribution-mathematical-analysis) exactly when its restriction to each $\mathcal D_K$ satisfies a finite [order of a distribution](#order-of-a-distribution) estimate; the order and constant may depend on $K$.

#### Density of test functions in distributions

↑ **Parent:** [Space of test functions](#space-of-test-functions)

Every [distribution](#distribution-mathematical-analysis) is a limit of [test functions](#test-function) in [weak convergence of distributions](#weak-convergence-of-distributions). With a [mollifier](#mollifier) $\rho_\varepsilon$ and an expanding [smooth cutoff function](analysis.md#smooth-cutoff-function) $\chi(x/j)$, the functions $\chi(x/j)(u*\rho_{1/j})(x)$ have compact support and converge to $u$. For each fixed test, the cutoff eventually equals one on its support, while the reflected mollifier approximates that test with all derivatives in a common compact set.

### Locally integrable function

↑ **Parent:** [Test function](#test-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_integrable_function)

A function is locally integrable when its absolute value has finite integral over every compact subset of its domain. It defines a regular [distribution](#distribution-mathematical-analysis) by integration against test functions.

## Distributional identity

↑ **Parent:** [Distribution theory](distribution-theory.md)

A distributional identity is an equality that holds after both sides act on every smooth compactly supported test function.

## Dirac delta function

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_delta_function)

The Dirac delta is the distribution defined by $\langle\delta,\varphi\rangle=\varphi(0)$.

### Folded sine approximation to a Dirac delta

↑ **Parent:** [Dirac delta function](#dirac-delta-function)

As [distributions](#distribution-mathematical-analysis) on the line, $m\sin(m|t|)\to2\delta_0$. Pairing with a [test function](#test-function) $A$ folds the integral to $\int_0^\infty m\sin(ms)[A(s)+A(-s)]\,ds$. One [integration by parts](calculus.md#integration-by-parts) yields $2A(0)$ plus a cosine integral tending to zero by the [Riemann-Lebesgue lemma](fourier-analysis.md#riemann-lebesgue-lemma). Pointwise convergence is unnecessary.

### Surface delta distribution

↑ **Parent:** [Dirac delta function](#dirac-delta-function)

For a smooth hypersurface $S$, its surface delta is the [distribution](#distribution-mathematical-analysis) $\langle\delta_S,\varphi\rangle=\int_S\varphi\,dS$. Its normalization uses geometric surface measure rather than a defining function. On the unit circle, $\delta_{S^1}$ pairs by integrating $\varphi(\cos t,\sin t)$ over $0\leq t\leq2\pi$.

#### Spherical surface measure convolution

↑ **Parent:** [Surface delta distribution](#surface-delta-distribution)

For the geometric [surface delta distribution](#surface-delta-distribution) on the radius-$a$ sphere in $\mathbb R^3$, $\langle u_a,\phi\rangle=a^2\int_{S^2}\phi(a\omega)\,d\sigma(\omega)$. Angular integration gives the [Fourier transform](analysis.md#fourier-transform) $\widehat u_a(\xi)=4\pi a\sin(a|\xi|)/|\xi|$, with removable value $4\pi a^2$ at zero. The [convolution of distributions with a compactly supported factor](fourier-analysis.md#convolution-of-distributions-with-a-compactly-supported-factor) gives the [regular distribution](#regular-distribution)

$$
u_a*u_b=\frac{2\pi ab}{|x|}\mathbf1_{\{|a-b|<|x|<a+b\}}.
$$

This density has total mass $16\pi^2a^2b^2$. Values on endpoint spheres do not affect the [distribution](#distribution-mathematical-analysis). When $a=b$, the inverse-distance singularity is locally integrable in three dimensions and is not an additional point mass. The annulus expresses the triangle inequality for the sum of two vectors of fixed lengths.

#### Level-set normalization of a surface delta

↑ **Parent:** [Surface delta distribution](#surface-delta-distribution)

If $g$ is smooth and $\nabla g\ne0$ on $S=\{g=0\}$, transverse local coordinates give $\langle\delta(g),\varphi\rangle=\int_S\varphi/|\nabla g|\,dS$. Thus $\delta_S=|\nabla g|\delta(g)$ as [distributions](#distribution-mathematical-analysis). In particular $\delta_{S^1}=2\delta(|x|^2-1)$. Omitting this Jacobian confuses the delta of a defining function with a geometric [surface delta distribution](#surface-delta-distribution).

### Fourier representation of the Dirac delta function

↑ **Parent:** [Dirac delta function](#dirac-delta-function)

The identity

$$
\delta(x)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{ikx}\,dk
$$

is interpreted distributionally: symmetric frequency cutoffs give $\sin(nx)/(\pi x)$, which converge to the Dirac delta function.

#### Delta derivatives from polynomial oscillatory amplitudes

↑ **Parent:** [Fourier representation of the Dirac delta function](#fourier-representation-of-the-dirac-delta-function)

With inverse [Fourier transform](analysis.md#fourier-transform) normalization $(2\pi)^{-1}$, $\int e^{is\theta}\theta^j\,d\theta=2\pi i^{-j}\delta^{(j)}(s)$ as an [oscillatory integral](#oscillatory-integral). The factor $i^{-j}$ and the sign convention $\langle\delta',g\rangle=-g'(0)$ are essential. For instance, amplitude $-ix_2\theta/(2\pi)$ with phase $x_1\theta$ gives $-x_2\delta'(x_1)$.

### Distributional derivative of the Heaviside step function

↑ **Parent:** [Dirac delta function](#dirac-delta-function)

For every test function $\varphi$,

$$
\langle H',\varphi\rangle=-\int_0^\infty\varphi'(t)dt=\varphi(0),
$$

so $H'=\delta$ as distributions.

#### Distributional jump formula for a Heaviside product

↑ **Parent:** [Distributional derivative of the Heaviside step function](#distributional-derivative-of-the-heaviside-step-function)

For a [smooth function](analysis.md#smooth-function) $u$, the [distributional derivative](#distributional-derivative) of the product of $u$ with the [Heaviside function](analysis.md#heaviside-step-function) is $D(Hu)=Hu'+u(0)\delta_0$. Induction gives the displayed formula. It records all boundary sources, including derivatives of the [Dirac delta distribution](#dirac-delta-function), and determines which initial derivatives must vanish in a [retarded fundamental solution](#retarded-fundamental-solution).

### Dirac delta scaling

↑ **Parent:** [Dirac delta function](#dirac-delta-function)

For nonzero $a$, $\delta(ax)=\delta(x)/|a|$ in the distributional sense.

### Derivative of the Dirac delta

↑ **Parent:** [Dirac delta function](#dirac-delta-function)

The derivative of the Dirac delta is the [distributional derivative](#distributional-derivative) defined by

$$
\langle\delta',\varphi\rangle=-\varphi'(0)
$$

for every [test function](#test-function) $\varphi$.

## Multi-index notation

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multi-index_notation)

A multi-index is a tuple of nonnegative integers used to abbreviate products and partial derivatives: $|\alpha|=\sum_j\alpha_j$, $x^\alpha=\prod_jx_j^{\alpha_j}$, and $D^\alpha=\prod_jD_j^{\alpha_j}$.

## Distributional derivative

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Distributional_derivative)

For a distribution $u$ and a [multi-index](#multi-index-notation) $\alpha$, its distributional derivative is defined by

$$
\langle D^\alpha u,\varphi\rangle=(-1)^{|\alpha|}\langle u,D^\alpha\varphi\rangle.
$$

### Distributional derivative of the logarithmic modulus

↑ **Parent:** [Distributional derivative](#distributional-derivative)

The [locally integrable function](#locally-integrable-function) $\log|x|$ has [distributional derivative](#distributional-derivative) equal to the [principal-value reciprocal distribution](#principal-value-reciprocal-distribution). Symmetric [integration by parts](calculus.md#integration-by-parts) makes the boundary term $\log\varepsilon[\varphi(\varepsilon)-\varphi(-\varepsilon)]$ tend to zero.

### A distribution with zero derivative is constant

↑ **Parent:** [Distributional derivative](#distributional-derivative)

If $v'=0$ on $\mathbb R$, then $v$ is a constant [distribution](#distribution-mathematical-analysis). Every [test function](#test-function) of integral zero is the derivative of its compactly supported primitive, so $v$ vanishes on those test functions. Choosing one test function $\eta$ of integral one gives $\langle v,\varphi\rangle=\langle v,\eta\rangle\int\varphi$. Iteration shows that a distribution with $m$th derivative zero is a [polynomial](polynomial.md) of degree at most $m-1$.

### Weak derivative

↑ **Parent:** [Distributional derivative](#distributional-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_derivative)

A locally integrable function $g$ is the $i$th weak derivative of $u$ when

$$
\int_UuD_i\varphi=-\int_Ug\varphi
$$

for every [test function](#test-function) $\varphi\in C_c^\infty(U)$. Thus a weak derivative is a [distributional derivative](#distributional-derivative) that is represented by a locally integrable function.

#### Bounded isolated-point removability for weak first derivatives

↑ **Parent:** [Weak derivative](#weak-derivative)

A bounded function which is $C^1$ away from one point in dimension $n\geq2$, and whose classical gradient is locally integrable across that point, has that gradient as its [weak derivative](#weak-derivative). Cut a [test function](#test-function) off within distance $\varepsilon$ of the point. The error from differentiating the cutoff is bounded by $C\|u\|_\infty\varepsilon^{n-1}$ and vanishes. The other terms converge by local integrability. In dimension one the [Heaviside step function](analysis.md#heaviside-step-function) is a counterexample: its classical derivative off the point is zero, but its distributional derivative is a [Dirac delta](#dirac-delta-function).

#### Locality of weak differentiability

↑ **Parent:** [Weak derivative](#weak-derivative)

A locally integrable function has [weak derivatives](#weak-derivative) on an open set exactly when it has them near every point. Local derivatives agree almost everywhere on overlaps because they define the same [distributional derivative](#distributional-derivative). A countable local cover therefore gives globally defined, locally integrable derivative functions. A smooth [partition of unity](differential-geometry.md#partition-of-unity) subordinate to the cover splits each compactly supported [test function](#test-function); summing the local integration identities yields the global weak-derivative identity.

#### Weak gradient

↑ **Parent:** [Weak derivative](#weak-derivative)

The weak gradient is the [vector](vector-space.md#vector) of first-order [weak derivatives](#weak-derivative) of a [function](function.md). Its $i$th component is specified by $\int u\partial_i\varphi=-\int(\partial_i u)\varphi$ for compactly supported [test functions](#test-function). For a differentiable function with appropriate local integrability it agrees with the classical [gradient](calculus.md#gradient).

#### Sobolev chain rule

↑ **Parent:** [Weak derivative](#weak-derivative)

If $u\in W^{1,2}_{\mathrm{loc}}$ and $\Phi$ is continuously differentiable with bounded derivative on the range in use, then $D(\Phi(u))=\Phi^{\prime}(u)Du$ [almost everywhere](measure-theory.md#almost-everywhere). One proves this first for [smooth functions](analysis.md#smooth-function) and then uses [density of smooth functions in a Sobolev space](sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space) and boundedness of $\Phi^{\prime}$. On compact sets one may truncate $\Phi$ away from the range of a bounded $u$.

##### Gradient of a Sobolev function vanishes on a level set

↑ **Parent:** [Sobolev chain rule](#sobolev-chain-rule)

If $u\in W^{1,2}_{\mathrm{loc}}$, then $Du=0$ [almost everywhere](measure-theory.md#almost-everywhere) on every [level set](topology.md#level-set) $\{u=t\}$. Choose smooth truncations $\Phi_\varepsilon(s)$ with $|\Phi_\varepsilon|\leq2\varepsilon$, derivative one near zero, bounded derivative, and derivative zero outside $(-2\varepsilon,2\varepsilon)$. The [Sobolev chain rule](#sobolev-chain-rule) gives $D\Phi_\varepsilon(u-t)\to\mathbf1_{\{u=t\}}Du$ in local $L^2$ by [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem), while $\Phi_\varepsilon(u-t)\to0$. The limiting [weak derivative](#weak-derivative) is therefore zero.

## Multiplication of a distribution by a smooth function

↑ **Parent:** [Distribution theory](distribution-theory.md)

For a [distribution](#distribution-mathematical-analysis) $u$ and a [smooth function](analysis.md#smooth-function) $a$, the product $au$ is defined by $\langle au,\varphi\rangle=\langle u,a\varphi\rangle$. It obeys the [Leibniz rule](calculus.md#leibniz-rule); in one dimension, $(au)'=a'u+au'$.

### Distribution annihilated by a function with simple zeros

↑ **Parent:** [Multiplication of a distribution by a smooth function](#multiplication-of-a-distribution-by-a-smooth-function)

If a smooth function $a$ on $\mathbb R$ has finitely many zeros $r_j$, all simple, then $aw=0$ exactly when $w=\sum_jc_j\delta_{r_j}$. Away from the zeros, divide a [test function](#test-function) by the nonvanishing $a$ to show $w$ vanishes. Near $r_j$, write $a(x)=(x-r_j)b_j(x)$ with smooth nonzero $b_j$. The [kernel of multiplication by a coordinate](#kernel-of-multiplication-by-a-coordinate), after translation and multiplication by $b_j$, says that the local distribution is a multiple of $\delta_{r_j}$. A [partition of unity](differential-geometry.md#partition-of-unity) gives the global sum. Simplicity of the zeros excludes derivatives of deltas.

#### Kernel of multiplication by a coordinate

↑ **Parent:** [Distribution annihilated by a function with simple zeros](#distribution-annihilated-by-a-function-with-simple-zeros)

In one dimension, $xw=0$ if and only if $w=c\delta_0$. Choose a [cutoff function](#cutoff-function) $\eta=1$ near zero and write every [test function](#test-function) as $\varphi=\varphi(0)\eta+x\psi$. The pairing with $x\psi$ vanishes, leaving $\langle w,\varphi\rangle=\varphi(0)\langle w,\eta\rangle$.

### Dirac delta multiplication identity

↑ **Parent:** [Multiplication of a distribution by a smooth function](#multiplication-of-a-distribution-by-a-smooth-function)

For smooth $a$ and a point $r$,

$$
a\delta_r=a(r)\delta_r,
\qquad a\delta'_r=a(r)\delta'_r-a'(r)\delta_r.
$$

These follow by applying both sides to a [test function](#test-function) and using the [Leibniz rule](calculus.md#leibniz-rule). In particular $(x-r)\delta'_r=-\delta_r$.

### Principal-value reciprocal distribution

↑ **Parent:** [Multiplication of a distribution by a smooth function](#multiplication-of-a-distribution-by-a-smooth-function)

The [Cauchy principal value](complex-analysis.md#cauchy-principal-value)

$$
\left\langle\operatorname{pv}\frac1x,\varphi\right\rangle
=\lim_{\varepsilon\downarrow0}\int_{|x|>\varepsilon}\frac{\varphi(x)}x\,dx
$$

defines a [distribution](#distribution-mathematical-analysis). Near zero the odd constant contribution cancels, and the remaining numerator is $O(x)$. It satisfies $x\operatorname{pv}(1/x)=1$. Hence all solutions of $xv=1$ are $v=\operatorname{pv}(1/x)+c\delta_0$ by the [kernel of multiplication by a coordinate](#kernel-of-multiplication-by-a-coordinate).

## Dilation of a distribution

↑ **Parent:** [Distribution theory](distribution-theory.md)

For $t>0$, the dilation $\delta_tu$ of a distribution on $\mathbb R^n$ is defined by

$$
\langle\delta_tu,\varphi\rangle=t^{-n}\langle u,\varphi(\mathord\cdot/t)\rangle.
$$

For a regular distribution this agrees with the function $x\mapsto u(tx)$.

### Support law for distributional dilation

↑ **Parent:** [Dilation of a distribution](#dilation-of-a-distribution)

For $t>0$, the [support of a distribution](#support-of-a-distribution) satisfies

$$
\operatorname{supp}(\delta_tu)=t^{-1}\operatorname{supp}u.
$$

The duality formula $\langle\delta_tu,\varphi\rangle=t^{-n}\langle u,\varphi(\mathord\cdot/t)\rangle$ proves one inclusion by transporting [test functions](#test-function); applying the inverse dilation proves the other. For a compact support, the [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem) gives another proof: $\widehat{\delta_tu}(\zeta)=t^{-n}\widehat u(\zeta/t)$ rescales the exponential growth indicator by $1/t$.

### Homogeneous distribution

↑ **Parent:** [Dilation of a distribution](#dilation-of-a-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homogeneous_distribution)

A distribution $u$ is homogeneous of degree $\sigma$ when $\delta_tu=t^\sigma u$ for every $t>0$. With the unnormalized angular-frequency convention, its [Fourier transform](analysis.md#fourier-transform) is homogeneous of degree $-n-\sigma$.

#### Fourier transform of a homogeneous distribution

↑ **Parent:** [Homogeneous distribution](#homogeneous-distribution)

The [scaling property of the Fourier transform](analysis.md#scaling-property-of-the-fourier-transform) extends by duality to

$$
\widehat{\delta_tu}=t^{-n}\delta_{1/t}\widehat u.
$$

Consequently a [homogeneous distribution](#homogeneous-distribution) of degree $\sigma$ transforms into one of degree $-n-\sigma$.

##### Fourier transform of a reciprocal positive quadratic form

↑ **Parent:** [Fourier transform of a homogeneous distribution](#fourier-transform-of-a-homogeneous-distribution)

For a real symmetric positive-definite three-dimensional [matrix](vector-space.md#matrix), the reciprocal [quadratic form](linear-algebra.md#quadratic-form) is locally integrable and defines a regular [tempered distribution](fourier-analysis.md#tempered-distribution). With the Fourier kernel $e^{-ix\cdot\xi}$, radial Abel regularization gives $\mathcal F(|x|^{-2})=2\pi^2/|\xi|$. The linear change of variables $y=G^{1/2}x$ gives the displayed formula. No [principal value](complex-analysis.md#cauchy-principal-value) or origin-supported correction is required. The result is homogeneous of degree $-1$ on the frequency side.

###### Accretive complex quadratic reciprocal Fourier transform

↑ **Parent:** [Fourier transform of a reciprocal positive quadratic form](#fourier-transform-of-a-reciprocal-positive-quadratic-form)

For a complex symmetric three-dimensional $A=G+iB$ with real symmetric $B$ and positive-definite $G$, the reciprocal is a regular [tempered distribution](fourier-analysis.md#tempered-distribution) since $|x^TAx|\geq x^TGx$. Holomorphic continuation of the real quadratic transform proves the displayed expression. The [determinant](linear-algebra.md#determinant) branch is the [analytic determinant square root for accretive symmetric matrices](vector-space.md#analytic-determinant-square-root-for-accretive-symmetric-matrices). The other root has positive real part because $\operatorname{Re}(\xi^TA^{-1}\xi)=\xi^TG^{-1/2}(1+C^2)^{-1}G^{-1/2}\xi>0$ for nonzero real $\xi$. Both the original and transformed singularities are locally integrable, so the continued identity holds as [distributions](#distribution-mathematical-analysis) at the origin too.

## Riesz potential

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz_potential)

For $0<\alpha<n$, the Riesz potential is convolution with a constant multiple of $|x|^{\alpha-n}$. Its [Fourier multiplier](analysis.md#fourier-multiplier-operator) is a constant multiple of $|\xi|^{-\alpha}$.

### Riesz kernel

↑ **Parent:** [Riesz potential](#riesz-potential)

The locally integrable homogeneous function $x\mapsto|x|^{-\alpha}$, $0<\alpha<n$, is a Riesz kernel. For $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$,

$$
\widehat{|x|^{-\alpha}}(\xi)
=2^{n-\alpha}\pi^{n/2}
\frac{\Gamma((n-\alpha)/2)}{\Gamma(\alpha/2)}
|\xi|^{\alpha-n}.
$$

### Hedberg inequality

↑ **Parent:** [Riesz potential](#riesz-potential)

If $1<p<n/\alpha$, the pointwise Hedberg inequality is

$$
I_\alpha|f|(x)
\leq C_{n,p,\alpha}
\lVert f\rVert_p^{\alpha p/n}
(Mf(x))^{1-\alpha p/n}.
$$

Split the integral at radius $r$. Dyadic annuli bound the near part by $C r^\alpha Mf(x)$, while [Hölder's inequality](real-analysis.md#holder-s-inequality) bounds the far part by $C\lVert f\rVert_p r^{\alpha-n/p}$. Choosing $r^{n/p}=\lVert f\rVert_p/Mf(x)$ balances the terms.

## Mollifier

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mollifier)

A standard mollifier is a nonnegative [test function](#test-function) $\rho$ with integral one. The rescaling $\rho_\varepsilon(x)=\varepsilon^{-n}\rho(x/\varepsilon)$ forms an approximation to the identity, and $u*\rho_\varepsilon$ is smooth wherever the convolution stays inside the domain.

### Mollification

↑ **Parent:** [Mollifier](#mollifier)

Mollification is the regularization of a [function](function.md) or [distribution](#distribution-mathematical-analysis) by [convolution](fourier-analysis.md#convolution) with a rescaled [mollifier](#mollifier). It creates [smooth functions](analysis.md#smooth-function) on interior regions, preserves constant-coefficient distributional equations there, and converges back to the original object in the appropriate local topology as the radius tends to zero. The process is distinct from the kernel used to perform it.

### Mollification of a divergence-forcing equation

↑ **Parent:** [Mollifier](#mollifier)

The distributional equation $\Delta u=\operatorname{div}(bu)+cu+f$ becomes the smooth interior equation $\Delta u_\sigma=\operatorname{div}(bu)_\sigma+(cu)_\sigma+f_\sigma$. The products are convolved as wholes. Only coefficient bounds on compact interior sets are needed, and the [divergence-forcing interior H1 estimate](#divergence-forcing-interior-h1-estimate) provides a uniform first derivative bound.

## Support of a distribution

↑ **Parent:** [Distribution theory](distribution-theory.md)

The support of a [distribution](#distribution-mathematical-analysis) is the complement of the largest [open set](topology.md#open-set) on which its pairing vanishes for every supported [test function](#test-function). A [partition of unity](differential-geometry.md#partition-of-unity) shows that the union of such open sets still has this vanishing property. For example, the [Dirac delta distribution](#dirac-delta-function) and all its derivatives have support $\{0\}$.

### Compactly supported distribution

↑ **Parent:** [Support of a distribution](#support-of-a-distribution)

A distribution has compact support when it vanishes on every test function supported outside some compact set. Every compactly supported distribution has finite order.

#### Negative Sobolev regularity of a compactly supported distribution

↑ **Parent:** [Compactly supported distribution](#compactly-supported-distribution)

A [compactly supported distribution](#compactly-supported-distribution) of [order of a distribution](#order-of-a-distribution) at most $M$ has a [smooth function](analysis.md#smooth-function) as its [Fourier transform](analysis.md#fourier-transform), bounded by $C\langle\xi\rangle^M$. It therefore belongs to every [Sobolev space](sobolev-space.md) $H^s$ with $s<-M-n/2$.

#### Fourier transform of a compactly supported distribution

↑ **Parent:** [Compactly supported distribution](#compactly-supported-distribution)

For $u\in\mathcal E'(\mathbb R^n)$, its [Fourier transform](analysis.md#fourier-transform) is the [smooth function](analysis.md#smooth-function)

$$
\widehat u(\lambda)=\langle u(x),e^{-i\lambda\cdot x}\rangle.
$$

It has at most [polynomial growth](analysis.md#polynomial-growth), and its extension to complex frequency is controlled more precisely by the [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem).

##### Shrinking-cutoff exponential-type estimate

↑ **Parent:** [Fourier transform of a compactly supported distribution](#fourier-transform-of-a-compactly-supported-distribution)

Let a [distribution](#distribution-mathematical-analysis) have support in a [compact convex set](mathematical-optimization.md#compact-convex-set) $K$. Fixed neighborhood cutoffs initially give an exponential bound larger than the [support function](mathematical-optimization.md#support-function) $H_K$. Cutoffs of width $\varepsilon$ cost powers of $\varepsilon^{-1}$ in derivative estimates but enlarge the exponential by only $e^{C\varepsilon|\operatorname{Im}z|}$. Choosing $\varepsilon=(1+|z|)^{-1}$ absorbs the cutoff cost into a polynomial and retains the exact exponential $e^{H_K(\operatorname{Im}z)}$.

##### Fourier decay in a bounded complex strip

↑ **Parent:** [Fourier transform of a compactly supported distribution](#fourier-transform-of-a-compactly-supported-distribution)

For a [test function](#test-function) $\varphi$ supported in a fixed ball of radius $R$ and a fixed height bound $H$, repeated [integration by parts](calculus.md#integration-by-parts) gives

$$
|\widehat\varphi(\xi+i\eta)|\leq C_{R,H,L}
\max_{|\alpha|\leq2L}\|\partial^\alpha\varphi\|_\infty(1+|\xi|^2)^{-L},
\qquad |\eta|\leq H.
$$

Apply $(1-\Delta)^L$ to the compactly supported smooth function $e^{x\cdot\eta}\varphi(x)$ inside the real-frequency Fourier integral. The bounded $\eta$ absorbs its derivative and exponential factors into the constant. This estimate makes the numerator of a [Hörmander staircase](#hormander-staircase) integral absolutely integrable and makes truncated contour endpoints vanish.

#### Structure theorem for compactly supported distributions

↑ **Parent:** [Compactly supported distribution](#compactly-supported-distribution)

Every compactly supported distribution is a finite sum of distributional derivatives of bounded continuous functions. One proof convolves it with a sufficiently high-order [Bessel potential](#bessel-potential) and then applies a power of $1-\Delta$.

##### Compact continuous-derivative representation of a distribution

↑ **Parent:** [Structure theorem for compactly supported distributions](#structure-theorem-for-compactly-supported-distributions)

Every [compactly supported distribution](#compactly-supported-distribution) on an [open set](topology.md#open-set) $X$ is a finite sum $u=\sum_\alpha\partial^\alpha f_\alpha$ with continuous $f_\alpha$ compactly supported inside $X$. One can first write $u=\partial^\gamma F$ for a continuous global [convolution](fourier-analysis.md#convolution) primitive, then multiply by a [cutoff function](#cutoff-function) equal to one near the support. The identity $\chi\partial^\gamma F=\sum_{\beta\leq\gamma}(-1)^{|\beta|}\binom\gamma\beta\partial^{\gamma-\beta}[(\partial^\beta\chi)F]$ localizes every coefficient. Finite global representation can fail for a [distribution of unbounded order](#distribution-of-unbounded-order).

##### Bessel potential

↑ **Parent:** [Structure theorem for compactly supported distributions](#structure-theorem-for-compactly-supported-distributions)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bessel_potential)

The Bessel potential of order $s$ is the Fourier multiplier $(1+|\xi|^2)^{-s/2}$. Sufficiently high order turns a compactly supported finite-order distribution into a bounded continuous function.

## Fundamental solution of a linear differential operator

↑ **Parent:** [Distribution theory](distribution-theory.md)

A fundamental solution of a linear differential operator $P(D)$ is a distribution $E$ satisfying $P(D)E=\delta_0$.

<h3 id="malgrange-ehrenpreis-theorem">Malgrange–Ehrenpreis theorem</h3>

↑ **Parent:** [Fundamental solution of a linear differential operator](#fundamental-solution-of-a-linear-differential-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Malgrange–Ehrenpreis_theorem)

Every nonzero constant-coefficient linear partial differential operator has a distributional fundamental solution.

<h4 id="hormander-staircase">Hörmander staircase</h4>

↑ **Parent:** [Malgrange–Ehrenpreis theorem](#malgrange-ehrenpreis-theorem)

Let $P(\xi',z)$ be a polynomial that is monic in the complex variable $z$. A Hörmander staircase partitions the real $\xi'$-space into measurable sets $\Delta_j$ and assigns bounded heights $c_j$ so that $P(\xi',s+ic_j)$ stays uniformly away from zero for $\xi'\in\Delta_j$ and $s\in\mathbb R$. Integrating $1/P$ over the resulting union of horizontal contours constructs a [fundamental solution of a linear differential operator](#fundamental-solution-of-a-linear-differential-operator).

##### Finite-height polynomial root avoidance

↑ **Parent:** [Hörmander staircase](#hormander-staircase)

Suppose $P(\xi',z)$ has degree $m$ in $z$ and a nonzero constant leading coefficient $a$. Among the $m+1$ heights $h_\ell=3\ell$, at least one satisfies

$$
|P(\xi',s+ih_\ell)|\geq|a|\qquad\text{for all }s\in\mathbb R
$$

at each real $\xi'$. Factor into $m$ linear factors with multiplicity. Each root's imaginary part can be within distance less than one of at most one candidate height. The [pigeonhole principle](algebra.md#pigeonhole-principle) leaves a height whose distance from every root is at least one, proving the product bound. The height can be chosen measurably: the set where a candidate succeeds is the closed intersection of $|P(\xi',q+ih_\ell)|\geq|a|$ over rational $q$, and selecting the first successful candidate gives a [Borel set](measure-theory.md#borel-set) partition. This avoids any need for continuous global root labels.

### Retarded fundamental solution

↑ **Parent:** [Fundamental solution of a linear differential operator](#fundamental-solution-of-a-linear-differential-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Retarded_fundamental_solution)

A retarded fundamental solution is supported in a chosen forward region, such as $[0,\infty)$ for an ordinary differential operator.

#### Retarded fundamental solution of a constant-coefficient ordinary differential operator

↑ **Parent:** [Retarded fundamental solution](#retarded-fundamental-solution)

For $P(z)=a_Nz^N+\cdots+a_0$ with $N\geq1$ and $a_N\ne0$, the unique [retarded fundamental solution](#retarded-fundamental-solution) is $E=Hu$, where $P(D)u=0$, $u^{(j)}(0)=0$ for $j<N-1$, and $u^{(N-1)}(0)=1/a_N$. The [distributional jump formula for a Heaviside product](#distributional-jump-formula-for-a-heaviside-product) gives $P(D)E=\delta_0$. Its explicit expression is

$$
u(x)=\sum_{P(\lambda)=0}\operatorname*{Res}_{z=\lambda}\frac{e^{zx}}{P(z)}.
$$

The [residue theorem](analysis.md#residue-theorem) gives the initial derivatives from the coefficients at infinity. Equivalently, the inverse [Fourier transform](analysis.md#fourier-transform) is integrated below all its poles, producing [support of a distribution](#support-of-a-distribution) in $[0,\infty)$. Uniqueness follows because the difference of two retarded solutions is an analytic homogeneous solution vanishing on the negative half-line.

## Elliptic differential operator

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_differential_operator)

A constant-coefficient operator of order $N$ is elliptic when its homogeneous principal symbol $P_N(\xi)$ is nonzero for every real $\xi\ne0$.

### Elliptic system of differential equations

↑ **Parent:** [Elliptic differential operator](#elliptic-differential-operator)

A square system whose entries have common maximal order $N$ is elliptic when its matrix [principal symbol](partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) is invertible at every nonzero real frequency. Unlike scalar operators, a system can be first-order elliptic in three dimensions: the [Pauli matrices](algebra.md#pauli-matrices) give $A(\xi)=\sum_j\sigma_j\xi_j$ with $A(\xi)^2=|\xi|^2\mathbf1$.

### Odd-order obstruction for scalar elliptic operators in at least three dimensions

↑ **Parent:** [Elliptic differential operator](#elliptic-differential-operator)

The [principal symbol](partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) of an odd-order scalar [differential operator](analysis.md#differential-operator) is an odd map from the frequency [sphere](geometry-and-topology.md#sphere) to the complex plane. The [Borsuk-Ulam theorem](algebraic-topology.md#borsuk-ulam-theorem) forces a zero on a two-dimensional [sphere](geometry-and-topology.md#sphere), contradicting ellipticity. Restriction to three variables proves the same obstruction in every greater dimension.

### High-frequency lower bound for an elliptic polynomial

↑ **Parent:** [Elliptic differential operator](#elliptic-differential-operator)

A scalar [elliptic differential operator](#elliptic-differential-operator) of order $N$ has a [principal symbol](partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) nonzero on the unit [sphere](geometry-and-topology.md#sphere). Compactness gives a positive minimum there, and homogeneity makes that term dominate all lower-degree terms at sufficiently large real frequencies.

### Elliptic regularity

↑ **Parent:** [Elliptic differential operator](#elliptic-differential-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_regularity)

Elliptic regularity says that solutions of an [elliptic equation](#elliptic-differential-operator) gain derivatives wherever the coefficients and forcing are regular. For the [Laplacian](calculus.md#laplacian), local estimates typically control two derivatives of $u$ by $\Delta u$ together with a lower-order norm of $u$.

#### Interior second-derivative estimate for the Poisson equation

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

If $u\in H^1(V)$ and $\Delta u=f\in L^2(V)$ weakly, then $u\in H^2_{\mathrm{loc}}(V)$. Test the weak equation with $-\delta_{-h}(\eta^2\delta_hu)$, move the first difference quotient onto $Du$, and bound the remaining quotient on the forcing side by the first derivative of $\eta^2\delta_hu$. [Young inequality](nonlinear-analysis.md#young-s-inequality-for-products) absorbs the localized second derivatives. Uniform bounds in $h$, together with the [Sobolev characterization by bounded difference quotients](sobolev-space.md#sobolev-characterization-by-bounded-difference-quotients), give the assertion without differentiating $f$. The constant depends only on dimension and the positive distance from $U$ to the boundary of $V$.

// Target: geometry-and-topology.bigb

#### Elliptic regularity bootstrap with smooth lower-order coefficients

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

Once an $L^2$ distributional solution of $\Delta u=\operatorname{div}(bu)+cu+f$ gains $H^1$ regularity, expand the divergence term. Smooth multiplication makes the right side belong to $H^{m-1}_{\mathrm{loc}}$ whenever $u\in H^m_{\mathrm{loc}}$. Interior Poisson regularity gives $H^{m+1}_{\mathrm{loc}}$. Iteration and the [Sobolev embedding theorem](sobolev-space.md#sobolev-embedding-theorem) produce a smooth representative.

#### Divergence-forcing interior H1 estimate

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

For $\Delta v=\operatorname{div}F+G$ and $U\subset\subset V$, a [cutoff function](#cutoff-function) energy estimate gives $\|v\|_{H^1(U)}\leq C(\|v\|_{L^2(V)}+\|F\|_{L^2(V)}+\|G\|_{L^2(V)})$. One derivative of forcing is permitted because [integration by parts](calculus.md#integration-by-parts) places it on the [test function](#test-function). This estimate allows a mollified distributional solution initially in $L^2$ to gain its first [weak derivative](#weak-derivative).

#### Interior gradient estimate near a zero Dirichlet side

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

For a smooth [uniformly elliptic](elliptic-boundary-value-problem.md#uniformly-elliptic-operator) homogeneous equation away from other boundaries, an interior [gradient](calculus.md#gradient) estimate on a ball of radius comparable to the distance $s$ from a flat side gives $|\nabla u|\leq Cs^{-1}\sup_{B_{cs}}|u|$. If $u$ extends continuously with value zero on that side, $s|\nabla u|\to0$ locally along it. This justifies vanishing boundary terms such as $u_x\sin(nx)$ in a distributional Fourier sine projection.

#### Second-derivative estimate at a flat Dirichlet boundary

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

For a [classical solution](partial-differential-equation.md#classical-solution) of $\Delta u=f$ on a half-ball with zero data on its flat face, a tangential [Caccioppoli inequality](partial-differential-equation.md#caccioppoli-inequality) controls every second [partial derivative](calculus.md#partial-derivative) having at least one tangential index. The equation recovers the remaining second [normal derivative](differential-geometry.md#normal-derivative). The resulting [Sobolev norm](sobolev-space.md#sobolev-norm) estimate has a dimension-only constant for the fixed radii one and two. Nonzero data are handled by [homogenization of Dirichlet boundary data](sobolev-space.md#homogenization-of-dirichlet-boundary-data), adding the $W^{2,2}$ norm of the supplied boundary extension. No condition is imposed on the curved face because the [smooth cutoff function](analysis.md#smooth-cutoff-function) vanishes there.

#### Cutoff bootstrap for local elliptic regularity

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

For a constant-coefficient [elliptic differential operator](#elliptic-differential-operator) $P(D)$ of order $N\geq1$, localizing the equation gives $P(D)(\chi u)=\chi P(D)u+[P(D),\chi]u$. The [commutator](lie-algebra.md#commutator) has order at most $N-1$, so a global [Fourier transform](analysis.md#fourier-transform) estimate raises the known [Local Sobolev space](sobolev-space.md#local-sobolev-space) index by one until the forcing index plus $N$ is reached.

#### Spectral characterization of elliptic Dirichlet domains

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

Let $(w_m)$ be the [orthonormal basis](linear-algebra.md#orthonormal-basis) of Dirichlet [eigenfunctions](linear-operator-theory.md#eigenfunction) for a strictly positive [Dirichlet realization of an elliptic operator](elliptic-boundary-value-problem.md#dirichlet-realization-of-an-elliptic-operator), with [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_m$. Then

$$
u\in D(A_D^{k/2})\iff\sum_m\lambda_m^k|(u,w_m)_{L^2}|^2<\infty.
$$

For integers $k$, these domains are the [Sobolev domains of powers of an elliptic Dirichlet operator](#sobolev-domains-of-powers-of-an-elliptic-dirichlet-operator). At $k=0$ the condition is just [Parseval identity](fourier-analysis.md#parseval-identity) and imposes no boundary condition. At $k=1,2$ it describes $H_0^1$ and $H^2\cap H_0^1$, respectively. Higher $k$ impose traces of powers of $L$, not only the trace of $u$. For $L=-d^2/dx^2$ on $(0,\pi)$, the smooth Dirichlet function $u=x(\pi-x)$ has sine coefficients proportional to $m^{-3}$ for odd $m$, so the weighted sum diverges at $k=3$ despite its ordinary $H^3$ regularity.

#### Sobolev domains of powers of an elliptic Dirichlet operator

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

For a strictly positive [Dirichlet realization of an elliptic operator](elliptic-boundary-value-problem.md#dirichlet-realization-of-an-elliptic-operator) with smooth coefficients and smooth boundary, put $X_0=L^2(U)$. For each integer $k\geq1$,

$$
X_k=\left\{u\in H^k(U):T(L^ju)=0\quad 0\leq j\leq\left\lfloor\frac{k-1}{2}\right\rfloor\right\}.
$$

These are the domains $D(A_D^{k/2})$, with norms equivalent to the indicated [Sobolev space](sobolev-space.md) norms. The [bilinear forms](linear-algebra.md#bilinear-form) $((u,v))_{2l}=(L^lu,L^lv)_{L^2}$ and $((u,v))_{2l+1}=B[L^lu,L^lv]$ are [inner products](linear-algebra.md#inner-product) on $X_{2l}$ and $X_{2l+1}$. The higher boundary conditions are essential: for $L=-d^2/dx^2$ and $u=x(\pi-x)$, $u$ is smooth and zero at the boundary but $L^2u=0$, so $\|L^2u\|_2$ is not a norm on all of $H^4\cap H_0^1$. Repeated [elliptic regularity](#elliptic-regularity) proves $A_D:X_{k+2}\to X_k$ is an isomorphism, which gives the norm equivalence inductively from $X_0$ and $X_1=H_0^1$.

#### Boundary elliptic regularity for the shifted Dirichlet Laplacian

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

On a smooth bounded domain, a solution of

$$
(\Delta-c)u=f,\qquad u|_{\partial\Omega}=0,
$$

for an invertible shift satisfies

$$
\|u\|_{H^{k+2}}\leq C_k\|f\|_{H^k}.
$$

Interior regularity and boundary flattening give the derivative gain, while invertibility controls the lower-order norm.

#### Dirichlet Poisson regularity theorem

↑ **Parent:** [Elliptic regularity](#elliptic-regularity)

If $U\subset\mathbb R^n$ is bounded with $C^2$ boundary, then every $F\in L^2(U)$ determines a unique $v\in H^2(U)\cap H_0^1(U)$ satisfying

$$
-\Delta v=F,
\qquad
\|v\|_{H^2(U)}\leq C\|F\|_{L^2(U)}.
$$

### Parametrix

↑ **Parent:** [Elliptic differential operator](#elliptic-differential-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parametrix)

A parametrix for $P$ is an operator $A$ such that $PA-I$ and, when relevant, $AP-I$ are regularizing operators.

#### High-frequency reciprocal parametrix kernel

↑ **Parent:** [Parametrix](#parametrix)

For a [polynomial](polynomial.md) with no sufficiently large real zero, a compact low-frequency [cutoff function](#cutoff-function) removes its remaining zeros. A reciprocal satisfying $|\partial^\alpha b|\lesssim\langle\xi\rangle^{-m-\delta|\alpha|}$, $m\geq0$, $0<\delta\leq1$, defines a [Fourier multiplier](analysis.md#fourier-multiplier) mapping $H^s$ to $H^{s+m}$. Its inverse-transform kernel is smooth off zero: repeated frequency [integration by parts](calculus.md#integration-by-parts) supplies arbitrary decay even after multiplying by powers of frequency for spatial [derivatives](calculus.md#derivative). Consequently a [compactly supported distribution](#compactly-supported-distribution) supported away from the target contributes only a smooth function there. In a local regularity proof, the [cutoff function](#cutoff-function) commutator is placed in that separated region rather than estimated only by its differential order.

### Symbol class

↑ **Parent:** [Elliptic differential operator](#elliptic-differential-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symbol_class)

A smooth function $a(x,\xi)$ belongs to $S^m_{1,0}$ when, on every compact $K\subset X$,

$$
|D_x^\alpha D_\xi^\beta a(x,\xi)|\leq C_{K,\alpha,\beta}\langle\xi\rangle^{m-|\beta|}.
$$

#### Symbol calculus

↑ **Parent:** [Symbol class](#symbol-class)

Frequency differentiation lowers symbol order, position differentiation preserves it, products add orders, and finite sums have order at most the maximum order.

## Oscillatory integral

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oscillatory_integral)

An oscillatory integral uses cancellation to define a distribution even when its integral is not absolutely convergent. Repeated integration by parts transfers derivatives to the amplitude and exposes decay.

### Abel regularization of an oscillatory integral

↑ **Parent:** [Oscillatory integral](#oscillatory-integral)

An exponential damping factor makes many otherwise conditionally convergent or divergent [oscillatory integrals](#oscillatory-integral) absolutely convergent. Removing the damping after integration defines an Abel limit when it exists. For the [Bessel function](analysis.md#bessel-function) $J_1$, $\int_0^\infty e^{-ak}J_1(kR)dk=R^{-1}(1-a/\sqrt{a^2+R^2})$, giving the [Mestel disk](astrophysics.md#mestel-disk) radial field as $a\downarrow0$. This does not remove an unrelated additive divergence of the potential at low wavenumber.

### Cutoff independence of an oscillatory integral

↑ **Parent:** [Oscillatory integral](#oscillatory-integral)

For an amplitude of symbol order $N$ in $k$ frequency variables, applying a phase integration operator $r>N+k$ times makes the pairing with a [test function](#test-function) absolutely integrable. Derivatives of a large-frequency cutoff are supported where $|\theta|\asymp R$ and give an error bounded by $CR^{N-r+k}$ times finitely many test derivatives. That error tends to zero, making the resulting [distribution](#distribution-mathematical-analysis) independent of the cutoff and of the admissible number of integrations.

### Symbol order reduction by a phase integration operator

↑ **Parent:** [Oscillatory integral](#oscillatory-integral)

For a homogeneous [phase function](#phase-function), let $q=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2$ and $L=(iq)^{-1}(\nabla_x\Phi\cdot\nabla_x+|\theta|^2\nabla_\theta\Phi\cdot\nabla_\theta)$. Then $Le^{i\Phi}=e^{i\Phi}$. The [formal transpose of a differential operator](analysis.md#formal-transpose-of-a-differential-operator) $L^t$ lowers the [symbol class](#symbol-class) order by one: the $x$ coefficients have order $-1$, while the order-zero frequency coefficients accompany a frequency derivative.

### Finite order of an oscillatory integral distribution

↑ **Parent:** [Oscillatory integral](#oscillatory-integral)

An [oscillatory integral](#oscillatory-integral) with a degree-one homogeneous [phase function](#phase-function), $k$ frequency variables, and [oscillatory integral amplitude](#amplitude-of-an-oscillatory-integral) in fixed [symbol class](#symbol-class) order $N$ has [order of a distribution](#order-of-a-distribution) at most any nonnegative integer $r>N+k$. The integer works on every [compact set](topology.md#compact-space); the continuity constant can vary with the [compact set](topology.md#compact-space).

### Amplitude of an oscillatory integral

↑ **Parent:** [Oscillatory integral](#oscillatory-integral)

An oscillatory integral amplitude multiplies $e^{i\Phi}$ in an [oscillatory integral](#oscillatory-integral) with [phase function](#phase-function) $\Phi$. A finite [symbol class](#symbol-class) order controls its frequency growth and the [order of a distribution](#order-of-a-distribution) obtained by [integration by parts](calculus.md#integration-by-parts).

#### Conic support of an oscillatory amplitude

↑ **Parent:** [Amplitude of an oscillatory integral](#amplitude-of-an-oscillatory-integral)

A closed conic enlargement of an [oscillatory integral amplitude](#amplitude-of-an-oscillatory-integral) support is obtained by taking the closure of its frequency-direction projection in $X\times S^{k-1}$ and lifting that set radially to nonzero frequencies. It records limiting spatial locations and frequency directions, including limits reached only at arbitrarily large frequency. Ordinary support in $X\times\mathbb R^k$ need not record those limits. This distinction is necessary in [singular support](#singular-support) bounds for an [oscillatory integral](#oscillatory-integral).

##### Stationary-direction bound for singular support

↑ **Parent:** [Conic support of an oscillatory amplitude](#conic-support-of-an-oscillatory-amplitude)

For a homogeneous [phase function](#phase-function) $\Phi$ and finite-order [symbol class](#symbol-class) amplitude $a$, the [singular support](#singular-support) of $I_\Phi(a)$ lies in the spatial projection of the closed conic amplitude support intersected with $\nabla_\theta\Phi=0$. Away from that set, the frequency gradient is uniformly nonzero on compact spatial sets and supported directions. Repeated frequency [integration by parts](calculus.md#integration-by-parts) lowers the amplitude order until every desired spatial derivative is absolutely integrable. If the ordinary amplitude support is already conic, it gives the same bound.

###### Slice-support obstruction for oscillatory singularities

↑ **Parent:** [Stationary-direction bound for singular support](#stationary-direction-bound-for-singular-support)

In one base and one phase variable, take $\Phi=x\theta$ and $a=x\eta(\theta)/|\theta|$, with an even smooth [cutoff function](#cutoff-function) equal to zero near zero and one for large $|\theta|$. This is a symbol of order $-1$. Its [oscillatory integral](#oscillatory-integral) is $-2x\log|x|$ plus a smooth function near zero. Thus it is singular there even though the restricted function $a(0,\cdot)$ has empty support. The joint closed [conic support of an oscillatory amplitude](#conic-support-of-an-oscillatory-amplitude) retains the limiting base point and its stationary directions. A support-sensitive regularity theorem must use that conic neighborhood information, not merely vanishing of an amplitude at one base point.

###### Ordinary amplitude support can miss a singular-support limit

↑ **Parent:** [Stationary-direction bound for singular support](#stationary-direction-bound-for-singular-support)

For $\Phi(s,t,\theta)=s\theta$, take a smooth symbol that turns on increasingly high frequencies in disjoint spatial bumps centered at $t_j\to0$. Superpolynomially small bump coefficients keep all [symbol class](#symbol-class) estimates valid. The amplitude vanishes near every finite-frequency point over $t=0$, yet its [oscillatory integral](#oscillatory-integral) has delta singularities at $(0,t_j)$. Closedness of [singular support](#singular-support) forces a singularity at $(0,0)$ as well. A bound using only ordinary, rather than closed conic, amplitude support can consequently fail.

### Phase function

↑ **Parent:** [Oscillatory integral](#oscillatory-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_function)

A phase function is a real smooth function $\Phi(x,\theta)$ on $X\times(\mathbb R^k\setminus\{0\})$ that is positively homogeneous of degree one in $\theta$ and has nonvanishing total differential. Its critical points in the frequency variable determine where an associated oscillatory integral may be singular.

## Singular support

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_support)

The singular support of a distribution is the complement of the largest open set on which it is represented by a smooth function.

<h2 id="paley-wiener-theorem">Paley–Wiener theorem</h2>

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Paley–Wiener_theorem)

Paley–Wiener theorems relate spatial support or decay to analytic continuation and growth of the [Fourier transform](analysis.md#fourier-transform). Different versions apply to square-integrable functions or to [distributions](#distribution-mathematical-analysis). The [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem) is the distributional version.

<h3 id="paley-wiener-schwartz-theorem">Paley–Wiener–Schwartz theorem</h3>

↑ **Parent:** [Paley–Wiener theorem](#paley-wiener-theorem)

For a compact convex set $K\subset\mathbb R^n$, the [Fourier transform](analysis.md#fourier-transform) gives a bijection between distributions supported in $K$ and entire functions satisfying

$$
|F(\zeta)|\leq C(1+|\zeta|)^N e^{H_K(\operatorname{Im}\zeta)},
\qquad H_K(\eta)=\sup_{x\in K}x\cdot\eta,
$$

for some $C,N$. Here $H_K$ is the [support function](mathematical-optimization.md#support-function). In the closed-ball case $K=\overline B_R$, the exponential factor is $e^{R|\operatorname{Im}\zeta|}$. Convexity is essential to infer support in $K$ from this bound: the support function cannot distinguish a nonconvex set from its convex hull.

#### Fourier independence from disjoint distribution supports

↑ **Parent:** [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem)

Nonzero [compactly supported distributions](#compactly-supported-distribution) with pairwise disjoint supports are linearly independent: a [smooth cutoff function](analysis.md#smooth-cutoff-function) isolating one support isolates its coefficient. Injectivity transfers this independence to their [Fourier transforms](analysis.md#fourier-transform). Exponential-type bounds and the [Translation property of the Fourier transform](fourier-analysis.md#translation-property-of-the-fourier-transform) can prove the needed support separation before the distributions themselves are known explicitly.

#### Polynomial division preservation of exponential type

↑ **Parent:** [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem)

Let $F$ be an [entire function](complex-analysis.md#entire-function) of one variable satisfying $|F(\zeta)|\leq C(1+|\zeta|)^Ne^{R|\operatorname{Im}\zeta|}$, and let $P$ be a nonzero [polynomial](polynomial.md). If $F/P$ is entire, it satisfies a bound of the same exponential type, with a possibly different polynomial power. Indeed, outside a sufficiently large disk, $|P(\zeta)|\geq c(1+|\zeta|)^{\deg P}$; inside the disk the extended quotient is bounded. Combining these estimates proves the claim. The same reasoning works with the exact [support function](mathematical-optimization.md#support-function) of a compact interval. Zeros of $F$ must cancel every root of $P$ with its full multiplicity.

<h4 id="contour-shift-proof-of-the-paley-wiener-schwartz-theorem">Contour-shift proof of the Paley–Wiener–Schwartz theorem</h4>

↑ **Parent:** [Paley–Wiener–Schwartz theorem](#paley-wiener-schwartz-theorem)

For the forward implication, finite [order of a distribution](#order-of-a-distribution) makes $F(\zeta)=\langle u,e^{-ix\cdot\zeta}\rangle$ entire. Use a smooth cutoff in an $\varepsilon$-neighborhood of the support set, with derivatives of order $j$ bounded by $C_j\varepsilon^{-j}$. Taking $\varepsilon=(1+|\zeta|)^{-1}$ in the finite-order estimate gives the polynomial factor and adds at most $e$ to the desired exponential bound. This shrinking cutoff recovers the exact support indicator, instead of an arbitrarily enlarged one.

For the converse, the real restriction of $F$ has [polynomial growth](analysis.md#polynomial-growth) and defines an inverse [tempered distribution](fourier-analysis.md#tempered-distribution). If a [test function](#test-function) $\varphi$ is supported in $x\cdot\omega\geq R+\eta$ for a unit vector $\omega$ and $\eta>0$, [contour shifting](complex-analysis.md#contour-shifting) gives

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int F(\xi+it\omega)\widehat\varphi(-\xi-it\omega)\,d\xi.
$$

Repeated [integration by parts](calculus.md#integration-by-parts) gives, for every integer $M$,

$$
|\widehat\varphi(-\xi-it\omega)|
\leq C_M(1+t)^{2M}e^{-(R+\eta)t}(1+|\xi|^2)^{-M}.
$$

Choosing $2M>N+n$ justifies the shift by [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) and bounds the pairing by $C'(1+t)^{N+2M}e^{-\eta t}$, which tends to zero. Half-spaces of this form cover the complement of the ball, and a [partition of unity](differential-geometry.md#partition-of-unity) proves the support inclusion. For general compact convex $K$, replace $R$ by $H_K(\omega)$ in each separating direction. [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) gives uniqueness. A related proof outline appears in [Richard Melrose's distribution-theory problem set](https://math.mit.edu/~rbm/Problems4.pdf).

##### Mollifier regularization for contour recovery of support

↑ **Parent:** [Contour-shift proof of the Paley–Wiener–Schwartz theorem](#contour-shift-proof-of-the-paley-wiener-schwartz-theorem)

For an [entire function](complex-analysis.md#entire-function) of polynomial growth and exponential type $H_K$, multiply it by $\widehat\rho(\varepsilon z)$ with a unit-mass [mollifier](#mollifier). The product becomes rapidly decreasing in real frequency, so its inverse [Fourier transform](analysis.md#fourier-transform) has an absolutely convergent contour integral. Shifting in a separating direction forces that smooth inverse to vanish outside $K+\varepsilon\overline B_1$. Letting $\varepsilon$ tend to zero recovers a [distribution](#distribution-mathematical-analysis) supported in $K$.

## Hypoelliptic operator

↑ **Parent:** [Distribution theory](distribution-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypoelliptic_operator)

A differential operator $P$ is hypoelliptic when $Pu$ smooth on an open set implies that $u$ is smooth there. Every elliptic differential operator is hypoelliptic, but the heat operator is hypoelliptic without being elliptic.

### Derivative-ratio Sobolev gain for a polynomial operator

↑ **Parent:** [Hypoelliptic operator](#hypoelliptic-operator)

Suppose a degree-$N$ [polynomial](polynomial.md) obeys $|\partial^\alpha Q(\xi)|\leq C_\alpha|\xi|^{-\delta|\alpha|}|Q(\xi)|$ at large real frequency, with $\delta>0$. A nonzero constant [derivative](calculus.md#derivative) of total order $N$ gives $|Q|\gtrsim\langle\xi\rangle^{\delta N}$. Reciprocal differentiation then bounds $\partial^\alpha(1/Q)$ by $\langle\xi\rangle^{-\delta N-\delta|\alpha|}$. The [high-frequency reciprocal parametrix kernel](#high-frequency-reciprocal-parametrix-kernel) therefore gains $\delta N$ Sobolev [derivatives](calculus.md#derivative). Localize the [distribution](#distribution-mathematical-analysis) by a [cutoff function](#cutoff-function) equal to one near the target; the commutator lies outside that target and the reciprocal kernel makes its contribution smooth. This proves the displayed gain without demanding global regularity of the original [distribution](#distribution-mathematical-analysis).

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3.md#15d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-107.md#1/b/solution)
