# Finite difference

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_difference)

A finite difference compares the values of a [function](function.md) at finitely separated arguments. For example, the forward finite difference with step $h$ is

$$
\Delta_hf(x)=f(x+h)-f(x).
$$

It is the discrete analogue of a [derivative](calculus.md#derivative) and lowers the degree of a nonconstant [polynomial](polynomial.md) by one.

**Table of contents**

- [Three-point asymmetric second-derivative formula](#three-point-asymmetric-second-derivative-formula)
- [Randomized symmetric finite-difference derivative estimator](#randomized-symmetric-finite-difference-derivative-estimator)
- [Finite difference method](#finite-difference-method)
  - [Midpoint flux stencil for one-dimensional diffusion](#midpoint-flux-stencil-for-one-dimensional-diffusion)
  - [Finite difference coefficient](#finite-difference-coefficient)
  - [Fourth-order two-step advection stencil](#fourth-order-two-step-advection-stencil)
  - [Mehrstellen method](#mehrstellen-method)
    - [Compact semidiscrete nine-point diffusion](#compact-semidiscrete-nine-point-diffusion)
  - [Rational implicit advection stencil with exact shift exceptions](#rational-implicit-advection-stencil-with-exact-shift-exceptions)
  - [Centered discrete advection is skew-adjoint](#centered-discrete-advection-is-skew-adjoint)
  - [Positive definiteness of the grounded nine-point Poisson stencil](#positive-definiteness-of-the-grounded-nine-point-poisson-stencil)
  - [Implicit advection scheme with exact integer shifts](#implicit-advection-scheme-with-exact-integer-shifts)
  - [Lax-Friedrichs method](#lax-friedrichs-method)
  - [L2-compatible initialization of grid data](#l2-compatible-initialization-of-grid-data)
    - [Cell-average projection](#cell-average-projection)
  - [Discrete summation by parts](#discrete-summation-by-parts)
    - [Inflow advection energy estimate from summation by parts](#inflow-advection-energy-estimate-from-summation-by-parts)
  - [Four-neighbour mean expansion](#four-neighbour-mean-expansion)
  - [Parabolic mesh refinement](#parabolic-mesh-refinement)
  - [Lax-Wendroff advection scheme](#lax-wendroff-advection-scheme)
  - [Symmetric half-grid diffusion consistency](#symmetric-half-grid-diffusion-consistency)
    - [Monotone half-grid diffusion update](#monotone-half-grid-diffusion-update)
  - [Upwind finite difference scheme](#upwind-finite-difference-scheme)
    - [Dissipative second-order forward advection stencil](#dissipative-second-order-forward-advection-stencil)
  - [Five-point Laplacian](#five-point-laplacian)
    - [Unweighted grid error for the five-point Poisson formula](#unweighted-grid-error-for-the-five-point-poisson-formula)
    - [Five-point heat-reaction stability threshold](#five-point-heat-reaction-stability-threshold)
  - [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)
    - [Five-point versus nine-point Laplacian eigenvalue accuracy](#five-point-versus-nine-point-laplacian-eigenvalue-accuracy)
    - [Harmonic superconvergence of the nine-point stencil](#harmonic-superconvergence-of-the-nine-point-stencil)
    - [Compact fourth-order Helmholtz stencil](#compact-fourth-order-helmholtz-stencil)
    - [Jacobi convergence for the nine-point Dirichlet stencil](#jacobi-convergence-for-the-nine-point-dirichlet-stencil)
    - [Negative definiteness of a nine-point Dirichlet stencil](#negative-definiteness-of-a-nine-point-dirichlet-stencil)
    - [Fourth-order correction of the nine-point Poisson stencil](#fourth-order-correction-of-the-nine-point-poisson-stencil)
      - [Sixth-order source correction of the nine-point Poisson stencil](#sixth-order-source-correction-of-the-nine-point-poisson-stencil)
      - [Maximum-norm convergence of the corrected nine-point Poisson scheme](#maximum-norm-convergence-of-the-corrected-nine-point-poisson-scheme)
  - [Fourier stability analysis](#fourier-stability-analysis)
    - [Fourier amplification symbol](#fourier-amplification-symbol)
      - [Scalar Fourier power criterion](#scalar-fourier-power-criterion)
      - [Uniform power bound for matrix Fourier symbols](#uniform-power-bound-for-matrix-fourier-symbols)
  - [Central finite difference](#central-finite-difference)
    - [Fourth-order centered second derivative](#fourth-order-centered-second-derivative)
    - [Sharp central-secant derivative error](#sharp-central-secant-derivative-error)
    - [Centered-advection refinement-dependent stability](#centered-advection-refinement-dependent-stability)
    - [Second-order central difference](#second-order-central-difference)
  - [Forward difference operator](#forward-difference-operator)
    - [Adjoint of a discrete forward gradient](#adjoint-of-a-discrete-forward-gradient)
    - [Discrete antiderivative](#discrete-antiderivative)
    - [Newton series for an integer-valued polynomial sequence](#newton-series-for-an-integer-valued-polynomial-sequence)
  - [von Neumann stability analysis](#von-neumann-stability-analysis)
    - [Nonnormal Fourier amplification matrix](#nonnormal-fourier-amplification-matrix)
    - [Uniform power bound from separated amplification roots](#uniform-power-bound-from-separated-amplification-roots)
    - [Stability of a spatially shifted BDF2 stencil](#stability-of-a-spatially-shifted-bdf2-stencil)
    - [Fourier symbol of a difference operator](#fourier-symbol-of-a-difference-operator)
    - [Power boundedness of a two-level Fourier scheme](#power-boundedness-of-a-two-level-fourier-scheme)
      - [Uniform stability of a shifted two-level advection scheme](#uniform-stability-of-a-shifted-two-level-advection-scheme)
    - [Forward Euler stability for centered advection-diffusion](#forward-euler-stability-for-centered-advection-diffusion)
    - [Laurent operator](#laurent-operator)
      - [Toeplitz operator](#toeplitz-operator)
        - [Toeplitz exponential determinant identity](#toeplitz-exponential-determinant-identity)
        - [Toeplitz index theorem for continuous symbols](#toeplitz-index-theorem-for-continuous-symbols)
    - [Boundary stability of a finite-difference method](#boundary-stability-of-a-finite-difference-method)
      - [Boundary closure of a difference scheme](#boundary-closure-of-a-difference-scheme)
      - [Uniform Kreiss--Lopatinskii condition](#uniform-kreiss-lopatinskii-condition)
    - [Eigenvalue stability analysis of a finite difference method](#eigenvalue-stability-analysis-of-a-finite-difference-method)
      - [Finite-time stability versus power boundedness](#finite-time-stability-versus-power-boundedness)
      - [Negative spectra do not imply uniform semidiscrete stability](#negative-spectra-do-not-imply-uniform-semidiscrete-stability)
      - [Nonnormal upwind amplification matrix](#nonnormal-upwind-amplification-matrix)
    - [Backward Euler diffusion scheme](#backward-euler-diffusion-scheme)
      - [No positive-Courant cancellation for backward Euler diffusion](#no-positive-courant-cancellation-for-backward-euler-diffusion)
      - [Backward Euler diffusion stability on a finite Dirichlet interval](#backward-euler-diffusion-stability-on-a-finite-dirichlet-interval)
    - [Forward Euler diffusion scheme](#forward-euler-diffusion-scheme)
      - [Explicit time stepping for bounded reaction diffusion](#explicit-time-stepping-for-bounded-reaction-diffusion)
    - [Stability of a two-parameter implicit-explicit diffusion scheme](#stability-of-a-two-parameter-implicit-explicit-diffusion-scheme)
    - [Amplification factor](#amplification-factor)
      - [Amplification factor of a two-sided one-step stencil](#amplification-factor-of-a-two-sided-one-step-stencil)
    - [Amplification polynomial of a multilevel finite difference scheme](#amplification-polynomial-of-a-multilevel-finite-difference-scheme)
      - [Leapfrog advection scheme](#leapfrog-advection-scheme)
        - [Two-dimensional leapfrog stability threshold](#two-dimensional-leapfrog-stability-threshold)
        - [Two-level stability at the leapfrog Courant boundary](#two-level-stability-at-the-leapfrog-courant-boundary)
      - [Leapfrog finite-difference scheme for the diffusion equation](#leapfrog-finite-difference-scheme-for-the-diffusion-equation)
    - [Crank-Nicolson diffusion scheme](#crank-nicolson-diffusion-scheme)
    - [Crank-Nicolson centered-advection scheme on a finite interval](#crank-nicolson-centered-advection-scheme-on-a-finite-interval)
    - [Centered three-level wave scheme](#centered-three-level-wave-scheme)
  - [Courant number](#courant-number)
    - [Diffusion Courant number](#diffusion-courant-number)
    - [Courant–Friedrichs–Lewy condition](#courant-friedrichs-lewy-condition)
  - [Dirichlet discrete Laplacian](#dirichlet-discrete-laplacian)
    - [Crank-Nicolson stability on a finite Dirichlet interval](#crank-nicolson-stability-on-a-finite-dirichlet-interval)
    - [Five-point Dirichlet Laplacian as a Kronecker sum](#five-point-dirichlet-laplacian-as-a-kronecker-sum)
      - [One-implicit-direction diffusion splitting](#one-implicit-direction-diffusion-splitting)
        - [Stability limit of one-implicit-direction diffusion splitting](#stability-limit-of-one-implicit-direction-diffusion-splitting)
        - [Unconditionally stable corrected directional diffusion splitting](#unconditionally-stable-corrected-directional-diffusion-splitting)
    - [Seven-point Dirichlet Laplacian](#seven-point-dirichlet-laplacian)
  - [Centered convection-diffusion semidiscretization](#centered-convection-diffusion-semidiscretization)
  - [Discrete maximum principle](#discrete-maximum-principle)
  - [Method of lines](#method-of-lines)
    - [Dissipative second-order forward advection semidiscretization](#dissipative-second-order-forward-advection-semidiscretization)
    - [Energy contraction for centered drift-diffusion](#energy-contraction-for-centered-drift-diffusion)
    - [Displacement stability of a symmetric semidiscrete wave equation](#displacement-stability-of-a-symmetric-semidiscrete-wave-equation)
      - [All-time boundedness of a semidiscrete reaction wave equation](#all-time-boundedness-of-a-semidiscrete-reaction-wave-equation)
    - [Norm conservation of a semidiscrete Schrödinger equation](#norm-conservation-of-a-semidiscrete-schrodinger-equation)
  - [Lax equivalence theorem](#lax-equivalence-theorem)

## Three-point asymmetric second-derivative formula

↑ **Parent:** [Finite difference](finite-difference.md)

Matching the monomials $1,x,x^2$ gives $f''(2)\approx(2/3)f(0)-f(1)+(1/3)f(3)$. With error defined as the true derivative minus this approximation, its [Peano kernel](numerical-analysis.md#peano-kernel) is $K(\theta)=2\mathbf1_{\{\theta<2\}}+(1-\theta)_+^2-(3-\theta)^2/3$ on $[0,3]$. The derivative evaluation causes a jump at two. Applying the [Peano kernel theorem](numerical-analysis.md#peano-kernel-theorem) gives $\lambda(f)=\tfrac12\int_0^3Kf^{(3)}$.

## Randomized symmetric finite-difference derivative estimator

↑ **Parent:** [Finite difference](finite-difference.md)

Given noisy evaluations at $x_0+hZ_i$, where the $Z_i$ are independent [Rademacher random variables](probability-theory.md#rademacher-distribution), the estimator

$$
\widehat g'_N(x_0)=\frac1N\sum_{i=1}^N\frac{Z_i(Y_i-g(x_0))}{h}
$$

averages one-sided finite differences from both directions. If $|g''|\leq M$ and the noise variance is $\sigma^2$, its [mean squared error](statistical-modelling.md#mean-squared-error) is at most $h^2M^2/4+\sigma^2/(Nh^2)$.

## Finite difference method

↑ **Parent:** [Finite difference](finite-difference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_difference_method)

A finite difference method replaces [derivatives](calculus.md#derivative) by algebraic combinations of values on a discrete space-time grid.

### Midpoint flux stencil for one-dimensional diffusion

↑ **Parent:** [Finite difference method](#finite-difference-method)

For $u_t=(au_x)_x$, this conservative [finite difference method](#finite-difference-method) uses coefficient samples at edge midpoints. For smooth $a,u$, its spatial residual is $h^2(au_{xxxx}/12+a'u_{xxx}/6+a''u_{xx}/8+a'''u_x/24)+O(h^4)$. With zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), $-v^TL_hv=h^{-2}\sum_j a_{j+1/2}(v_{j+1}-v_j)^2$. If $0<a\leq a_+$, its [eigenvalues](linear-operator-theory.md#eigenvalue) lie in $[-4a_+/h^2,0]$, giving the mesh-independent [Forward Euler method](numerical-analysis.md#euler-method) bound $\Delta t/h^2\leq1/(2a_+)$. Constant $a=a_+$ proves sharpness as the grid is refined.

### Finite difference coefficient

↑ **Parent:** [Finite difference method](#finite-difference-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_difference_coefficient)

Finite difference coefficients are the weights in a linear combination of sampled function values approximating a derivative. Matching polynomial moments determines the weights and approximation order. Forward, backward and centered stencils have different coefficients.

### Fourth-order two-step advection stencil

↑ **Parent:** [Finite difference method](#finite-difference-method)

For $u_t=u_x$, the recurrence $U_m^{n+1}-U_m^{n-1}=\sum_{j=\pm1,\pm2}a_jU_{m+j}^n$ has fourth-order normalized [consistency of a numerical method](numerical-analysis.md#consistency-of-a-numerical-method) at fixed $\mu=k/h$ if

$$
a_1=\mu(4-\mu^2)/3,\quad a_2=\mu(\mu^2-1)/6,\quad a_{-j}=-a_j.
$$

To derive this, match moments $M_r=\sum_ja_jj^r$ to the temporal [Taylor series](calculus.md#taylor-series): $M_0=M_2=M_4=0$, $M_1=2\mu$, $M_3=2\mu^3$. The even conditions force antisymmetry; the two odd conditions then determine the displayed coefficients. The normalized residual begins with $h^4(\mu^2-1)(\mu^2-4)u_{xxxxx}/120$. Its [amplification polynomial of a multilevel finite difference scheme](#amplification-polynomial-of-a-multilevel-finite-difference-scheme) is $G^2-2iA(\theta)G-1$, where $A=a_1\sin\theta+a_2\sin2\theta$. At $\mu=1/2$, $|A|\le3/4$, giving a uniform power bound. At $\mu=3/2$, $A(\pi/3)=19\sqrt3/32>1$, and [wave packets](wave-equation.md#wave-packet) on the growing [polynomial root](polynomial.md#root-of-a-polynomial) prove Cauchy [linear instability](algebra.md#linear-instability).

### Mehrstellen method

↑ **Parent:** [Finite difference method](#finite-difference-method)

A [Mehrstellen method](#mehrstellen-method) increases the accuracy of a compact [finite difference method](#finite-difference-method) discretization by using the [differential equation](differential-equation.md) to express its leading truncation terms in terms of the prescribed source. For $\Delta u=f$, the square-grid [nine-point finite-difference stencil](#nine-point-finite-difference-stencil) for the [Laplacian](calculus.md#laplacian) satisfies $D_9u=\Delta u+h^2\Delta^2u/12+O(h^4)$. Replacing $\Delta^2u$ by $\Delta f$ and approximating this source [derivative](calculus.md#derivative) gives $D_9U=(I+h^2D_5/12)f$, with fourth-order normalized [consistency of a numerical method](numerical-analysis.md#consistency-of-a-numerical-method) while retaining a compact nine-point [matrix](vector-space.md#matrix). The uncorrected [nine-point finite-difference stencil](#nine-point-finite-difference-stencil) operator is only second-order accurate on general functions.

#### Compact semidiscrete nine-point diffusion

↑ **Parent:** [Mehrstellen method](#mehrstellen-method)

On a square grid, let $C_h$ sum the four axial neighbors and $K_h$ the four diagonal neighbors. With $M_h=2I/3+C_h/12$ and $L_h=(-10I/3+2C_h/3+K_h/6)/h^2$, the [method of lines](#method-of-lines) has fourth-order normalized spatial [numerical consistency](numerical-analysis.md#consistency-of-a-numerical-method). Its mass symbol is $(4+\cos\xi+\cos\eta)/6\geq1/3$, and its diffusion symbol is $[-10+4(\cos\xi+\cos\eta)+2\cos\xi\cos\eta]/(3h^2)\leq0$. Every continuous-time mode therefore contracts, and [Parseval identity](fourier-analysis.md#parseval-identity) gives mesh-independent discrete L2 [stability](numerical-analysis.md#stability-of-a-numerical-method). No time-step restriction is involved until a time integrator is selected.

### Rational implicit advection stencil with exact shift exceptions

↑ **Parent:** [Finite difference method](#finite-difference-method)

Consider a one-step stencil with new-level coefficients $a=\mu(1+\mu)/2$, $b=(1+\mu)(2-\mu)$ and $c=(1-\mu)(2-\mu)/2$ at offsets $-1,0,1$, and old-level coefficients $d=2-\mu$, $e=1+\mu$ at offsets $0,1$. For $u_t=u_x$, its exact-solution residual starts at fourth degree with coefficient $\mu(\mu-2)(\mu-1)(\mu+1)/24$. Thus its normalized [local truncation error](numerical-analysis.md#local-truncation-error) is third order at fixed nonzero [Courant number](#courant-number), except at the exact-shift values $-1,1,2$; zero gives the zero-step identity. For its [Fourier symbol](#fourier-symbol-of-a-difference-operator), $|D|^2-|N|^2=\mu(\mu-2)(\mu-1)(\mu+1)(1-\cos\theta)^2$. Uniformly invertible stable steps occur for $\mu\leq-1$, $0\leq\mu\leq1$ or $\mu\geq2$.

### Centered discrete advection is skew-adjoint

↑ **Parent:** [Finite difference method](#finite-difference-method)

With zero endpoints, the centered first-difference matrix has opposite off-diagonal entries and is a [skew-adjoint operator](functional-analysis.md#skew-adjoint-generator) in the mesh-weighted Euclidean inner product. Adding a real multiple of it to the negative symmetric second-difference matrix does not change the real energy form. The semidiscrete convection-diffusion solution therefore obeys a mesh-independent [energy estimate](partial-differential-equation.md#energy-estimate), even when its drift is large compared with its diffusion coefficient.

### Positive definiteness of the grounded nine-point Poisson stencil

↑ **Parent:** [Finite difference method](#finite-difference-method)

On a rectangular grid with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the nine-point [Poisson equation](partial-differential-equation.md#poisson-equation) matrix has diagonal $10/3$, axial off-diagonal entries $-2/3$, and diagonal-neighbor entries $-1/6$. Its [quadratic form](linear-algebra.md#quadratic-form) is the sum of squared differences over internal links, weighted by $2/3$ or $1/6$, plus the weighted squares of values linked to the fixed zero boundary. The connected axial grid forces a zero [quadratic form](linear-algebra.md#quadratic-form) to have all entries zero. This proves [positive-definite matrix](linear-algebra.md#positive-definite-matrix) in every ordering. The [Jacobi method](numerical-analysis.md#jacobi-method) converges because its nonnegative iteration matrix has row sums at most one, with a strict deficit at boundary-adjacent vertices; a hypothetical unit-modulus eigenvector would propagate its maximum modulus to such a deficit row, which is impossible.

### Implicit advection scheme with exact integer shifts

↑ **Parent:** [Finite difference method](#finite-difference-method)

A three-point implicit advection stencil can match translated data through cubic [Taylor expansion](calculus.md#taylor-expansion) while retaining a rational [Fourier amplification symbol](#fourier-amplification-symbol). For the coefficient family $a=\mu(1+\mu)/6$, $b=(2-\mu)(1+\mu)/3$, $c=(2-\mu)(1-\mu)/6$, $d=(2-\mu)/3$, $e=(1+\mu)/3$, its factor is $G=(d+e e^{i\theta})/(a e^{-i\theta}+b+c e^{i\theta})$. Direct subtraction gives $|D|^2-|N|^2=\mu(\mu-2)(\mu-1)(\mu+1)(1-\cos\theta)^2/9$. The displayed ranges are the contraction ranges in the [discrete L2 norm](functional-analysis.md#discrete-l2-norm), with a nonvanishing denominator there. For forward time and positive speed parameter, retain the nonnegative ranges. For fixed nonzero nonexceptional [Courant number](#courant-number), the normalized truncation error is third order; at $\mu=-1,0,1,2$ the update is the corresponding exact grid translation.

### Lax-Friedrichs method

↑ **Parent:** [Finite difference method](#finite-difference-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lax–Friedrichs_method)

For $u_t+cu_x=0$ on a uniform grid, the update $U_m^{n+1}=(U_{m-1}^n+U_{m+1}^n)/2-\nu(U_{m+1}^n-U_{m-1}^n)/2$ has symbol $\cos\theta-i\nu\sin\theta$, where $\nu=c\Delta t/h$. Its squared modulus is $1+(\nu^2-1)\sin^2\theta$, giving contraction exactly for $|\nu|\leq1$. Stability is separate from the dissipative and dispersive approximation errors.

### L2-compatible initialization of grid data

↑ **Parent:** [Finite difference method](#finite-difference-method)

An arbitrary $L^2$ initial function has no well-defined nodal point samples. Cell averages or a bounded projection to the discrete approximation space supply grid data independently of its pointwise representative. [Jensen's inequality](real-analysis.md#jensen-s-inequality) bounds the cell-average discrete [L2 norm](real-analysis.md#l2-norm) by the continuous [L2 norm](real-analysis.md#l2-norm). Combining consistent bounded initialization, stability, and density of smooth data can extend convergence to rough initial functions, without claiming their nonexistent classical derivatives.

#### Cell-average projection

↑ **Parent:** [L2-compatible initialization of grid data](#l2-compatible-initialization-of-grid-data)

The cell-average projection replaces a function by its average on each grid cell. It is independent of the representative of an [L2 function](measure-theory.md#square-integrable-function), unlike point sampling. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $h|U_m|^2\le\int_{\text{cell }m}|u|^2dx$, hence $h\sum_m|U_m|^2\le\|u\|_{L^2}^2$. Viewed as a piecewise constant function, the projection is the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto the grid's piecewise constant [linear subspace](vector-space.md#vector-subspace). Density of continuous compactly supported functions and the contraction estimate give convergence in the [L2 norm](real-analysis.md#l2-norm) as the mesh tends to zero.

### Discrete summation by parts

↑ **Parent:** [Finite difference method](#finite-difference-method)

On a periodic uniform grid, shifting an index in the discrete [inner product](linear-algebra.md#inner-product) gives the displayed skew-adjoint identity for the centered first difference. It also gives $\langle U,D_{xx}V\rangle_h=-\langle D_+U,D_+V\rangle_h$. With finite boundaries there are additional boundary terms unless the prescribed endpoint traces eliminate them. These identities are discrete counterparts of [integration by parts](calculus.md#integration-by-parts) and prove energy estimates for [finite difference methods](#finite-difference-method).

#### Inflow advection energy estimate from summation by parts

↑ **Parent:** [Discrete summation by parts](#discrete-summation-by-parts)

For $U_t=-cDU$ with $c>0$, a positive discrete norm matrix $H$ satisfying the displayed identity gives $d(U^THU)/dt=-c(U_N^2-U_0^2)$. Homogeneous inflow data $U_0=0$ therefore leave only the nonpositive outflow flux. Inhomogeneous inflow contributes a controlled boundary forcing term. This estimate includes the numerical boundary closure, unlike an interior-only [Fourier stability analysis](#fourier-stability-analysis). For any dissipative semidiscrete operator in the $H$ norm, [Backward Euler method](numerical-analysis.md#backward-euler-method) steps preserve the contraction by the identity $\|U^{n+1}\|_H^2-\|U^n\|_H^2=2k\langle U^{n+1},AU^{n+1}\rangle_H-\|U^{n+1}-U^n\|_H^2$.

### Four-neighbour mean expansion

↑ **Parent:** [Finite difference method](#finite-difference-method)

Averaging a smooth [function](function.md) at the four points $x\pm he_1,x\pm he_2$ cancels odd [Taylor expansion](calculus.md#taylor-expansion) terms and leaves $h^2\Delta u/4$. The fourth-order correction is $h^4(u_{1111}+u_{2222})/48$. Equality to the center value at every sufficiently small radius therefore forces $\Delta u=0$ at that point, but does not establish harmonicity throughout a neighbourhood.

### Parabolic mesh refinement

↑ **Parent:** [Finite difference method](#finite-difference-method)

A parabolic refinement keeps the time step proportional to the square of the spatial step: $k=rd^2$ for a fixed positive [diffusion Courant number](#diffusion-courant-number) $r$. A consistency bound $O(k+d^2)$ then becomes $O(d^2)$, though its separate time order remains one.

### Lax-Wendroff advection scheme

↑ **Parent:** [Finite difference method](#finite-difference-method)

For the [advection equation](partial-differential-equation.md#transport-equation) $u_t+cu_x=0$ on a uniform grid, the Lax-Wendroff update is

$$
 U_j^{n+1}=U_j^n-\frac\nu2(U_{j+1}^n-U_{j-1}^n)+\frac{\nu^2}2(U_{j+1}^n-2U_j^n+U_{j-1}^n),\qquad \nu=c\Delta t/\Delta x.
$$

Its [amplification factor](#amplification-factor) is $G=1-i\nu\sin\theta+\nu^2(\cos\theta-1)$, with $|G|^2=1-4\nu^2(1-\nu^2)\sin^4(\theta/2)$. Thus [von Neumann stability analysis](#von-neumann-stability-analysis) on an infinite or periodic grid gives stability for $|\nu|\leq1$. The scheme has second [order of a numerical method](numerical-analysis.md#order-of-a-numerical-method) for sufficiently smooth solutions; finite-interval [boundary conditions](differential-equation.md#boundary-condition) still need separate treatment.

### Symmetric half-grid diffusion consistency

↑ **Parent:** [Finite difference method](#finite-difference-method)

Evaluating a variable diffusion coefficient at both adjacent half-grid points makes odd spatial Taylor terms cancel. The conservative spatial bracket is $h^2(au_x)_x+O(h^4)$, yielding a fourth-order one-step residual when the forward time step is proportional to $h^2$.

#### Monotone half-grid diffusion update

↑ **Parent:** [Symmetric half-grid diffusion consistency](#symmetric-half-grid-diffusion-consistency)

For $0<a(x)\le\beta$, the explicit conservative diffusion update has weights $ka_{m-1/2}/h^2$, $1-k(a_{m-1/2}+a_{m+1/2})/h^2$, and $ka_{m+1/2}/h^2$. Under the displayed restriction they are nonnegative and sum to one. With zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), each new value is a [convex combination](mathematical-optimization.md#convex-combination) of old interior and boundary values, proving contraction in the discrete [maximum norm](functional-analysis.md#supremum-norm). The spatial [matrix](vector-space.md#matrix) is also [symmetric](set-theory.md#symmetric-relation) with $v^TL_hv=-h^{-2}\sum a_{m+1/2}(v_{m+1}-v_m)^2$. This puts its [eigenvalues](linear-operator-theory.md#eigenvalue) in $[-4\beta/h^2,0]$, so the same restriction gives [L2 norm](real-analysis.md#l2-norm) contraction. A stable recurrence need not be consistent with a different proposed differential equation.

### Upwind finite difference scheme

↑ **Parent:** [Finite difference method](#finite-difference-method)

For constant-speed advection $u_t+a u_x=0$ with $a>0$, the explicit upwind scheme uses $U_j^{n+1}=(1-\nu)U_j^n+\nu U_{j-1}^n$, $\nu=ak/h$. For $a<0$ the neighbour must be on the other side. When $0\leq\nu\leq1$, the update is a convex combination and is contractive in the maximum [norm](functional-analysis.md#norm) on a periodic grid, or with appropriate controlled inflow data.

On a periodic grid, [von Neumann stability analysis](#von-neumann-stability-analysis) gives $G=1-\nu+\nu e^{-i\theta}$ and $|G|^2=1-2\nu(1-\nu)(1-\cos\theta)$, proving the same exact contraction range in the discrete [L2 norm](real-analysis.md#l2-norm). Boundary estimates are still required on a finite interval; stable scalar [eigenvalues](linear-operator-theory.md#eigenvalue) of a triangular boundary update alone need not give a mesh-uniform bound.

#### Dissipative second-order forward advection stencil

↑ **Parent:** [Upwind finite difference scheme](#upwind-finite-difference-scheme)

For the equation $u_t=u_x$, the second-order forward difference has [Fourier symbol](#fourier-symbol-of-a-difference-operator) $[-(1-\cos\theta)^2+i\sin\theta(2-\cos\theta)]/h$. The nonpositive real part gives a contractive semidiscrete evolution in the discrete [L2 norm](real-analysis.md#l2-norm). Equivalently, for the unitary lattice shift $S$, $\operatorname{Re}\langle u,D_{+,2}u\rangle=-\|(S-I)^2u\|^2/(4h)$. A centred difference in another direction contributes only a skew-adjoint term, preserving this energy estimate.

### Five-point Laplacian

↑ **Parent:** [Finite difference method](#finite-difference-method)

On a square mesh, the dimensionless five-point Laplacian is $\Gamma_5u=u_{i+1,j}+u_{i-1,j}+u_{i,j+1}+u_{i,j-1}-4u_{i,j}$. The scaled operator $h^{-2}\Gamma_5$ approximates the [Laplacian](calculus.md#laplacian) with error $O(h^2)$ for sufficiently smooth functions.

#### Unweighted grid error for the five-point Poisson formula

↑ **Parent:** [Five-point Laplacian](#five-point-laplacian)

For a smooth solution with bounded fourth derivatives on the unit square, the five-point local residual is $O(h^2)$. The smallest eigenvalue of the unscaled Dirichlet matrix is $8\sin^2(\pi h/2)\ge8h^2$. With $M^2$ interior points and $M\asymp h^{-1}$, the residual has unweighted Euclidean norm $O(h)$. The equation $Ae=h^2\tau$ therefore gives unweighted error $O(h)$, equivalent to second-order error in the area-weighted grid norm.

#### Five-point heat-reaction stability threshold

↑ **Parent:** [Five-point Laplacian](#five-point-laplacian)

On a unit-square uniform mesh with $h=1/(M+1)$ and zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the semidiscrete [five-point Laplacian](#five-point-laplacian) has eigenvalues $-4h^{-2}[\sin^2(j\pi h/2)+\sin^2(k\pi h/2)]$. Adding reaction $\kappa I$ gives a contractive continuous-time grid evolution exactly under the displayed threshold. The threshold is $2\pi^2-\pi^4h^2/6+O(h^4)$, slightly below the continuum threshold. This is an all-time non-growth criterion; finite-time mesh-uniform bounds also hold for fixed larger reaction rates.

### Nine-point finite-difference stencil

↑ **Parent:** [Finite difference method](#finite-difference-method)

A nine-point finite-difference stencil on a square grid couples a central value to its four axial neighbours and four diagonal neighbours. Ordering the grid by columns produces a block tridiagonal matrix whose diagonal and off-diagonal blocks are [symmetric tridiagonal Toeplitz matrices](linear-algebra.md#symmetric-tridiagonal-toeplitz-matrix).

#### Five-point versus nine-point Laplacian eigenvalue accuracy

↑ **Parent:** [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)

For the [Dirichlet discrete Laplacian](#dirichlet-discrete-laplacian) on a square, let $T=h^{-2}\operatorname{tridiag}(1,-2,1)$. The standard axial five-point operator is $T\otimes I+I\otimes T$, and the axial-weight $2/3$, corner-weight $1/6$ nine-point operator additionally contains $h^2T\otimes T/6$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are therefore strictly larger than the five-point values for the same sine modes. Both lie above the corresponding negative continuum [Laplacian](calculus.md#laplacian) [eigenvalues](linear-operator-theory.md#eigenvalue), so the five-point operator has smaller spectral error. For fixed mode numbers the leading errors are respectively $\pi^4h^2(k^4+l^4)/12$ and $\pi^4h^2(k^2+l^2)^2/12$.

#### Harmonic superconvergence of the nine-point stencil

↑ **Parent:** [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)

For the square-grid [nine-point finite-difference stencil](#nine-point-finite-difference-stencil) for the [Laplacian](calculus.md#laplacian),

$$
D_9u=\Delta u+\frac{h^2}{12}\Delta^2u+\frac{h^4}{360}(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy})+O(h^6).
$$

If $\Delta u=0$, both displayed correction terms vanish: the mixed sixth [derivatives](calculus.md#derivative) sum to $\Delta u_{xxyy}=0$, and the pure sixth [derivatives](calculus.md#derivative) sum to the negative of that sum. Expanding two orders further yields $D_9u=h^6u_{xxxxxxxx}/3024+O(h^8)$ for a smooth [harmonic function](partial-differential-equation.md#harmonic-function). Thus the compact harmonic scheme has sixth-order normalized [consistency of a numerical method](numerical-analysis.md#consistency-of-a-numerical-method) and, with the [discrete maximum principle](#discrete-maximum-principle) inverse bound, sixth-order nodal convergence on a square with exact smooth [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data). For example $\operatorname{Re}(x+iy)^8$ shows that the sixth-order term need not vanish.

#### Compact fourth-order Helmholtz stencil

↑ **Parent:** [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)

Let $\Gamma_9$ have center weight $-10/3$, axial weights $2/3$ and diagonal weights $1/6$, and let $M_h$ have center weight $2/3$ and axial weights $1/12$. [Taylor expansion](calculus.md#taylor-expansion) gives $h^{-2}\Gamma_9u=\Delta u+h^2\Delta^2u/12+O(h^4)$ and $M_hu=u+h^2\Delta u/12+O(h^4)$. On a smooth solution of the constant-coefficient [Helmholtz equation](partial-differential-equation.md#helmholtz-equation), the second-order term becomes $h^2\Delta(\Delta u+\lambda u)/12=0$. Thus the normalized PDE residual is fourth order, while the original unscaled stencil residual is sixth order. This local cancellation alone does not prove uniform global accuracy at or near a resonance.

#### Jacobi convergence for the nine-point Dirichlet stencil

↑ **Parent:** [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)

The [Jacobi method](numerical-analysis.md#jacobi-method) has axial neighbour weights $1/5$ and diagonal weights $1/20$. Interior row sums are one, boundary-adjacent sums are smaller, and the positive-weight graph is connected. If an eigenvalue had modulus one, a maximal-modulus eigenvector component would force all its neighbours to have the same modulus. Propagation reaches a deficient row, a contradiction. This proves strict spectral-radius control even though the infinity norm of the iteration matrix can equal one.

#### Negative definiteness of a nine-point Dirichlet stencil

↑ **Parent:** [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)

Extend the interior grid vector by zero. With axial weights $2/(3h^2)$ and diagonal weights $1/(6h^2)$, the negative central coefficient equals the total neighbour weight. Expanding the edge-square sum gives the displayed quadratic form. Equality forces all axial differences to vanish, and connection to the zero exterior forces the vector to be zero. Simultaneous row and column permutations preserve symmetry and negative definiteness.

#### Fourth-order correction of the nine-point Poisson stencil

↑ **Parent:** [Nine-point finite-difference stencil](#nine-point-finite-difference-stencil)

For a smooth solution of $\Delta u=f$, the corrected formula $\Gamma_9u=h^2f+(h^2/12)\Gamma_5f$ has unscaled residual $O(h^6)$ and normalized [local truncation error](numerical-analysis.md#local-truncation-error) $O(h^4)$. The inverse interior matrix has Euclidean [operator norm](continuous-dual-space.md#operator-norm) $O(h^{-2})$; on $O(h^{-2})$ grid points this gives unweighted Euclidean nodal error $O(h^3)$. Uniform derivatives up to the boundary are required for a grid-independent remainder bound.

##### Sixth-order source correction of the nine-point Poisson stencil

↑ **Parent:** [Fourth-order correction of the nine-point Poisson stencil](#fourth-order-correction-of-the-nine-point-poisson-stencil)

The [nine-point finite-difference stencil](#nine-point-finite-difference-stencil) for the [Laplacian](calculus.md#laplacian) has expansion $D_9u=\Delta u+h^2\Delta^2u/12+h^4(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy})/360+O(h^6)$. If $\Delta u=f$, differentiating this equation gives $u_{xxxxyy}+u_{xxyyyy}=f_{xxyy}$ and $u_{xxxxxx}+u_{yyyyyy}=\Delta^2f-3f_{xxyy}$. Hence the corrected compact equation

$$
D_9U=f+\frac{h^2}{12}\Delta f+\frac{h^4}{360}(f_{xxxx}+4f_{xxyy}+f_{yyyy})
$$

has sixth-order normalized [consistency of a numerical method](numerical-analysis.md#consistency-of-a-numerical-method). Source [derivatives](calculus.md#derivative) can be supplied analytically; numerical approximation of $\Delta f$ must be fourth order and of the fourth [derivatives](calculus.md#derivative) second order. With exact square-grid [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data) and uniformly smooth solution, the [discrete maximum principle](#discrete-maximum-principle) inverse bound converts this residual into sixth-order nodal convergence. The unknown stencil stays compact even if more distant known source values are used.

##### Maximum-norm convergence of the corrected nine-point Poisson scheme

↑ **Parent:** [Fourth-order correction of the nine-point Poisson stencil](#fourth-order-correction-of-the-nine-point-poisson-stencil)

On the unit square with exact [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data), let $D_9U=B_hf$ and suppose the normalized residual on the exact smooth solution has [supremum norm](functional-analysis.md#supremum-norm) at most $\varepsilon$. The error satisfies $D_9e=-\tau$ and vanishes on the boundary. The barrier $q=[x(1-x)+y(1-y)]/4$ has $D_9q=-1$, $q\ge0$ on the boundary, and maximum $1/8$. Apply the [discrete maximum principle](#discrete-maximum-principle) to $e-\varepsilon q$ and $-e-\varepsilon q$, obtaining $|e|\le\varepsilon q$. Thus $\|e\|_\infty\le\varepsilon/8$, and fourth-order residual gives fourth-order [supremum norm](functional-analysis.md#supremum-norm) nodal convergence. The proof needs a uniform smoothness bound and a compatible boundary discretization.

### Fourier stability analysis

↑ **Parent:** [Finite difference method](#finite-difference-method)

Fourier stability analysis transforms a translation-invariant finite-difference scheme into scalar or matrix recurrences indexed by wavenumber. The [Parseval identity](fourier-analysis.md#parseval-identity) then converts uniform multiplier bounds into discrete $2$-norm bounds.

#### Fourier amplification symbol

↑ **Parent:** [Fourier stability analysis](#fourier-stability-analysis)

A constant-coefficient translation-invariant grid update is diagonalized spatially by [discrete Fourier modes](numerical-analysis.md#discrete-fourier-mode). Its scalar or matrix multiplier is the displayed symbol. In a semidiscrete evolution, the analogous symbol is a continuous-time generator and its exponential propagates each mode. [Discrete Parseval identity](numerical-analysis.md#discrete-parseval-identity) converts uniform modal bounds to discrete [L2 norm](real-analysis.md#l2-norm) bounds.

##### Scalar Fourier power criterion

↑ **Parent:** [Fourier amplification symbol](#fourier-amplification-symbol)

For a scalar constant-coefficient grid update, Fourier transformation turns $S$ into multiplication by its symbol $G$. [Parseval identity](fourier-analysis.md#parseval-identity) proves the displayed norm equality; necessity is obtained by concentrating Fourier data near a maximizing frequency. Contractivity for every step is equivalent to $|G|\leq1$. Mesh-uniform fixed-time [stability](numerical-analysis.md#stability-of-a-numerical-method), on $nk\leq T$, permits $\sup|G|\leq1+Ck$: powers are bounded by $e^{CT}$. Conversely a uniform bound at $n=\lfloor T/k\rfloor$ gives this $1+O(k)$ restriction as $k\to0$. For [matrix](vector-space.md#matrix) symbols, use the existing [uniform power bound for matrix Fourier symbols](#uniform-power-bound-for-matrix-fourier-symbols) rather than only [eigenvalue](linear-operator-theory.md#eigenvalue) moduli.

##### Uniform power bound for matrix Fourier symbols

↑ **Parent:** [Fourier amplification symbol](#fourier-amplification-symbol)

This uniform bound is the actual fixed-time stability requirement for a vector-valued periodic grid evolution. Eigenvalue moduli alone are insufficient for [nonnormal matrices](linear-operator-theory.md#non-normal-matrix). A unit Jordan block with an order-one off-diagonal entry grows like $n$, while an entry proportional to $\Delta t$ can give bounded growth on $n\Delta t\leq T$. Uniform eigenvector conditioning or a suitable discrete energy estimate can establish the bound. Mesh-dependent diagonalizations cannot be treated as automatically harmless.

### Central finite difference

↑ **Parent:** [Finite difference method](#finite-difference-method)

The centered unit-step approximation to a second derivative is

$$
f''(0)\approx f(-1)-2f(0)+f(1).
$$

The weights $1,-2,1$ are [finite difference coefficients](#finite-difference-coefficient) for this centered second-derivative approximation.

#### Fourth-order centered second derivative

↑ **Parent:** [Central finite difference](#central-finite-difference)

This symmetric [finite difference method](#finite-difference-method) approximates a second derivative with $D_{4,h}u=u''-h^4u^{(6)}/90+O(h^6)$ for sufficiently [smooth](analysis.md#smooth-function) functions. Matching the constant, second-derivative and fourth-derivative coefficients of a symmetric five-node [Taylor expansion](calculus.md#taylor-expansion) determines the displayed weights uniquely; its sixth-derivative coefficient is nonzero. The [Fourier symbol](#fourier-symbol-of-a-difference-operator) is $-4h^{-2}\sin^2(\theta/2)[1+\sin^2(\theta/2)/3]\le0$. Thus the semidiscrete [heat equation](diffusion-equation.md#heat-equation) $\dot U=D_{4,h}U$ is contractive in the discrete [L2 norm](real-analysis.md#l2-norm) by the [discrete Parseval identity](numerical-analysis.md#discrete-parseval-identity). This says nothing by itself about stability of a subsequently chosen time update.

#### Sharp central-secant derivative error

↑ **Parent:** [Central finite difference](#central-finite-difference)

For $f\in C^3[x-h,x+h]$, the [Peano kernel](numerical-analysis.md#peano-kernel) for the error of the central secant slope has one sign. Integrating its absolute value gives the displayed constant $h^2/6$, and a cubic polynomial attains it. At $x=1$, $h=1$, the unnormalized order-two kernel is $-\theta^2/2$ on $[0,1]$ and $-(2-\theta)^2/2$ on $[1,2]$; the integral representation includes the factor $1/2!$.

#### Centered-advection refinement-dependent stability

↑ **Parent:** [Central finite difference](#central-finite-difference)

Forward time with centered advection has amplification magnitude greater than one at nonzero modes. Under a fixed nonzero Courant number, its powers blow up as the time step vanishes. If instead $\Delta t/h^2$ stays bounded, then $\log|G|\leq c^2\Delta t^2/(2h^2)$, so $|G|^n\leq\exp(c^2T\Delta t/(2h^2))$ is uniformly bounded on fixed time intervals. This severe parabolic refinement supplies stability without contraction; it does not validate the usual hyperbolic-step choice.

#### Second-order central difference

↑ **Parent:** [Central finite difference](#central-finite-difference)

On a uniform grid of spacing $h$, the second-order central difference

$$
\frac{f(x-h)-2f(x)+f(x+h)}{h^2}
$$

approximates $f''(x)$ with error $O(h^2)$ for a sufficiently smooth function.

### Forward difference operator

↑ **Parent:** [Finite difference method](#finite-difference-method)

The forward difference of a sequence or function on the [integers](number-theory.md#integer) is

$$
(\Delta f)(n)=f(n+1)-f(n).
$$

#### Adjoint of a discrete forward gradient

↑ **Parent:** [Forward difference operator](#forward-difference-operator)

On an $N$-pixel line with last forward difference zero, $D^*p$ has first entry $-p_1$, interior entries $p_{i-1}-p_i$, and last entry $p_{N-1}$, with $D^*=0$ for $N=1$. On a square grid add these expressions along rows and columns. Unused last-edge components contribute nothing. The identity $\langle Du,p\rangle=\langle u,D^*p\rangle$ fixes every boundary sign. On the unscaled square grid, $\|D\|^2=8\cos^2(\pi/(2N))\le8$ for $N>1$.

#### Discrete antiderivative

↑ **Parent:** [Forward difference operator](#forward-difference-operator)

A discrete antiderivative of $f$ is a function $F$ satisfying $\Delta F=f$. [Pascal's identity](combinatorics.md#pascal-s-rule) gives

$$
\Delta\binom nr=\binom n{r-1}.
$$

#### Newton series for an integer-valued polynomial sequence

↑ **Parent:** [Forward difference operator](#forward-difference-operator)

If $\Delta^{k+1}f=0$, then $f$ is an integer linear combination of $1,\binom n1,\ldots,\binom nk$ whenever $f$ is integer-valued. Successive differences recover the coefficients.

### von Neumann stability analysis

↑ **Parent:** [Finite difference method](#finite-difference-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/von_Neumann_stability_analysis)

Von Neumann analysis inserts the Fourier mode $u_m^n=G^n e^{im\theta}$ into a constant-coefficient difference scheme. A one-step method is stable in the discrete $2$-norm when its amplification factor satisfies $|G(\theta)|\leq1$ for every resolvable wavenumber.

#### Nonnormal Fourier amplification matrix

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a system or a multilevel method, each [Fourier mode](fourier-analysis.md#fourier-mode) evolves through an amplification matrix $G(\theta)$. Stability requires bounds on $G(\theta)^n$ uniform in frequencies and mesh parameters. Eigenvalue moduli alone do not suffice: $G=\begin{pmatrix}1&1\\0&1\end{pmatrix}$ has unit eigenvalues but $G^n$ has off-diagonal entry $n$. Uniformly bounded eigenvector matrices, or a uniformly positive energy symmetrizer, can supply the missing power bound.

#### Uniform power bound from separated amplification roots

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a uniformly bounded two-level Fourier companion [matrix](vector-space.md#matrix) $C(\theta)$ with distinct roots $g_1,g_2$ of modulus at most one, its powers satisfy

$$
C^n=\frac{g_1^n(C-g_2I)-g_2^n(C-g_1I)}{g_1-g_2}.
$$

A positive frequency-uniform gap therefore gives a uniform bound on every power. The [Parseval identity](fourier-analysis.md#parseval-identity) then supplies spatial [L2 norm](real-analysis.md#l2-norm) stability. When the gap closes at a repeated unit root, a [Jordan block](linear-operator-theory.md#jordan-block) can produce growth proportional to the number of steps despite both roots having modulus one.

#### Stability of a spatially shifted BDF2 stencil

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For the periodic-grid recurrence

$$
U_{m+2}^{n+2}-\frac43U_m^{n+1}+\frac13U_m^n
=\frac23\mu(U_{m-1}^{n+2}-2U_m^{n+2}+U_{m+1}^{n+2}),
$$

the exact [von Neumann stability analysis](#von-neumann-stability-analysis) range at fixed $\mu>0$ is $\mu\geq3$. The [Fourier symbol](#fourier-symbol-of-a-difference-operator) gives $A(\theta)\xi^2-4\xi+1=0$, $A=3e^{2i\theta}+8\mu\sin^2(\theta/2)$. The root near one obeys $|\xi|^2=1+(6-2\mu)\theta^2+O(\theta^4)$, proving instability for $\mu<3$.

For $\mu\geq3$, $\operatorname{Re}A-3=6(\cos\theta-1)^2+4(\mu-3)(1-\cos\theta)\geq0$. Writing the modal recurrence as $3v^{n+2}-4v^{n+1}+v^n=-(A-3)v^{n+2}$, the [BDF2 discrete energy identity](numerical-analysis.md#bdf2-discrete-energy-identity) proves nonincrease of $\lvert v^{n+1}\rvert^2+\lvert2v^{n+1}-v^n\rvert^2$. Summing modes proves [stability](numerical-analysis.md#stability-of-a-numerical-method) uniformly even when $\mu$ varies within $[3,\infty)$.

This shifted scheme is not a consistent standard heat discretization under $k=\mu h^2$: dividing its extra spatial-shift defect by $2k/3$ produces $3hu_x/k+O(h^2/k)$. On a finite interval with [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) it also requires an extra boundary closure. Thus the periodic stability theorem is not a theorem of convergence to the [heat equation](diffusion-equation.md#heat-equation) or of stability for an unspecified boundary treatment.

#### Fourier symbol of a difference operator

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a translation-invariant difference operator $(Lu)_m=\sum_j a_j u_{m+j}$, its Fourier symbol is $\ell(\theta)=\sum_j a_je^{ij\theta}$. Applying $L$ to a [Fourier mode](fourier-analysis.md#fourier-mode) $e^{im\theta}$ multiplies that mode by $\ell(\theta)$. Symbols turn constant-coefficient stencil equations into scalar algebraic equations and expose their [von Neumann stability analysis](#von-neumann-stability-analysis).

#### Power boundedness of a two-level Fourier scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a two-level Fourier recurrence $\widehat u^{n+1}=a(\theta)\widehat u^n+b(\theta)\widehat u^{n-1}$, the amplification [matrix](vector-space.md#matrix) is

$$
T(\theta)=\begin{pmatrix}a(\theta)&b(\theta)\\1&0\end{pmatrix}.
$$

[Stability](numerical-analysis.md#stability-of-a-numerical-method) requires its powers to be uniformly bounded in the time index and the mesh frequencies. If its two amplification roots have [modulus](complex-analysis.md#modulus) at most one and their separation has a positive mesh-independent lower bound, the [eigenvectors](linear-operator-theory.md#eigenvector) $(\xi_j,1)^T$ give a uniformly bounded [diagonalization of a matrix](linear-operator-theory.md#diagonalization-of-a-matrix), proving stability. A repeated unit-modulus root of this companion [matrix](vector-space.md#matrix) instead produces a [Jordan block](linear-operator-theory.md#jordan-block) and linear growth in time. Thus checking only the [moduli](complex-analysis.md#modulus) of the roots is insufficient.

##### Uniform stability of a shifted two-level advection scheme

↑ **Parent:** [Power boundedness of a two-level Fourier scheme](#power-boundedness-of-a-two-level-fourier-scheme)

For $U_m^{n+1}=(1-2\mu)(U_m^n-U_{m+1}^n)+U_{m+1}^{n-1}$, write an [amplification root](numerical-analysis.md#amplification-root) as $G=e^{i\theta/2}\lambda$. Its equation is $\lambda^2+2i(1-2\mu)\sin(\theta/2)\lambda-1=0$. The roots have modulus one and a positive frequency-uniform separation exactly for $0<\mu<1$, giving [L2 norm](real-analysis.md#l2-norm) [stability](numerical-analysis.md#stability-of-a-numerical-method) through a uniformly bounded diagonalization. At either endpoint the Nyquist symbol has a repeated unit root and a [Jordan block](linear-operator-theory.md#jordan-block), producing linear growth. The normalized [local truncation error](numerical-analysis.md#local-truncation-error) is generally second order; at $\mu=1/2$ and $1$ exactly sampled characteristics solve the recurrence, although the latter parameter is unstable for arbitrary perturbations.

#### Forward Euler stability for centered advection-diffusion

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For $u_t=u_{xx}+\alpha u_x$ on the whole line, apply centered differences in space and the [Forward Euler method](numerical-analysis.md#euler-method) in time. With $r=\Delta t/(\Delta x)^2$ and $c=\alpha\Delta t/\Delta x$, the amplification factor is

$$
G(\theta)=1-4r\sin^2(\theta/2)+ic\sin\theta.
$$

Putting $s=\sin^2(\theta/2)$ gives

$$
|G|^2-1=4s\{c^2-2r+(4r^2-c^2)s\}.
$$

For $\Delta t>0$, the affine expression in braces is nonpositive on $[0,1]$ exactly when $r\leq1/2$ and $c^2\leq2r$. Hence [von Neumann stability analysis](#von-neumann-stability-analysis) gives

$$
\Delta t\leq\frac{(\Delta x)^2}{2},
\qquad\alpha^2\Delta t\leq2.
$$

These conditions are weaker than requiring every stencil weight to be nonnegative; [stability](numerical-analysis.md#stability-of-a-numerical-method) in the discrete [L2 norm](real-analysis.md#l2-norm) need not imply monotonicity.

#### Laurent operator

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laurent_operator)

A Laurent operator on the whole integer lattice is a translation-invariant bi-infinite matrix. Under the [discrete Fourier transform](numerical-analysis.md#discrete-fourier-transform) it becomes multiplication by its symbol, so its $2$-operator norm is the essential supremum of the symbol's modulus.

##### Toeplitz operator

↑ **Parent:** [Laurent operator](#laurent-operator)

A Toeplitz operator is a constant-diagonal operator on a one-sided sequence space. It models the restriction of a translation-invariant stencil to a half-line, where the boundary prevents direct diagonalization by the full-lattice Fourier transform.

###### Toeplitz exponential determinant identity

↑ **Parent:** [Toeplitz operator](#toeplitz-operator)

Split a smooth symbol into its strictly negative and strictly positive Fourier modes. Their Toeplitz operators $A,B$ exponentiate exactly to the Toeplitz operators of the corresponding exponentials, and $T(e^f)T(e^{-f})=e^Ae^Be^{-A}e^{-B}$. The trace of $[A,B]$ is $\sum_{n>0}nf_nf_{-n}$ because the shift relation gives $\operatorname{Tr}[(S^*)^m,S^n]=n\delta_{mn}$. Smoothness makes the series converge in trace norm, so the [Fredholm determinant of an exponential commutator](compact-operator.md#fredholm-determinant-of-an-exponential-commutator) applies.

###### Toeplitz index theorem for continuous symbols

↑ **Parent:** [Toeplitz operator](#toeplitz-operator)

On the [Hardy space of the circle](hilbert-space.md#hardy-space-of-the-circle), a continuous symbol gives a [Fredholm](functional-analysis.md#fredholm-operator) Toeplitz operator exactly when it never vanishes. Nonvanishing gives a parametrix $T_{1/f}$ modulo compact semicommutators. Write $f(z)=z^ne^{h(z)}$, where $n$ is its counterclockwise [winding number](complex-analysis.md#winding-number) and $h$ is continuous. Homotopy through nonvanishing symbols and [local constancy of the Fredholm index](functional-analysis.md#local-constancy-of-the-fredholm-index) reduce the index to that of the shift $T_{z^n}$, namely $-n$. If $f$ vanishes at a point, normalized Hardy reproducing kernels concentrating there are weakly null unit vectors on which $T_f$ tends to zero, contradicting a Fredholm parametrix.

#### Boundary stability of a finite-difference method

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

Boundary stability is a mesh-uniform estimate for a finite-difference initial-boundary problem with forced boundary data. Stability of the whole-line Cauchy scheme is necessary but may fail to control boundary-supported numerical modes.

##### Boundary closure of a difference scheme

↑ **Parent:** [Boundary stability of a finite-difference method](#boundary-stability-of-a-finite-difference-method)

A boundary closure supplies the boundary rows or ghost values needed by a spatial [finite difference method](#finite-difference-method). It must reflect the PDE boundary data and preserve a mesh-uniform stability estimate. Interior [von Neumann stability analysis](#von-neumann-stability-analysis) cannot detect an arbitrary unstable boundary row; for example a row $U_1^{n+1}=2U_1^n$ produces growth even beside an otherwise stable heat stencil.

<h5 id="uniform-kreiss-lopatinskii-condition">Uniform Kreiss--Lopatinskii condition</h5>

↑ **Parent:** [Boundary stability of a finite-difference method](#boundary-stability-of-a-finite-difference-method)

After transforming time and tangential variables, the uniform Kreiss--Lopatinskii condition requires the boundary equations to determine every decaying normal mode with an inverse bounded uniformly over transformed frequencies. It rules out growing or weakly controlled boundary modes.

#### Eigenvalue stability analysis of a finite difference method

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a normal amplification matrix $Q$, the bound $\rho(Q)\leq1$ with semisimple unit-modulus eigenvalues controls every power $Q^n$. For a nonnormal family, eigenvalues alone do not control transient growth or give a mesh-uniform bound; eigenvector conditioning, pseudospectra, or a direct energy estimate is then needed.

##### Finite-time stability versus power boundedness

↑ **Parent:** [Eigenvalue stability analysis of a finite difference method](#eigenvalue-stability-analysis-of-a-finite-difference-method)

Stability of the [partial differential equation](partial-differential-equation.md) requires a bound uniform over refining meshes and time steps on every fixed physical time interval. This is distinct from demanding an all-time bound for one fixed [matrix](vector-space.md#matrix). A fixed [matrix](vector-space.md#matrix) is power bounded exactly when all [eigenvalues](linear-operator-theory.md#eigenvalue) are in the closed [unit disk](geometry-and-topology.md#unit-disk) and its unit-modulus [Jordan blocks](linear-operator-theory.md#jordan-block) have size one. A time-step family can nevertheless have harmless [polynomial](polynomial.md) physical-time growth: $G_\tau=I+\tau N$ with $N^2=0$ gives $G_\tau^n=I+n\tau N$, uniformly bounded for $n\tau\leq T$ despite its nontrivial unit-modulus [Jordan block](linear-operator-theory.md#jordan-block). Mesh dependence and the scaling of the step must therefore be kept in an [eigenvalue](linear-operator-theory.md#eigenvalue) argument.

##### Negative spectra do not imply uniform semidiscrete stability

↑ **Parent:** [Eigenvalue stability analysis of a finite difference method](#eigenvalue-stability-analysis-of-a-finite-difference-method)

Every eigenvalue of this [nonnormal matrix](linear-operator-theory.md#non-normal-matrix) is $-1$, but $e^{tL_h}=e^{-t}\begin{pmatrix}1&t/h\\0&1\end{pmatrix}$. Applied to the second coordinate unit vector, its norm at $t=1$ is at least $1/(eh)$. Thus negative eigenvalues give no mesh-uniform semigroup bound by themselves. [Normal matrices](linear-operator-theory.md#normal-matrix), uniformly conditioned eigenvector bases, or a direct dissipative energy estimate supply the missing control.

##### Nonnormal upwind amplification matrix

↑ **Parent:** [Eigenvalue stability analysis of a finite difference method](#eigenvalue-stability-analysis-of-a-finite-difference-method)

On a finite inflow grid, explicit upwinding has a triangular amplification matrix whose only eigenvalue is $1-\mu$. For $1<\mu<2$ this eigenvalue lies inside the unit disk, although interior high-frequency data are amplified by $|1-2\mu|>1$ before reaching the boundary. This shows why eigenvalue analysis without uniform normality can give the wrong stability range.

#### Backward Euler diffusion scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For the centered spatial second difference, backward Euler has amplification factor $G(\theta)=[1+4\mu\sin^2(\theta/2)]^{-1}$ and is stable for every physical Courant number $\mu\geq0$.

##### No positive-Courant cancellation for backward Euler diffusion

↑ **Parent:** [Backward Euler diffusion scheme](#backward-euler-diffusion-scheme)

For a smooth solution of the [heat equation](diffusion-equation.md#heat-equation), backward Euler with the centered second difference has residual divided by $k$ equal to $-(k/2+d^2/12)u_{xxxx}+O(k^2+kd^2+d^4)$. Both leading terms have the same sign. Under [parabolic mesh refinement](#parabolic-mesh-refinement) their coefficient is $-d^2(r/2+1/12)$, which cannot vanish for a positive [diffusion Courant number](#diffusion-courant-number). Consistency of an update $U^{n+1}-U^n=\alpha(r)\delta^2U^{n+1}$ forces $\alpha(r)=r$ for every fixed positive $r$.

##### Backward Euler diffusion stability on a finite Dirichlet interval

↑ **Parent:** [Backward Euler diffusion scheme](#backward-euler-diffusion-scheme)

On $J$ interior Dirichlet grid points, backward Euler diffusion is stable for $\mu\geq0$ and also for the nonphysical branch $\mu\leq-[2\sin^2(\pi/(2(J+1)))]^{-1}$. The latter makes every amplification denominator at most $-1$.

#### Forward Euler diffusion scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For the centered spatial second difference, forward Euler has the update

$$
u_m^{n+1}=\mu u_{m-1}^n+(1-2\mu)u_m^n+\mu u_{m+1}^n.
$$

It is stable for $0\leq\mu\leq1/2$. In this range the update is a convex combination, which gives a direct maximum-norm proof as well as the Fourier proof.

##### Explicit time stepping for bounded reaction diffusion

↑ **Parent:** [Forward Euler diffusion scheme](#forward-euler-diffusion-scheme)

Let $D_h$ be the scaled [Dirichlet discrete Laplacian](#dirichlet-discrete-laplacian) and $V_h$ a bounded diagonal reaction matrix. If $0\leq k/h_x^2\leq1/2$, the heat update $H_h=I+kD_h$ is contractive in both the maximum [norm](functional-analysis.md#norm) and the mesh-weighted [L2 norm](real-analysis.md#l2-norm). For $\|V_h\|\leq A$,

$$
 \|(H_h+kV_h)^n\|\leq(1+kA)^n\leq e^{Ank}.
$$

This proves finite-time mesh-uniform [stability](numerical-analysis.md#stability-of-a-numerical-method) without requiring the full update to have nonnegative entries or to be contractive. Negative reaction terms can destroy nonnegativity at the endpoint $k/h_x^2=1/2$, so it is the heat part alone that is treated as a nonnegative contraction.

#### Stability of a two-parameter implicit-explicit diffusion scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For the scheme

$$
\left(aI-\frac{\mu-c}{4}L\right)u^{n+1}
=\left(aI+\frac{\mu+c}{4}L\right)u^n,
$$

where $L=[1,-2,1]$ is the Dirichlet second-difference matrix and $\mu>0$, the modal amplification factor is

$$
G(s)=\frac{a-(\mu+c)s}{a+(\mu-c)s},
\qquad 0<s<1.
$$

Mesh-uniform stability holds exactly when

$$
a\geq0,
\qquad
c\leq a.
$$

For consistency with $u_t=u_{xx}$ under the displayed normalization one additionally chooses $a=1/2$; stability then requires $c\leq1/2$.

#### Amplification factor

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a one-step translation-invariant recurrence, the amplification factor is the multiplier satisfying

$$
\widehat u^{\,n+1}(\theta)=H(\theta)\widehat u^{\,n}(\theta).
$$

The [Parseval identity](fourier-analysis.md#parseval-identity) converts the pointwise bound $|H|\leq1$ into non-growth of the discrete $2$-norm.

##### Amplification factor of a two-sided one-step stencil

↑ **Parent:** [Amplification factor](#amplification-factor)

For

$$
\sum_{k=r}^sa_ku^{n+1}_{m+k}
=\sum_{k=r}^sb_ku^n_{m+k},
$$

the Fourier convention $\widehat u(\theta)=\sum_me^{-im\theta}u_m$ gives

$$
H(\theta)=
\frac{\sum_{k=r}^sb_ke^{ik\theta}}
{\sum_{k=r}^sa_ke^{ik\theta}},
$$

provided the denominator does not vanish.

#### Amplification polynomial of a multilevel finite difference scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For a scheme

$$
\sum_{r,j}a_{rj}u_{m+j}^{n+r}=0,
$$

the Fourier ansatz gives the amplification polynomial

$$
\sum_{r,j}a_{rj}G^r e^{ij\theta}=0.
$$

Its roots are the amplification factors of that Fourier mode.

##### Leapfrog advection scheme

↑ **Parent:** [Amplification polynomial of a multilevel finite difference scheme](#amplification-polynomial-of-a-multilevel-finite-difference-scheme)

Centered space and leapfrog time discretization of $u_t+cu_x=0$ gives

$$
u_j^{n+1}=u_j^{n-1}-\nu(u_{j+1}^n-u_{j-1}^n),
\qquad \nu=c\Delta t/\Delta x.
$$

Its amplification polynomial is $G^2+2i\nu\sin\theta\,G-1$. The two roots have unit modulus for $|\nu\sin\theta|\leq1$, but a repeated unit root at equality violates the uniform root condition.

###### Two-dimensional leapfrog stability threshold

↑ **Parent:** [Leapfrog advection scheme](#leapfrog-advection-scheme)

For $u_t=u_x+u_y$ with equal spatial mesh sizes, the centered leapfrog recurrence has [amplification polynomial of a multilevel finite difference scheme](#amplification-polynomial-of-a-multilevel-finite-difference-scheme) $G^2-2i\mu(\sin\xi+\sin\eta)G-1$. Uniform [stability](numerical-analysis.md#stability-of-a-numerical-method) for arbitrary two-level starting perturbations holds exactly for $0<\mu<1/2$. At $\mu=1/2$ the phase pair $(\pi/2,\pi/2)$ gives $(G-i)^2$, and its [companion matrix](linear-operator-theory.md#companion-matrix) has a nontrivial [Jordan block](linear-operator-theory.md#jordan-block), producing growth proportional to the number of steps. For larger $\mu$ one [polynomial root](polynomial.md#root-of-a-polynomial) has modulus greater than one. Bounds on [eigenvalue](linear-operator-theory.md#eigenvalue) moduli alone therefore give a misleading non-strict endpoint.

###### Two-level stability at the leapfrog Courant boundary

↑ **Parent:** [Leapfrog advection scheme](#leapfrog-advection-scheme)

For the centered two-level advection recurrence, the Fourier roots at Courant number one coalesce at $i$ for phase $\pi/2$. The resulting nontrivial Jordan block admits linearly growing solutions despite both eigenvalues having modulus one. Uniform two-level stability for arbitrary starting perturbations therefore requires the strict inequality $0<\mu<1$. A specially consistent startup can select the exact translating branch at the boundary, which is a restriction on the data rather than a uniform bound on the full update.

##### Leapfrog finite-difference scheme for the diffusion equation

↑ **Parent:** [Amplification polynomial of a multilevel finite difference scheme](#amplification-polynomial-of-a-multilevel-finite-difference-scheme)

Applying a centered leapfrog step in time and the centered second difference in space to $u_t=u_{xx}$ gives

$$
u_m^{n+1}=u_m^{n-1}+2\mu(u_{m-1}^n-2u_m^n+u_{m+1}^n).
$$

For every $\mu>0$, each nonconstant Fourier mode has an amplification root of modulus greater than one, so the scheme is unconditionally unstable.

#### Crank-Nicolson diffusion scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For the centered spatial second difference, the Crank-Nicolson diffusion scheme has amplification factor

$$
G(\theta)=\frac{1-2\mu\sin^2(\theta/2)}
{1+2\mu\sin^2(\theta/2)}.
$$

It is stable for every $\mu\geq0$.

#### Crank-Nicolson centered-advection scheme on a finite interval

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

Let $D$ be the real skew-symmetric tridiagonal matrix with superdiagonal $1$ and subdiagonal $-1$. The centered-space Crank-Nicolson discretization of $u_t=u_x$ has amplification matrix

$$
Q=(I-\mu D/4)^{-1}(I+\mu D/4).
$$

The eigenvalues of $D$ are $2i\cos(j\pi/(M+1))$, so those of $Q$ are Cayley transforms

$$
q_j=\frac{1+i(\mu/2)\cos(j\pi/(M+1))}
{1-i(\mu/2)\cos(j\pi/(M+1))}.
$$

They all have modulus one, and their common orthonormal eigenbasis makes $Q$ normal. Hence the method is stable for every $\mu>0$.

#### Centered three-level wave scheme

↑ **Parent:** [von Neumann stability analysis](#von-neumann-stability-analysis)

For

$$
v_m^{n+1}-2\rho v_m^n+v_m^{n-1}
=\mu(v_{m+1}^n-2v_m^n+v_{m-1}^n),
$$

the amplification polynomial is

$$
G^2+(4\mu\sin^2(\theta/2)-2\rho)G+1=0.
$$

All modes have unit-modulus roots only when $\rho=1$ and $0\leq\mu\leq1$.

### Courant number

↑ **Parent:** [Finite difference method](#finite-difference-method)

The Courant number is the dimensionless ratio of physical propagation during one time step to one spatial grid spacing, commonly $\mu=c\Delta t/\Delta x$.

#### Diffusion Courant number

↑ **Parent:** [Courant number](#courant-number)

The diffusion [Courant number](#courant-number) is $r=\nu k/d^2$ for diffusivity $\nu$, time step $k$ and spatial step $d$. Keeping $r$ fixed is a [parabolic mesh refinement](#parabolic-mesh-refinement). For the [Forward Euler diffusion scheme](#forward-euler-diffusion-scheme) it is bounded by $1/2$ on a uniform one-dimensional grid; the [Backward Euler diffusion scheme](#backward-euler-diffusion-scheme) has no positive upper stability restriction.

<h4 id="courant-friedrichs-lewy-condition">Courant–Friedrichs–Lewy condition</h4>

↑ **Parent:** [Courant number](#courant-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Courant–Friedrichs–Lewy_condition)

A Courant–Friedrichs–Lewy condition requires the numerical domain of dependence to contain the differential equation's physical domain of dependence. It commonly bounds a ratio such as $c\Delta t/\Delta x$ for an explicit hyperbolic scheme.

### Dirichlet discrete Laplacian

↑ **Parent:** [Finite difference method](#finite-difference-method)

On $J$ interior points, the one-dimensional centered second-difference matrix with homogeneous Dirichlet boundaries has eigenvalues

$$
\lambda_j=-4\sin^2\left(\frac{j\pi}{2(J+1)}\right),
\qquad 1\leq j\leq J.
$$

#### Crank-Nicolson stability on a finite Dirichlet interval

↑ **Parent:** [Dirichlet discrete Laplacian](#dirichlet-discrete-laplacian)

If $L$ is the negative semidefinite Dirichlet discrete Laplacian, the Crank-Nicolson amplification matrix

$$
Q=(I-\mu L/2)^{-1}(I+\mu L/2)
$$

has eigenvalues $(1+\mu\lambda_j/2)/(1-\mu\lambda_j/2)$ of modulus at most one for every $\mu\geq0$.

#### Five-point Dirichlet Laplacian as a Kronecker sum

↑ **Parent:** [Dirichlet discrete Laplacian](#dirichlet-discrete-laplacian)

If $T$ is the one-dimensional Dirichlet second-difference matrix on $m$ interior points, the two directional parts of the two-dimensional five-point Laplacian are

$$
A_x=T\otimes I_m,
\qquad
A_y=I_m\otimes T.
$$

They commute, and $A_x+A_y$ is the Kronecker-sum discretization of the Laplacian.

##### One-implicit-direction diffusion splitting

↑ **Parent:** [Five-point Dirichlet Laplacian as a Kronecker sum](#five-point-dirichlet-laplacian-as-a-kronecker-sum)

The split step

$$
(I-\mu A_y)u^{n+1/2}=u^n,
\qquad
u^{n+1}=(I+\mu A_x)u^{n+1/2}
$$

has amplification matrix

$$
C=(I+\mu A_x)(I-\mu A_y)^{-1}.
$$

On a common directional eigenvector its eigenvalue is $(1+\mu\lambda_p)/(1-\mu\lambda_q)$.

###### Stability limit of one-implicit-direction diffusion splitting

↑ **Parent:** [One-implicit-direction diffusion splitting](#one-implicit-direction-diffusion-splitting)

On the $m$ by $m$ Dirichlet grid with $h=1/(m+1)$, the exact discrete stability condition for $m>1$ is

$$
0<\mu\leq\frac1{2\cos(\pi h)}.
$$

The mesh-independent sufficient condition is $0<\mu\leq1/2$, and the exact bound tends to $1/2$ as $h\to0$.

###### Unconditionally stable corrected directional diffusion splitting

↑ **Parent:** [One-implicit-direction diffusion splitting](#one-implicit-direction-diffusion-splitting)

Adding the correction

$$
u^{n+1}=\widetilde u^{n+1}+\mu A_x(u^{n+1}-u^n)
$$

gives

$$
D=(I-\mu A_x)^{-1}(I+\mu^2A_xA_y)(I-\mu A_y)^{-1}.
$$

Its common-basis eigenvalues are

$$
d_{pq}=\frac{1+\mu^2\lambda_p\lambda_q}
{(1-\mu\lambda_p)(1-\mu\lambda_q)}.
$$

Since $\lambda_p,\lambda_q<0$, one has $0<d_{pq}\leq1$ for every $\mu>0$.

#### Seven-point Dirichlet Laplacian

↑ **Parent:** [Dirichlet discrete Laplacian](#dirichlet-discrete-laplacian)

On a three-dimensional Cartesian grid, the seven-point Dirichlet Laplacian adds the six nearest-neighbour values and subtracts six times the central value. Extending a grid vector by zero on the boundary gives the discrete energy identity

$$
v^TL_hv=-\sum_{\{i,j\}\text{ grid edge}}(v_i-v_j)^2,
$$

so its matrix is symmetric negative definite.

### Centered convection-diffusion semidiscretization

↑ **Parent:** [Finite difference method](#finite-difference-method)

With homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), centered differences turn one-dimensional diffusion into a symmetric negative-definite matrix and constant advection into a skew-symmetric matrix. Their sum dissipates the discrete [Euclidean norm](functional-analysis.md#euclidean-norm), giving mesh-uniform energy stability for every fixed advection coefficient.

### Discrete maximum principle

↑ **Parent:** [Finite difference method](#finite-difference-method)

A discrete elliptic operator satisfies a discrete maximum principle when a grid function with nonnegative discrete Laplacian cannot have a positive interior maximum unless it is constant. It yields uniqueness and max-norm stability estimates for Dirichlet finite-difference problems.

### Method of lines

↑ **Parent:** [Finite difference method](#finite-difference-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_lines)

The method of lines discretizes space in a time-dependent partial differential equation while leaving time continuous, producing a finite system of ordinary differential equations.

#### Dissipative second-order forward advection semidiscretization

↑ **Parent:** [Method of lines](#method-of-lines)

For periodic indexing let $S$ be the unitary forward shift. The operator is $A=-3I/2+2S-S^2/2$. A [discrete Fourier transform](numerical-analysis.md#discrete-fourier-transform) diagonalizes it with eigenvalue $\lambda(\theta)=-3/2+2e^{i\theta}-e^{2i\theta}/2$ and real part $-(1-\cos\theta)^2$. Consequently $\|e^{tA/h}\|_2\le1$ for every $t\ge0$, uniformly in the grid. Equivalently $A+A^*=-\tfrac12(2I-S-S^*)^2$, proving decay of the discrete energy directly. The result is semidiscrete [stability](numerical-analysis.md#stability-of-a-numerical-method); a further time discretization must also have adequate [absolute stability](numerical-analysis.md#linear-stability-domain).

#### Energy contraction for centered drift-diffusion

↑ **Parent:** [Method of lines](#method-of-lines)

For homogeneous Dirichlet endpoints, the centered first-difference [matrix](vector-space.md#matrix) is skew-Hermitian and the centered second-difference [matrix](vector-space.md#matrix) is negative definite. Thus $\dot U=(D_{xx}-\alpha D_x)U$ is contractive in the [discrete L2 norm](functional-analysis.md#discrete-l2-norm) for every real $\alpha$ and every mesh width. The displayed identity follows by [summation by parts](analytic-number-theory.md#abel-s-summation-formula). Nonnegative off-diagonal entries additionally require $|\alpha|h\leq2$; that maximum-principle condition is not necessary for the L2 energy estimate. [numerical consistency](numerical-analysis.md#consistency-of-a-numerical-method) and Duhamel's formula then give second-order [numerical convergence](numerical-analysis.md#convergence-of-a-numerical-method) for smooth solutions and compatible initial approximations.

#### Displacement stability of a symmetric semidiscrete wave equation

↑ **Parent:** [Method of lines](#method-of-lines)

Let $K_h$ be a symmetric nonnegative [matrix](vector-space.md#matrix) and consider $U''=(\alpha I-K_h)U$ with fixed real $\alpha$. In any [inner product](linear-algebra.md#inner-product) for which $K_h$ is self-adjoint, [diagonalization of a matrix](linear-operator-theory.md#diagonalization-of-a-matrix) gives

$$
\|U(t)\|\leq e^{\sqrt{\max(\alpha,0)}t}
\bigl(\|U(0)\|+t\|U'(0)\|\bigr).
$$

Indeed each modal coefficient is either a cosine and sine divided by its frequency, a linear function at zero frequency, or a hyperbolic cosine and sine divided by its growth rate. The bounds $|\cos(\omega t)|\leq1$, $|\sin(\omega t)/\omega|\leq t$, and $\sinh(\beta t)/\beta\leq t e^{\beta t}$ prove the estimate. It is uniform in the spectrum of $K_h$ and therefore gives finite-time displacement [stability](numerical-analysis.md#stability-of-a-numerical-method). Uniform velocity estimates need additional control of the initial spatial energy. All-time displacement bounds require a strictly positive lower bound for $K_h-\alpha I$, a different condition.

##### All-time boundedness of a semidiscrete reaction wave equation

↑ **Parent:** [Displacement stability of a symmetric semidiscrete wave equation](#displacement-stability-of-a-symmetric-semidiscrete-wave-equation)

For $U''=(\alpha I-K_h)U$ with symmetric positive definite $K_h$, all-data displacement is bounded for all time on a fixed grid exactly when $\alpha<\lambda_{\min}(K_h)$. [Diagonalization of a matrix](linear-operator-theory.md#diagonalization-of-a-matrix) reduces this assertion to oscillators. At equality, an initial velocity in a zero-frequency mode produces linear growth; above it a growing hyperbolic mode is available. A lower bound on $\lambda_{\min}(K_h)-\alpha$ uniform in the mesh gives a uniform displacement estimate. This all-time statement is stronger than [displacement stability of a symmetric semidiscrete wave equation](#displacement-stability-of-a-symmetric-semidiscrete-wave-equation) on fixed finite time intervals.

<h4 id="norm-conservation-of-a-semidiscrete-schrodinger-equation">Norm conservation of a semidiscrete Schrödinger equation</h4>

↑ **Parent:** [Method of lines](#method-of-lines)

If a spatial [method of lines](#method-of-lines) has a [Hermitian matrix](hilbert-space.md#hermitian-operator) $H$, its generator $-iH$ is a [skew-Hermitian matrix](linear-operator-theory.md#skew-hermitian-matrix). The [matrix exponential](linear-operator-theory.md#matrix-exponential) $e^{-itH}$ is a [unitary matrix](linear-operator-theory.md#unitary-matrix), so it preserves the [Euclidean norm](functional-analysis.md#euclidean-norm) and any constant-volume [discrete L2 norm](functional-analysis.md#discrete-l2-norm). Equivalently, differentiating the squared [norm](functional-analysis.md#norm) gives $2\operatorname{Re}(-iU^*HU)=0$. A real sampled potential preserves the Hermitian property of a symmetric discrete Laplacian. Subsequent time discretization must be assessed separately.

### Lax equivalence theorem

↑ **Parent:** [Finite difference method](#finite-difference-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lax_equivalence_theorem)

For a well-posed linear initial-value problem and a consistent finite-difference approximation, stability is equivalent to convergence.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (17)

- [Binomial inversion](combinatorics.md#binomial-inversion)
- [Discrete sine transform Poisson solver](numerical-analysis.md#discrete-sine-transform-poisson-solver)
- [Mahler expansion of continuous p-adic functions](measure-theory.md#mahler-expansion-of-continuous-p-adic-functions)
- [Overlap multiplicity bound for piecewise difference operators](inverse-problem.md#overlap-multiplicity-bound-for-piecewise-difference-operators)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#39a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#15d/e/solution)
- [Reaction-diffusion spectral decay threshold](diffusion-equation.md#reaction-diffusion-spectral-decay-threshold)
- [Truncation error](numerical-analysis.md#truncation-error)
- [Uniform convergence of Bernstein polynomial derivatives](functional-analysis.md#uniform-convergence-of-bernstein-polynomial-derivatives)
- [Weyl differencing](analytic-number-theory.md#weyl-differencing)
