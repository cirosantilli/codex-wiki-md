# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2009/PaperIB_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2009/PaperIB_1.pdf)

**Table of contents**

- [1G](#1g)
  - [1](#1g/1)
    - [Solution](#1g/1/solution)
  - [2](#1g/2)
    - [Solution](#1g/2/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8H](#8h)
  - [Solution](#8h/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
- [11E](#11e)
  - [Solution](#11e/solution)
- [12F](#12f)
  - [i](#12f/i)
    - [Solution](#12f/i/solution)
  - [ii](#12f/ii)
    - [Solution](#12f/ii/solution)
  - [iii](#12f/iii)
    - [Solution](#12f/iii/solution)
- [13D](#13d)
  - [Solution](#13d/solution)
- [14B](#14b)
  - [Solution](#14b/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16A](#16a)
  - [a](#16a/a)
    - [Solution](#16a/a/solution)
  - [b](#16a/b)
    - [Solution](#16a/b/solution)
  - [c](#16a/c)
    - [Solution](#16a/c/solution)
- [17D](#17d)
  - [Solution](#17d/solution)
  - [i](#17d/i)
    - [Solution](#17d/i/solution)
  - [ii](#17d/ii)
    - [Solution](#17d/ii/solution)
  - [iii](#17d/iii)
    - [Solution](#17d/iii/solution)
- [18H](#18h)
  - [Solution](#18h/solution)
- [19H](#19h)
  - [Solution](#19h/solution)

## 1G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1g/1">1</h3>

↑ **Parent:** [1G](#1g)

<h4 id="1g/1/solution">Solution</h4>

↑ **Parent:** [1](#1g/1)

Let $r=\dim\operatorname{im}T$. Since the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) and its [image](../../../set-theory.md#image-of-a-function) agree, the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives $\dim V=r+r$. Thus **$\dim V=2r$ is even**. Every $Tv$ lies in $\ker T$, so $T^2=0$. The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) therefore divides $X^2$. It cannot be $1$, and it cannot be $X$ since $T\ne0$; hence **the minimal [polynomial](../../../polynomial.md) is $X^2$**.

<h3 id="1g/2">2</h3>

↑ **Parent:** [1G](#1g)

<h4 id="1g/2/solution">Solution</h4>

↑ **Parent:** [2](#1g/2)

Choose $0\ne v\in A_3$ and write $v=a_1+a_2$ using the [direct sum of vector spaces](../../../vector-space.md#direct-sum) $V=A_1\oplus A_2$. Neither component is zero: otherwise $v$ would lie in one of the zero intersections $A_3\cap A_1$ or $A_3\cap A_2$. They are [linearly independent](../../../vector-space.md#linear-independence), so $W=\operatorname{span}\{a_1,a_2\}$ is a two-dimensional [vector subspace](../../../vector-space.md#vector-subspace). Uniqueness of the direct-sum decomposition gives $W\cap A_1=\operatorname{span}\{a_1\}$ and $W\cap A_2=\operatorname{span}\{a_2\}$. Also $v\in W\cap A_3$, but $W$ cannot be contained in $A_3$ because $a_1\in A_1\setminus\{0\}$. Hence $W\cap A_3$ is one-dimensional. This constructs the required **[common plane for three pairwise complementary subspaces](../../../vector-space.md#common-plane-for-three-pairwise-complementary-subspaces)**.

## 2G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

An [ideal hyperbolic triangle](../../../geometry-and-topology.md#ideal-triangle) has its three vertices at infinity, with sides given by [geodesics](../../../riemannian-geometry.md#geodesic). In curvature $-1$ its angles are zero and its area is **$\pi$**, using the [hyperbolic triangle area](../../../geometry-and-topology.md#hyperbolic-triangle-area) formula $\pi-(\alpha+\beta+\gamma)$.

To calculate the [area of a hyperbolic disc](../../../geometry-and-topology.md#area-of-a-hyperbolic-disc), use the [Poincare disc model](../../../geometry-and-topology.md#poincare-disk-model) centered at the origin. Hyperbolic radial distance is $\rho=\int_0^R2\,dr/(1-r^2)=2\operatorname{artanh}R$, so its Euclidean radius is $R=\tanh(\rho/2)$. The metric area density is $4r\,dr\,d\theta/(1-r^2)^2$, giving

$$
A(\rho)=2\pi\int_0^R\frac{4r}{(1-r^2)^2}\,dr=4\pi\left(\frac1{1-R^2}-1\right)=\boxed{2\pi(\cosh\rho-1)}.
$$

Every [hyperbolic triangle](../../../geometry-and-topology.md#hyperbolic-triangle), including ones with ideal vertices, has area at most $\pi$. But $A(2)=2\pi(\cosh2-1)>\pi$. A [hyperbolic triangle](../../../geometry-and-topology.md#hyperbolic-triangle) is geodesically convex, so if it contains a complete [hyperbolic circle](../../../geometry-and-topology.md#hyperbolic-circle), it also contains the enclosed [hyperbolic disc](../../../geometry-and-topology.md#hyperbolic-disc), its [geodesic](../../../riemannian-geometry.md#geodesic) convex hull. This would violate the area comparison. Therefore **no hyperbolic triangle contains a complete circle of radius two**.

## 3D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

For a [holomorphic function](../../../complex-analysis.md#holomorphic-function), compute its complex [derivative](../../../calculus.md#derivative) along the real and imaginary directions. The real direction gives $f'=u_x+iv_x$, while division by an imaginary increment gives $f'=v_y-iu_y$. Equating real and imaginary parts proves the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations):

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

For the specified real part, $u_x=-e^{-x}\cos y$ and $u_y=-e^{-x}\sin y$. Integrating $v_y=u_x$ gives $v=-e^{-x}\sin y+C(x)$; the other relation in the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) then forces $C'(x)=0$. Thus the [harmonic conjugate](../../../partial-differential-equation.md#harmonic-conjugate) and the [holomorphic function](../../../complex-analysis.md#holomorphic-function) are

$$
\boxed{v(x,y)=-e^{-x}\sin y+C,\qquad f(z)=e^{-z}+iC,\quad C\in\mathbb R.}
$$

## 4C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

Use $x^\mu=(ct,x,y,z)$ and metric signature $(+,-,-,-)$. Since $d\tau=dt/\gamma$, the [four-velocity](../../../special-relativity.md#four-velocity) and [four-momentum](../../../special-relativity.md#four-momentum) are

$$
U^\mu=\gamma(c,\mathbf v),\qquad p^\mu=M U^\mu=(\gamma Mc,\gamma M\mathbf v)=(E/c,\mathbf p),\qquad \gamma=(1-v^2/c^2)^{-1/2}.
$$

These use the [proper time](../../../special-relativity.md#proper-time) and [Lorentz factor](../../../special-relativity.md#lorentz-factor); the [mass shell](../../../special-relativity.md#mass-shell) identity is $E^2-c^2|\mathbf p|^2=M^2c^4$.

Initially the parent [four-momentum](../../../special-relativity.md#four-momentum) is $(Mc,\mathbf0)$. By [four-momentum conservation](../../../special-relativity.md#four-momentum-conservation), the remaining single particle has energy $Mc^2-E$ and three-momentum $-\mathbf p$. Applying its [mass shell](../../../special-relativity.md#mass-shell) identity gives $m^2c^4=(Mc^2-E)^2-c^2|\mathbf p|^2$, hence

$$
\boxed{m=\sqrt{\left(M-\frac{E}{c^2}\right)^2-\frac{|\mathbf p|^2}{c^2}}.}
$$

The positive root is selected for the rest mass; physically admissible decay data also give nonnegative remaining energy.

## 5D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

The [divergence](../../../calculus.md#divergence) of this axisymmetric [velocity field](../../../fluid-mechanics.md#velocity-field) is $r^{-1}\partial_r(-\alpha r^2)+\partial_z(2\alpha z)=-2\alpha+2\alpha=0$. Thus it satisfies [incompressibility](../../../fluid-mechanics.md#incompressible-flow). The apparent axis singularity in the azimuthal component is removable, since $u_\theta\sim\gamma\beta r$ as $r\to0$.

Only the axial [vorticity](../../../fluid-mechanics.md#vorticity) component is nonzero:

$$
\boxed{\boldsymbol\omega=\nabla\times\mathbf u=(0,0,w(r)),\qquad w(r)=2\beta\gamma e^{-\beta r^2}.}
$$

The [cross product](../../../vector-space.md#cross-product) is $\mathbf u\times\boldsymbol\omega=(u_\theta w,\alpha r w,0)$. Its components are independent of $z$ and $\theta$, so its [curl](../../../calculus.md#curl) also has only an axial component:

$$
\bigl[\nabla\times(\mathbf u\times\boldsymbol\omega)\bigr]_z=\frac1r\frac d{dr}(\alpha r^2w)=\alpha(2w+rw')=2\alpha(1-\beta r^2)w.
$$

Meanwhile $w'=-2\beta rw$ and $w''=(-2\beta+4\beta^2r^2)w$, giving

$$
\nabla^2\boldsymbol\omega=(0,0,w''+w'/r)=(0,0,-4\beta(1-\beta r^2)w).
$$

Thus the required steady [vorticity equation](../../../physics.md#vorticity-equation) holds with **$\nu=\alpha/(2\beta)$**. This is the balance between vortex stretching and viscous diffusion in a [Burgers vortex](../../../continuum-mechanics.md#burgers-vortex).

## 6C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

Subtract the exact solution from the [Jacobi method](../../../numerical-analysis.md#jacobi-method) to get $e_n=He_{n-1}$, hence $e_n=H^ne_0$. Convergence from every initial vector is equivalent to $H^n\to0$. If every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) has modulus below one, a [Jordan block](../../../linear-operator-theory.md#jordan-block) $\lambda I+N$ has powers that are finite sums $\binom nk\lambda^{n-k}N^k$. The [polynomial](../../../polynomial.md) factor in $n$ is dominated by geometric decay; for $\lambda=0$, the block is nilpotent. Consequently $H^n\to0$.

Conversely, for a complex [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$, $H^nv=\lambda^nv$. Convergence for real errors also implies convergence for their complexification, so this tends to zero only if $|\lambda|<1$. Therefore **the iteration converges from every starting vector if and only if $\rho(H)<1$**, where $\rho$ is the [spectral radius](../../../analysis.md#spectral-radius).

For the specified [matrix](../../../vector-space.md#matrix),

$$
H=\begin{pmatrix}0&0&\mu\\\mu/3&0&\mu/3\\\mu&0&0\end{pmatrix},\qquad \det(tI-H)=t(t^2-\mu^2).
$$

Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $0,\mu,-\mu$, so $\rho(H)=|\mu|$. Hence **$-1<\mu<1$** is the convergence range. The original coefficient [matrix](../../../vector-space.md#matrix) has determinant $12(1-\mu^2)$, so the endpoints also violate its assumed nonsingularity.

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

An [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) $\widehat\theta$ satisfies $\mathbb E_\theta\widehat\theta=\theta$ for every parameter value. Under the standard full-column-rank assumption on the [design matrix](../../../linear-regression.md#design-matrix), the Gaussian [log-likelihood](../../../statistical-modelling.md#log-likelihood) for the [normal linear model](../../../statistical-modelling.md#normal-linear-model), up to terms independent of $\beta$, is $-\|Y-X\beta\|^2/(2\sigma^2)$. Its maximum is the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) minimum. Differentiating gives $X^TX\widehat\beta=X^TY$, and full column rank makes $X^TX$ positive definite. Thus

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Since $\mathbb EY=X\beta$, its expectation is $(X^TX)^{-1}X^TX\beta=\beta$, proving **unbiasedness**. Estimating an unknown $\sigma^2$ as well does not change the maximizing coefficient vector.

The printed hypotheses give $p<n$ but do not explicitly require full column rank. Without that condition the [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator) are not unique: they are $X^+Y+z$ with $z\in\ker X$, as in [rank-deficient ordinary least squares](../../../statistical-modelling.md#rank-deficient-ordinary-least-squares). If $0\ne z\in\ker X$, the observation distributions at $\beta$ and $\beta+z$ are identical. Every estimator then has the same expectation at both parameters, so no estimator can be unbiased for both entire coefficient vectors. This proves [nonidentifiability prevents unbiased coefficient estimation](../../../statistical-modelling.md#nonidentifiability-prevents-unbiased-coefficient-estimation). The stated estimator and unbiasedness claim require the usual full-rank condition.

## 8H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8h/solution">Solution</h3>

↑ **Parent:** [8H](#8h)

The point $(x_1,x_2,x_3)=(4,2,2)$ is nonnegative and makes all three inequalities equalities, with objective value $20$. To certify global optimality, combine the first upper bound with coefficient $1/2$, the second with coefficient one, and the lower bound with coefficient $-3/2$:

$$
\begin{aligned}
3x_1+2x_2+2x_3&=\tfrac12(7x_1+3x_2+5x_3)+(x_1+2x_2+x_3)-\tfrac32(x_1+x_2+x_3)\\
&\le\tfrac12\cdot44+10-\tfrac32\cdot8=20.
\end{aligned}
$$

This is a [weak duality](../../../mathematical-optimization.md#weak-duality) certificate for the [linear program](../../../mathematical-optimization.md#linear-programming). The feasible point attains the bound, so **the optimal solution is $(4,2,2)$ and the maximum is $20$**. Equality forces each of the three constraints to be active; their simultaneous equations have this unique solution.

## 9G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

The [dual space](../../../linear-algebra.md#dual-space) is $V^*=\operatorname{Hom}_F(V,F)$, the [vector space](../../../vector-space.md) of all [linear functionals](../../../linear-algebra.md#linear-functional) with pointwise operations. For finite $d=\dim V$, choose a basis $v_1,\ldots,v_d$ and define its [dual basis](../../../linear-algebra.md#dual-basis) by $\varepsilon_j(v_i)=\delta_{ij}$. Every [linear functional](../../../linear-algebra.md#linear-functional) is $\ell=\sum_j\ell(v_j)\varepsilon_j$, and evaluation on each $v_i$ proves that the $\varepsilon_j$ are [linearly independent](../../../vector-space.md#linear-independence). Thus **$\dim V^*=\dim V=d$**. This dimension formula is a finite-dimensional assertion.

On the space of [polynomials](../../../polynomial.md) of degree at most $n$, define the evaluation map $E(p)=(p(a_0),\ldots,p(a_n))$. Its kernel is zero: a nonzero degree-at-most-$n$ [polynomial](../../../polynomial.md) cannot have $n+1$ distinct roots. Since domain and codomain both have dimension $n+1$, $E$ is an [isomorphism](../../../algebra.md#isomorphism). The evaluations therefore form a basis of the [dual space](../../../linear-algebra.md#dual-space). The [linear functional](../../../linear-algebra.md#linear-functional) $p\mapsto p'(0)$ has a unique expansion in that basis, proving the existence and uniqueness of the requested weights.

Explicitly, use the [Lagrange interpolation polynomial](../../../numerical-analysis.md#lagrange-polynomial) basis

$$
\ell_j(x)=\prod_{i\ne j}\frac{x-a_i}{a_j-a_i},\qquad p(x)=\sum_{j=0}^np(a_j)\ell_j(x).
$$

The [differentiation weights from nodal evaluations](../../../numerical-analysis.md#differentiation-weights-from-nodal-evaluations) are **$\lambda_j=\ell_j'(0)$**. If a node is zero, no singular reciprocal formula is needed: differentiate the finite product directly. For $n=0$ the sole weight is zero.

## 10F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

In a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), an ascending chain of [ideals](../../../commutative-algebra.md#ideal) stabilizes: its union is an [ideal](../../../commutative-algebra.md#ideal) $(d)$, and its generator belongs to one member, which then contains the union. This proves the needed [ascending chain condition](../../../algebra.md#ascending-chain-condition). If a nonzero nonunit had no finite irreducible factorization, split it into two nonunits and select a factor that still has no such factorization. Continuing would give a strictly ascending chain of principal [ideals](../../../commutative-algebra.md#ideal), because $a=bc$ with $c$ a nonunit implies $(a)\subsetneq(b)$. This contradicts the chain condition, so factorization exists.

An [irreducible element](../../../commutative-algebra.md#irreducible-element) $p$ generates a [maximal ideal](../../../commutative-algebra.md#maximal-ideal): any intermediate [ideal](../../../commutative-algebra.md#ideal) is $(d)$ with $p=dc$, and irreducibility forces $d$ or $c$ to be a unit. Therefore $p$ is a [prime element](../../../commutative-algebra.md#prime-element). In any two irreducible factorizations, the first prime factor divides a factor of the other, hence is associate to it. Cancel and continue. This proves **every [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) is a [unique factorization domain](../../../algebra.md#unique-factorization-domain)**.

In $\mathbb Z[\sqrt{-3}]$, the multiplicative [field norm](../../../algebraic-number-theory.md#field-norm) is $N(a+b\sqrt{-3})=a^2+3b^2$. The only [units](../../../algebra.md#unit-in-a-ring) are $\pm1$. There is no element of norm two, so every element of norm four is irreducible: a factorization into nonunits would require norms two and two. Consequently

$$
\boxed{4=2\cdot2=(1+\sqrt{-3})(1-\sqrt{-3})}
$$

is a pair of genuinely different irreducible factorizations. Neither $1+\sqrt{-3}$ nor $1-\sqrt{-3}$ is associate to $2$.

Take the [Eisenstein integers](../../../commutative-algebra.md#eisenstein-integer) $R=\mathbb Z[\omega]$, where $\omega=(-1+\sqrt{-3})/2$ and $\omega^2+\omega+1=0$. Since $\sqrt{-3}=1+2\omega$, the embedded subring is $\mathbb Z+2\mathbb Z\omega$, whose additive index in $R$ is two. Its larger ring has [Eisenstein-integer norm](../../../commutative-algebra.md#eisenstein-integer-norm) $N(a+b\omega)=a^2-ab+b^2$ and is Euclidean. Indeed, write a complex quotient in the real basis $1,\omega$ and round both coordinates to integers. The coordinate errors $u,v$ satisfy $|u|,|v|\le1/2$, giving $|u+v\omega|^2=u^2-uv+v^2\le3/4<1$. Thus division leaves a remainder of smaller norm. A [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), because division by a nonzero element of least norm in an ideal leaves zero remainder. This gives the requested **index-two embedding into a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain)**.

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/solution">Solution</h3>

↑ **Parent:** [11E](#11e)

Let $\phi(t)=\operatorname{dist}(t,\mathbb Z)$. It is continuous and takes values in $[0,1/2]$. The finite sums $f_N(x)=\sum_{n=1}^N2^{-n}\phi(2^nx)$ are continuous and their tails obey

$$
|f(x)-f_N(x)|\le\frac12\sum_{n>N}2^{-n}=2^{-N-1}
$$

for every real $x$. To prove continuity without invoking an unproved uniform-limit theorem, fix $x$ and $\varepsilon>0$. Choose $N$ with $2\cdot2^{-N-1}<\varepsilon/2$, then use continuity of $f_N$ to make $|f_N(y)-f_N(x)|<\varepsilon/2$ near $x$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) then gives $|f(y)-f(x)|<\varepsilon$. Thus **$f$ is continuous**; it is the scaled [Takagi function](../../../calculus.md#blancmange-curve) $T(2x)/2$.

For the general secant claim, differentiability gives $g(x+h)=g(x)+g'(x)h+r(h)$, where $|r(h)|\le\varepsilon|h|$ for sufficiently small $h$, with $r(0)=0$. Since the two endpoints straddle $x$,

$$
\left|\frac{g(v_n)-g(u_n)}{v_n-u_n}-g'(x)\right|\le\varepsilon\frac{|v_n-x|+|u_n-x|}{v_n-u_n}=\varepsilon.
$$

Hence **the secant limit is $g'(x)$**, including cases where an endpoint equals $x$. This proves [secants straddling a differentiability point](../../../analysis.md#secants-straddling-a-differentiability-point).

Now take the nested dyadic intervals $u_N=2^{-N}\lfloor2^Nx\rfloor$, $v_N=u_N+2^{-N}$. They straddle $x$ and shrink to it. For every $n\ge N$, $2^nu_N$ and $2^nv_N$ are integers, so the corresponding summand vanishes at both endpoints. For $n<N$, all corners of that summand lie on the dyadic grid of mesh $2^{-N}$; on the chosen open interval it is linear with slope $\varepsilon_n\in\{-1,1\}$. Therefore its total secant slope is

$$
S_N=\frac{f(v_N)-f(u_N)}{v_N-u_N}=\sum_{n=1}^{N-1}\varepsilon_n.
$$

Refining to the nested interval preserves the slopes of all old terms and adds exactly one new term of slope $+1$ or $-1$. Thus $|S_{N+1}-S_N|=1$ for every $N$, so $S_N$ cannot converge. This contradicts the secant consequence of differentiability at any $x$. Therefore **$f$ is nowhere differentiable**. At dyadic $x$ the intervals chosen on its right satisfy the same argument. The printed reference to a denominator $2^{-n}$ is naturally read as mesh $2^{-n}$, or denominator $2^n$, as used here.

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/i">i</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/i/solution">Solution</h4>

↑ **Parent:** [I](#12f/i)

Suppose $(x_n,f(x_n))$ converges to $(x,y)$. [Continuity](../../../calculus.md#continuous-function) gives $f(x_n)\to f(x)$, and uniqueness of limits in a [metric space](../../../topological-analysis.md#metric-space) gives $y=f(x)$. Hence every convergent sequence in the graph has its limit in the graph, proving **$\Gamma_f$ is closed**.

<h3 id="12f/ii">ii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12f/ii)

If $f$ were not continuous at $x$, there would be $\varepsilon>0$ and $x_n\to x$ with $d_Y(f(x_n),f(x))\ge\varepsilon$. A [compact metric space](../../../topological-analysis.md#compact-metric-space) is sequentially compact, so some subsequence $f(x_{n_k})$ converges to $y$. The closed graph then contains its product limit $(x,y)$, forcing $y=f(x)$, contrary to the lower bound. Thus **$f$ is continuous**, the compact-codomain form of the [closed graph theorem for compact spaces](../../../topology.md#closed-graph-theorem-for-compact-spaces).

<h3 id="12f/iii">iii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12f/iii)

Take **$f(0)=0$ and $f(x)=1/x$ for $x\ne0$**. Its graph is $\{(x,y):xy=1\}\cup\{(0,0)\}$, a union of two [closed sets](../../../topology.md#closed-set), since multiplication is continuous. But $f(1/n)=n$ does not tend to $f(0)$, so the function is not continuous.

## 13D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13d/solution">Solution</h3>

↑ **Parent:** [13D](#13d)

Choose the principal [branch of a multivalued function](../../../complex-analysis.md#branch-of-a-multivalued-function), $-\pi<\arg s<\pi$, for $s^{1/2}$. The integrand $G(s)=e^{st}/((s^2+1)\sqrt s)$ has simple poles at $\pm i$ and a [branch cut](../../../analysis.md#branch-cut) along the negative real axis. Its residues are

$$
\operatorname{Res}_{i}G=\frac{e^{it-i\pi/4}}{2i},\qquad \operatorname{Res}_{-i}G=-\frac{e^{-it+i\pi/4}}{2i},
$$

whose sum is $\sin(t-\pi/4)$.

For $t>0$, close the [Bromwich contour](../../../complex-analysis.md#bromwich-contour) to the left using a rectangle with outer real part $-R$ and horizontal edges at imaginary parts $\pm R$, indenting the cut and zero. On every distant edge, $|s^2+1|\ge|s|^2-1$, $|\sqrt s|=|s|^{1/2}$ and $|e^{st}|\le e^{\gamma t}$. Each edge has length $O(R)$ and $|s|\ge R$, so its [integral](../../../calculus.md#integral) is $O(R^{-3/2})$. The small circle of radius $\varepsilon$ about zero contributes $O(\varepsilon^{1/2})$. The tails of the original vertical [integral](../../../calculus.md#integral) are absolutely bounded by $O(R^{-3/2})$ as well.

On the upper and lower banks at $s=-r$, the square roots are $i\sqrt r$ and $-i\sqrt r$, respectively. With the upper bank traversed toward zero and the lower bank away from zero, their combined [integral](../../../calculus.md#integral) is

$$
-2i\int_\varepsilon^R\frac{e^{-rt}}{(r^2+1)\sqrt r}\,dr.
$$

The cut [integral](../../../calculus.md#integral) converges near zero since $r^{-1/2}$ is integrable, and at infinity by exponential decay. The [residue theorem](../../../analysis.md#residue-theorem), followed by $R\to\infty$ and $\varepsilon\to0$, therefore gives

$$
\boxed{f(t)=\sin(t-\pi/4)+\frac1\pi\int_0^\infty\frac{e^{-rt}}{(r^2+1)\sqrt r}\,dr\quad(t>0).}
$$

For $t<0$, close the [Bromwich contour](../../../complex-analysis.md#bromwich-contour) to the right. There are no enclosed poles or cuts, and $|e^{st}|\le e^{\gamma t}$ there. The same distant-edge estimates show **$f(t)=0$ for $t<0$**.

<a id="13d/image-left-closing-bromwich-contour-with-the-principal-square-root-cut-two-pole-residues-and-a-small-indentation-at-zero"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1-bromwich.png)

**[Figure 1](#13d/image-left-closing-bromwich-contour-with-the-principal-square-root-cut-two-pole-residues-and-a-small-indentation-at-zero). Left-closing Bromwich contour with the principal square-root cut, two pole residues, and a small indentation at zero**.

For the large-$t$ expansion, $1/(1+r^2)=1-r^2+r^4/(1+r^2)$. Scaling $r=u/t$ and using the given [integral](../../../calculus.md#integral) yields $\int_0^\infty e^{-rt}r^{-1/2}\,dr=\sqrt\pi\,t^{-1/2}$. Integration by parts twice gives the next coefficient $\Gamma(5/2)=3\sqrt\pi/4$. The remainder is bounded by $\int_0^\infty e^{-rt}r^{7/2}\,dr=\Gamma(9/2)t^{-9/2}$. Thus, without needing a globally convergent termwise integration of the local power series,

$$
f(t)=\sin(t-\pi/4)+\frac1{\sqrt{\pi t}}-\frac3{4\sqrt\pi\,t^{5/2}}+O(t^{-9/2}).
$$

In particular, the requested two leading terms are **$\sin(t-\pi/4)+(\pi t)^{-1/2}$**, interpreted as an additive asymptotic expansion. This is [Bromwich inversion with a square-root branch cut](../../../complex-analysis.md#bromwich-inversion-with-a-square-root-branch-cut).

## 14B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14b/solution">Solution</h3>

↑ **Parent:** [14B](#14b)

Write $y=\sum_{k\ge0}c_kx^k$ with $c_0=1$. Substitution into the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) gives

$$
(k+1)^2c_{k+1}+(\lambda-k)c_k=0,\qquad c_k=\frac{\prod_{j=0}^{k-1}(j-\lambda)}{(k!)^2}.
$$

Unless the series terminates, its coefficient ratio is $O(1/k)$, so it converges for every finite $x$. A coefficient first vanishes exactly when $\lambda$ is a nonnegative integer $n$, and then $c_n=(-1)^n/n!\ne0$, $c_{n+1}=0$. Thus **$y$ is a [polynomial](../../../polynomial.md) precisely for $\lambda=n\in\{0,1,2,\ldots\}$**, in which case

$$
y_n(x)=\sum_{k=0}^n(-1)^k\binom nk\frac{x^k}{k!}
$$

is the normalized [Laguerre polynomial](../../../linear-operator-theory.md#laguerre-polynomial).

Multiplying the differential equation by $e^{-x}$ gives $(xe^{-x}y_n')'+ne^{-x}y_n=0$. Multiply by $y_m$, subtract the equation with the indices exchanged, and integrate over $[0,\infty)$. The boundary term $xe^{-x}(y_my_n'-y_ny_m')$ vanishes both at zero and infinity. Therefore

$$
\boxed{\int_0^\infty e^{-x}y_m(x)y_n(x)\,dx=0\quad(m\ne n).}
$$

This is the weighted [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the [Laguerre polynomials](../../../linear-operator-theory.md#laguerre-polynomial).

Their leading coefficients show $\deg(y_my_n)=m+n$. Since $y_0,\ldots,y_{m+n}$ have distinct degrees, they form a basis of that [polynomial](../../../polynomial.md) space. Hence $y_my_n=\sum_{p=0}^{m+n}a_py_p$, and comparison of leading coefficients gives **$a_{m+n}=(m+n)!/(m!n!)\ne0$**. Likewise the degrees of $y_m$ and $y_my_n$ for $0\le m<n$ run through $0,\ldots,n-1$ and $n,\ldots,2n-1$, respectively. A nontrivial [linear combination](../../../vector-space.md#linear-combination) cannot cancel its highest-degree term, so these $2n$ functions are [linearly independent](../../../vector-space.md#linear-independence).

For $n=2$, this gives the basis $y_0,y_1,y_2,y_1y_2$ of the cubic [polynomial](../../../polynomial.md) space, establishing the specified expansion. Its weighted [integral](../../../calculus.md#integral) is $a_0$: $y_0=1$ integrates to one, $y_1$ and $y_2$ are orthogonal to $y_0$, and $y_1y_2$ integrates to zero. At the two roots $\alpha_1,\alpha_2$ of $y_2$, the expansion reduces to $f(\alpha_i)=a_0+a_1y_1(\alpha_i)$. Solving these two equations for $a_0$ gives

$$
\boxed{\int_0^\infty e^{-x}f(x)\,dx=w_1f(\alpha_1)+w_2f(\alpha_2),\quad w_1=\frac{y_1(\alpha_2)}{y_1(\alpha_2)-y_1(\alpha_1)},\quad w_2=\frac{-y_1(\alpha_1)}{y_1(\alpha_2)-y_1(\alpha_1)}.}
$$

For explicit verification, the recurrence gives $y_1=1-x$, $y_2=1-2x+x^2/2$. Thus $\alpha_1=2-\sqrt2$, $\alpha_2=2+\sqrt2$ are distinct positive roots and $w_1=(2+\sqrt2)/4$, $w_2=(2-\sqrt2)/4$. This is the two-node [Gauss-Laguerre quadrature](../../../numerical-analysis.md#gauss-laguerre-quadrature) rule, exact for every cubic.

## 15B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

The [parity operator](../../../quantum-mechanics.md#parity-operator) acts by $(P\psi)(x)=\psi(-x)$. For an even potential, differentiating twice and using $V(-x)=V(x)$ proves $HP=PH$ on the parity-invariant domain of the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics). Therefore each [energy eigenspace](../../../quantum-mechanics.md#energy-eigenspace) is invariant under $P$. The projectors $(I+P)/2$ and $(I-P)/2$ split it into even and odd subspaces, giving a basis of simultaneous [eigenstates](../../../quantum-mechanics.md#eigenstate). An odd state obeys $\psi(0)=-\psi(0)$, hence **$\psi_{\rm odd}(0)=0$**.

The infinite walls impose **$\psi(-a)=\psi(a)=0$**, with the [wavefunction](../../../quantum-mechanics.md#wave-function) zero outside. It is continuous at the central [delta potential](../../../quantum-mechanics.md#delta-potential). Integrate the stationary [Schrödinger equation](../../../physics.md#schrodinger-equation) over $[-\varepsilon,\varepsilon]$; the energy [integral](../../../calculus.md#integral) tends to zero and the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) contributes $\kappa\psi(0)$. This gives

$$
\boxed{\frac{\hbar^2}{2m}\bigl(\psi'(0+)-\psi'(0-)\bigr)=\kappa\psi(0).}
$$

For the given piecewise positive-energy form, $E=\hbar^2\lambda^2/(2m)$. Replacing $x$ by $-x$ swaps the two pieces and leaves their values unchanged, proving $P\psi=\psi$. The value at zero is $A$, and the one-sided [derivatives](../../../calculus.md#derivative) are $-B\lambda$ and $B\lambda$. The jump condition gives $B=-m\kappa A/(\hbar^2\lambda)$. The wall at $a$ gives $A\cos(\lambda a)-B\sin(\lambda a)=0$, hence

$$
\boxed{\tan(\lambda a)=-\frac{\hbar^2\lambda}{m\kappa}.}
$$

For $\kappa=0$ the undivided wall equation instead gives the usual free even roots. For $\kappa>0$, set $c=m\kappa/\hbar^2>0$ and $k_n=(n+1/2)\pi/a$. In every interval $k_n<\lambda<(n+1)\pi/a$ there is exactly one root: writing $\delta=a(\lambda-k_n)\in(0,\pi/2)$ gives $\cot\delta=\lambda/c$, whose two sides are respectively strictly decreasing and increasing. These are all positive even roots; the quadratic form $\hbar^2\int|\psi'|^2/(2m)+\kappa|\psi(0)|^2$ is nonnegative, so there are no negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Thus $\lambda_n>k_n$ and **$\eta_n=\hbar^2(\lambda_n^2-k_n^2)/(2m)>0$**.

The printed limit of this absolute energy difference is false. The exact quantization equation gives $\delta_n=\arctan(c/\lambda_n)$, so $\delta_n\to0$ but $\lambda_n\delta_n\to c$. Consequently

$$
\lambda_n^2-k_n^2=\frac{2\lambda_n\delta_n}{a}-\frac{\delta_n^2}{a^2}\longrightarrow\frac{2c}{a},\qquad \boxed{\lim_{n\to\infty}\eta_n=\frac{\kappa}{a}.}
$$

Thus the [high-energy shift from a central delta barrier](../../../quantum-mechanics.md#high-energy-shift-from-a-central-delta-barrier) is a finite positive constant, not zero. The corrected vanishing statement is the relative shift $\eta_n/E_n^{(0)}\to0$, or the wave-number difference $\lambda_n-k_n\to0$. Physically, highly energetic particles are weakly affected in relative terms by a fixed point barrier. The free even [wavefunction](../../../quantum-mechanics.md#wave-function) normalized in $[-a,a]$ has density $1/a$ at the origin, so the barrier's first-order expectation is $\kappa/a$, matching the exact limit.

Odd states vanish at zero, so the delta term and the [derivative](../../../calculus.md#derivative) jump both vanish. Their normalized [wavefunctions](../../../quantum-mechanics.md#wave-function) and energies are

$$
\boxed{\psi_j(x)=a^{-1/2}\sin(j\pi x/a)\quad(|x|<a),\qquad E_j^{\rm odd}=\frac{\hbar^2\pi^2j^2}{2ma^2},\quad j=1,2,\ldots,}
$$

with zero [wavefunction](../../../quantum-mechanics.md#wave-function) outside. They do not depend on $\kappa$. These even and odd sectors describe the [central delta barrier in a symmetric infinite well](../../../quantum-mechanics.md#central-delta-barrier-in-a-symmetric-infinite-well).

## 16A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16a/a">a</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/a/solution">Solution</h4>

↑ **Parent:** [A](#16a/a)

In electrostatic equilibrium, the [electric field](../../../electromagnetism.md#electric-field) inside a [perfect conductor](../../../electromagnetism.md#perfect-conductor) is zero. Apply the [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) $\oint\mathbf E\cdot d\mathbf l=0$ to a thin rectangular loop crossing the surface, with its long sides tangential and its short sides shrinking to zero. It yields continuity of the tangential [electric field](../../../electromagnetism.md#electric-field). Since its interior value is zero, **$E_x(0+)=E_y(0+)=0$**. Earthing fixes the [electric potential](../../../electromagnetism.md#electric-potential) at the plane to zero. For completeness, a thin [Gauss law](../../../electromagnetism.md#gauss-s-law) pillbox gives $E_z(0+)=\sigma/\varepsilon_0$; the normal component can be nonzero because of induced surface charge. These are the [electrostatic boundary conditions at a conductor](../../../electromagnetism.md#electrostatic-boundary-conditions-at-a-conductor).

<h3 id="16a/b">b</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/b/solution">Solution</h4>

↑ **Parent:** [B](#16a/b)

The charge and its proposed [image charge](../../../electromagnetism.md#image-charge) give the exterior [electric potential](../../../electromagnetism.md#electric-potential)

$$
\Phi(r,z)=\frac q{4\pi\varepsilon_0}\left(\frac1{\sqrt{r^2+(z-d)^2}}-\frac1{\sqrt{r^2+(z+d)^2}}\right).
$$

At $z=0$ the terms cancel, so $\Phi=0$ everywhere on the plane and its tangential [derivatives](../../../calculus.md#derivative) vanish. Thus **the image construction satisfies the earthed-conductor boundary conditions**. It has the correct point-charge singularity, is harmonic elsewhere in $z>0$, and decays at infinity; electrostatic uniqueness identifies it with the exterior solution.

<h3 id="16a/c">c</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/c/solution">Solution</h4>

↑ **Parent:** [C](#16a/c)

At instantaneous height $z$, the [image charge](../../../electromagnetism.md#image-charge) is a distance $2z$ below the real charge, giving force $m\ddot z=-K/z^2$ with $K=q^2/(16\pi\varepsilon_0)$. Multiplying by $\dot z$ and using rest at $z=d$ gives

$$
\frac m2\dot z^2=K\left(\frac1z-\frac1d\right).
$$

The induced-conductor potential energy is $-K/z$, not the full energy of a pair of independently movable charges. On the falling branch, integrate the reciprocal speed:

$$
t_{\rm hit}=\sqrt{\frac m{2K}}\int_0^d\sqrt{\frac{zd}{d-z}}\,dz=\sqrt{\frac{md^3}{2K}}\int_0^1\sqrt{\frac{s}{1-s}}\,ds=\frac\pi2\sqrt{\frac{md^3}{2K}}.
$$

The last [integral](../../../calculus.md#integral) is $\pi/2$ by $s=\sin^2\theta$. Hence the [fall time of a charge toward a grounded plane](../../../electromagnetism.md#fall-time-of-a-charge-toward-a-grounded-plane) in the electrostatic Newtonian model is

$$
\boxed{t_{\rm hit}=\frac{\pi\sqrt{2\pi\varepsilon_0md^3}}{|q|}.}
$$

For $q=0$ there is no force and the particle remains at rest.

## 17D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17d/solution">Solution</h3>

↑ **Parent:** [17D](#17d)

Use the steady inviscid, hydrostatic, slowly varying channel approximation, without a [hydraulic jump](../../../physics.md#hydraulic-jump). Conservation of volume flux per unit width gives $Q=u(x)h(x)=u_1h_1$. The free-surface [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) is

$$
D(x)+h(x)+\frac{Q^2}{2gh(x)^2}=h_1+\frac{u_1^2}{2g}.
$$

Dividing by $h_1$ yields

$$
\boxed{\frac D{h_1}=1-\frac h{h_1}-\frac F2\left(\frac{h_1^2}{h^2}-1\right),\qquad F=\frac{u_1^2}{gh_1}.}
$$

The parameter $F$ here is the squared upstream [Froude number](../../../reduced-gravity.md#froude-number). For nonzero discharge, regarding $D$ as a function of $h$, its [derivative](../../../calculus.md#derivative) is $dD/dh=-1+Q^2/(gh^3)$. It has its unique maximum at $h_c=(Q^2/g)^{1/3}=h_1F^{1/3}$, where the local [Froude number](../../../reduced-gravity.md#froude-number) is one. Substitution gives $D^*=h_1(1-3F^{1/3}/2+F/2)$. This maximum is the [hydraulic control over a smooth hump](../../../fluid-mechanics.md#hydraulic-control-over-a-smooth-hump).

<h3 id="17d/i">i</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/i/solution">Solution</h4>

↑ **Parent:** [I](#17d/i)

The upstream flow is [subcritical flow](../../../reduced-gravity.md#subcritical-flow), with $h_1>h_c$. On this branch $dD/dh<0$, so the depth decreases as the bed rises; the velocity $Q/h$ increases. Since the crest height is below $D^*$, the depth remains above $h_c$ and never becomes critical. Over the falling side of the hump the depth increases again to **$h_1$ downstream**. The free surface falls over the hump: $d(h+D)/dD=-\mathrm{Fr}^2/(1-\mathrm{Fr}^2)<0$ on the subcritical branch.

<h3 id="17d/ii">ii</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#17d/ii)

The upstream flow is [supercritical flow](../../../reduced-gravity.md#supercritical-flow), with $h_1<h_c$. Now $dD/dh>0$, so the depth increases over the rising hump and the velocity decreases, while the free surface rises. Since $D_{\max}<D^*$, the depth stays below $h_c$. On the descending bed it decreases back to **$h_1$ downstream**, remaining supercritical throughout.

<h3 id="17d/iii">iii</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#17d/iii)

At the crest the two depth branches meet at **$h=h_c=h_1F^{1/3}$**. For a smooth nondegenerate maximum of the bed, $D^*-D$ is proportional to $(x-x_c)^2$, while expansion of the depth relation gives $D^*-D\sim3(h-h_c)^2/(2h_c)$. A differentiable flow through the crest therefore switches branches rather than following the cusp obtained by staying on the same branch. Subcritical upstream flow becomes supercritical downstream; supercritical upstream flow becomes subcritical downstream.

When $F<1$ and the bed returns to zero, put $y=h_{\rm down}/h_1$. The head equation becomes $2y^3-(2+F)y^2+F=0$, or

$$
(y-1)(2y^2-Fy-F)=0.
$$

The root $y=1$ is the original subcritical branch. The other positive root is smaller and lies on the supercritical branch, giving

$$
\boxed{h_{\rm down}=\frac{h_1}{4}\left(F+\sqrt{F^2+8F}\right).}
$$

This is the smooth transcritical, shock-free solution. A downstream [hydraulic jump](../../../physics.md#hydraulic-jump) would require further downstream conditions and energy loss. A degenerate flat crest can also require a branch-selection condition; the standard critical-control interpretation uses a nondegenerate smooth crest. For $F=1$, $D^*=0$, so a positive hump is incompatible with the prescribed upstream critical head. If $F=0$, the head equation is the still-water relation $h+D=h_1$; a crest of height $h_1$ dries out, so the wet transcritical-flow interpretation requires $F>0$.

## 18H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18h/solution">Solution</h3>

↑ **Parent:** [18H](#18h)

A [critical region](../../../statistical-modelling.md#rejection-region) $C$ is the set of sample outcomes on which a test rejects its [null hypothesis](../../../statistical-modelling.md#null-hypothesis). Its [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) is $\beta(\theta)=\mathbb P_\theta(X\in C)$; its [size of a statistical test](../../../statistical-modelling.md#size-of-a-statistical-test) is $\sup_{\theta\in\Theta_0}\beta(\theta)$. Randomized tests replace the indicator of $C$ by a rejection [probability](../../../probability-theory.md#probability) $\phi(X)\in[0,1]$.

The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) states that for two simple hypotheses with densities $p_0,p_1$, the test $\phi^*$ that is one where $p_1>kp_0$, zero where $p_1<kp_0$, and randomized on equality to have null rejection [probability](../../../probability-theory.md#probability) $\alpha$, maximizes power among tests of size at most $\alpha$. Here $k\ge0$. To prove it, let $\phi$ be any competing test. Pointwise, $(\phi^*-\phi)(p_1-kp_0)\ge0$, since both factors have the same sign off the equality set. Integrating gives

$$
\mathbb E_1\phi^*-\mathbb E_1\phi\ge k(\mathbb E_0\phi^*-\mathbb E_0\phi)\ge0.
$$

This proves the lemma, including equality-set randomization and points where $p_0=0$.

Take the exponential parameter to be its rate: $p_\lambda(x)=\lambda e^{-\lambda x}$ for $x\ge0$. For $T=\sum_iX_i$, the joint [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is $(\lambda_1/\lambda_0)^n e^{-(\lambda_1-\lambda_0)T}$, decreasing in $T$. Hence for $0<\alpha<1$ the most powerful test is

$$
\boxed{\text{reject when }T\le c_\alpha,\qquad \mathbb P_{\lambda_0}(T\le c_\alpha)=\alpha.}
$$

There is no boundary randomization because $T$ has a continuous [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution). Its density follows by repeated convolution: $p_T(t)=\lambda^nt^{n-1}e^{-\lambda t}/(n-1)!$. Integrating by parts gives the [exponential-rate likelihood-ratio test](../../../statistical-modelling.md#exponential-rate-likelihood-ratio-test) power

$$
\boxed{\beta(\lambda)=1-e^{-\lambda c_\alpha}\sum_{j=0}^{n-1}\frac{(\lambda c_\alpha)^j}{j!}.}
$$

The threshold is the unique positive solution of this formula at $\lambda=\lambda_0$ with value $\alpha$. Differentiating the finite sum yields

$$
\beta'(\lambda)=c_\alpha e^{-\lambda c_\alpha}\frac{(\lambda c_\alpha)^{n-1}}{(n-1)!}>0.
$$

Thus the [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) is strictly increasing, and its supremum over $0<\lambda\le\lambda_0$ is $\beta(\lambda_0)=\alpha$. Therefore **the same test has size $\alpha$ for the composite null $\lambda\le\lambda_0$**. Since the threshold does not depend on the particular larger rate, it is also uniformly most powerful against all $\lambda>\lambda_0$. The endpoint sizes zero and one have their trivial constant tests.

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/solution">Solution</h3>

↑ **Parent:** [19H](#19h)

Read the maze as two four-cycles: outer vertices $O_j$, inner vertices $I_j$ for $j$ modulo four, edges $O_jO_{j+1}$, $I_jI_{j+1}$, and $O_jI_j$, together with edges from every $I_j$ to the target $T$. The starting vertex is an outer vertex. Outer degrees are three and inner degrees are four.

For the ordinary [random walk on a graph](../../../markov-process.md#random-walk-on-a-graph), symmetry gives a common [expected hitting time](../../../markov-process.md#expected-hitting-time) $O$ from an outer vertex and $I$ from an inner one. First-step conditioning gives

$$
O=1+\frac23O+\frac13I,\qquad I=1+\frac14O+\frac12I.
$$

Thus $O=I+3$ and $I=2+O/2$, yielding **$I=7$ and the requested starting mean $O=10$ moves**.

For the [non-backtracking random walk](../../../markov-process.md#non-backtracking-random-walk), the current vertex alone does not form a [Markov chain](../../../markov-process.md#markov-chain). Use states $(a,b)$ recording previous and current vertices. Before hitting $T$, its transitions are $(a,b)\to(b,c)$ with [probability](../../../probability-theory.md#probability) $1/(\deg b-1)$ for each neighbor $c\ne a$. Add a starting state with no preceding vertex, choosing its first neighbor with [probability](../../../probability-theory.md#probability) $1/3$, and an absorbing hit state. This specifies the full [Markov chain](../../../markov-process.md#markov-chain).

Its directed edges aggregate into types $OO,OI,IO,II$, determined by the two vertex layers. From $OO$ the next type is $OO$ or $OI$ with [probability](../../../probability-theory.md#probability) $1/2$ each. From $OI$ it is $II$ with [probability](../../../probability-theory.md#probability) $2/3$ and the absorbing state with [probability](../../../probability-theory.md#probability) $1/3$. From $IO$ it is always $OO$. From $II$ it is $II$, $IO$ or the absorbing state with [probability](../../../probability-theory.md#probability) $1/3$ each. Every nonabsorbing type has a positive uniformly bounded chance of hitting within at most three more moves, so its mean time is finite.

<a id="19h/image-transition-probabilities-between-the-four-directed-edge-types-of-the-non-backtracking-maze-walk-and-its-absorbing-target"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1-nonbacktracking.png)

**[Figure 2](#19h/image-transition-probabilities-between-the-four-directed-edge-types-of-the-non-backtracking-maze-walk-and-its-absorbing-target). Transition probabilities between the four directed-edge types of the non-backtracking maze walk and its absorbing target**.

Let their remaining mean times be $A,B,C,D$ in that order. The first-step equations are

$$
A=1+\tfrac12A+\tfrac12B,\quad B=1+\tfrac23D,\quad C=1+A,\quad D=1+\tfrac13C+\tfrac13D.
$$

Solving gives $A=13/2$, $B=9/2$, $C=15/2$, $D=21/4$. The first move from the initial outer vertex reaches type $OO$ with [probability](../../../probability-theory.md#probability) $2/3$ and type $OI$ with [probability](../../../probability-theory.md#probability) $1/3$, so the intelligent starting mean is

$$
\boxed{1+\frac23\frac{13}{2}+\frac13\frac92=\frac{41}{6}\text{ moves}.}
$$

This [hitting a hub from two four-cycles](../../../markov-process.md#hitting-a-hub-from-two-four-cycles) calculation reduces the mean from $10$ to $41/6$, saving $19/6$ moves. Excluding immediate reversal removes wasteful two-step returns, although it does not guarantee that the next move is toward the target.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
