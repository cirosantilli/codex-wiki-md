# Green's function

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Green's_function)

**Table of contents**

- [Time support from poles of a Fourier Green function](#time-support-from-poles-of-a-fourier-green-function)
- [Fourier Green function in a spatially varying background](#fourier-green-function-in-a-spatially-varying-background)
- [Advanced Green function](#advanced-green-function)
- [Source-position-dependent Fourier Green function](#source-position-dependent-fourier-green-function)
- [Neumann Green function with constant boundary flux](#neumann-green-function-with-constant-boundary-flux)
- [Half-line Green function for the first cylindrical harmonic](#half-line-green-function-for-the-first-cylindrical-harmonic)
- [Bounded Green kernel for a radial Euler operator](#bounded-green-kernel-for-a-radial-euler-operator)
- [Green function of an undamped oscillator](#green-function-of-an-undamped-oscillator)
- [Green kernels for a radial dipole Euler equation](#green-kernels-for-a-radial-dipole-euler-equation)
- [Green kernel and endpoint compatibility for a singular Euler equation](#green-kernel-and-endpoint-compatibility-for-a-singular-euler-equation)
- [Radial modified Helmholtz Green function on the half-line](#radial-modified-helmholtz-green-function-on-the-half-line)
- [Green kernel with a vanishing Wronskian at an interior singular point](#green-kernel-with-a-vanishing-wronskian-at-an-interior-singular-point)
- [Decaying two-sided Green function of a constant-coefficient ordinary differential equation](#decaying-two-sided-green-function-of-a-constant-coefficient-ordinary-differential-equation)
- [Nonunique Green kernel at a singular endpoint with two vanishing modes](#nonunique-green-kernel-at-a-singular-endpoint-with-two-vanishing-modes)
- [Fourth-order Green kernel with two decay scales](#fourth-order-green-kernel-with-two-decay-scales)
- [Causal Green function for a repeated-root Euler operator](#causal-green-function-for-a-repeated-root-euler-operator)
- [Boundary-decaying Green kernel for an inverse-square differential operator](#boundary-decaying-green-kernel-for-an-inverse-square-differential-operator)
- [Radial Helmholtz Dirichlet Green function](#radial-helmholtz-dirichlet-green-function)
- [Dipole Green tensor angular cancellation](#dipole-green-tensor-angular-cancellation)
- [Robin half-line Green function from left and right solutions](#robin-half-line-green-function-from-left-and-right-solutions)
- [Green function on a Riemann surface](#green-function-on-a-riemann-surface)
- [Impulse response](#impulse-response)
- [Complex transport Green function](#complex-transport-green-function)
- [Dirichlet Green function](#dirichlet-green-function)
  - [Sign conventions for a Dirichlet Green function](#sign-conventions-for-a-dirichlet-green-function)
  - [Dirichlet Green kernel for an Euler operator with exponents one and minus four](#dirichlet-green-kernel-for-an-euler-operator-with-exponents-one-and-minus-four)
  - [Dirichlet Green function inside the unit disk](#dirichlet-green-function-inside-the-unit-disk)
  - [Dirichlet image kernel for the three-dimensional modified Helmholtz equation](#dirichlet-image-kernel-for-the-three-dimensional-modified-helmholtz-equation)
  - [Dirichlet Green function for a conjugated harmonic oscillator](#dirichlet-green-function-for-a-conjugated-harmonic-oscillator)
  - [Dirichlet Green function between parallel planes](#dirichlet-green-function-between-parallel-planes)
  - [Dirichlet Green function inside a sphere](#dirichlet-green-function-inside-a-sphere)
    - [Dirichlet Green function inside a hemisphere](#dirichlet-green-function-inside-a-hemisphere)
  - [Bounded exterior disk Green function](#bounded-exterior-disk-green-function)
  - [Dirichlet Green function for a radial power operator on an interval](#dirichlet-green-function-for-a-radial-power-operator-on-an-interval)
  - [Dirichlet Helmholtz Green function on an interval](#dirichlet-helmholtz-green-function-on-an-interval)
  - [Green function of killed planar Brownian motion](#green-function-of-killed-planar-brownian-motion)
  - [Dirichlet Green function in a quadrant](#dirichlet-green-function-in-a-quadrant)
  - [Regular part of the planar Dirichlet Green function](#regular-part-of-the-planar-dirichlet-green-function)
- [Green-function representation](#green-function-representation)
- [One-dimensional modified Helmholtz Green function](#one-dimensional-modified-helmholtz-green-function)
  - [Dirichlet modified Helmholtz Green function on an interval](#dirichlet-modified-helmholtz-green-function-on-an-interval)
  - [Dirichlet half-line Green function for minus d2 plus 1](#dirichlet-half-line-green-function-for-minus-d2-plus-1)
    - [Dirichlet half-line response to uniform interval forcing](#dirichlet-half-line-response-to-uniform-interval-forcing)
  - [Fourier decay from a Green-function derivative jump](#fourier-decay-from-a-green-function-derivative-jump)
  - [Dirichlet half-line Green function for d2 minus 1](#dirichlet-half-line-green-function-for-d2-minus-1)
- [Dirichlet Green function for an infinite strip](#dirichlet-green-function-for-an-infinite-strip)
- [Neumann Green function for a second-order ordinary differential equation](#neumann-green-function-for-a-second-order-ordinary-differential-equation)
  - [Neumann Green function for the modified Helmholtz equation on an interval](#neumann-green-function-for-the-modified-helmholtz-equation-on-an-interval)
- [Causal Green function](#causal-green-function)
  - [Causality versus stability of a Green function](#causality-versus-stability-of-a-green-function)
  - [Jump conditions for a third-order Green function](#jump-conditions-for-a-third-order-green-function)
- [One-dimensional outgoing Green function](#one-dimensional-outgoing-green-function)

## Time support from poles of a Fourier Green function

↑ **Parent:** [Green's function](green-s-function.md)

For the inverse transform $G(\tau)=\int d\omega\,e^{-i\omega\tau}g(\omega)/(2\pi)$, positive $\tau$ requires closing a decaying contour below the real axis, clockwise; negative $\tau$ requires closing above, counterclockwise. [Poles](isolated-singularity.md#pole) strictly below give a [retarded Green function](quantum-field-theory.md#retarded-green-function), while [poles](isolated-singularity.md#pole) strictly above give an [advanced Green function](#advanced-green-function). Real-axis [poles](isolated-singularity.md#pole) need a prescription. The sign convention in the Fourier exponential is essential.

## Fourier Green function in a spatially varying background

↑ **Parent:** [Green's function](green-s-function.md)

A static background permits a [Fourier transform](fourier-transform.md) of time difference, but a spatially varying coefficient generally prevents dependence on position difference alone. A momentum-space [Green function](green-s-function.md) then carries an incoming and an outgoing [momentum](momentum.md), or equivalently one [momentum](momentum.md) together with the source position. Multiplication by a background field becomes a convolution, with a source-position phase when the Fourier basis is written as $e^{i\mathbf k\cdot(\mathbf r-\mathbf r')}$. A diagonal single-momentum representation is justified only with additional spatial [translation](geometry-and-topology.md#translation-geometry) symmetry or an explicitly fixed source origin.

## Advanced Green function

↑ **Parent:** [Green's function](green-s-function.md)

An [advanced Green function](#advanced-green-function) has support only before its source time. It is selected by a future [boundary condition](differential-equation.md#boundary-condition), rather than an initial causal response. For $L=\partial_t^2+2\lambda\partial_t+\omega_0^2$ with $\lambda<0$ and $\Omega^2=\omega_0^2-\lambda^2>0$, the real-axis inverse [Fourier transform](fourier-transform.md) of $(-\omega^2-2i\lambda\omega+\omega_0^2)^{-1}$ is $-H(-t)e^{-\lambda t}\sin(\Omega t)/\Omega$. Its first derivative jumps by one at zero. A growing retarded solution exists with a different inverse [contour](complex-analysis.md#complex-integration-contour); this illustrates [causality versus stability of a Green function](#causality-versus-stability-of-a-green-function).

## Source-position-dependent Fourier Green function

↑ **Parent:** [Green's function](green-s-function.md)

A static but spatially inhomogeneous linear operator has time [translation](geometry-and-topology.md#translation-geometry) [symmetry](physics.md#symmetry-physics) without spatial [translation](geometry-and-topology.md#translation-geometry) [symmetry](physics.md#symmetry-physics). At fixed [source](perturbative-quantum-field-theory.md#source-quantum-field-theory) position $\mathbf r'$, one may still [Fourier transform](fourier-transform.md) its [Green function](green-s-function.md) in $\mathbf x=\mathbf r-\mathbf r'$. The coefficient retains $\mathbf r'$ as a parameter. A multiplication by $V(\mathbf r)$ becomes a [convolution](fourier-analysis.md#convolution) with $V_{\mathbf r'}(\mathbf q)=e^{i\mathbf q\cdot\mathbf r'}\widetilde V(\mathbf q)$, not a spatially diagonal multiplier unless $V$ is constant. Suppressing the source-position subscript is only a notational convention.

## Neumann Green function with constant boundary flux

↑ **Parent:** [Green's function](green-s-function.md)

For a smooth bounded connected [domain](topology.md#domain-mathematical-analysis) $V$ with boundary $S$, integrating the [Green function](green-s-function.md) equation and applying the [divergence theorem](multivariable-calculus.md#divergence-theorem) forces $\int_S\partial_nG\,dS=1$. Thus zero [Neumann boundary data](differential-equation.md#neumann-boundary-data) are incompatible with an unmodified unit point source. The displayed constant boundary derivative has the required total flux. For $\Delta\Phi=\sigma$ and $\partial_n\Phi=f$, the compatibility condition is $\int_V\sigma\,dV=\int_Sf\,dS$. [Green's second identity](partial-differential-equation.md#green-second-identity) then yields

$$
\Phi(x_0)=\int_VG(x,x_0)\sigma(x)dV-\int_SG(x,x_0)f(x)dS+\frac1{|S|}\int_S\Phi\,dS.
$$

The last term is an undetermined additive constant. Adding a constant to $G$ does not change the other two terms together, because of the compatibility condition. This construction keeps the unit [Dirac delta](distribution-theory.md#dirac-delta-function) source; using a mean-subtracted source with zero normal derivative is a different normalization.

## Half-line Green function for the first cylindrical harmonic

↑ **Parent:** [Green's function](green-s-function.md)

For $Ly=y''+y'/x-y/x^2$ on $x>0$, impose $y(0)=0$ by a continuous limit and $y(x)\to0$ at infinity. The adapted homogeneous solutions are $x$ at zero and $1/x$ at infinity, with [Wronskian](linear-ordinary-differential-equation.md#wronskian) $-2/x$. The displayed [Green function](green-s-function.md) is continuous and its first [derivative](calculus.md#derivative) has jump one at $x=s$, so $L_xG(x,s)=\delta(x-s)$ with ordinary source measure $ds$. For continuous $f$ with $\int_0^\infty(1+s^2)|f(s)|ds<\infty$,

$$
y(x)=\int_0^\infty G(x,s)f(s)ds=-\frac1{2x}\int_0^xs^2f(s)ds-\frac x2\int_x^\infty f(s)ds.
$$

This solves $Ly=f$ with the stated endpoint limits. No nonzero combination of $x,1/x$ meets both homogeneous endpoint conditions, proving [uniqueness](mathematical-logic.md#uniqueness). Multiplying $L$ by $x$ gives the self-adjoint expression $(xy')'-y/x$, explaining the weighted reciprocity $xG(x,s)=sG(s,x)$.

## Bounded Green kernel for a radial Euler operator

↑ **Parent:** [Green's function](green-s-function.md)

For $L y=(x^2y')'-2y$ on $x>0$, choose solutions bounded at zero and infinity. The homogeneous [Cauchy-Euler equation](linear-ordinary-differential-equation.md#cauchy-euler-equation) has basis $x,x^{-2}$. Joining the left-regular and right-regular solutions continuously and imposing $s^2[G_x]_{s^-}^{s^+}=1$ gives the displayed [Green's function](green-s-function.md) with ordinary integration measure $ds$. For bounded forcing,

$$
y(x)=-\frac1{3x^2}\int_0^x sf(s)ds-\frac x3\int_x^\infty\frac{f(s)}{s^2}ds.
$$

The integrals converge and give the unique bounded solution: no nonzero homogeneous combination is bounded at both ends. If $0\leq f\leq M$, negativity of the kernel gives $-M/2\leq y\leq0$. Differentiation cancels the two moving-endpoint terms, leaving

$$
y'(x)=\frac2{3x^3}\int_0^x sf(s)ds-\frac13\int_x^\infty\frac{f(s)}{s^2}ds,
$$

which implies $|y'(x)|\leq M/(3x)$. For constant forcing $f=M$, the bounded solution is $-M/2$; the endpoint conditions are boundedness, rather than zero endpoint values.

## Green function of an undamped oscillator

↑ **Parent:** [Green's function](green-s-function.md)

For zero initial value and slope, the causal [Green function](green-s-function.md) is $G_0(x,s)=H(x-s)\sin[k(x-s)]/k$, with $k\ne0$ and $H$ the [Heaviside step function](integral-transform.md#heaviside-step-function). For zero values at endpoints $a<b$, put $\kappa=|k|$. The [Dirichlet Green function](#dirichlet-green-function) is

$$
G_D(x,s)=-\frac{\sin[\kappa(x_<-a)]\sin[\kappa(b-x_>)]}{\kappa\sin[\kappa(b-a)]}.
$$

Both are continuous at the source and have a first-derivative jump of one, giving $L_xG=\delta(x-s)$. The Dirichlet inverse exists when $\sin[\kappa(b-a)]\ne0$; a zero denominator signals a nontrivial homogeneous mode and a [Fredholm solvability condition](sturm-liouville-theory.md#fredholm-solvability-condition). The endpoint kernel is the zero-conjugation case of the [Dirichlet Green function for a conjugated harmonic oscillator](#dirichlet-green-function-for-a-conjugated-harmonic-oscillator). Boundary conditions determine which kernel must be integrated against a forcing term.

## Green kernels for a radial dipole Euler equation

↑ **Parent:** [Green's function](green-s-function.md)

The homogeneous [Cauchy-Euler equation](linear-ordinary-differential-equation.md#cauchy-euler-equation) $Ly=0$ has fundamental solutions $x,x^{-1}$ on $x>0$, with [Wronskian](linear-ordinary-differential-equation.md#wronskian) $-2/x$. Requiring decay at both endpoints gives the unweighted [Green's function](green-s-function.md)

$$
G_D(x,\xi)=\begin{cases}-x/2,&x\leq\xi,\\-\xi^2/(2x),&x\geq\xi.\end{cases}
$$

Requiring zero initial value and derivative at zero instead gives the forward kernel

$$
G_0(x,\xi)=\begin{cases}0,&x\leq\xi,\\(x-\xi^2/x)/2,&x\geq\xi.\end{cases}
$$

Both kernels are continuous and have first-derivative jump one at $x=\xi$, so $L_xG=\delta(x-\xi)$. Away from that point they solve the homogeneous equation. Integrating against the forcing with ordinary measure $d\xi$ yields the respective solutions whenever the integral and endpoint limits converge. Their difference is $G_0-G_D=x/2$, independent of $\xi$, so the solutions differ by the homogeneous term $(x/2)\int f(\xi)d\xi$ for integrable forcing. For example, the two choices for an indicator forcing on $(0,1)$ differ by $x/2$. Specifying a differential operator without its endpoint conditions does not specify its Green kernel.

## Green kernel and endpoint compatibility for a singular Euler equation

↑ **Parent:** [Green's function](green-s-function.md)

For $0<x<1$, the homogeneous [Cauchy-Euler equation](linear-ordinary-differential-equation.md#cauchy-euler-equation) has solutions $x,x^{-1}$. The left-vanishing solution $x$ and right-vanishing solution $x-x^{-1}$ give the unweighted [Green function](green-s-function.md) $G(x,s)=x(1-s^{-2})/2$ for $x\leq s$ and $(x-x^{-1})/2$ for $x\geq s$. It is continuous at $x=s$ and its first derivative has jump $1/s^2$, so $L_xG=\delta(x-s)$.

For continuous forcing $f$ on $[0,1]$, its integral is

$$
u(x)=\frac{x-x^{-1}}2\int_0^xf(s)ds+\frac x2\int_x^1(1-s^{-2})f(s)ds.
$$

This is bounded at zero and vanishes at one, but $u(0^+)=-f(0)$. The first singular term uses the average $x^{-1}\int_0^xf\to f(0)$. In the other, the substitution $t=x/s$ gives $x\int_x^1f(s)s^{-2}ds=\int_x^1f(x/t)dt\to f(0)$ by [dominated convergence](measure-theory.md#dominated-convergence-theorem). Thus the two zero endpoint values require $f(0)=0$. When compatible, the solution is unique among bounded solutions because no nonzero combination of $x,x^{-1}$ meets both homogeneous endpoint conditions. This example shows why pointwise endpoint behavior of a [Green function](green-s-function.md) does not itself justify passing a limit through its integral.

## Radial modified Helmholtz Green function on the half-line

↑ **Parent:** [Green's function](green-s-function.md)

For $Ly=-x^{-2}(x^2y')'+y$ on $x>0$, require boundedness at zero and at infinity. The substitution $z=xy$ reduces the homogeneous equation to $-z''+z=0$. The adapted solutions are $\sinh x/x$ at zero and $e^{-x}/x$ at infinity, with [Wronskian](linear-ordinary-differential-equation.md#wronskian) $-x^{-2}$. The displayed [Green function](green-s-function.md) is continuous and has first-derivative jump $-1$, so $L_xG=\delta(x-\xi)$ with ordinary source measure $d\xi$. It satisfies weighted reciprocity $x^2G(x,\xi)=\xi^2G(\xi,x)$. For forcing equal to one on $[0,R]$ and zero outside, integration gives $y=1-(R+1)e^{-R}\sinh x/x$ inside and $y=(R\cosh R-\sinh R)e^{-x}/x$ outside. Limits define the regular value at zero.

## Green kernel with a vanishing Wronskian at an interior singular point

↑ **Parent:** [Green's function](green-s-function.md)

The usual [Green function](green-s-function.md) formula for a monic second-order equation requires a nonzero [Wronskian](linear-ordinary-differential-equation.md#wronskian) at the source. At an interior [singular point](algebraic-geometry.md#singular-point-of-an-algebraic-variety) it may fail to define an ordinary inverse for arbitrary forcing. For example, for $Ly=y''-(1+x)y'/x+y/x$ on $[-1,1]$, choose $u=1+x$ and $v=e^x-e(1+x)/2$. They satisfy the left and right [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), and $W=uv'-u'v=xe^x$. The displayed kernel is valid for $\xi\ne0$ and has unit jump in its first $x$ derivative. Its $1/\xi$ behaviour prevents unrestricted integration through zero. For smooth forcing $f(x)=xq(x)$, the product $G(x,\xi)f(\xi)$ has a removable singularity, and its integral gives the unique solution extending with two continuous derivatives through zero. That matching condition matters: merely requiring one continuous derivative allows additional piecewise homogeneous solutions. A smooth forcing with $f(0)\ne0$ cannot have a solution with two continuous derivatives there, as expansion of $xy''-(1+x)y'+y=xf$ shows.

## Decaying two-sided Green function of a constant-coefficient ordinary differential equation

↑ **Parent:** [Green's function](green-s-function.md)

Let $p(D)$ be a constant-coefficient differential operator, $D=d/dt$, with distinct characteristic roots $\lambda_j$ having nonzero real parts. The solution of $p(D)K=\delta$ decaying at both temporal infinities is

$$
K(t)=H(t)\sum_{\operatorname{Re}\lambda_j<0}\frac{e^{\lambda_jt}}{p'(\lambda_j)}-H(-t)\sum_{\operatorname{Re}\lambda_j>0}\frac{e^{\lambda_jt}}{p'(\lambda_j)},
$$

where $H$ is the [Heaviside step function](integral-transform.md#heaviside-step-function). This follows by [partial fraction decomposition](isolated-singularity.md#partial-fraction-decomposition) of $1/p(z)$ and the first-order kernels $e^{\lambda t}H(t)$ for $\operatorname{Re}\lambda<0$, or $-e^{\lambda t}H(-t)$ for $\operatorname{Re}\lambda>0$. Both first-order kernels jump by one and solve $(D-\lambda)K_\lambda=\delta$ as [distributions](distribution-theory.md#distribution-mathematical-analysis).

For example, $p(D)=(D+1)(D-2)(D+2)$ gives

$$
K(t)=\begin{cases}-e^{2t}/12,&t<0,\\-e^{-t}/3+e^{-2t}/4,&t>0.\end{cases}
$$

It is continuous together with its first derivative; its second derivative jumps by one, as required by the [jump conditions for a third-order Green function](#jump-conditions-for-a-third-order-green-function). A solution of $p(D)y=f$ is the [convolution](fourier-analysis.md#convolution) $K*f$ when it exists. If positive-real-part roots occur, decay at both ends generally requires a nonzero negative-time branch: this is the distinction captured by [causality versus stability of a Green function](#causality-versus-stability-of-a-green-function). A causal kernel would retain growing positive-time terms and need not have a real-axis [Fourier transform](fourier-transform.md).

## Nonunique Green kernel at a singular endpoint with two vanishing modes

↑ **Parent:** [Green's function](green-s-function.md)

On $0<x<1$, both independent homogeneous solutions $x,x^3$ vanish at the singular endpoint zero. Consequently imposing $y(0)=y(1)=0$ leaves the nonzero homogeneous solution $x^3-x$ and does not determine a unique inverse. One valid right [Green function](green-s-function.md), with $L_xG=\delta(x-z)$ and zero endpoint values, is

$$
G_0(x,z)=\begin{cases}x(z^3-z)/(2z^3),&x\leq z,\\(x^3-x)/(2z^2),&x\geq z.\end{cases}
$$

Its first [derivative](calculus.md#derivative) has jump one because the [Wronskian](linear-ordinary-differential-equation.md#wronskian) of $x$ and $x^3-x$ is $2z^3$. Every kernel $G_0+(x^3-x)h(z)$ preserves these properties when the integrals exist. For sources supported away from zero, integration yields one particular solution; the full endpoint-constrained family adds $C(x^3-x)$. An additional endpoint selection, such as $y(x)/x\to0$, can choose a unique member. This is a singular-endpoint phenomenon, not an ordinary regular two-point uniqueness theorem.

## Fourth-order Green kernel with two decay scales

↑ **Parent:** [Green's function](green-s-function.md)

For $0<a<b$, the displayed decaying [Green function](green-s-function.md) solves $(-\partial_x^2+a^2)(-\partial_x^2+b^2)K=\delta_0$ on the real line. Its [Fourier transform](fourier-transform.md) is

$$
\widetilde K(k)=\frac1{(k^2+a^2)(k^2+b^2)}
=\frac1{b^2-a^2}\left(\frac1{k^2+a^2}-\frac1{k^2+b^2}\right).
$$

Invert each term using the [one-dimensional modified Helmholtz Green function](#one-dimensional-modified-helmholtz-green-function). Then a decaying solution with forcing $h$ is the [convolution](fourier-analysis.md#convolution) $K*h$. For $a=1,b=2$, this gives $K=e^{-|x|}/6-e^{-2|x|}/12$ for the operator $\partial_x^4-5\partial_x^2+4$. Its first-derivative jump cancels, while its third-derivative jump is one, providing the unit [Dirac delta distribution](distribution-theory.md#dirac-delta-function) required by the fourth-order operator.

## Causal Green function for a repeated-root Euler operator

↑ **Parent:** [Green's function](green-s-function.md)

For $L=y''+\alpha y'/x+(\alpha-1)^2y/(4x^2)$ on $x>0$, the repeated [indicial root](linear-ordinary-differential-equation.md#indicial-root) is $r=(1-\alpha)/2$ and the homogeneous solutions are $x^r,x^r\log x$. Their [Wronskian](linear-ordinary-differential-equation.md#wronskian) is $x^{-\alpha}$. The displayed [causal Green function](#causal-green-function) is continuous at each source $\xi>0$, has a unit jump in its first [derivative](calculus.md#derivative), and satisfies $L_xG=\delta(x-\xi)$. It is zero near the origin, so its value and first derivative there vanish. Those origin conditions alone fail to give uniqueness when $\alpha<-1$: then both homogeneous solutions and their first derivatives vanish as $x\downarrow0$. For forcing $f(x)=x$, source integration from zero converges when $\alpha>-5$ and gives $y_p=4x^3/(\alpha+5)^2$. All zero-origin-data solutions in $-5<\alpha<-1$ are $y_p+x^r(C_1+C_2\log x)$; for $\alpha\geq-1$ the solution is unique. Causality selects the displayed kernel even when the bare singular-endpoint conditions are insufficient.

## Boundary-decaying Green kernel for an inverse-square differential operator

↑ **Parent:** [Green's function](green-s-function.md)

For $L=d^2/dx^2-2/x^2$ on $x>0$, the homogeneous solutions $x^2,x^{-1}$ satisfy respectively the zero and infinity [boundary conditions](differential-equation.md#boundary-condition). Their [Wronskian](linear-ordinary-differential-equation.md#wronskian) is $-3$. The displayed [Green's function](green-s-function.md) is continuous at $x=\xi$ and its first [derivative](calculus.md#derivative) has jump one, so $L_xG=\delta(x-\xi)$ in the [distribution](distribution-theory.md#distribution-mathematical-analysis) sense. Integration against a compactly supported forcing gives the unique solution decaying at both boundaries.

## Radial Helmholtz Dirichlet Green function

↑ **Parent:** [Green's function](green-s-function.md)

For $L=d^2/dx^2+(2/x)d/dx+k^2$ on $0<x<1$, impose finiteness at zero and zero value at one. Set $H=xG$; then $H''+k^2H=\xi\delta(x-\xi)$ with ordinary zero-endpoint conditions. The displayed [Green function](green-s-function.md) follows from the left/right sine solutions, where $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. Its derivative jumps by one. It exists for $k\notin\pi\mathbb Z\setminus\{0\}$; at zero take the removable limit $G=-\xi x_<(1-x_>)/x$. At nonzero integer multiples of pi the radial problem has a nonzero homogeneous solution and a [Fredholm solvability condition](sturm-liouville-theory.md#fredholm-solvability-condition). Integrating against the constant forcing gives $y=k^{-2}[1-\sin(kx)/(x\sin k)]$, with $y=(x^2-1)/6$ at $k=0$.

## Dipole Green tensor angular cancellation

↑ **Parent:** [Green's function](green-s-function.md)

For the three-dimensional reference Green function $g(r)=1/(4\pi br)$, the distributional mixed Hessian $K=\nabla_x\nabla_{x'}g$ has the displayed contact and principal-value parts. Since the spherical mean of $n\otimes n$ is $I/3$, its ordinary dipole part has zero angular integral. Radial weighting therefore isolates the contact term, provided boundary truncation is absent or negligible in the bulk limit.

## Robin half-line Green function from left and right solutions

↑ **Parent:** [Green's function](green-s-function.md)

For a monic second-order operator, choose a homogeneous solution $u$ satisfying the left [Robin boundary condition](differential-equation.md#robin-boundary-condition) and a solution $v$ satisfying the right decay condition. With $W=uv'-u'v\ne0$, the displayed kernel is continuous and its first derivative has jump one. It therefore satisfies $LG=\delta$ and the two boundary conditions. The operator's first derivative term generally makes $W$ nonconstant and the resulting [Green function](green-s-function.md) nonsymmetric in the unweighted variables.

## Green function on a Riemann surface

↑ **Parent:** [Green's function](green-s-function.md)

With the positive logarithmic convention, a Green function with pole $p$ on a noncompact [Riemann surface](riemann-surfaces.md) is positive and harmonic away from $p$, has local form $-\log|\zeta|$ plus a harmonic function in a coordinate $\zeta(p)=0$, and is minimal among positive functions with these properties. It is obtained, when finite, as the increasing limit of zero-boundary Green functions on an exhaustion by compact bordered subdomains. On the [unit disk](euclidean-geometry.md#unit-disk) it is

$$
G_{\mathbb D}(z,p)=\log\left|\frac{1-\overline pz}{z-p}\right|.
$$

Its sign convention is $-\Delta G=2\pi\delta_p$ in a conformal coordinate, with the opposite overall sign from conventions using $\log|\zeta|$ as the singular part.

## Impulse response

↑ **Parent:** [Green's function](green-s-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Impulse_response)

The impulse response records the response to a unit impulse, with specified initial or boundary conditions. In continuous time the impulse is a [Dirac delta function](distribution-theory.md#dirac-delta-function); in discrete time it is the [Kronecker delta](multilinear-algebra.md#kronecker-delta) $\delta[n]$. For a [linear time-invariant system](electrical-engineering.md#linear-time-invariant-system) with zero initial state, the response to a general [input](theoretical-computer-science.md#input-computer-science) is its [convolution](fourier-analysis.md#convolution) with the impulse response. The impulse response of a [causal filter](electrical-engineering.md#causal-filter) is zero before the impulse.

For the five-sample [moving average](electrical-engineering.md#moving-average), a discrete impulse produces $h[n]=1/5$ at $n=0,1,2,3,4$ and zero otherwise. The response lasts five samples, so this is a [finite impulse response](electrical-engineering.md#finite-impulse-response) system. Its [frequency response](electrical-engineering.md#frequency-response) is the finite sum of the five delayed phase contributions: one short input experiment determines how every sustained sinusoid is filtered.

## Complex transport Green function

↑ **Parent:** [Green's function](green-s-function.md)

For $L_k=k\partial_z+k^{-1}\partial_{\bar z}$, $k\ne0$, $|k|\ne1$, this kernel satisfies $L_kG_k=\delta_0$. A real-linear change of complex coordinate reduces its derivation to the [Cauchy-Green operator](complex-geometry.md#cauchy-green-operator); the determinant changes sign at the unit circle. For $|k|=1$ the operator becomes a real directional [transport equation](transport-equation.md), whose characteristic singularity requires limiting prescriptions. The kernel has $G_k\sim k/(\pi z)$ at zero and $G_k\sim1/(\pi k\bar z)$ at infinity.

## Dirichlet Green function

↑ **Parent:** [Green's function](green-s-function.md)

A Dirichlet Green function for a differential operator satisfies homogeneous Dirichlet boundary conditions in one variable. It converts source and boundary data into an integral representation of the solution.

### Sign conventions for a Dirichlet Green function

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

Let $G$ vanish on the boundary of a domain and satisfy $\Delta G(\cdot,y)=\delta_y$. [Green's second identity](partial-differential-equation.md#green-second-identity) gives

$$
u(y)=\int_\Omega G(x,y)\Delta u(x)dx+\int_{\partial\Omega}u(x)\partial_{n_x}G(x,y)dS_x.
$$

Thus the [Poisson kernel](partial-differential-equation.md#poisson-kernel) is $+\partial_nG$ for this convention. If instead $-\Delta K=\delta$, then $K=-G$ and the same kernel is $-\partial_nK$. At the boundary of $x>0$, the outward normal is $-e_x$, so the first convention gives $P=-\partial_xG$. Changing the delta-source sign or replacing the outward derivative by an inward coordinate derivative changes a sign; changing both leaves the physical kernel unchanged.

### Dirichlet Green kernel for an Euler operator with exponents one and minus four

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For $L=d^2/dx^2+4x^{-1}d/dx-4x^{-2}$ on $(0,1)$, regularity at zero selects the homogeneous solution $u=x$, while the right [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) selects $v=x^{-4}-x$. Their [Wronskian](linear-ordinary-differential-equation.md#wronskian) is $-5x^{-4}$. Thus the displayed [Green function](green-s-function.md), with $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$, is continuous, has unit first-derivative jump and satisfies $L_xG=\delta(x-\xi)$. For bounded forcing $f$, $y(x)=\int_0^1G(x,\xi)f(\xi)d\xi$ is the unique solution continuous at zero with zero endpoint values. The singular homogeneous branch $x^{-4}$ is excluded by that regularity. The kernel uses ordinary source measure $d\xi$, not the measure for the multiplied [self-adjoint](linear-operator-theory.md#self-adjoint-operator) operator.

### Dirichlet Green function inside the unit disk

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

With the convention $\Delta_zG_D=\delta(z-\zeta)$, the displayed [Dirichlet Green function](#dirichlet-green-function) vanishes on the [unit circle](complex-analysis.md#complex-unit-circle). Indeed $|z-\zeta|=|1-z\bar\zeta|$ when $|z|=1$. For $\zeta\ne0$, the second logarithm corresponds to an opposite image source at $\zeta/|\zeta|^2$, outside the [unit disc](topology.md#unit-disc); it is a [harmonic function](partial-differential-equation.md#harmonic-function) throughout the interior. At $\zeta=0$ the formula becomes $(2\pi)^{-1}\log|z|$. Its outward [normal derivative](differential-geometry.md#normal-derivative) in the boundary variable is $(2\pi)^{-1}(1-|\zeta|^2)/|z-\zeta|^2$, the [Poisson kernel](partial-differential-equation.md#poisson-kernel) divided by $2\pi$. [Green's second identity](partial-differential-equation.md#green-second-identity) therefore gives the [Poisson integral on the unit disk](partial-differential-equation.md#poisson-integral-on-the-unit-disk).

### Dirichlet image kernel for the three-dimensional modified Helmholtz equation

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For $\kappa\geq0$ in the upper half-space, let $r'^*$ be the reflection of the interior source $r'$ across its boundary plane. The displayed decaying [Green function](green-s-function.md) solves $(\Delta-\kappa^2)G_D=\delta(r-r')$ with zero [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition). The direct term supplies the source; the image source lies outside the domain and its opposite sign makes the two terms cancel on the plane. The minus sign relative to the positive [static Yukawa Green function](nuclear-force.md#static-yukawa-green-function) comes from the operator convention. The case $\kappa=0$ is the Coulomb limit. An infinity condition is needed for uniqueness on an unbounded domain.

### Dirichlet Green function for a conjugated harmonic oscillator

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For $D=d/dx$ and $L_a=(D-a)^2+b^2$ on $(0,L)$, with $b>0$ and $\sin(bL)\ne0$, the substitution $y=e^{ax}v$ gives $L_ay=e^{ax}(v''+b^2v)$. Here $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. The displayed [Green function](green-s-function.md) vanishes at the endpoints, is continuous at $x=\xi$, and its first [derivative](calculus.md#derivative) has jump one, so $L_{a,x}G=\delta(x-\xi)$. It is the usual sine [Dirichlet Green function](#dirichlet-green-function) conjugated by the exponential factor. At $bL\in\pi\mathbb Z\setminus\{0\}$ there is a homogeneous zero mode, so the inverse kernel does not exist without a [solvability condition](linear-operator-theory.md#solvability-condition) and a normalization.

### Dirichlet Green function between parallel planes

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For a three-dimensional slab $0<x_1<L$ and source $y=(y_1,y_2,y_3)$, define image positions $y_n^+=(y_1+2nL,y_2,y_3)$ and $y_n^-=(-y_1+2nL,y_2,y_3)$. The displayed [method of images](mathematics.md#method-of-images) series uses convention $\Delta_xG_D=+\delta(x-y)$. Reflection in $x_1=0$ pairs the plus image $n$ with the minus image $-n$, while reflection in $x_1=L$ pairs it with the minus image $1-n$. Both boundary values therefore vanish. Only $y_0^+=y$ lies in the slab. Each bracket is $O(n^{-2})$, giving absolute convergence of the paired series away from sources. This selects the usual [Dirichlet Green function](#dirichlet-green-function) that decays at large transverse separation.

### Dirichlet Green function inside a sphere

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For the three-dimensional ball $|x|<a$, the displayed [Dirichlet Green function](#dirichlet-green-function) has convention $\Delta_xG_D=+\delta(x-y)$. Its [method of images](mathematics.md#method-of-images) uses the exterior inverse point $y^*=a^2y/|y|^2$. On $|x|=a$, the distance identity $|x-y^*|=(a/|y|)|x-y|$ makes the boundary value zero. The image lies outside the ball and therefore adds no source singularity to the domain. At a central source the weighted image term tends to $1/a$, giving $G_D(x,0)=-(4\pi|x|)^{-1}+(4\pi a)^{-1}$. Spherical inversion with the required radial weight is the [Kelvin transform](partial-differential-equation.md#kelvin-transform).

#### Dirichlet Green function inside a hemisphere

↑ **Parent:** [Dirichlet Green function inside a sphere](#dirichlet-green-function-inside-a-sphere)

For the upper half of a three-dimensional ball, let $\overline y$ be the reflection of an interior source $y$ in the equatorial plane. The [Dirichlet Green function inside a sphere](#dirichlet-green-function-inside-a-sphere), evaluated at the source and its reflection and then subtracted, vanishes on both the spherical cap and flat equatorial disc. Reflection makes the source distances and image distances agree on the plane. Only the original source is in the upper half-ball; the reflected source is in the lower half-ball, and both inversion images are outside the ball. Thus the difference has precisely the required [Dirac delta distribution](distribution-theory.md#dirac-delta-function) and [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition).

### Bounded exterior disk Green function

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For the exterior of the unit disc in two dimensions, with the sign convention $\Delta_xG=+\delta(x-y)$, this is the [Dirichlet Green function](#dirichlet-green-function) that vanishes on the circle and is bounded at infinity. The [method of images](mathematics.md#method-of-images) places an opposite logarithmic source at the inverse point $y/|y|^2$. The constant $-(2\pi)^{-1}\log|y|$ enforces the zero boundary value. The [inversion in a circle](group-theory.md#inversion-in-a-circle) identity $|x-y|=|y|\,|x-y/|y|^2|$ for $|x|=1$ verifies that condition directly.

The outward normal of the exterior domain is $-x$ on the unit circle. Its [normal derivative](differential-geometry.md#normal-derivative) gives the positive exterior [Poisson kernel](partial-differential-equation.md#poisson-kernel)

$$
\partial_nG(x,y)=\frac{|y|^2-1}{2\pi|x-y|^2},\qquad |x|=1<|y|.
$$

For bounded [harmonic functions](partial-differential-equation.md#harmonic-function) this kernel integrates boundary data to the interior value. Boundedness at infinity is essential to uniqueness: without it, a multiple of $\log|y|$ can be added without changing the circle's [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition).

### Dirichlet Green function for a radial power operator on an interval

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

Let $0<a<b$ and impose zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) at $a,b$. With the convention $L_xG(x,s)=\delta(x-s)$ for the [Dirac delta distribution](distribution-theory.md#dirac-delta-function), the [Green's function](green-s-function.md) is continuous and its first [derivative](calculus.md#derivative) has jump one. For $n\ne0$ choose $\ell(x)=x^{-n}-a^{-n}$ and $r(x)=x^{-n}-b^{-n}$. Their [Wronskian](linear-ordinary-differential-equation.md#wronskian) is $n(a^{-n}-b^{-n})s^{-n-1}$, so

$$
G(x,s)=\frac{s^{n+1}(x_<^{-n}-a^{-n})(x_>^{-n}-b^{-n})}{n(a^{-n}-b^{-n})},\qquad x_<=\min(x,s),\quad x_>=\max(x,s).
$$

For $n=0$, take the continuous limit or use $\ell=\log(x/a)$ and $r=\log(x/b)$ to obtain

$$
G(x,s)=\frac{s\log(x_</a)\log(x_>/b)}{\log(b/a)}.
$$

The solution is $u(x)=\int_a^bG(x,s)f(s)\,ds$. These kernels use ordinary measure $ds$. The factor $s^{n+1}$ comes from the nonconstant [Wronskian](linear-ordinary-differential-equation.md#wronskian) and must not be discarded by confusing the original operator with its multiplied [divergence form](analysis.md#divergence-form) $(x^{n+1}u')'$.

### Dirichlet Helmholtz Green function on an interval

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For $\partial_x^2+k^2$ on $(0,\ell)$ with zero endpoint values and $\sin(k\ell)\ne0$, let $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. The displayed [Green function](green-s-function.md) is continuous at $x=\xi$ and its first derivative has jump one, giving unit [Dirac delta](distribution-theory.md#dirac-delta-function) forcing. The formula follows from the left solution $\sin(kx)$ and right solution $\sin(k(\ell-x))$, whose [Wronskian](linear-ordinary-differential-equation.md#wronskian) is $-k\sin(k\ell)$. At $k=0$ its limit is $-x_<(\ell-x_>)/\ell$, although zero is excluded by a condition that $k$ is not an integer in the length-$\pi$ version.

### Green function of killed planar Brownian motion

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

The density of expected [Brownian occupation time](brownian-motion.md#brownian-occupation-time) before exit from a planar domain. For [planar Brownian motion](brownian-motion.md#planar-brownian-motion) with [infinitesimal generator](stochastic-process.md#infinitesimal-generator-stochastic-processes) $\tfrac12\Delta$, it obeys $-\tfrac12\Delta_wG_D(z,w)=\delta_z(w)$ and has singularity $-\pi^{-1}\log|w-z|$. A [conformal bijection](riemann-surfaces.md#biholomorphism) preserves this [Dirichlet Green function](#dirichlet-green-function): the squared derivative in the [conformal Brownian clock](brownian-motion.md#conformal-brownian-clock) cancels the area [Jacobian determinant](multivariable-calculus.md#jacobian-determinant).

### Dirichlet Green function in a quadrant

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For the positive Laplacian convention $\Delta G=\delta$, the [method of images](mathematics.md#method-of-images) in the first quadrant reflects an interior pole $(a,b)$ across each axis with negative sign and across both with positive sign:

$$
G_Q(x,y;a,b)=\frac1{2\pi}\left[\log|(x,y)-(a,b)|-\log|(x,y)-(-a,b)|-\log|(x,y)-(a,-b)|+\log|(x,y)-(-a,-b)|\right].
$$

The [Dirichlet Green function](#dirichlet-green-function) vanishes on both axes. Its outward normal derivative on the horizontal axis is

$$
\partial_nG_Q(t,0;a,b)=\frac{4abt}{\pi[(t-a)^2+b^2][(t+a)^2+b^2]},
$$

and the vertical-axis kernel follows by exchange of coordinates. [Green second identity](partial-differential-equation.md#green-second-identity) converts these derivatives into the quadrant [Poisson integral](partial-differential-equation.md#poisson-integral) for boundary data.

### Regular part of the planar Dirichlet Green function

↑ **Parent:** [Dirichlet Green function](#dirichlet-green-function)

For the canonical [Dirichlet Green function](#dirichlet-green-function) with logarithmic singularity, its harmonic correction satisfies $G_z(z)=-\log\operatorname{crad}_D(z)$. If $\phi$ maps the unit disc to $D$ with $\phi(0)=z$, then

$$
G_z(\phi(w))=-\log\left|\frac{\phi(w)-\phi(0)}w\right|.
$$

The quotient extends at zero to $\phi'(0)$. On unbounded domains the canonical Green function, rather than boundary values alone, fixes the harmonic correction.

## Green-function representation

↑ **Parent:** [Green's function](green-s-function.md)

If $G(x;\xi)$ satisfies the boundary conditions and $L_xG(x;\xi)=\delta(x-\xi)$, then a solution of $Ly=f$ is

$$
y(x)=\int G(x;\xi)f(\xi)\,d\xi,
$$

up to any homogeneous contribution required by nonhomogeneous boundary data.

## One-dimensional modified Helmholtz Green function

↑ **Parent:** [Green's function](green-s-function.md)

For $\operatorname{Re}m>0$, the decaying solution of

$$
-G''+m^2G=\delta_0
$$

is

$$
G(x)=\frac{e^{-m|x|}}{2m}.
$$

It is continuous at zero and has derivative jump $G'(0+)-G'(0-)=-1$.

### Dirichlet modified Helmholtz Green function on an interval

↑ **Parent:** [One-dimensional modified Helmholtz Green function](#one-dimensional-modified-helmholtz-green-function)

For $\kappa>0$, the [Green function](green-s-function.md) of $D_x^2-\kappa^2$ on $(0,L)$ with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) is the displayed negative kernel. Here $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. The left and right homogeneous solutions are $\sinh(\kappa x)$ and $\sinh(\kappa(L-x))$, with [Wronskian](linear-ordinary-differential-equation.md#wronskian) $-\kappa\sinh(\kappa L)$. The kernel is continuous and its first [derivative](calculus.md#derivative) jumps by $+1$, giving $(D_x^2-\kappa^2)G=\delta(x-\xi)$. Reversing the operator sign reverses the kernel sign.

### Dirichlet half-line Green function for minus d2 plus 1

↑ **Parent:** [One-dimensional modified Helmholtz Green function](#one-dimensional-modified-helmholtz-green-function)

On the positive half-line, the [Green function](green-s-function.md) for $-d^2/dx^2+1$ with a zero [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) at the origin and decay at infinity is

$$
G(x,\xi)=\sinh(\min(x,\xi))e^{-\max(x,\xi)}=\frac12\left(e^{-|x-\xi|}-e^{-(x+\xi)}\right).
$$

It is continuous, has [derivative](calculus.md#derivative) jump $G_x(\xi+,\xi)-G_x(\xi-,\xi)=-1$, and is nonnegative. It is the negative of the [Dirichlet half-line Green function for d2 minus 1](#dirichlet-half-line-green-function-for-d2-minus-1); the sign of the leading differential term matters.

#### Dirichlet half-line response to uniform interval forcing

↑ **Parent:** [Dirichlet half-line Green function for minus d2 plus 1](#dirichlet-half-line-green-function-for-minus-d2-plus-1)

For $\mu>0$, the decaying solution of $-y''+y=\mathbf1_{[0,\mu]}$ on the positive half-line with $y(0)=0$ follows by integrating the [Dirichlet half-line Green function for minus d2 plus 1](#dirichlet-half-line-green-function-for-minus-d2-plus-1):

$$
y(x)=\begin{cases}1-e^{-x}-e^{-\mu}\sinh x,&0\leq x\leq\mu,\\(\cosh\mu-1)e^{-x},&x\geq\mu.\end{cases}
$$

Both $y$ and $y'$ are continuous at $\mu$, whereas $y''$ has the jump required by the bounded step in the forcing. Its common value there is $(1-e^{-\mu})^2/2$.

### Fourier decay from a Green-function derivative jump

↑ **Parent:** [One-dimensional modified Helmholtz Green function](#one-dimensional-modified-helmholtz-green-function)

If $H$ is continuous, piecewise twice differentiable, and has derivative jump $[H']=H'(y+)-H'(y-)$ at $y$, then its distributional second [derivative](calculus.md#derivative) is $H''_{\mathrm{reg}}+[H']\delta_y$. If the regular part is integrable and the boundary terms vanish, two [integrations by parts](calculus.md#integration-by-parts) give the displayed [asymptotic expansion](asymptotic-expansion.md) by the [Riemann-Lebesgue lemma](fourier-analysis.md#riemann-lebesgue-lemma). A jump $[H]$ in $H$ itself instead produces $[H]e^{-iqy}/(iq)$ at leading order. This distinguishes the different decay rates of the [streamfunction](fluid-mechanics.md#stream-function) and streamwise [velocity](classical-mechanics.md#velocity) in [linear inviscid damping in unbounded Couette flow](hydrodynamic-stability.md#linear-inviscid-damping-in-unbounded-couette-flow).

### Dirichlet half-line Green function for d2 minus 1

↑ **Parent:** [One-dimensional modified Helmholtz Green function](#one-dimensional-modified-helmholtz-green-function)

For $x,\xi>0$, the [Green function](green-s-function.md) satisfying

$$
(\partial_x^2-1)G(x;\xi)=\delta(x-\xi),\qquad
G(0;\xi)=0,\qquad G(x;\xi)\to0
$$

as $x\to\infty$ is

$$
G(x;\xi)=-\sinh(\min\{x,\xi\})e^{-\max\{x,\xi\}}.
$$

## Dirichlet Green function for an infinite strip

↑ **Parent:** [Green's function](green-s-function.md)

On $\mathbb R\times(0,a)$, separation into sine modes gives the Dirichlet Green function for the Laplacian

$$
G(x,y;b,c)=-\frac1\pi\sum_{n=1}^\infty
\frac{e^{-n\pi|x-b|/a}}n
\sin\frac{n\pi y}{a}\sin\frac{n\pi c}{a}.
$$

## Neumann Green function for a second-order ordinary differential equation

↑ **Parent:** [Green's function](green-s-function.md)

Let $y_1,y_2$ solve $y''+\alpha y'+\beta y=0$ with $y_1'(0)=0$ and $y_2'(1)=0$. For Neumann boundary conditions, the Green function is

$$
G(x,\xi)=\frac1{W(\xi)}
\begin{cases}
y_1(x)y_2(\xi),&x<\xi,\\
y_2(x)y_1(\xi),&x>\xi,
\end{cases}
$$

where $W=y_1y_2'-y_1'y_2$. The derivative jump is one. If $\alpha=0$, the Abel identity makes $W$ constant and $G$ symmetric.

### Neumann Green function for the modified Helmholtz equation on an interval

↑ **Parent:** [Neumann Green function for a second-order ordinary differential equation](#neumann-green-function-for-a-second-order-ordinary-differential-equation)

For real $\kappa\ne0$, this [Green function](green-s-function.md) inverts $d^2/dx^2-\kappa^2$ on $[0,1]$ with homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). It is continuous and its first [derivative](calculus.md#derivative) has jump one at $x=\xi$. At $\kappa=0$, a Green function with the same unit [Dirac delta](distribution-theory.md#dirac-delta-function) source and zero boundary derivatives does not exist: integrating its defining equation would give zero equal to one. The equation $y''=f$ with these boundary conditions instead requires $\int_0^1f(x)\,dx=0$ and determines $y$ only up to a constant.

## Causal Green function

↑ **Parent:** [Green's function](green-s-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Causal_Green_function)

A causal Green function vanishes before the source time and has the derivative jump required by a delta source.

### Causality versus stability of a Green function

↑ **Parent:** [Causal Green function](#causal-green-function)

With inverse [Fourier transform](fourier-transform.md) $G(t)=\int G(\omega)e^{-i\omega t}d\omega/(2\pi)$, a tempered retarded response vanishes for $t<0$ and is analytic in the upper frequency half-plane with suitable large-frequency growth bounds. Poles strictly below the real axis describe decaying modes; upper-half-plane poles obstruct a bounded retarded real-axis Fourier response. However causality alone does not imply stability: a retarded exponentially growing Green function can exist without an ordinary Fourier transform. Its [Laplace transform](integral-transform.md#laplace-transform) inversion contour must pass above the growth poles in the frequency plane. Moving the contour to the real axis changes the boundary condition and can introduce a pre-response.

### Jump conditions for a third-order Green function

↑ **Parent:** [Causal Green function](#causal-green-function)

For $\mathcal L=D^3+a_2D^2+a_1D+a_0$ with smooth coefficients and leading coefficient one, a [Green function](green-s-function.md) solving $\mathcal L G=\delta_\xi$ is continuous together with its first derivative at an interior source, and its second derivative jumps by one. Distributional differentiation shows why: a jump in $G$ would create a delta second derivative, a jump in $G'$ a delta first derivative, and a jump in $G''$ the required delta. For a causal initial-value Green function, take the left branch zero and choose the right branch with initial values $0,0,1$ at the source.

## One-dimensional outgoing Green function

↑ **Parent:** [Green's function](green-s-function.md)

For positive $k$, $e^{ik|x-x'|}$ is outgoing on both sides of $x'$ and obeys

$$
\left(\frac{d^2}{dx^2}+k^2\right)e^{ik|x-x'|}=2ik\delta(x-x').
$$

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (38)

- [Boundary-decaying Green kernel for an inverse-square differential operator](#boundary-decaying-green-kernel-for-an-inverse-square-differential-operator)
- [Bounded Green kernel for a radial Euler operator](#bounded-green-kernel-for-a-radial-euler-operator)
- [Dirichlet Green function for a radial power operator on an interval](#dirichlet-green-function-for-a-radial-power-operator-on-an-interval)
- [Green kernels for a radial dipole Euler equation](#green-kernels-for-a-radial-dipole-euler-equation)
- [Matter-era forced radiation response](linear-cosmological-perturbation-theory.md#matter-era-forced-radiation-response)
- [Normal-mode response to a step seismic moment](wave-equation.md#normal-mode-response-to-a-step-seismic-moment)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#11h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-48.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-67.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#8/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#8/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1.md#8/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#5/d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#10/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#3/c/solution)
- [Quasiparticle residue](fermi-liquid.md#quasiparticle-residue)
- [Static Yukawa Green function](nuclear-force.md#static-yukawa-green-function)
- [Yukawa meson theory of nuclear forces](nuclear-force.md#yukawa-meson-theory-of-nuclear-forces)
