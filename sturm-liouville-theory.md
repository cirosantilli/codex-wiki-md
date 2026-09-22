# Sturm-Liouville theory

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sturm-Liouville_theory)

**Table of contents**

- [Sturm-Liouville equation](#sturm-liouville-equation)
- [Sturm oscillation theorem](#sturm-oscillation-theorem)
- [Drift-removing substitution for a Dirichlet Sturm-Liouville problem](#drift-removing-substitution-for-a-dirichlet-sturm-liouville-problem)
- [Orthogonality of Sturm-Liouville eigenfunctions](#orthogonality-of-sturm-liouville-eigenfunctions)
  - [Derivative orthogonality when the Sturm-Liouville potential vanishes](#derivative-orthogonality-when-the-sturm-liouville-potential-vanishes)
- [Gegenbauer polynomial](#gegenbauer-polynomial)
  - [Gegenbauer differential equation](#gegenbauer-differential-equation)
  - [Roots of a Gegenbauer polynomial](#roots-of-a-gegenbauer-polynomial)
- [Sturm-Liouville form](#sturm-liouville-form)
  - [Sturm-Liouville operator](#sturm-liouville-operator)
    - [Cubic-coordinate reduction of a singular Sturm-Liouville operator](#cubic-coordinate-reduction-of-a-singular-sturm-liouville-operator)
    - [Flux-domain realization of a one-dimensional elliptic operator](#flux-domain-realization-of-a-one-dimensional-elliptic-operator)
    - [Lagrange identity for a Sturm-Liouville operator](#lagrange-identity-for-a-sturm-liouville-operator)
- [Sturm-Liouville problem](#sturm-liouville-problem)
  - [Exponential ground state of a linearly weighted Sturm-Liouville problem](#exponential-ground-state-of-a-linearly-weighted-sturm-liouville-problem)
  - [No-log boundary condition at a linearly vanishing Sturm-Liouville endpoint](#no-log-boundary-condition-at-a-linearly-vanishing-sturm-liouville-endpoint)
  - [Dirichlet-Robin eigenvalues on a finite interval](#dirichlet-robin-eigenvalues-on-a-finite-interval)
  - [Radial Dirichlet spectrum in three dimensions](#radial-dirichlet-spectrum-in-three-dimensions)
  - [Inverse-square weighted Dirichlet spectrum](#inverse-square-weighted-dirichlet-spectrum)
  - [Dirichlet eigenvalue](#dirichlet-eigenvalue)
    - [First Dirichlet eigenvalue](#first-dirichlet-eigenvalue)
  - [Sturm-Liouville eigenfunction expansion](#sturm-liouville-eigenfunction-expansion)
    - [Nonpositive modes in a Dirichlet-Robin interval expansion](#nonpositive-modes-in-a-dirichlet-robin-interval-expansion)
    - [Spectral Green function of a regular Sturm-Liouville problem](#spectral-green-function-of-a-regular-sturm-liouville-problem)
      - [Normalized Sturm-Liouville spectral Green kernel](#normalized-sturm-liouville-spectral-green-kernel)
      - [Odd reciprocal-square sum from a Dirichlet Green function](#odd-reciprocal-square-sum-from-a-dirichlet-green-function)
- [Self-adjoint differential operator](#self-adjoint-differential-operator)
  - [Self-adjoint fourth-order scalar differential operator](#self-adjoint-fourth-order-scalar-differential-operator)
  - [Self-adjoint differential equation](#self-adjoint-differential-equation)
  - [Solvability condition at a Sturm-Liouville eigenvalue](#solvability-condition-at-a-sturm-liouville-eigenvalue)
    - [Fredholm solvability condition](#fredholm-solvability-condition)
      - [Translation-mode solvability for a bistable front](#translation-mode-solvability-for-a-bistable-front)
        - [Moving-defect locking of a cubic-quintic front](#moving-defect-locking-of-a-cubic-quintic-front)
    - [Leading nonlinear eigenvalue shift in a Sturm-Liouville problem](#leading-nonlinear-eigenvalue-shift-in-a-sturm-liouville-problem)

## Sturm-Liouville equation

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)

A second-order differential equation in the displayed divergence form. Under the usual regular spectral assumptions, $p>0$, $w>0$, the coefficients have suitable regularity, and separated self-adjoint boundary conditions specify a [Sturm-Liouville problem](#sturm-liouville-problem). Multiplying by $y$ and using zero endpoint values gives the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) $\lambda=\int(py'^2+qy^2)dx/\int wy^2dx$ for a nonzero real [eigenfunction](linear-operator-theory.md#eigenfunction). Sign conventions for the potential and eigenvalue vary; they must be read from the stated equation.

## Sturm oscillation theorem

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)

For a real one-dimensional [Sturm-Liouville problem](#sturm-liouville-problem) with separated self-adjoint boundary conditions and discrete simple spectrum, the eigenfunction for the $n$th eigenvalue has exactly $n$ interior zeros, numbering from zero. For a confining real [Schrödinger operator](mathematical-physics.md#schrodinger-operator) on the line, the same ordering makes the ground state nodeless and the first excited state have one node. If the potential is even, uniqueness and reflection symmetry imply that these states are respectively even and odd.

## Drift-removing substitution for a Dirichlet Sturm-Liouville problem

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)

For $\mathcal Ly=-y''-2ay'$, setting $y=e^{-ax}v$ gives $\mathcal Ly=e^{-ax}(-v''+a^2v)$. Dirichlet conditions are unchanged. The weighted self-adjoint form is $-e^{-2ax}(e^{2ax}y')'$, with weight $e^{2ax}$. On an interval of length $L$, [eigenvalues](linear-operator-theory.md#eigenvalue) are $(n\pi/L)^2+a^2$ and [eigenfunctions](linear-operator-theory.md#eigenfunction) are $e^{-ax}\sin(n\pi x/L)$.

## Orthogonality of Sturm-Liouville eigenfunctions

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)

For a regular [self-adjoint](linear-operator-theory.md#self-adjoint-operator) [Sturm-Liouville problem](#sturm-liouville-problem) with positive weight $w$ and self-adjoint boundary conditions, [eigenfunctions](linear-operator-theory.md#eigenfunction) with distinct [eigenvalues](linear-operator-theory.md#eigenvalue) are [orthogonal](inner-product.md#orthogonal-vectors) in the weighted [inner product](inner-product.md) $\int w\overline uv$. [Integration by parts](calculus.md#integration-by-parts) proves this by equating $\int\overline u Lv$ and $\int\overline{Lu}v$.

### Derivative orthogonality when the Sturm-Liouville potential vanishes

↑ **Parent:** [Orthogonality of Sturm-Liouville eigenfunctions](#orthogonality-of-sturm-liouville-eigenfunctions)

For the [Sturm-Liouville problem](#sturm-liouville-problem) $-(py_n')'=\lambda_nwy_n$, assume that the boundary term $[py_n'y_m]_a^b$ vanishes. One [integration by parts](calculus.md#integration-by-parts) gives the displayed identity. Distinct [eigenvalues](linear-operator-theory.md#eigenvalue) make the right side zero by [orthogonality of Sturm-Liouville eigenfunctions](#orthogonality-of-sturm-liouville-eigenfunctions), so the derivatives are orthogonal with weight $p$, while the original functions are orthogonal with weight $w$. This conclusion uses the absence of the $qy$ term: for a general potential the extra integral $-\int qy_ny_m$ need not vanish. For the [Chebyshev polynomial of the second kind](numerical-analysis.md#chebyshev-polynomial-of-the-second-kind) of degree $n-1$, the two weights are $w=\sqrt{1-x^2}$ and $p=(1-x^2)^{3/2}$.

## Gegenbauer polynomial

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gegenbauer_polynomial)

For $\alpha>0$, the Gegenbauer polynomial $C_n^\alpha$ is the degree-$n$ polynomial solution of

$$
(1-x^2)y''-(2\alpha+1)xy'+n(n+2\alpha)y=0.
$$

These polynomials are orthogonal on $(-1,1)$ with weight $(1-x^2)^{\alpha-1/2}$.

### Gegenbauer differential equation

↑ **Parent:** [Gegenbauer polynomial](#gegenbauer-polynomial)

The Gegenbauer differential equation is the displayed Sturm–Liouville eigenvalue equation defining the [Gegenbauer polynomial](#gegenbauer-polynomial). Multiplication by $(1-x^2)^{\alpha-1/2}$ puts it in self-adjoint form.

### Roots of a Gegenbauer polynomial

↑ **Parent:** [Gegenbauer polynomial](#gegenbauer-polynomial)

For $\alpha>0$, all $n$ roots of $C_n^\alpha$ are simple and lie in $(-1,1)$. If the product $q$ of its interior linear factors had degree below $n$, orthogonality would make $\int C_n^\alpha q w=0$, while $C_n^\alpha q=q^2(C_n^\alpha/q)$ has a constant strict sign away from finitely many points.

## Sturm-Liouville form

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)

A scalar second-order differential operator is in Sturm–Liouville form when it is written as

$$
Lu=-(p(x)u')'+q(x)u,
$$

possibly together with a positive weight in an eigenvalue problem.

### Sturm-Liouville operator

↑ **Parent:** [Sturm-Liouville form](#sturm-liouville-form)

The weighted operator $L=W^{-1}[-(P\xi\prime)\prime+Q\xi]$, with real coefficients and $P,W>0$ in the interior, defines a [Sturm-Liouville problem](#sturm-liouville-problem). Its realization as a [self-adjoint differential operator](#self-adjoint-differential-operator) requires a domain whose endpoint conditions annihilate the boundary form $[P(\eta\prime^*\xi-\eta^*\xi\prime)]$. Its [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) uses the weight $W$ in the denominator.

#### Cubic-coordinate reduction of a singular Sturm-Liouville operator

↑ **Parent:** [Sturm-Liouville operator](#sturm-liouville-operator)

For $0<x<1$ and zero endpoint values, write $L=w^{-1}[-(p y')'+qy]$ with $p=x^{-2}$, $w=x^2$ and $q=-ax^2$. The change of variable $z=x^3/3$ has $dz=x^2dx$ and sends $y'=x^2Y_z$, $y''=2xY_z+x^4Y_{zz}$. Thus it is an isometry from the [weighted inner product](inner-product.md#weighted-inner-product) to the ordinary integral on $0<z<1/3$, and the apparent singular operator becomes $-Y_{zz}-aY$. Its [Dirichlet eigenvalues](#dirichlet-eigenvalue) are $9n^2\pi^2-a$ and its normalized [eigenfunctions](linear-operator-theory.md#eigenfunction) are $\sqrt6\sin(n\pi x^3)$, $n\geq1$. The singular endpoint is handled through this transformed regular domain; a zero eigenvalue occurs exactly when $a=9n^2\pi^2$.

#### Flux-domain realization of a one-dimensional elliptic operator

↑ **Parent:** [Sturm-Liouville operator](#sturm-liouville-operator)

For continuous $p>0$ and bounded real $q$, the form $a(u,v)=\int(pu'v'+quv)$ on the [zero-trace Sobolev space](sobolev-space.md#zero-trace-sobolev-space) defines the weak operator $L=-(pu')'+qu$. Its literal $L^2$ operator domain is the displayed flux domain. If a weak solution has right-hand side $f\in L^2$, then $(pu')'=qu-f\in L^2$, so it belongs to that domain. This avoids assuming that a merely differentiable coefficient has bounded derivative. With $p\in C^1$ bounded away from zero, the domain reduces to $H^2\cap H_0^1$.

#### Lagrange identity for a Sturm-Liouville operator

↑ **Parent:** [Sturm-Liouville operator](#sturm-liouville-operator)

For $L(v)=(pv')'+av$, direct differentiation gives $uL(v)-vL(u)=[p(uv'-vu')]'$. The potential terms cancel. Integrating with common homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) eliminates the endpoint term. If $L(u)=0$ and $L(v)=f$, this gives $\int uf=0$, a necessary [solvability condition](linear-operator-theory.md#solvability-condition) for the inhomogeneous equation.

## Sturm-Liouville problem

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)

A regular Sturm-Liouville eigenvalue problem has the form

$$
+(p y')'+q y=-\lambda w y
$$

on a bounded interval with self-adjoint boundary conditions and positive weight $w$.

### Exponential ground state of a linearly weighted Sturm-Liouville problem

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

For $\omega>0$ on $x>0$, use the regular finite branch at zero, decay at infinity, and a finite quadratic-form energy. For trial functions with $[xy^2]_0^\infty=0$, [integration by parts](calculus.md#integration-by-parts) gives

$$
\int_0^\infty x(y'^2+\omega^2y^2)dx=\omega\int_0^\infty y^2dx+\int_0^\infty x(y'+\omega y)^2dx.
$$

The [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is at least $\omega$, with equality exactly for a nonzero multiple of $e^{-\omega x}$. Direct substitution verifies that this is an [eigenfunction](linear-operator-theory.md#eigenfunction) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\omega$, so the lower bound is attained. The zero coefficient $p(0)=0$ makes this a singular-endpoint [Sturm-Liouville problem](#sturm-liouville-problem); regularity replaces a prescribed zero endpoint value. Continuous piecewise differentiable trials of finite form energy are allowed in the [Rayleigh-Ritz method](finite-element-method.md#rayleigh-ritz-method), even if their derivative has a jump away from the endpoint.

### No-log boundary condition at a linearly vanishing Sturm-Liouville endpoint

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

Suppose $p(x)=c(x-a)+O((x-a)^2)$ with $c>0$, and the other coefficients in $(py')'+(\lambda w-q)y=0$ extend continuously to $a$, with $w(a)>0$. A bounded [eigenfunction](linear-operator-theory.md#eigenfunction) has $(py')'=O(1)$, hence $py'=C+O(x-a)$. A nonzero $C$ would give $y'\sim C/[c(x-a)]$ and an unbounded [logarithmic singularity](analysis.md#logarithmic-singularity). Thus $C=0$, and the regular branch has bounded first [derivative](calculus.md#derivative). The second local branch carries a logarithm. The title condition excludes that branch.

For two regular [eigenfunctions](linear-operator-theory.md#eigenfunction), $p(\overline u v'-\overline{u'}v)\to0$. This removes the singular-end contribution to the [Lagrange identity for a Sturm-Liouville operator](#lagrange-identity-for-a-sturm-liouville-operator). Together with a separated self-adjoint condition at the other endpoint, it selects the regular [self-adjoint differential operator](#self-adjoint-differential-operator) realization. The precise operator domain uses the maximal differential-operator domain and the no-log endpoint condition; boundedness of classical eigenfunctions is its convenient local expression, not a replacement for specifying an operator domain.

### Dirichlet-Robin eigenvalues on a finite interval

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

For $\ell>0$ and $k>0$, the [Sturm-Liouville problem](#sturm-liouville-problem) with one [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) and one [Robin boundary condition](differential-equation.md#robin-boundary-condition) has positive [eigenvalues](linear-operator-theory.md#eigenvalue). Indeed, [integration by parts](calculus.md#integration-by-parts) gives

$$
\lambda\int_0^\ell y^2\,dx=\int_0^\ell(y')^2\,dx+k y(\ell)^2>0
$$

for every nonzero [eigenfunction](linear-operator-theory.md#eigenfunction). Let $z=\ell\sqrt\lambda$ and $\kappa=k\ell$. The [eigenfunctions](linear-operator-theory.md#eigenfunction) are proportional to $\sin(zx/\ell)$, with

$$
\tan z=-\frac z\kappa.
$$

For each $n\geq1$, there is exactly one root $z_n$ in $((n-1/2)\pi,n\pi)$: on that interval $\tan z+z/\kappa$ increases strictly from $-\infty$ to a positive value. There are no other positive roots. The apparent root $z=0$ gives only the zero sine function and is not an [eigenvalue](linear-operator-theory.md#eigenvalue).

For fixed $k,\ell$, write $z_n=(n-1/2)\pi+\varepsilon_n$. The root equation becomes $\kappa\cot\varepsilon_n=(n-1/2)\pi+\varepsilon_n$, hence

$$
\varepsilon_n=\frac{\kappa}{(n-1/2)\pi}+O(n^{-3}),\qquad
\lambda_n=\frac{(n-1/2)^2\pi^2}{\ell^2}+\frac{2k}{\ell}+O(n^{-2}).
$$

An optional unit normalization uses $\int_0^\ell\sin^2(\sqrt{\lambda_n}x)\,dx=\ell/2+k/[2(k^2+\lambda_n)]$. The positive sign of the Robin boundary term matters: reversing it can introduce nonpositive modes, as in [nonpositive modes in a Dirichlet-Robin interval expansion](#nonpositive-modes-in-a-dirichlet-robin-interval-expansion).

### Radial Dirichlet spectrum in three dimensions

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

For the radial [Laplace operator](partial-differential-equation.md#laplace-operator) $L=-r^{-2}(r^2u')'$ on $0<r<R$, require a finite value at the origin and $u(R)=0$. The map $u\mapsto v=ru$ preserves the [norm](normed-vector-space.md#norm) from $L^2((0,R),r^2dr)$ to $L^2(0,R)$ and sends $L$ to $-d^2/dr^2$. The regular endpoint condition becomes $v(0)=0$. The [self-adjoint](linear-operator-theory.md#self-adjoint-operator) realization therefore corresponds to the ordinary [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) for the one-dimensional second [derivative](calculus.md#derivative). Its [eigenvalues](linear-operator-theory.md#eigenvalue) and [eigenfunctions](linear-operator-theory.md#eigenfunction) are displayed above, with $u_n(0)=n\pi/R$ understood by a [limit](calculus.md#limit-of-a-function). Their squared weighted [norm](normed-vector-space.md#norm) is $R/2$. Completeness and [orthogonality](inner-product.md#orthogonal-vectors) follow from the [Fourier sine series](fourier-series.md#fourier-sine-series) on $(0,R)$.

### Inverse-square weighted Dirichlet spectrum

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

For $y''+\lambda x^{-2}y=0$ on $0<a<x<b$ with zero endpoint values, write $t=\log(x/a)$ and $y=\sqrt{x}\,w(t)$. The [Euler-Cauchy equation](linear-ordinary-differential-equation.md#euler-cauchy-equation) becomes $w''+(\lambda-1/4)w=0$. Thus $y_n=\sqrt{x}\sin[n\pi\log(x/a)/\log(b/a)]$ and the exact spectrum is displayed above. Leading [WKB quantization](analysis.md#wkb-quantization-condition) omits the constant $1/4$, while producing the same leading eigenfunction shape after quantization.

### Dirichlet eigenvalue

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

A Dirichlet eigenvalue is an eigenvalue for an eigenfunction constrained to vanish at the endpoints of its interval or on the boundary of its domain.

#### First Dirichlet eigenvalue

↑ **Parent:** [Dirichlet eigenvalue](#dirichlet-eigenvalue)

For a bounded domain $\Omega$, the first Dirichlet eigenvalue of $-\Delta$ has the variational characterization

$$
\lambda_1=\inf_{0\ne u\in H_0^1(\Omega)}
\frac{\int_\Omega|\nabla u|^2}{\int_\Omega|u|^2}.
$$

### Sturm-Liouville eigenfunction expansion

↑ **Parent:** [Sturm-Liouville problem](#sturm-liouville-problem)

For a regular self-adjoint Sturm-Liouville problem, eigenfunctions are orthogonal in the weighted inner product

$$
\langle f,g\rangle_w=\int fgw,
$$

and the coefficient of $y_n$ is $\langle f,y_n\rangle_w/\langle y_n,y_n\rangle_w$.

#### Nonpositive modes in a Dirichlet-Robin interval expansion

↑ **Parent:** [Sturm-Liouville eigenfunction expansion](#sturm-liouville-eigenfunction-expansion)

For $-y''=\lambda y$, positive [eigenvalues](linear-operator-theory.md#eigenvalue) have [eigenfunctions](linear-operator-theory.md#eigenfunction) $\sin(q_nx)$, where $\tan q_n=\alpha q_n$ and $q_n>0$. Their squared [norms](normed-vector-space.md#norm) are $N_n=1/2-\sin(2q_n)/(4q_n)$. A zero [eigenvalue](linear-operator-theory.md#eigenvalue) occurs precisely at $\alpha=1$, with [eigenfunction](linear-operator-theory.md#eigenfunction) $x$. A negative [eigenvalue](linear-operator-theory.md#eigenvalue) occurs precisely at $0<\alpha<1$: it is $-\kappa^2$ with [eigenfunction](linear-operator-theory.md#eigenfunction) $\sinh(\kappa x)$, where $\tanh\kappa=\alpha\kappa$. There is exactly one such $\kappa$, since $\tanh\kappa/\kappa$ decreases strictly from $1$ to $0$. The [integration by parts](calculus.md#integration-by-parts) identity

$$
\langle y,-y''\rangle=\int_0^1|y'|^2dx-\frac{|y(1)|^2}{\alpha}
$$

and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) show positivity for $\alpha>1$ and nonnegativity at equality. The complete expansion of a [square-integrable function](measure-theory.md#square-integrable-function) therefore includes the extra term $3x\int_0^1tf(t)dt$ when $\alpha=1$, or $\sinh(\kappa x)\int_0^1f(t)\sinh(\kappa t)dt/[\sinh(2\kappa)/(4\kappa)-1/2]$ when $\alpha<1$, in addition to $\sum_n[\int_0^1f(t)\sin(q_nt)dt/N_n]\sin(q_nx)$. Omitting that extra mode makes the system incomplete. In particular, $f=x$ at $\alpha=1$ is orthogonal to every positive sine mode and is an immediate counterexample to a sine-only expansion.

#### Spectral Green function of a regular Sturm-Liouville problem

↑ **Parent:** [Sturm-Liouville eigenfunction expansion](#sturm-liouville-eigenfunction-expansion)

Write $\mathcal A y=-(py')'+qy$ and $\mathcal A y_n=\lambda_n r y_n$, where $r$ is the positive weight. Normalize the real [eigenfunctions](linear-operator-theory.md#eigenfunction) using $\int r y_my_n=\delta_{mn}$. For $\mu$ outside the [spectrum](linear-operator-theory.md#spectrum-functional-analysis), applying $\mathcal A-\mu r$ to the displayed [Green function](green-s-function.md) expansion gives $r(x)\sum_n y_n(x)y_n(\xi)=\delta(x-\xi)$ by weighted completeness. This is the kernel with respect to ordinary source integration $d\xi$; using the weighted measure would change its normalization.

##### Normalized Sturm-Liouville spectral Green kernel

↑ **Parent:** [Spectral Green function of a regular Sturm-Liouville problem](#spectral-green-function-of-a-regular-sturm-liouville-problem)

Let $L=w^{-1}[-(d/dx)(p\,d/dx)+q]$ be the regular self-adjoint operator of a [Sturm-Liouville problem](#sturm-liouville-problem), with [eigenfunctions](linear-operator-theory.md#eigenfunction) orthonormal for the [weighted inner product](inner-product.md#weighted-inner-product) $\int w\overline uv$. For $\mu$ outside its [spectrum](linear-operator-theory.md#spectrum-functional-analysis), the displayed kernel satisfies $(L_x-\mu)G_\mu=\delta(x-\xi)$ with an ordinary, unweighted [Dirac delta](distribution-theory.md#dirac-delta-function). Indeed weighted completeness gives $w(\xi)\sum_ny_n(x)y_n(\xi)^*=\delta(x-\xi)$. Thus $u(x)=\int G_\mu(x,\xi)f(\xi)d\xi$ solves $(L-\mu)u=f$. A kernel integrated against $w(\xi)d\xi$ instead omits the prefactor. For real coefficients, the weighted reciprocity relation is $G_\mu(x,\xi)/w(\xi)=G_\mu(\xi,x)/w(x)$ when the spectral parameter is real and outside the spectrum. A zero eigenvalue prevents inversion at $\mu=0$ without a forcing compatibility condition or a projected inverse.

##### Odd reciprocal-square sum from a Dirichlet Green function

↑ **Parent:** [Spectral Green function of a regular Sturm-Liouville problem](#spectral-green-function-of-a-regular-sturm-liouville-problem)

For $L=d^2/dx^2$ on $(0,\pi)$ with zero endpoints, the zero-parameter [Green function](green-s-function.md) is $-x_<(\pi-x_>)/\pi$. Its [eigenfunctions](linear-operator-theory.md#eigenfunction) are $\sqrt{2/\pi}\sin(nx)$ with eigenvalues $-n^2$. At $x=\xi=\pi/2$, the kernel is $-\pi/4$ and its expansion contains precisely the odd reciprocal squares, giving the displayed identity.

## Self-adjoint differential operator

↑ **Parent:** [Sturm-Liouville theory](sturm-liouville-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Self-adjoint_differential_operator)

A differential operator is self-adjoint when integration by parts makes its inner products symmetric on its domain.

### Self-adjoint fourth-order scalar differential operator

↑ **Parent:** [Self-adjoint differential operator](#self-adjoint-differential-operator)

For real coefficient functions, the fourth-order scalar operator

$$
L=D^4+pD^2+qD+r
$$

is formally self-adjoint exactly when $q=p'$. Indeed, $(pD^2)^*=pD^2+2p'D+p''$ and $(qD)^*=-qD-q'$. Under [clamped boundary conditions](differential-equation.md#clamped-boundary-condition), its quadratic form is

$$
\langle y,Ly\rangle=\int\left[(y'')^2-p(y')^2+ry^2\right]dx.
$$

### Self-adjoint differential equation

↑ **Parent:** [Self-adjoint differential operator](#self-adjoint-differential-operator)

A second-order scalar differential equation is in self-adjoint form when it can be written

$$
(p(x)y')'+q(x)y=0.
$$

Multiplication by $y$ and integration by parts then gives an energy identity.

### Solvability condition at a Sturm-Liouville eigenvalue

↑ **Parent:** [Self-adjoint differential operator](#self-adjoint-differential-operator)

If $L(y_0;\lambda_0)=0$ and $y_0,y$ satisfy homogeneous separated boundary conditions, the Lagrange identity gives

$$
\int y_0L(y;\lambda_0)\,dx
=\int yL(y_0;\lambda_0)\,dx=0.
$$

Thus $L(y;\lambda_0)=f$ can be solved only if $f$ is orthogonal to the null mode $y_0$.

#### Fredholm solvability condition

↑ **Parent:** [Solvability condition at a Sturm-Liouville eigenvalue](#solvability-condition-at-a-sturm-liouville-eigenvalue)

At a simple eigenvalue of a self-adjoint linear operator, an inhomogeneous equation is solvable only when its forcing is orthogonal to the null eigenfunction. In weakly nonlinear expansions, this condition determines the amplitude equation.

##### Translation-mode solvability for a bistable front

↑ **Parent:** [Fredholm solvability condition](#fredholm-solvability-condition)

Suppose $u_t=Du_{xx}+f_0(u)+\varepsilon h(u)$ has a balanced stationary front $U_0(z)$, where $z=(x-q)/\sqrt D$ and $U_0''+f_0(U_0)=0$. Take $\dot q/\sqrt D=\varepsilon c_1+\cdots$ and $u=U_0+\varepsilon U_1+\cdots$. At first order, $LU_1=-c_1U_0'-h(U_0)$ with $L=d^2/dz^2+f_0'(U_0)$. Differentiating the front equation proves $LU_0'=0$. Integration by parts against the decaying [translation](geometry-and-topology.md#translation-geometry) mode gives

$$
c_1=-\frac{\int_{-\infty}^\infty U_0'h(U_0)\,dz}{\int_{-\infty}^\infty(U_0')^2\,dz}.
$$

This is the [Fredholm solvability condition](#fredholm-solvability-condition) determining the velocity, derived from the [self-adjoint differential operator](#self-adjoint-differential-operator) rather than assumed. An orthogonality condition or a fixed midpoint removes the freedom to add a multiple of $U_0'$ to $U_1$. For the [bistable cubic reaction-diffusion equation](diffusion-equation.md#bistable-cubic-reaction-diffusion-equation), $h=-aU_0(1-U_0)$ gives $c_1=-\sqrt2a$, and its first-order forcing vanishes pointwise, so the phase-fixed shape correction is zero.

###### Moving-defect locking of a cubic-quintic front

↑ **Parent:** [Translation-mode solvability for a bistable front](#translation-mode-solvability-for-a-bistable-front)

At the [Maxwell balance for a scalar reaction-diffusion front](analysis.md#maxwell-balance-for-a-scalar-reaction-diffusion-front), let $q=3\alpha/4$, $\beta=\sqrt3\alpha/2$, and perturb the linear growth rate by $\varepsilon K\delta(x+cT)$, $T=\varepsilon t$. Projection onto the front's translation mode gives $X_T=-K\operatorname{sech}^2(\beta Z/2)$, where $Z=X+cT+\beta^{-1}\log q$. Hence $Z_T=c-K\operatorname{sech}^2(\beta Z/2)$. Finite locked positions exist for $0<c/K\le1$. For a strict inequality, the root with $KZ<0$ is stable and the other unstable; they meet in a [saddle-node bifurcation](bifurcation-theory.md#saddle-node-bifurcation) at $c=K$. This is a leading-order [solvability condition](linear-operator-theory.md#solvability-condition), not an exact finite-perturbation solution.

#### Leading nonlinear eigenvalue shift in a Sturm-Liouville problem

↑ **Parent:** [Solvability condition at a Sturm-Liouville eigenvalue](#solvability-condition-at-a-sturm-liouville-eigenvalue)

For $L(y;\lambda)=y^{m+1}$ near a normalized simple null mode $y_0$, put $y=\varepsilon y_0+O(\varepsilon^2)$ and $\lambda-\lambda_0=\varepsilon^m\mu$. Orthogonality to $y_0$ yields

$$
\mu=\int y_0^{m+2}\,dx+O(\varepsilon).
$$

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (6)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-42.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3.md#5a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#13a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2.md#3b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#6/a/ii/solution)
- [Sturm-Liouville formulation with Bessel order as eigenvalue](bessel-function.md#sturm-liouville-formulation-with-bessel-order-as-eigenvalue)
