# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2001/PaperIB_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2001/PaperIB_1.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
  - [i](#1a/i)
    - [Solution](#1a/i/solution)
  - [ii](#1a/ii)
    - [Solution](#1a/ii/solution)
  - [iii](#1a/iii)
    - [Solution](#1a/iii/solution)
- [2H](#2h)
  - [Solution](#2h/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6G](#6g)
  - [Solution](#6g/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9F](#9f)
  - [Solution](#9f/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11H](#11h)
  - [Solution](#11h/solution)
- [12D](#12d)
  - [Solution](#12d/solution)
- [13B](#13b)
  - [Solution](#13b/solution)
- [14C](#14c)
  - [a](#14c/a)
    - [Solution](#14c/a/solution)
  - [b](#14c/b)
    - [Solution](#14c/b/solution)
- [15G](#15g)
  - [Solution](#15g/solution)
- [16E](#16e)
  - [Solution](#16e/solution)
- [17B](#17b)
  - [Solution](#17b/solution)
- [18F](#18f)
  - [a](#18f/a)
    - [Solution](#18f/a/solution)
  - [b](#18f/b)
    - [Solution](#18f/b/solution)

## 1A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1a/solution">Solution</h3>

↑ **Parent:** [1A](#1a)

A [function](../../../function.md) $f:I\to\mathbb R$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity) if

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in I:\quad |x-y|<\delta\Longrightarrow|f(x)-f(y)|<\varepsilon.
$$

The crucial point is that $\delta$ works throughout the [interval](../../../real-analysis.md#interval-mathematics), not just near one chosen point.

**Yes, it is bounded on the closed unit interval.** Choose $\delta$ for $\varepsilon=1$, and choose finitely many grid points $t_j$ such that every $x\in[0,1]$ is within $\delta$ of some $t_j$. Then $|f(x)|\leq1+\max_j|f(t_j)|$, a finite bound. Equivalently, [uniform continuity](../../../topological-analysis.md#uniform-continuity) implies [continuity](../../../calculus.md#continuous-function), and a continuous real [function](../../../function.md) on a [compact set](../../../topology.md#compact-space) is bounded.

**Yes, a bounded [derivative](../../../calculus.md#derivative) gives [uniform continuity](../../../topological-analysis.md#uniform-continuity) on the half-line.** If $|f'|\leq K$, the [mean value theorem](../../../calculus.md#mean-value-theorem) gives $|f(x)-f(y)|\leq K|x-y|$. This is a [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity), so for $K>0$ use $\delta=\varepsilon/K$. If $K=0$, the [function](../../../function.md) is constant. As usual for a [derivative](../../../calculus.md#derivative) on this closed half-line, [continuity](../../../calculus.md#continuous-function) at its endpoint is included.

<h3 id="1a/i">i</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/i/solution">Solution</h4>

↑ **Parent:** [I](#1a/i)

**Not uniformly continuous.** Take $x_n=n$, $y_n=n+1/n$. Then $|x_n-y_n|\to0$, but

$$
|y_n^2-x_n^2|=2+\frac1{n^2}\geq2.
$$

This contradicts the defining implication for [uniform continuity](../../../topological-analysis.md#uniform-continuity), for example with $\varepsilon=1$. The [sequential criterion for uniform continuity](../../../topological-analysis.md#sequential-criterion-for-uniform-continuity) makes explicit why arbitrarily close arguments at large distances from the origin matter.

<h3 id="1a/ii">ii</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1a/ii)

**Not uniformly continuous.** Choose

$$
x_n=\sqrt{2\pi n+\frac\pi2},\qquad y_n=\sqrt{2\pi n+\frac{3\pi}2}.
$$

Their separation is $\pi/(x_n+y_n)\to0$, while $\sin(x_n^2)=1$ and $\sin(y_n^2)=-1$. Thus the [function](../../../function.md) values stay distance two apart, contradicting [uniform continuity](../../../topological-analysis.md#uniform-continuity). Boundedness of the [function](../../../function.md) does not prevent increasingly rapid oscillations.

<h3 id="1a/iii">iii</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1a/iii)

**Uniformly continuous.** For $x\geq1$, the [derivative](../../../calculus.md#derivative) satisfies

$$
\left|\frac{d}{dx}\frac{\sin x}{x}\right|=\left|\frac{\cos x}{x}-\frac{\sin x}{x^2}\right|\leq2.
$$

The [mean value theorem](../../../calculus.md#mean-value-theorem) therefore gives a [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity) with constant two, hence [uniform continuity](../../../topological-analysis.md#uniform-continuity).

## 2H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2h/solution">Solution</h3>

↑ **Parent:** [2H](#2h)

For the real even [function](../../../function.md), let $s_N=a_0/2+\sum_{n=1}^Na_n\cos nx$. [Fourier orthogonality](../../../fourier-series.md#fourier-orthogonality) gives $\int_{-\pi}^{\pi}\cos nx\,dx=0$ for $n\geq1$ and $\int_{-\pi}^{\pi}\cos nx\cos mx\,dx=\pi\delta_{nm}$. Consequently

$$
\frac1\pi\int_{-\pi}^{\pi}s_N^2\,dx=\frac{a_0^2}{2}+\sum_{n=1}^Na_n^2.
$$

For an even [square-integrable function](../../../measure-theory.md#square-integrable-function), the complete [Fourier cosine series](../../../fourier-series.md#fourier-cosine-series) converges in the [L2 norm](../../../real-analysis.md#l2-norm); hence its norms converge. Taking $N\to\infty$ proves [Parseval's identity](../../../fourier-analysis.md#parseval-identity) in the required normalization:

$$
\boxed{\frac1\pi\int_{-\pi}^{\pi}f(x)^2\,dx=\frac{a_0^2}{2}+\sum_{n=1}^{\infty}a_n^2}.
$$

This limit argument avoids multiplying an infinite series without a justification of [L2 norm](../../../real-analysis.md#l2-norm) convergence.

For the quadratic [function](../../../function.md), the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are

$$
a_0=\frac1\pi\int_{-\pi}^{\pi}x^2\,dx=\frac{2\pi^2}{3},\qquad
a_n=\frac2\pi\int_0^\pi x^2\cos nx\,dx=\frac{4(-1)^n}{n^2}.
$$

The last equality follows from two [integrations by parts](../../../calculus.md#integration-by-parts), using $\sin n\pi=0$. Thus

$$
\boxed{x^2=\frac{\pi^2}{3}+4\sum_{n=1}^{\infty}\frac{(-1)^n}{n^2}\cos nx\quad(-\pi\leq x\leq\pi)}.
$$

This [Fourier series](../../../fourier-series.md) is [absolutely convergent](../../../real-analysis.md#absolute-convergence); the periodically extended quadratic is continuous, so it represents its values also at the endpoints. Substituting its coefficients into [Parseval's identity](../../../fourier-analysis.md#parseval-identity) gives

$$
\frac{2\pi^4}{5}=\frac{2\pi^4}{9}+16\sum_{n=1}^{\infty}\frac1{n^4},
\qquad \boxed{\sum_{n=1}^{\infty}\frac1{n^4}=\frac{\pi^4}{90}}.
$$

## 3D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

Put $S_1=\sum_{i=1}^nX_i$, $S_2=\sum_{i=1}^nX_i^2$. The joint [normal distribution](../../../probability-theory.md#normal-distribution) density can be written as

$$
p_\mu(\boldsymbol x)=(2\pi)^{-n/2}e^{-n/2}\mu^{-n}\exp\left(-\frac{S_2}{2\mu^2}+\frac{S_1}{\mu}\right).
$$

The [Fisher-Neyman factorization theorem](../../../probability-and-statistics.md#fisher-neyman-factorization-theorem) says that, for a family dominated by a common measure, a statistic $T$ is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic) when its densities have the form $g_\mu(T(\boldsymbol x))h(\boldsymbol x)$ with $h$ independent of the parameter. The displayed factorization therefore shows that **$(S_1,S_2)$ is a two-dimensional [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic)**.

For [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation), discard parameter-independent terms from the [log-likelihood](../../../statistical-modelling.md#log-likelihood):

$$
\ell(\mu)=-n\log\mu-\frac{S_2}{2\mu^2}+\frac{S_1}{\mu},\qquad
\ell'(\mu)=\frac{S_2-S_1\mu-n\mu^2}{\mu^3}.
$$

If $S_2>0$, the quadratic equation has exactly one positive root. The numerator is positive before that root and negative after it, while the [likelihood](../../../statistical-modelling.md#likelihood-function) tends to zero at both ends of $\mu>0$. Hence the [normal likelihood with variance equal to squared mean](../../../statistical-modelling.md#normal-likelihood-with-variance-equal-to-squared-mean) gives the global maximizer

$$
\boxed{\widehat\mu=\frac{\sqrt{S_1^2+4nS_2}-S_1}{2n}}.
$$

This holds almost surely. The exceptional all-zero sample has $S_2=0$ and [likelihood](../../../statistical-modelling.md#likelihood-function) proportional to $\mu^{-n}$, so its supremum is approached as $\mu\downarrow0$ and there is no positive maximizer.

## 4B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

The curvature-minus-one [Poincaré disk model](../../../geometry-and-topology.md#poincare-disk-model) has [Riemannian metric](../../../differential-geometry.md#riemannian-metric)

$$
\boxed{ds^2=\frac{4|dw|^2}{(1-|w|^2)^2}},\qquad |w|<1.
$$

The [geodesics](../../../riemannian-geometry.md#geodesic) through zero are Euclidean diameters. Indeed, for a path written in polar coordinates, its length is at least $\int2|\dot r|/(1-r^2)\,dt$, and hence at least $2\operatorname{artanh}r$ between zero and a point of modulus $r$. The radial segment attains this lower bound. By uniqueness of a [geodesic](../../../riemannian-geometry.md#geodesic) with given initial tangent, these radial paths describe all [geodesics](../../../riemannian-geometry.md#geodesic) through the origin. The radial [hyperbolic distance](../../../geometry-and-topology.md#hyperbolic-distance) is

$$
\rho=\int_0^r\frac{2\,ds}{1-s^2}=\log\frac{1+r}{1-r},
\qquad \boxed{r=\tanh(\rho/2)}.
$$

Thus a [hyperbolic circle in the Poincare disc](../../../geometry-and-topology.md#hyperbolic-circle-in-the-poincare-disc) is the indicated Euclidean circle.

An [isometry](../../../riemannian-geometry.md#isometry) from the [Poincaré half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model) to the [Poincaré disk model](../../../geometry-and-topology.md#poincare-disk-model) is the [Cayley transform between the half-plane and disk](../../../complex-analysis.md#cayley-transform-between-the-half-plane-and-disk),

$$
w=\frac{z-i}{z+i},\qquad z=i\frac{1+w}{1-w}.
$$

Writing $z=x+iy$, one has $1-|w|^2=4y/|z+i|^2$ and $|dw|^2=4|dz|^2/|z+i|^4$. Substitution into the disk [Riemannian metric](../../../differential-geometry.md#riemannian-metric) gives $ds^2=|dz|^2/y^2$, the half-plane [metric](../../../topological-analysis.md#metric), and $i$ maps to zero.

Put $r=\tanh(\rho/2)$. The inverse image of $|w|=r$ obeys

$$
x^2+(y-1)^2=r^2\bigl(x^2+(y+1)^2\bigr).
$$

Since $(1+r^2)/(1-r^2)=\cosh\rho$, completing the square yields

$$
\boxed{x^2+(y-\cosh\rho)^2=\sinh^2\rho}.
$$

This proves that the [hyperbolic circle in the upper half-plane](../../../geometry-and-topology.md#hyperbolic-circle-in-the-upper-half-plane) has Euclidean centre $i\cosh\rho$ and radius $\sinh\rho$.

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

Expansion of the [determinant](../../../linear-algebra.md#determinant) along the first row gives

$$
\det M=2x^2-(3-x)+2x(1-x)=3(x-1).
$$

Thus **the [matrix](../../../vector-space.md#matrix) is invertible exactly when $x\ne1$**. The minor formed from the first two rows and the last two columns is $-1$, independently of $x$, so the [matrix rank](../../../vector-space.md#matrix-rank) is always at least two. Therefore

$$
\boxed{\operatorname{rank}M=\begin{cases}3,&x\ne1,\\2,&x=1.\end{cases}}
$$

Taking cofactors and transposing them gives the [adjugate matrix](../../../linear-algebra.md#adjugate-matrix)

$$
\boxed{\operatorname{adj}M=
\begin{pmatrix}
2x&2x-1&-1\\
x-3&x-2&1\\
2x(1-x)&2(1-x^2)&x-1
\end{pmatrix}}.
$$

The [adjugate identity](../../../linear-algebra.md#adjugate-identity) $M\operatorname{adj}M=(\det M)I$ then gives

$$
\boxed{M^{-1}=\frac1{3(x-1)}\operatorname{adj}M\quad(x\ne1)}.
$$

In particular, the singular case has rank two, rather than a further exceptional rank-one value.

## 6G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6g/solution">Solution</h3>

↑ **Parent:** [6G](#6g)

Take $z$ positive downwards, and let the surface pressure be $p_0$. Static force balance gives the [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) equation $dp/dz=\rho g$. Hence

$$
\boxed{p(z)=p_0+\rho gz}.
$$

On a submerged body's surface, pressure traction is $-p\boldsymbol n$, where $\boldsymbol n$ points out of the body. The [divergence theorem](../../../calculus.md#divergence-theorem) gives the resultant

$$
\boldsymbol F=-\int_{\partial V}p\boldsymbol n\,dS
=-\int_V\nabla p\,dV=-\rho gV\boldsymbol e_z.
$$

Thus **the buoyancy is upward with magnitude $\rho gV$**, proving [Archimedes' principle](../../../fluid-mechanics.md#archimedes-principle). The constant surface pressure makes no contribution because $\int_{\partial V}\boldsymbol n\,dS=0$.

For a floating iceberg of total volume $V$, the displaced seawater volume is $V-V_I$. Neglecting air buoyancy, equality of weight and buoyancy gives $\rho_IgV=\rho_wg(V-V_I)$. Consequently

$$
\boxed{V=\frac{\rho_w}{\rho_w-\rho_I}V_I},
$$

with $0<\rho_I<\rho_w$, as required for partial flotation.

## 7E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

The [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) states that if $f$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on a neighbourhood of a simple closed positively oriented contour and its interior, then, for an interior point $z$,

$$
f(z)=\frac1{2\pi i}\oint\frac{f(\xi)}{\xi-z}\,d\xi.
$$

Fix $0<r<1$ and apply it on $|\xi|=r$. For $|z|<r$, the [geometric series](../../../real-analysis.md#geometric-series)

$$
\frac1{\xi-z}=\sum_{n=0}^{\infty}\frac{z^n}{\xi^{n+1}}
$$

converges uniformly in $\xi$ and locally uniformly in $z$. Indeed, for $|z|\leq s<r$ its absolute terms are bounded by $s^n/r^{n+1}$. Since $f$ is bounded on the contour, termwise [contour integration](../../../complex-analysis.md#contour-integration) is valid, giving

$$
f(z)=\sum_{n=0}^{\infty}c_nz^n,\qquad
c_n=\frac1{2\pi i}\oint_{|\xi|=r}\frac{f(\xi)}{\xi^{n+1}}\,d\xi.
$$

Termwise differentiation of this locally convergent [power series](../../../real-analysis.md#power-series) gives $f^{(n)}(0)=n!c_n$. Therefore

$$
\boxed{f^{(n)}(0)=\frac{n!}{2\pi i}\oint_{|\xi|=r}\frac{f(\xi)}{\xi^{n+1}}\,d\xi\quad(n\geq0)}.
$$

This also derives the needed [Taylor series](../../../calculus.md#taylor-series) representation rather than assuming an unjustified interchange at the boundary of the analytic disk.

## 8B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

The [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) is $d=b^2-4ac$. If the form is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form), evaluating it at $(1,0)$ gives $a>0$. For $a\ne0$, [completing the square](../../../polynomial.md#completing-the-square) gives

$$
q(x,y)=a\left(x+\frac b{2a}y\right)^2+\frac{4ac-b^2}{4a}y^2.
$$

Evaluating along $x=-by/(2a)$ shows that positivity also requires $d<0$. Conversely these two inequalities make both displayed coefficients positive, proving

$$
\boxed{q\text{ is positive definite}\Longleftrightarrow a>0>d}.
$$

A [reduced positive definite binary quadratic form](../../../number-theory.md#reduced-positive-definite-binary-quadratic-form) satisfies $|b|\leq a\leq c$, with $b\geq0$ if $|b|=a$ or $a=c$. The last convention avoids counting both boundary representatives. For fixed negative [discriminant](../../../polynomial.md#discriminant), these inequalities imply

$$
|d|=4ac-b^2\geq3a^2,\qquad 1\leq a\leq\sqrt{|d|/3}.
$$

There are finitely many such integers $a$, finitely many integers $b$ with $|b|\leq a$, and then $c=(b^2-d)/(4a)$ is determined. Hence **the number of reduced forms is finite**. If no admissible integer coefficients have the given [discriminant](../../../polynomial.md#discriminant), this number is zero.

For $d=-39$, the bound gives $a=1,2,3$. The integrality of $c=(b^2+39)/(4a)$ and the boundary sign convention give respectively

$$
(a,b,c)=(1,1,10),\quad(2,1,5),(2,-1,5),\quad(3,3,4).
$$

These are all the [reduced positive definite binary quadratic forms of discriminant minus thirty-nine](../../../number-theory.md#reduced-positive-definite-binary-quadratic-forms-of-discriminant-minus-thirty-nine). Thus

$$
\boxed{h(-39)=4},
$$

represented by $x^2+xy+10y^2$, $2x^2+xy+5y^2$, $2x^2-xy+5y^2$, and $3x^2+3xy+4y^2$.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/solution">Solution</h3>

↑ **Parent:** [9F](#9f)

For an incident particle from the left, take $E>0$ and $E>V_0$, and define

$$
k=\frac{\sqrt{2mE}}\hbar,\qquad q=\frac{\sqrt{2m(E-V_0)}}\hbar.
$$

The [Time-independent Schrödinger equation](../../../physics.md#time-independent-schrodinger-equation) gives an incident plus reflected [plane wave](../../../quantum-mechanics.md#plane-wave) on the left and an outgoing transmitted [plane wave](../../../quantum-mechanics.md#plane-wave) on the right:

$$
\psi(x)=e^{ikx}+re^{-ikx}\quad(x<0),\qquad \psi(x)=te^{iqx}\quad(x>0).
$$

[Continuity](../../../calculus.md#continuous-function) of the [wavefunction](../../../quantum-mechanics.md#wave-function) and its [derivative](../../../calculus.md#derivative) at a finite potential jump yields $1+r=t$ and $k(1-r)=qt$. Hence $r=(k-q)/(k+q)$ and $t=2k/(k+q)$. The incident and reflected [probability currents](../../../quantum-mechanics.md#probability-current) have equal wave-number magnitude, so

$$
\boxed{P=|r|^2=\left(\frac{\sqrt E-\sqrt{E-V_0}}{\sqrt E+\sqrt{E-V_0}}\right)^2}.
$$

As a check, the transmitted current fraction is $(q/k)|t|^2=4kq/(k+q)^2$, and the two probabilities sum to one.

For a positive step, $E\downarrow V_0$ makes $q\downarrow0$, so **$P\to1$**. For a negative step with fixed positive incident energy, $V_0\to-\infty$ makes $q\to\infty$, so again **$P\to1$**. The latter is quantum reflection from an increasingly large wave-number mismatch, even though the step is downward.

## 10A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

Assume $a<b$. On [continuous functions](../../../calculus.md#continuous-function) on this compact interval, both proposed distances are finite and symmetric, and vanish on identical [functions](../../../function.md). For the [supremum norm](../../../functional-analysis.md#supremum-norm), zero distance plainly implies pointwise equality. For the [L2 norm](../../../real-analysis.md#l2-norm), if a continuous difference is nonzero at any point, it stays bounded away from zero on a subinterval of positive length. Its squared [integral](../../../calculus.md#integral) is then positive, so zero distance also implies equality.

For the first [metric](../../../topological-analysis.md#metric), the pointwise [triangle inequality](../../../topological-analysis.md#triangle-inequality) followed by the supremum gives $d_1(x,z)\leq d_1(x,y)+d_1(y,z)$. For the second, put $u=x-y$, $v=y-z$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\|u+v\|_2^2\leq\|u\|_2^2+2\|u\|_2\|v\|_2+\|v\|_2^2=(\|u\|_2+\|v\|_2)^2.
$$

Taking square roots proves the required [triangle inequality](../../../topological-analysis.md#triangle-inequality). Thus both are [metrics](../../../topological-analysis.md#metric).

**The continuous-function space is complete in the uniform [metric](../../../topological-analysis.md#metric).** If $(x_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in $d_1$, at each $t$ its scalar values have a limit $x(t)$, by completeness of the scalar field. Given $\varepsilon>0$, choose $N$ with $\|x_n-x_m\|_\infty<\varepsilon$ for $m,n\geq N$. Letting $m\to\infty$ gives $|x_n(t)-x(t)|\leq\varepsilon$ uniformly in $t$. Hence there is [uniform convergence](../../../real-analysis.md#uniform-convergence). To see that the limit is continuous at $t_0$, approximate it uniformly by one continuous $x_n$ and use

$$
|x(t)-x(t_0)|\leq|x(t)-x_n(t)|+|x_n(t)-x_n(t_0)|+|x_n(t_0)-x(t_0)|.
$$

The outer terms can be made small uniformly, and the middle term is small near $t_0$. This proves the needed [uniform limit theorem](../../../real-analysis.md#uniform-limit-theorem) and [completeness](../../../topological-analysis.md#completeness).

For the second [metric](../../../topological-analysis.md#metric), let $H$ be zero on $(-1,0)$ and one on $(0,1)$; its value at zero is immaterial to the [integral](../../../calculus.md#integral). The supplied ramp [functions](../../../function.md) are continuous and satisfy

$$
\|x_n-H\|_2^2=\int_0^{1/n}(1-nt)^2\,dt=\frac1{3n}.
$$

Although $H$ is not in the continuous-function space, the [integral](../../../calculus.md#integral) [triangle inequality](../../../topological-analysis.md#triangle-inequality) yields $d_2(x_m,x_n)\leq(3m)^{-1/2}+(3n)^{-1/2}\to0$. Thus the [sequence](../../../real-analysis.md#sequence) is [Cauchy](../../../real-analysis.md#cauchy-sequence). If it converged in $d_2$ to a continuous $x$, the same inequality would give $\|x-H\|_2=0$. [Continuity](../../../calculus.md#continuous-function) would then force $x=0$ on the negative half-interval and $x=1$ on the positive half-interval, contradicting [continuity](../../../calculus.md#continuous-function) at zero. Therefore **the continuous-function space is not complete in $d_2$**; its limit in the larger [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) is the discontinuous step.

## 11H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11h/solution">Solution</h3>

↑ **Parent:** [11H](#11h)

Substituting $y=x^p$ in the homogeneous [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) gives $p(p-1)-2=(p-2)(p+1)=0$. Thus

$$
\boxed{y_h=Cx^2+D/x}.
$$

For a [Green's function](../../../analysis.md#green-s-function) decaying at the two ends, use $u(x)=x^2$ on the side of zero and $v(x)=x^{-1}$ on the side of infinity. Their [Wronskian](../../../differential-equation.md#wronskian) is $uv'-u'v=-3$. The [function](../../../function.md) must be continuous at $x=\xi$, or its second [derivative](../../../calculus.md#derivative) would contain a [derivative](../../../calculus.md#derivative) of a [Dirac delta](../../../distribution-theory.md#dirac-delta-function). Its [derivative](../../../calculus.md#derivative) jump must be one, to give the specified positive delta source. These two conditions yield the [boundary-decaying Green kernel for an inverse-square differential operator](../../../analysis.md#boundary-decaying-green-kernel-for-an-inverse-square-differential-operator):

$$
\boxed{G(x,\xi)=-\frac13\begin{cases}x^2/\xi,&x\leq\xi,\\\xi^2/x,&x\geq\xi.\end{cases}}
$$

Its [derivatives](../../../calculus.md#derivative) at the join are $-2/3$ on the left and $1/3$ on the right, confirming the jump one. Away from the join each branch solves the homogeneous equation, and both endpoint conditions hold.

Integrate this [Green's function](../../../analysis.md#green-s-function) against the forcing, whose support is between zero and one. For $0<x\leq1$,

$$
y(x)=-\frac13\left(\frac1x\int_0^x\xi^2\,d\xi+x^2\int_x^1\frac{d\xi}{\xi}\right)=\frac{x^2}{3}\log x-\frac{x^2}{9}.
$$

For $x\geq1$, only the right branch contributes. Therefore

$$
\boxed{y(x)=\begin{cases}\dfrac{x^2}{3}\log x-\dfrac{x^2}{9},&0<x\leq1,\\-\dfrac1{9x},&x\geq1.\end{cases}}
$$

On the first branch, $y'=(2x/3)\log x+x/9$ and $y''=(2/3)\log x+7/9$, so $y''-2y/x^2=1$. The second branch is a multiple of the homogeneous solution $x^{-1}$, so its forcing is zero. At $x=1$, both $y$ and $y'$ agree, with values $-1/9$ and $1/9$, so there is no additional delta source. Finally $x^2\log x\to0$ as $x\downarrow0$ and $x^{-1}\to0$ as $x\to\infty$. A homogeneous solution obeying both [boundary conditions](../../../differential-equation.md#boundary-condition) has $C=D=0$, establishing uniqueness.

## 12D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12d/solution">Solution</h3>

↑ **Parent:** [12D](#12d)

A [simple hypothesis](../../../statistical-modelling.md#simple-hypothesis) specifies a single probability law, with no unknown parameter remaining. For a possibly randomized [hypothesis test](../../../statistical-modelling.md#statistical-hypothesis-test), let $\varphi(x)\in[0,1]$ be its conditional rejection probability. Its [test size](../../../statistical-modelling.md#size-of-a-statistical-test) is $E_0\varphi(X)$ and its [statistical power](../../../probability-and-statistics.md#statistical-power) against the specified alternative is $E_1\varphi(X)$.

The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) states that for two densities $f_0,f_1$ with respect to a common measure, a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) rejecting when $f_1/f_0>k$, accepting when it is below $k$, and randomizing on equality to obtain size $\alpha$, maximizes power among all tests of size at most $\alpha$.

Here the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is

$$
\Lambda(x)=\frac{\sqrt{2\pi}}4\exp\left(\frac{x^2-|x|}{2}\right).
$$

Writing $r=|x|$, its logarithm apart from the constant is $(r^2-r)/2$. This decreases until $r=1/2$ and then increases. In particular it is nonpositive for $0\leq r\leq1$ and positive for $r>1$. The supplied normal-tail value and $\alpha<1/4$ imply that the quantile $t$ defined by $2[1-\Phi(t)]=\alpha$ satisfies $t>1$. Hence the threshold $\Lambda(t)$ is above every central value on $r\leq1$; outside that interval the ratio is strictly increasing. The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) therefore selects precisely the two tails:

$$
\boxed{\text{reject }H_0\text{ if }|X|>t,\qquad \Phi(t)=1-\alpha/2}.
$$

The equality boundary has probability zero under both continuous laws, so no randomization is needed. Under the alternative density, the [statistical power](../../../probability-and-statistics.md#statistical-power) is

$$
\boxed{\int_{|x|>t}\frac14e^{-|x|/2}\,dx=e^{-t/2}}.
$$

The central dip in the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is why checking the threshold against the entire central region, rather than assuming monotonicity in $|x|$ everywhere, is necessary.

## 13B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13b/solution">Solution</h3>

↑ **Parent:** [13B](#13b)

Project from the north pole $N=(0,0,1)$ onto the equatorial plane, identifying that plane with the [complex plane](../../../complex-analysis.md#complex-plane). The line from $N$ to $P=(X,Y,Z)$ meets the plane in

$$
\boxed{\phi(P)=\frac{X+iY}{1-Z}},\qquad \phi(N)=\infty.
$$

This is [stereographic projection](../../../complex-analysis.md#stereographic-projection). Its inverse is

$$
P(u)=\frac1{1+|u|^2}\bigl(2\operatorname{Re}u,2\operatorname{Im}u,|u|^2-1\bigr).
$$

Rotation through $\theta$ about the $z$-axis changes $X+iY$ to $e^{i\theta}(X+iY)$ and preserves $Z$, so it becomes the [Möbius transformation](../../../group-theory.md#mobius-transformation) $u\mapsto e^{i\theta}u$.

Let $B$ be the rotation [matrix](../../../vector-space.md#matrix) supplied in the question. It sends the $z$-axis to the $x$-axis, and therefore $R_x(\theta)=BR_z(\theta)B^{-1}$. If $b=\phi B\phi^{-1}$ is its given [Möbius transformation](../../../group-theory.md#mobius-transformation), then

$$
\phi R_x(\theta)\phi^{-1}=b\circ(u\mapsto e^{i\theta}u)\circ b^{-1},
$$

which is again a [Möbius transformation](../../../group-theory.md#mobius-transformation). Such $z$- and $x$-axis rotations can send any chosen point of the sphere to the south pole: first rotate its horizontal projection onto the $y$-axis, then rotate in the $yz$-plane. This supplies the rotations needed below.

The [antipodal stereographic coordinate relation](../../../complex-analysis.md#antipodal-stereographic-coordinate-relation) is $\phi(-P)=-1/\overline{\phi(P)}$, as follows immediately from the inverse formula. Fix the [cross-ratio](../../../group-theory.md#cross-ratio) convention

$$
[a,b;c,d]=\frac{(a-c)(b-d)}{(a-d)(b-c)}.
$$

We claim the required ordering is

$$
\boxed{\left[u,-\frac1{\bar u};v,-\frac1{\bar v}\right]=-\tan^2(d/2)}.
$$

For the [antipodal cross-ratio and spherical distance](../../../complex-analysis.md#antipodal-cross-ratio-and-spherical-distance) identity, rotate $P$ to the south pole. Its coordinate becomes zero and its antipode becomes infinity. A point at angular [spherical distance](../../../geometry-and-topology.md#great-circle-distance) $d$ from the south pole has vertical coordinate $-\cos d$ and horizontal magnitude $\sin d$, so its new projected coordinate $v'$ has modulus $\sin d/(1+\cos d)=\tan(d/2)$. By [Möbius invariance of the cross-ratio](../../../group-theory.md#mobius-invariance-of-the-cross-ratio), the displayed expression equals

$$
[0,\infty;v',-1/\bar v']=\frac{-v'}{1/\bar v'}=-|v'|^2=-\tan^2(d/2).
$$

For finite nonsingular coordinates the same ratio is $-|u-v|^2/|1+u\bar v|^2$. Zero or infinite antipodal coordinates are interpreted by limits. When $Q=-P$, $d=\pi$ and the ratio has the extended value infinity; the finite real formula applies for $0<d<\pi$.

## 14C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14c/a">a</h3>

↑ **Parent:** [14C](#14c)

<h4 id="14c/a/solution">Solution</h4>

↑ **Parent:** [A](#14c/a)

Write $J_k(\lambda)$ for the [Jordan block](../../../linear-operator-theory.md#jordan-block) with diagonal $\lambda$ and ones on the superdiagonal. Its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) and [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) are both $(x-\lambda)^k$. Therefore one answer to the first request is

$$
\boxed{M=J_3(2)\oplus J_2(-1)}.
$$

For the second request, take

$$
\boxed{M_1=J_2(3)\oplus J_2(3)\oplus J_1(3)\oplus J_2(1)},
$$



$$
\boxed{M_2=J_2(3)\oplus J_1(3)\oplus J_1(3)\oplus J_1(3)\oplus J_2(1)}.
$$

The algebraic multiplicities are five and two, and the largest block at each [eigenvalue](../../../linear-operator-theory.md#eigenvalue) has size two, so both prescribed [polynomials](../../../polynomial.md) hold. They are not [similar matrices](../../../linear-algebra.md#matrix-similarity): the [eigenspace](../../../linear-operator-theory.md#eigenspace) at three has dimensions three and four respectively, and similarity preserves [eigenspace](../../../linear-operator-theory.md#eigenspace) dimension.

**There is no third similarity class.** At [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one, the total size two and maximal block size two force the single block $J_2(1)$. At [eigenvalue](../../../linear-operator-theory.md#eigenvalue) three, the blocks partition five, each has size at most two, and at least one has size two. The only partitions are $2+2+1$ and $2+1+1+1$. The uniqueness of [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) up to block order therefore leaves exactly the two classes already exhibited.

<h3 id="14c/b">b</h3>

↑ **Parent:** [14C](#14c)

<h4 id="14c/b/solution">Solution</h4>

↑ **Parent:** [B](#14c/b)

Let $I$ denote the identity endomorphism. The two-root [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) gives $(\alpha-\lambda_1I)(\alpha-\lambda_2I)=0$. Every [vector](../../../vector-space.md#vector) has the decomposition

$$
v=\frac{(\alpha-\lambda_2I)v}{\lambda_1-\lambda_2}+\frac{(\alpha-\lambda_1I)v}{\lambda_2-\lambda_1}.
$$

The first summand lies in the [eigenspace](../../../linear-operator-theory.md#eigenspace) $E_1=\ker(\alpha-\lambda_1I)$, and the second in $E_2$. If a [vector](../../../vector-space.md#vector) belongs to both, subtracting its two [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equations gives $(\lambda_1-\lambda_2)v=0$, hence $v=0$. Thus $V=E_1\oplus E_2$.

For distinct real roots $\lambda_1,\ldots,\lambda_m$, define [polynomial](../../../polynomial.md) projectors

$$
P_i=\prod_{j\ne i}\frac{\alpha-\lambda_jI}{\lambda_i-\lambda_j}.
$$

The [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) [polynomials](../../../polynomial.md) in this expression sum to one: their sum has degree at most $m-1$ and equals one at the $m$ distinct roots. Hence $\sum_iP_i=I$. Also $(\alpha-\lambda_iI)P_i=0$, because its numerator is the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) evaluated at $\alpha$. Thus every [vector](../../../vector-space.md#vector) is a sum of [eigenvectors](../../../linear-operator-theory.md#eigenvector), $v=\sum_iP_iv$. On $E_j$, $P_i$ acts as $\delta_{ij}I$, so applying $P_i$ to any zero sum of [vectors](../../../vector-space.md#vector) from the [eigenspaces](../../../linear-operator-theory.md#eigenspace) shows that every summand is zero. Therefore

$$
\boxed{V=\bigoplus_{i=1}^m\ker(\alpha-\lambda_iI)}.
$$

Choosing a basis in each [eigenspace](../../../linear-operator-theory.md#eigenspace) proves [diagonalizability](../../../linear-operator-theory.md#diagonalizable-matrix) over the reals. Conversely, if a real [matrix](../../../vector-space.md#matrix) is similar over the reals to a diagonal [matrix](../../../vector-space.md#matrix), a [polynomial](../../../polynomial.md) annihilates it exactly when it vanishes at each distinct real diagonal entry. Its [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is therefore the product of those distinct linear factors. We have proved **real diagonalizability is equivalent to a [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) with distinct real roots**.

## 15G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15g/solution">Solution</h3>

↑ **Parent:** [15G](#15g)

Put $\theta=x-t$. Taking the [gradient](../../../calculus.md#gradient) of the [velocity potential](../../../fluid-mechanics.md#velocity-potential) gives

$$
\boxed{\boldsymbol u=(-\epsilon y\sin\theta,\ \epsilon\cos\theta)},\qquad
\boxed{\nabla\cdot\boldsymbol u=-\epsilon y\cos\theta}.
$$

The motion is not generally incompressible; a [velocity potential](../../../fluid-mechanics.md#velocity-potential) ensures irrotationality, not zero [divergence](../../../calculus.md#divergence). Both components have zero time average at each fixed point because their sine and cosine averages vanish.

The fluid acceleration is the [material derivative](../../../continuum-mechanics.md#material-derivative) $D\boldsymbol u/Dt=\partial_t\boldsymbol u+(\boldsymbol u\cdot\nabla)\boldsymbol u$. Direct differentiation gives

$$
a_x=\epsilon y\cos\theta+\epsilon^2(y^2-1)\sin\theta\cos\theta,
\qquad
a_y=\epsilon\sin\theta+\epsilon^2y\sin^2\theta.
$$

Averaging over one period at fixed $(x,y)$ therefore yields

$$
\boxed{\overline{\boldsymbol a}=(0,\epsilon^2y/2)}.
$$

This need not be the [derivative](../../../calculus.md#derivative) of the mean velocity: the nonlinear advective term remains after averaging.

The dyed particle obeys the [Lagrangian trajectory](../../../continuum-mechanics.md#lagrangian-trajectory) equations

$$
\dot x=-\epsilon y\sin(x-t),\qquad \dot y=\epsilon\cos(x-t),\qquad x(0)=y(0)=0.
$$

Expand $x=\epsilon x_1+\epsilon^2x_2+O(\epsilon^3)$ and $y=\epsilon y_1+\epsilon^2y_2+O(\epsilon^3)$, for bounded times. The first-order equations give $x_1=0$, $\dot y_1=\cos t$, so $y_1=\sin t$. At second order,

$$
\dot x_2=\sin^2t,\qquad \dot y_2=0.
$$

Integrating with zero initial values verifies

$$
\boxed{x(t)=\epsilon^2\left(\frac t2-\frac{\sin2t}{4}\right)+O(\epsilon^3),\qquad y(t)=\epsilon\sin t+O(\epsilon^3)}.
$$

The velocity averaged along this particle over $0\leq t\leq2\pi$ is its displacement divided by $2\pi$. Hence

$$
\boxed{\overline{\boldsymbol u}_{\mathrm{particle}}=(\epsilon^2/2,0)+O(\epsilon^3)}.
$$

This [Stokes drift](../../../continuum-mechanics.md#stokes-drift) is a Lagrangian mean; it does not contradict the zero [Eulerian mean velocity](../../../geophysical-fluid-dynamics.md#eulerian-mean-flow) at a fixed point. The secular term is a small-parameter expansion, not an assertion of uniform accuracy as $t\to\infty$.

## 16E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16e/solution">Solution</h3>

↑ **Parent:** [16E](#16e)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat F(k)=\int_{\mathbb R}F(x)e^{-ikx}\,dx$. First compute the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) of the periodized sum. Absolute integrability gives

$$
\sum_{j\in\mathbb Z}\int_0^{2\pi}|F(2\pi j+\tau)|\,d\tau=\int_{\mathbb R}|F(x)|\,dx<\infty.
$$

Thus [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) justifies termwise integration. For integer $m$, the change of variable $x=2\pi j+\tau$ and $e^{2\pi imj}=1$ give

$$
c_m=\frac1{2\pi}\int_0^{2\pi}f(\tau)e^{-im\tau}\,d\tau
=\frac1{2\pi}\sum_j\int_{2\pi j}^{2\pi(j+1)}F(x)e^{-imx}\,dx
=\boxed{\frac{\widehat F(m)}{2\pi}}.
$$

Reindexing a convergent periodization gives periodicity; the [integral](../../../calculus.md#integral) argument always gives its periodic representative almost everywhere. This proves the Fourier-coefficient content of the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula).

There is a genuine qualification to the printed pointwise claim: the [periodization of an integrable function](../../../fourier-analysis.md#periodization-of-an-integrable-function) need not agree pointwise with its [Fourier series](../../../fourier-series.md) under the stated hypotheses alone. Set $F(0)=1$ and $F(x)=0$ for $x\ne0$. This is absolutely integrable, and on one closed period the periodization has only two possibly nonzero summands, so the series is uniformly convergent. Yet $f(0)=1$, while $\widehat F(m)=0$ for every $m$. The claimed pointwise equality at zero is therefore false. This counterexample also works for Riemann integrability, not only for an almost-everywhere convention.

The coefficient identity gives a rigorous general replacement: the weighted [Fejér sums](../../../fourier-series.md#fejer-sum)

$$
\sigma_Nf(\tau)=\frac1{2\pi}\sum_{|m|\leq N}\left(1-\frac{|m|}{N+1}\right)\widehat F(m)e^{im\tau}
$$

converge to the periodization in the [integral](../../../calculus.md#integral) norm, and at every [continuity](../../../calculus.md#continuous-function) point. Indeed they are its convolution with the normalized [Fejér kernel](../../../fourier-series.md#fejer-kernel); that kernel is nonnegative, has [integral](../../../calculus.md#integral) one, and has [integral](../../../calculus.md#integral) tending to zero outside every fixed neighbourhood of zero. For convergence in the [L1 norm](../../../functional-analysis.md#l1-norm), split the convolution error into small translations, controlled by [continuity](../../../calculus.md#continuous-function) of translation in the [integral](../../../calculus.md#integral) norm, and the remaining tail. The same split gives [pointwise convergence](../../../real-analysis.md#pointwise-convergence) at a [continuity](../../../calculus.md#continuous-function) point. If the periodization is piecewise continuously differentiable, the ordinary [Fourier series](../../../fourier-series.md) has the usual midpoint limit; if it is continuous and its coefficients are absolutely summable, the displayed unweighted formula holds pointwise. These are sufficient interpretations of the intended identity.

For the specified exponential example all the needed [Fourier series](../../../fourier-series.md) convergence properties do hold. Split its [Fourier transform](../../../analysis.md#fourier-transform) at zero to obtain

$$
\widehat F(k)=\int_0^\infty e^{-(1+ik)x}\,dx+\int_0^\infty e^{-(1-ik)x}\,dx
=\frac{2}{1+k^2}.
$$

Its periodization is continuous, with uniformly geometrically bounded tails, and the sampled coefficients are absolutely summable. The absolutely summable coefficients define a uniformly convergent [Fourier series](../../../fourier-series.md) with the computed coefficients. Its continuous sum equals the continuous periodization: their difference has every [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) zero, hence is zero in the [L2 norm](../../../real-analysis.md#l2-norm) by Fourier completeness, and continuity upgrades that to equality everywhere. Therefore its ordinary [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) is valid. Evaluate it at zero:

$$
\sum_{j\in\mathbb Z}e^{-2\pi|j|}=1+\frac{2e^{-2\pi}}{1-e^{-2\pi}}=\coth\pi
=\frac1\pi\sum_{n\in\mathbb Z}\frac1{1+n^2}.
$$

Thus the fully justified requested sum is

$$
\boxed{\sum_{n=-\infty}^{\infty}\frac1{1+n^2}=\pi\coth\pi}.
$$

## 17B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17b/solution">Solution</h3>

↑ **Parent:** [17B](#17b)

First work over a field of characteristic different from two. If a nonzero [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) had $\phi(v,v)=0$ for every [vector](../../../vector-space.md#vector), polarization would give

$$
2\phi(u,v)=\phi(u+v,u+v)-\phi(u,u)-\phi(v,v)=0,
$$

a contradiction. Hence choose $e$ with $\phi(e,e)\ne0$. Every $v$ decomposes uniquely as

$$
v=\frac{\phi(v,e)}{\phi(e,e)}e+\left(v-\frac{\phi(v,e)}{\phi(e,e)}e\right),
$$

with the second summand orthogonal to $e$. Induct on the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) to obtain a diagonal basis. If the restricted form becomes zero, any basis of that remaining space completes the diagonalization. In this basis the [rank of a quadratic form](../../../linear-algebra.md#rank-of-a-quadratic-form) is exactly the number of nonzero diagonal coefficients; the remaining basis [vectors](../../../vector-space.md#vector) span its [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form).

Over the reals, rescale the nonzero basis [vectors](../../../vector-space.md#vector) so the diagonal entries are $p$ copies of $+1$, $q$ copies of $-1$ and $z=n-p-q$ zeros. Define the [signature of a quadratic form](../../../linear-algebra.md#signature-of-a-quadratic-form) by $\sigma=p-q$, so $r=p+q$. To prove it is basis independent, note that $p$ is the largest dimension of a [linear subspace](../../../vector-space.md#vector-subspace) on which the form is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form). The positive coordinate [linear subspace](../../../vector-space.md#vector-subspace) attains dimension $p$; on any other positive [linear subspace](../../../vector-space.md#vector-subspace), projection to those positive coordinates is injective, since its kernel has nonpositive quadratic value. Thus its dimension is at most $p$. The same argument for the negative form characterizes $q$. This proves [Sylvester's law of inertia](../../../linear-algebra.md#sylvester-s-law-of-inertia) and that the signature is well-defined.

Let $e_i$ and $f_i$ be positive and negative normalized basis [vectors](../../../vector-space.md#vector), and let $Z$ be the [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form). The span of $Z$ and $e_i+f_i$ for $1\leq i\leq\min(p,q)$ is a [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace): all mutual bilinear pairings vanish. Its dimension is $z+\min(p,q)$. Conversely, project any [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace) $U$ to the nondegenerate positive-plus-negative quotient. The projected [linear subspace](../../../vector-space.md#vector-subspace) is still null, and its projections to both the positive and negative coordinate spaces are injective: a [vector](../../../vector-space.md#vector) with one component zero would have strictly signed quadratic value unless it vanished. Its dimension is therefore at most $\min(p,q)$, while the kernel of the quotient map on $U$ has dimension at most $z$. Hence

$$
\boxed{\max\dim U=z+\min(p,q)=n-\frac{r+|\sigma|}{2}}.
$$

This proves both construction and sharpness of the [maximum dimension of a totally isotropic subspace](../../../linear-algebra.md#maximum-dimension-of-a-totally-isotropic-subspace).

For the five-variable example, the symmetric coefficient [matrix](../../../vector-space.md#matrix) is

$$
A=\begin{pmatrix}
0&1&0&0&1\\1&0&1&0&0\\0&1&0&1&0\\0&0&1&0&1\\1&0&0&1&0
\end{pmatrix}.
$$

Its cyclic structure makes the [vectors](../../../vector-space.md#vector) $(1,\zeta^k,\zeta^{2k},\zeta^{3k},\zeta^{4k})$, $\zeta=e^{2\pi i/5}$, [eigenvectors](../../../linear-operator-theory.md#eigenvector) with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\zeta^k+\zeta^{-k}=2\cos(2\pi k/5)$. Thus the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
2,\qquad \frac{\sqrt5-1}{2}\ \text{(twice)},\qquad -\frac{\sqrt5+1}{2}\ \text{(twice)}.
$$

Their product is $2$, and three are positive and two negative. Therefore

$$
\boxed{\det A=2,\qquad r=5,\qquad\sigma=1}.
$$

The real and imaginary parts of each conjugate pair of [eigenvectors](../../../linear-operator-theory.md#eigenvector) give the corresponding real two-dimensional [eigenspaces](../../../linear-operator-theory.md#eigenspace), consistent with the real inertia calculation.

## 18F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18f/a">a</h3>

↑ **Parent:** [18F](#18f)

<h4 id="18f/a/solution">Solution</h4>

↑ **Parent:** [A](#18f/a)

Infinite walls impose the [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) $\psi(-a)=\psi(a)=0$. Inside the [infinite square well](../../../quantum-mechanics.md#infinite-square-well), the [Time-independent Schrödinger equation](../../../physics.md#time-independent-schrodinger-equation) is $-\hbar^2\psi''/(2m)=E\psi$. Its nonzero solutions satisfying both endpoint conditions have wave numbers $k_n=n\pi/(2a)$, $n\geq1$. Since

$$
\int_{-a}^a\sin^2\left(\frac{n\pi(x+a)}{2a}\right)dx=a,
$$

the normalized [energy eigenstates](../../../quantum-mechanics.md#energy-eigenstate) are the sine modes with prefactor $1/\sqrt a$. They are orthonormal by sine [orthogonality](../../../linear-algebra.md#orthogonal-vectors) and complete by the [Fourier sine series](../../../fourier-series.md#fourier-sine-series) on an interval of length $2a$. Differentiating twice gives

$$
\boxed{E_n=\frac{\hbar^2\pi^2n^2}{8ma^2}\quad(n=1,2,\ldots)}.
$$

<h3 id="18f/b">b</h3>

↑ **Parent:** [18F](#18f)

<h4 id="18f/b/solution">Solution</h4>

↑ **Parent:** [B](#18f/b)

The initial [wavefunction](../../../quantum-mechanics.md#wave-function) has unit norm, since $\int_0^a(2/a)\sin^2(\pi x/a)\,dx=1$. On its nonzero half, $-\hbar^2\psi''/(2m)=E_*\psi$ with $E_*=\hbar^2\pi^2/(2ma^2)$. A small domain qualification is important: the [derivative](../../../calculus.md#derivative) jumps at zero, so the state is not in the operator domain of the Dirichlet [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics). Its finite energy [expectation value](../../../quantum-mechanics.md#expectation-value) is nevertheless defined by the [quadratic form of a positive quantum Hamiltonian](../../../quantum-mechanics.md#quadratic-form-of-a-positive-quantum-hamiltonian). The [energy form of a half-well sine state](../../../quantum-mechanics.md#energy-form-of-a-half-well-sine-state) gives

$$
\langle E\rangle=\frac{\hbar^2}{2m}\int_{-a}^a|\psi'(x)|^2dx
=\frac{\hbar^2}{2m}\frac{2\pi^2}{a^3}\int_0^a\cos^2(\pi x/a)\,dx
=\boxed{\frac{\hbar^2\pi^2}{2ma^2}}.
$$

This is also the rigorous weak interpretation of the printed $\int\psi H\psi$. Indeed the distributional second [derivative](../../../calculus.md#derivative) is $\psi''=-(\pi/a)^2\psi+\sqrt{2/a}(\pi/a)\delta_0$ inside the well. The [Dirac delta](../../../distribution-theory.md#dirac-delta-function) term pairs to zero because $\psi(0)=0$. One should not instead conclude that this state is an [energy eigenstate](../../../quantum-mechanics.md#energy-eigenstate) from its equation on just the positive half.

Its coefficients in the full-well [energy eigenstates](../../../quantum-mechanics.md#energy-eigenstate) are

$$
a_n=\frac{\sqrt2}{a}\int_0^a\sin\frac{\pi x}{a}\sin\frac{n\pi(x+a)}{2a}\,dx.
$$

For even $n$, sine [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives $a_2=-1/\sqrt2$ and all other even coefficients zero. For $n=2p+1$, set $u=x/a$ and use $\sin[n\pi(u+1)/2]=(-1)^p\cos(n\pi u/2)$. Product-to-sum integration then gives

$$
\int_0^1\sin\pi u\cos\frac{n\pi u}{2}\,du=\frac{4}{\pi(4-n^2)},\qquad
\boxed{a_{2p+1}=\frac{4\sqrt2(-1)^p}{\pi[4-(2p+1)^2]}}.
$$

Since these coefficients are $O(n^{-2})$, $\sum_nE_n|a_n|^2$ converges, confirming that the state has finite energy. With $E_n=n^2E_1$, the spectral expression is

$$
\langle E\rangle=\frac12E_2+\frac{32E_1}{\pi^2}\sum_{p=0}^{\infty}\frac{(2p+1)^2}{[(2p+1)^2-4]^2}.
$$

The kinetic-energy [quadratic form](../../../linear-algebra.md#quadratic-form) equals this spectral sum: expanding the weak [derivative](../../../calculus.md#derivative) in the corresponding orthonormal cosine modes and using [Parseval's identity](../../../fourier-analysis.md#parseval-identity) gives $\int|\psi'|^2=\sum_nk_n^2|a_n|^2$. Equating it to the directly integrated value $4E_1$ proves

$$
\boxed{1=\frac12+\frac8{\pi^2}\sum_{p=0}^{\infty}\frac{(2p+1)^2}{[(2p+1)^2-4]^2}}.
$$

In contrast, $\sum_nE_n^2|a_n|^2$ diverges, consistently showing why $H\psi$ is not an ordinary square-integrable [vector](../../../vector-space.md#vector) even though the energy expectation is finite.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
