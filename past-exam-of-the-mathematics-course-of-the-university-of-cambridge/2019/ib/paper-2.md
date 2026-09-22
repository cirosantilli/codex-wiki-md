# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperib_2_2019.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperib_2_2019.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3E](#3e)
  - [a](#3e/a)
    - [Solution](#3e/a/solution)
  - [b](#3e/b)
    - [Solution](#3e/b/solution)
- [4G](#4g)
  - [a](#4g/a)
    - [Solution](#4g/a/solution)
  - [b](#4g/b)
    - [Solution](#4g/b/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7C](#7c)
  - [Solution](#7c/solution)
- [8H](#8h)
  - [a](#8h/a)
    - [Solution](#8h/a/solution)
  - [b](#8h/b)
    - [Solution](#8h/b/solution)
  - [c](#8h/c)
    - [Solution](#8h/c/solution)
- [9H](#9h)
  - [Solution](#9h/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
  - [d](#10f/d)
    - [Solution](#10f/d/solution)
- [11G](#11g)
  - [a](#11g/a)
    - [Solution](#11g/a/solution)
  - [b](#11g/b)
    - [Solution](#11g/b/solution)
  - [c](#11g/c)
    - [Solution](#11g/c/solution)
- [12E](#12e)
  - [a](#12e/a)
    - [i](#12e/a/i)
      - [Solution](#12e/a/i/solution)
    - [ii](#12e/a/ii)
      - [Solution](#12e/a/ii/solution)
    - [iii](#12e/a/iii)
      - [Solution](#12e/a/iii/solution)
  - [b](#12e/b)
    - [i](#12e/b/i)
      - [Solution](#12e/b/i/solution)
    - [ii](#12e/b/ii)
      - [Solution](#12e/b/ii/solution)
- [13D](#13d)
  - [Solution](#13d/solution)
- [14E](#14e)
  - [Solution](#14e/solution)
- [15A](#15a)
  - [Solution](#15a/solution)
- [16D](#16d)
  - [Solution](#16d/solution)
- [17B](#17b)
  - [Solution](#17b/solution)
- [18A](#18a)
  - [Solution](#18a/solution)
- [19C](#19c)
  - [Solution](#19c/solution)
- [20H](#20h)
  - [a](#20h/a)
    - [Solution](#20h/a/solution)
  - [b](#20h/b)
    - [Solution](#20h/b/solution)
  - [c](#20h/c)
    - [Solution](#20h/c/solution)

## 1F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

Let $r=dim(U\cap W)$. Choose a [basis](../../../vector-space.md#basis) $e_1,\ldots,e_r$ of the [intersection of vector subspaces](../../../vector-space.md#intersection-of-vector-subspaces), extend it to a basis $e_1,\ldots,e_r,u_{r+1},\ldots,u_m$ of $U$, and independently extend it to a basis $e_1,\ldots,e_r,w_{r+1},\ldots,w_n$ of $W$. The combined list

$$
e_1,\ldots,e_r,u_{r+1},\ldots,u_m,w_{r+1},\ldots,w_n
$$

spans the [sum of vector subspaces](../../../vector-space.md#sum-of-vector-subspaces) $U+W$. It is also [linearly independent](../../../vector-space.md#linear-independence): a vanishing [linear combination](../../../vector-space.md#linear-combination) says that a combination of the $u_i$ belongs to $U\cap W$, and its expression in the chosen basis of $U$ forces all its coefficients to vanish; the coefficients of the $w_i$ then vanish in the same way. This proves the [dimension formula for a sum of subspaces](../../../vector-space.md#dimension-formula-for-a-sum-of-subspaces)

$$
\boxed{\dim(U+W)=\dim U+\dim W-\dim(U\cap W)}.
$$

Parametrize the two [linear subspaces](../../../vector-space.md#vector-subspace) as

$$
U=\operatorname{span}\{(7,-5,1,0),(8,-6,0,1)\},
\qquad
W=\operatorname{span}\{(-2,1,0,0),(-3,0,1,0)\}.
$$

Putting a vector of $U$ in $W$ first forces its fourth coordinate to vanish; the remaining defining equation is then automatic. Thus

$$
U\cap W=\operatorname{span}\{(7,-5,1,0)\},
$$

and the dimension formula gives $\dim(U+W)=2+2-1=3$.

The [linear functional](../../../linear-algebra.md#linear-functional)

$$
\boxed{\ell(x)=x_1+2x_2+3x_3+4x_4}
$$

vanishes on each displayed generator of $U$ and $W$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is three-dimensional because $\ell\ne0$, so the inclusion $U+W\subseteq\ker\ell$ between two three-dimensional subspaces is equality.

## 2G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

Let the [torsion submodule](../../../module-theory.md#torsion-submodule) of the [module over a ring](../../../module-theory.md#module-mathematics) $M$ be

$$
T(M)=\{m\in M:rm=0\text{ for some }0\ne r\in R\}.
$$

This is a [submodule](../../../module-theory.md#submodule). Indeed, if $rm=0$ and $sn=0$ with $r,s\ne0$, then $rs\ne0$ because the scalar ring is an [integral domain](../../../commutative-algebra.md#integral-domain), and $rs(m+n)=0$; scalar multiples and additive inverses are handled similarly.

Take the [quotient module](../../../module-theory.md#quotient-module) $M_0=M/T(M)$ and let $q:M\to M_0$ be the quotient [R-module homomorphism](../../../module-theory.md#module-homomorphism). It is [torsion-free](../../../module-theory.md#torsion-free-module): if $0\ne r\in R$ and $r(m+T(M))=0$, then $rm\in T(M)$, so $srm=0$ for some $s\ne0$. Since $sr\ne0$, this puts $m$ in $T(M)$ and therefore $m+T(M)=0$.

Now let $N$ be torsion-free and let $f:M\to N$ be an $R$-module homomorphism. If $m\in T(M)$ and $rm=0$ for $r\ne0$, then $r f(m)=f(rm)=0$, so torsion-freeness gives $f(m)=0$. Hence $T(M)\subseteq\ker f$, and the [universal property of a quotient module](../../../module-theory.md#universal-property-of-a-quotient-module) gives a unique homomorphism

$$
f_0:M/T(M)\longrightarrow N,
\qquad f_0(m+T(M))=f(m),
$$

with $\boxed{f=f_0\circ q}$. Thus $M/T(M)$ is the [maximal torsion-free quotient](../../../module-theory.md#maximal-torsion-free-quotient) of $M$.

## 3E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3e/a">a</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/a/solution">Solution</h4>

↑ **Parent:** [A](#3e/a)

For $x\ne0$, all component functions are continuously differentiable and the [Jacobian matrix](../../../calculus.md#jacobian-matrix) is

$$
\boxed{Df(x,y)=
\begin{pmatrix}
\dfrac1{3x^{2/3}}&2y\\[4pt]
0&5y^4
\end{pmatrix}}.
$$

At a point $(0,y_0)$, the first component cannot be [differentiable](../../../analysis.md#differentiable-function): along the first coordinate axis its difference quotient contains $h^{1/3}/h=h^{-2/3}$, which is unbounded as $h\to0$. Therefore $f$ is [continuously differentiable](../../../calculus.md#continuously-differentiable-function) exactly at the points with $x\ne0$.

<h3 id="3e/b">b</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/b/solution">Solution</h4>

↑ **Parent:** [B](#3e/b)

At a point with $xy\ne0$, the [determinant](../../../linear-algebra.md#determinant) of the [derivative](../../../calculus.md#derivative) is

$$
\det Df(x,y)=\frac{5y^4}{3x^{2/3}}\ne0.
$$

The [inverse function theorem](../../../calculus.md#inverse-function-theorem) therefore supplies neighbourhoods on which $f$ has a continuously differentiable, hence [differentiable](../../../analysis.md#differentiable-function), inverse. Concretely, if $(u,v)=f(x,y)$, the local inverse is the restriction of

$$
\boxed{y=v^{1/5},\qquad x=(u-v^{2/5})^3},
$$

which is continuously differentiable near the image whenever $y\ne0$.

## 4G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4g/a">a</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/a/solution">Solution</h4>

↑ **Parent:** [A](#4g/a)

Suppose for contradiction that the [continuous image of a connected space](../../../geometry-and-topology.md#continuous-image-of-a-connected-space) $Y=f(X)$ is disconnected. Then there are disjoint nonempty sets $U,V$, open in the [subspace topology](../../../topology.md#subspace-topology) on $Y$, with $Y=U\cup V$. By [continuity](../../../calculus.md#continuous-function), $f^{-1}(U)$ and $f^{-1}(V)$ are disjoint open subsets of $X$; by [surjectivity](../../../algebra.md#surjective-function) both are nonempty, and their union is $X$. This is a [separation of a topological space](../../../geometry-and-topology.md#separation-of-a-topological-space) of $X$, contradicting that $X$ is a [connected space](../../../geometry-and-topology.md#connected-space). Hence $Y$ is connected.

<h3 id="4g/b">b</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/b/solution">Solution</h4>

↑ **Parent:** [B](#4g/b)

First recall from the [least-upper-bound property](../../../real-analysis.md#least-upper-bound-property) that every [real interval](../../../real-analysis.md#interval-mathematics) is connected. For completeness, if $[a,b]=U\cup V$ were a separation with $a\in U$, let $s$ be the [supremum](../../../real-analysis.md#supremum) of the points $t$ for which $[a,t]$ remains in $U$. Relative openness rules out both $s\in U$ and $s\in V$: in the first case one can move slightly to the right while staying in $U$, and in the second one finds points of $V$ slightly to the left of $s$, contrary to the definition of $s$. Thus no separation exists.

Part (a) now makes $g([0,1])$ a [connected subset of the real line](../../../geometry-and-topology.md#connected-subset-of-the-real-line). Such a set is an interval: if it contained $u<v$ but omitted $y\in(u,v)$, its intersections with $(-\infty,y)$ and $(y,\infty)$ would separate it. Since $g([0,1])$ contains $g(0)$ and $g(1)$, it consequently contains every number between them. Therefore for each such $y$ there is an $x\in[0,1]$ with $\boxed{g(x)=y}$. This derives the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) from connectedness.

## 5B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

For an axisymmetric separated solution of the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) whose angular factor is the [Legendre polynomial](../../../differential-equation.md#legendre-polynomial) $P_n(\cos\theta)$, the radial [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) has the two powers $r^n$ and $r^{-n-1}$. Thus

$$
\boxed{\Phi(r,\theta,\phi)=(A r^n+B r^{-n-1})P_n(\cos\theta)}
$$

for constants $A,B$.

Write $x=\cos\theta$. Since $3\cos(2\theta)=6x^2-3=4P_2(x)-P_0(x)$, only the [spherical harmonics](../../../analysis.md#spherical-harmonic) of degrees zero and two occur. The degree-zero radial coefficient satisfying its two [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) is $1-2/r$. For degree two, write $Cr^2+Dr^{-3}$; then

$$
C+D=4,
\qquad 4C+\frac D8=0,
$$

so $C=-4/31$ and $D=128/31$. By linearity and uniqueness of this [boundary value problem](../../../differential-equation.md#boundary-value-problem),

$$
\boxed{\Phi(r,\theta)=1-\frac2r+
\frac4{31}\left(\frac{32}{r^3}-r^2\right)P_2(\cos\theta)}.
$$

Direct substitution at $r=1,2$ verifies both boundary values.

## 6A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

The free-space [Green function of the Laplacian](../../../partial-differential-equation.md#green-function-of-the-laplacian) for the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) gives the [electric potential](../../../electromagnetism.md#electric-potential)

$$
\boxed{\phi(\mathbf x)=\frac1{4\pi\epsilon_0}
\int_{\mathbb R^3}\frac{\rho(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x'}.
$$

For $r=|\mathbf x|\gg R$, its [electric multipole expansion](../../../electromagnetism.md#electric-multipole-expansion) begins with

$$
\frac1{|\mathbf x-\mathbf x'|}
=\frac1r+\frac{\widehat{\mathbf x}\cdot\mathbf x'}{r^2}+O(r^{-3}).
$$

Define the [total electric charge](../../../electromagnetism.md#electric-charge) and [electric dipole moment](../../../electromagnetism.md#electric-dipole-moment) by

$$
Q=\int\rho(\mathbf x')\,d^3x',
\qquad
\mathbf p=\int\mathbf x'\rho(\mathbf x')\,d^3x'.
$$

Then

$$
\boxed{\phi(\mathbf x)=\frac1{4\pi\epsilon_0}
\left(\frac Qr+\frac{\mathbf p\cdot\widehat{\mathbf x}}{r^2}+O(r^{-3})\right)}.
$$

The analogous solution for the [magnetic vector potential](../../../electromagnetism.md#magnetic-vector-potential) is

$$
\boxed{\mathbf A(\mathbf x)=\frac{\mu_0}{4\pi}
\int_{\mathbb R^3}\frac{\mathbf J(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x'}.
$$

Its apparent $r^{-1}$ coefficient is $\mu_0(4\pi)^{-1}\int\mathbf J\,d^3x'$. For each component, the supplied identity and the [divergence-free vector field](../../../fluid-mechanics.md#divergence-free-vector-field) condition give

$$
\int J_i\,d^3x'
=\int\frac{\partial}{\partial x'_j}(x'_iJ_j)\,d^3x'.
$$

The [divergence theorem](../../../calculus.md#divergence-theorem) turns this into a surface integral outside the compact support of the [current density](../../../electromagnetism.md#current-density), where $\mathbf J=0$. Hence $\int\mathbf J\,d^3x'=0$, so the $1/r$ term vanishes.

## 7C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

The velocity field is [incompressible](../../../fluid-mechanics.md#incompressible-flow) because

$$
\nabla\cdot\mathbf u
=\frac{\partial u_x}{\partial x}+\frac{\partial u_y}{\partial y}
=\cos x\cos y-\cos x\cos y=0.
$$

With the convention $u_x=\psi_y$ and $u_y=-\psi_x$, a [stream function](../../../fluid-mechanics.md#stream-function) is

$$
\boxed{\psi(x,y)=\sin x\sin y}.
$$

The [vorticity](../../../fluid-mechanics.md#vorticity) is vertical:

$$
\boldsymbol\omega=\nabla\times\mathbf u
=(0,0,\partial_xu_y-\partial_yu_x)
=\boxed{(0,0,2\sin x\sin y)}=2\psi\,\mathbf e_z.
$$

For a steady inviscid incompressible flow, the [vorticity equation](../../../physics.md#vorticity-equation) is $(\mathbf u\cdot\nabla)\boldsymbol\omega=(\boldsymbol\omega\cdot\nabla)\mathbf u$. Here the right side is zero because the flow is independent of $z$, while the left side is $2(\mathbf u\cdot\nabla\psi)\mathbf e_z=0$ because velocity is tangent to the level sets of $\psi$. Thus the equation is satisfied.

The [streamlines](../../../fluid-mechanics.md#streamline) are the level curves $\sin x\sin y=\text{constant}$. The lines $x=\pi$ and $y=\pi$, together with the boundary, are separatrices; each of the four cells contains closed nested curves around a centre at $(\pi/2,\pi/2)$, $(3\pi/2,\pi/2)$, $(\pi/2,3\pi/2)$, or $(3\pi/2,3\pi/2)$.

<a id="7c/image-streamlines-of-a-cellular-fluid-flow"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2-cellular-flow-streamlines.png)

**[Figure 1](#7c/image-streamlines-of-a-cellular-fluid-flow). Streamlines of a cellular fluid flow**.

## 8H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8h/a">a</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/a/solution">Solution</h4>

↑ **Parent:** [A](#8h/a)

Let $S=\sum_{i=1}^nX_i$ be the number of heads. The [likelihood function](../../../statistical-modelling.md#likelihood-function) for the [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) sample is proportional to $\theta^S(1-\theta)^{n-S}$. A [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) prior on $[0,1]$ is the $\operatorname{Beta}(1,1)$ distribution, so [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy) gives the [posterior distribution](../../../statistical-inference.md#bayesian-posterior)

$$
\boxed{\theta\mid X_1,\ldots,X_n\sim\operatorname{Beta}(S+1,n-S+1)}.
$$

<h3 id="8h/b">b</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/b/solution">Solution</h4>

↑ **Parent:** [B](#8h/b)

The [quadratic loss](../../../statistical-inference.md#squared-error-loss), also called squared-error loss, for reporting an action $a$ when the parameter is $\theta$ is

$$
\boxed{L(\theta,a)=(a-\theta)^2}.
$$

<h3 id="8h/c">c</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/c/solution">Solution</h4>

↑ **Parent:** [C](#8h/c)

For any action $a$, decompose the posterior expected [quadratic loss](../../../statistical-inference.md#squared-error-loss) around the [posterior mean](../../../statistical-inference.md#posterior-mean):

$$
\mathbb E[(a-\theta)^2\mid X]
=(a-\mathbb E[\theta\mid X])^2+\operatorname{Var}(\theta\mid X).
$$

The unique minimizer is therefore the [Bayes estimator under squared error loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss). Using the mean of the posterior [Beta distribution](../../../probability-theory.md#beta-distribution) gives

$$
\boxed{\widehat\theta=\mathbb E[\theta\mid X]
=\frac{S+1}{n+2}}.
$$

Under repeated sampling at parameter value $\theta$, $S$ has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with expected value $n\theta$. Consequently

$$
\boxed{\mathbb E_\theta[\widehat\theta]=\frac{n\theta+1}{n+2}},
$$

so its [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator) is $(1-2\theta)/(n+2)$.

## 9H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9h/solution">Solution</h3>

↑ **Parent:** [9H](#9h)

The [Lagrange sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem) for maximizing $f$ subject to $g_i\geq0$ and $h_j=0$ states that if a feasible point $x^*$ and multipliers $\lambda_i\geq0,\mu_j$ satisfy complementary slackness and $x^*$ globally maximizes the [Lagrangian function in constrained optimization](../../../calculus-of-variations.md#lagrangian-function-in-constrained-optimization)

$$
L(x)=f(x)+\sum_i\lambda_i g_i(x)+\sum_j\mu_jh_j(x),
$$

then $x^*$ globally maximizes $f$ on the feasible set.

For the equality constraint, take

$$
L=\log x+\log y+\log z+\lambda(1-x^2-y^2-z^2).
$$

The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations give

$$
\frac1x=2\lambda x,
\qquad
\frac1y=2\lambda y,
\qquad
\frac1z=2\lambda z,
$$

so positivity and the constraint imply

$$
x=y=z=\frac1{\sqrt3},
\qquad \lambda=\frac32.
$$

For this multiplier, $L$ is a [strictly concave function](../../../real-analysis.md#strictly-concave-function) on the positive octant and its stationary point is its unique global maximum. The sufficiency theorem therefore proves that the constrained maximum is

$$
\boxed{\max\log(xyz)=\log\frac1{3\sqrt3}=-\frac32\log3}.
$$

For $x^2+y^2+z^2\leq1$, use $g=1-x^2-y^2-z^2$. The same point and multiplier satisfy feasibility, stationarity, $\lambda\geq0$, and [complementary slackness](../../../mathematical-optimization.md#complementary-slackness), and they again globally maximize the Lagrangian. Hence the answer is unchanged. Equivalently, any point with strict inequality can be radially scaled outward, increasing all three positive coordinates and therefore increasing $\log(xyz)$.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

If $A$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), then

$$
BA=A^{-1}(AB)A.
$$

**Thus $AB$ and $BA$ are [similar matrices](../../../linear-algebra.md#matrix-similarity), and similar matrices have the same [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial).**

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

For all but finitely many $s\in\mathbb C$, the matrix $A-sI$ is invertible. Part (a), applied to $A-sI$ and $B$, then gives

$$
\det\!\left(tI-(A-sI)B\right)
=\det\!\left(tI-B(A-sI)\right).
$$

Both sides are [polynomials](../../../polynomial.md) in the two variables $s,t$. Since they agree for infinitely many values of $s$, their coefficients as polynomials in $s$ agree. Setting $s=0$ yields

$$
\boxed{\det(tI-AB)=\det(tI-BA)}
$$

even when $A$ is [singular](../../../linear-algebra.md#singular-matrix).

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

Take

$$
A=\begin{pmatrix}1&0\\0&0\end{pmatrix},
\qquad
B=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
$$

Then $AB=B\ne0$ and $(AB)^2=0$, whereas $BA=0$. Hence their [minimal polynomials](../../../linear-operator-theory.md#minimal-polynomial) are

$$
\boxed{m_{AB}(t)=t^2,\qquad m_{BA}(t)=t}.
$$

<h3 id="10f/d">d</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/d/solution">Solution</h4>

↑ **Parent:** [D](#10f/d)

For every nonnegative integer $k$,

$$
(BA)^{k+1}=B(AB)^kA.
$$

Consequently, if $m_{AB}(AB)=0$, then

$$
(BA)m_{AB}(BA)=B\,m_{AB}(AB)A=0.
$$

By the divisibility characterization of the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial),

$$
m_{BA}(t)\mid t,m_{AB}(t).
$$

Interchanging $A$ and $B$ also gives $m_{AB}(t)\mid t,m_{BA}(t)$. Therefore the [Minimal polynomials of AB and BA](../../../linear-operator-theory.md#minimal-polynomials-of-ab-and-ba) can differ only in the exponent of the factor $t$, and that exponent differs by at most one.

If $AB$ is [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix), its minimal polynomial has no repeated roots. The preceding divisibility says that every nonzero [Jordan block](../../../linear-operator-theory.md#jordan-block) of $BA$ has size one and every zero-eigenvalue block has size at most two. Squaring $BA$ preserves the one-dimensional nonzero blocks and sends every size-at-most-two nilpotent block to zero. Thus the [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) of $(BA)^2$ is diagonal, so

$$
\boxed{AB\text{ diagonalizable}\ \Longrightarrow\ (BA)^2\text{ diagonalizable}}.
$$

## 11G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11g/a">a</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/a/solution">Solution</h4>

↑ **Parent:** [A](#11g/a)

Because $f$ is [irreducible](../../../polynomial.md#irreducible-polynomial), the ideal $(f)$ is maximal in the [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $k[X]$. Hence

$$
F=k[X]/(f)
$$

is a [field extension](../../../algebra.md#field-extension) of $k$. Let $\alpha=X+(f)\in F$. Evaluation in the quotient gives $f(\alpha)=0$, and the [factor theorem](../../../polynomial.md#factor-theorem) in $F[X]$ gives

$$
\boxed{f(X)=(X-\alpha)g(X)}
$$

for some $g\in F[X]$. This is the standard [adjoining a root of an irreducible polynomial](../../../algebra.md#adjoining-a-root-of-an-irreducible-polynomial) construction.

<h3 id="11g/b">b</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/b/solution">Solution</h4>

↑ **Parent:** [B](#11g/b)

Proceed by induction on $d=\deg f$. A nonconstant [polynomial](../../../polynomial.md) over a [field](../../../algebra.md#field) has an irreducible factor $h$. Part (a) gives an extension $k_1/k$ containing a root $\alpha_1$ of $h$, hence of $f$. The factor theorem gives

$$
f(X)=(X-\alpha_1)f_1(X),
\qquad f_1\in k_1[X],
$$

where $f_1$ is monic of degree $d-1$. Apply the induction hypothesis over $k_1$ and compose the resulting field extensions. The final field $F$ contains roots $\alpha_1,\ldots,\alpha_d$ and

$$
\boxed{f(X)=\prod_{i=1}^d(X-\alpha_i)}.
$$

Equivalently, every polynomial has a [splitting field](../../../galois-theory.md#splitting-field).

<h3 id="11g/c">c</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/c/solution">Solution</h4>

↑ **Parent:** [C](#11g/c)

Put $q=p^n$. Every extension of $k=\mathbb F_p$ has [characteristic](../../../algebra.md#characteristic-of-a-field) $p$, so the iterated [Frobenius endomorphism](../../../galois-theory.md#frobenius-endomorphism) satisfies

$$
(a+b)^q=a^q+b^q,
\qquad
(ab)^q=a^qb^q.
$$

The root set is $K=\{a\in F:a^q=a\}$. It contains $0$ and $1$. If $a,b\in K$, then

$$
(a-b)^q=a^q-b^q=a-b,
\qquad
(ab)^q=a^qb^q=ab,
$$

so it is closed under subtraction and multiplication. If $a\in K$ is nonzero, then

$$
(a^{-1})^q=(a^q)^{-1}=a^{-1}.
$$

Thus $K$ is closed under multiplicative inverses as well, and is therefore a [field](../../../algebra.md#field). This is the [polynomial characterization of a finite field](../../../algebra.md#polynomial-characterization-of-a-finite-field); in fact it is the [finite field](../../../algebra.md#finite-field) with $q$ elements, since $X^q-X$ has degree $q$ and no repeated roots.

## 12E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12e/a">a</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/a/i">i</h4>

↑ **Parent:** [A](#12e/a)

<h5 id="12e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#12e/a/i)

Two [norms](../../../functional-analysis.md#norm) $\|\cdot\|$ and $\|\cdot\|'$ on one [vector space](../../../vector-space.md) are [Lipschitz equivalent](../../../functional-analysis.md#equivalent-norms) when constants $c,C>0$ exist such that

$$
\boxed{c\|v\|\leq\|v\|'\leq C\|v\|\quad\text{for every }v}.
$$

<h4 id="12e/a/ii">ii</h4>

↑ **Parent:** [A](#12e/a)

<h5 id="12e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12e/a/ii)

Choose a [basis](../../../vector-space.md#basis) of the finite-dimensional vector space and let $|x|_\infty$ be the maximum absolute coordinate. For any norm $N$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
N(x)\leq\left(\sum_{i=1}^nN(e_i)\right)|x|_\infty,
$$

so $N$ is [continuous](../../../calculus.md#continuous-function) in the coordinate topology. On the compact set $\{x:|x|_\infty=1\}$, the positive continuous function $N$ attains a positive minimum $m$ and a finite maximum $M$. By [absolute homogeneity](../../../functional-analysis.md#norm),

$$
m|x|_\infty\leq N(x)\leq M|x|_\infty.
$$

This proves the [equivalence of norms in finite dimensions](../../../topological-vector-space.md#equivalence-of-norms-in-finite-dimensions): every norm is equivalent to the maximum norm, and [transitivity](../../../set-theory.md#transitive-relation) of these inequalities proves that any two norms on a [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) are Lipschitz equivalent.

<h4 id="12e/a/iii">iii</h4>

↑ **Parent:** [A](#12e/a)

<h5 id="12e/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#12e/a/iii)

Suppose

$$
c\|v\|\leq\|v\|'\leq C\|v\|.
$$

If $(v_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in $\|\cdot\|$, then

$$
\|v_n-v_m\|'\leq C\|v_n-v_m\|\longrightarrow0.
$$

Conversely, $\|v_n-v_m\|\leq c^{-1}\|v_n-v_m\|'\to0$. Hence the sequence is Cauchy for one norm exactly when it is Cauchy for the other.

<h3 id="12e/b">b</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/b/i">i</h4>

↑ **Parent:** [B](#12e/b)

<h5 id="12e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12e/b/i)

For each positive integer $N$, let $x^{(N)}$ have its first $N$ coordinates equal to one and all later coordinates zero. This is an element of the [l-p sequence space](../../../banach-space.md#l-p-sequence-space) for every finite $p$, and

$$
\|x^{(N)}\|_\infty=1,
\qquad
\|x^{(N)}\|_p=N^{1/p}.
$$

**No constant can bound $\|x\|_p$ by a fixed multiple of $\|x\|_\infty$ for all $N$.** Thus $\|\cdot\|_p$ and $\|\cdot\|_\infty$ are not Lipschitz equivalent.

<h4 id="12e/b/ii">ii</h4>

↑ **Parent:** [B](#12e/b)

<h5 id="12e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12e/b/ii)

For $1\leq p<q<\infty$, the same finitely supported sequence gives

$$
\frac{\|x^{(N)}\|_p}{\|x^{(N)}\|_q}
=N^{1/p-1/q}\longrightarrow\infty.
$$

One of the two inequalities required for [equivalent norms](../../../functional-analysis.md#equivalent-norms) therefore fails. Hence

$$
\boxed{\text{no pair }1\leq p<q<\infty\text{ gives Lipschitz-equivalent norms on }V}.
$$

## 13D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13d/solution">Solution</h3>

↑ **Parent:** [13D](#13d)

Let $v_1,v_2\ne0$ be tangent vectors to the two smooth curves at $p$. [complex differentiability at a point](../../../complex-analysis.md#complex-differentiability-at-a-point) gives

$$
f(p+h)=f(p)+f'(p)h+o(|h|).
$$

When $f'(p)\ne0$, its real derivative is multiplication by a nonzero complex number, which is a rotation followed by a positive scaling. It therefore preserves the angle between $v_1$ and $v_2$, so $f$ is [conformal](../../../geometry-and-topology.md#conformal-map) at $p$. The condition is essential: $f(z)=z^2$ has $f'(0)=0$ and sends rays making angle $\pi/4$ at zero to rays making angle $\pi/2$.

For $J(z)=z+z^{-1}$,

$$
J(z)=J(w)\quad\Longleftrightarrow\quad (z-w)(zw-1)=0.
$$

If $z,w$ both satisfy $|z|>1$, or both satisfy $0<|z|<1$, the alternative $zw=1$ is impossible unless the points lie on the omitted unit circle. Hence $J$ is one-to-one on each region. Also $J'(z)=1-z^{-2}$ has no zero there, so the restrictions are conformal. Solving $z^2-wz+1=0$ shows that $w\in[-2,2]$ exactly when both roots lie on the unit circle; otherwise one root is inside and the other outside. Thus each region has image

$$
\boxed{\mathbb C\setminus[-2,2]}.
$$

Taking the reciprocal of the interior restriction and filling its removable value at zero gives

$$
\boxed{g(z)=\frac1{J(z)}=\frac{z}{1+z^2}}.
$$

The reciprocal sends $\mathbb C\setminus[-2,2]$ onto

$$
\mathbb C\setminus\bigl(({-\infty},-1/2]\cup[1/2,\infty)\bigr),
$$

and $g(0)=0$. Therefore $g$ is the required one-to-one conformal map from the [unit disc](../../../topology.md#unit-disc).

## 14E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14e/solution">Solution</h3>

↑ **Parent:** [14E](#14e)

A [smooth surface](../../../differential-geometry.md#smooth-surface) in $\mathbb R^3$ is a subset locally parametrized by a smooth map of two variables whose derivative has rank two and which is a homeomorphism onto its image.

Writing $\rho=\sqrt{x^2+y^2}$, the first surface equation becomes

$$
(\rho-2\sqrt2)^2+z^2=1.
$$

It is the [torus](../../../topology.md#torus) of major radius $R=2\sqrt2$ and minor radius $r=1$, with smooth parametrization

$$
\boxed{X(u,v)=((2\sqrt2+\cos v)\cos u,
(2\sqrt2+\cos v)\sin u,\sin v)},
\qquad u,v\in\mathbb R/(2\pi\mathbb Z).
$$

Since $R>r$, this is an embedding. The [Gaussian curvature of a torus](../../../differential-geometry.md#gaussian-curvature-of-a-torus) is

$$
\boxed{K(u,v)=\frac{\cos v}{2\sqrt2+\cos v}}.
$$

For the second surface, use the [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation)

$$
X=\frac{x+z}{\sqrt2},
\qquad Y=y,
\qquad Z=\frac{z-x}{\sqrt2}.
$$

Its equation becomes the same torus equation $(\sqrt{X^2+Y^2}-2\sqrt2)^2+Z^2=1$. Orthogonal transformations are Euclidean [isometries](../../../riemannian-geometry.md#isometry) and preserve [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature). Curvature vanishes where $\cos v=0$, equivalently $Z=\pm1$. In the original coordinates the zero-curvature points are therefore exactly

$$
\boxed{z-x=\pm\sqrt2,
\qquad (x+z)^2+2y^2=16}.
$$

## 15A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15a/solution">Solution</h3>

↑ **Parent:** [15A](#15a)

The two [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) are

$$
\frac d{dx}\frac{\partial f}{\partial u'}-\frac{\partial f}{\partial u}=0,
\qquad
\frac d{dx}\frac{\partial f}{\partial w'}-\frac{\partial f}{\partial w}=0.
$$

Differentiating $\kappa=f-u'f_{u'}-w'f_{w'}$ along an extremal and using these equations gives $d\kappa/dx=f_x$. Hence the [Beltrami identity](../../../analysis.md#beltrami-identity) makes $\kappa$ constant when $f$ has no explicit dependence on $x$. If $f$ omits $u$ or $w$, that variable is a [cyclic coordinate](../../../classical-mechanics.md#cyclic-coordinate) and the corresponding momentum $f_{u'}$ or $f_{w'}$ is an additional [first integral](../../../differential-equation.md#first-integral); continuous symmetries give the analogous conserved quantities through [Noether's theorem](../../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry).

Put $A=1-m/u$. Since $w$ is cyclic,

$$
2Aw'=2\lambda,
\qquad Aw'=\lambda
$$

for a constant $\lambda$. The Beltrami integral is

$$
\kappa=f-u'f_{u'}-w'f_{w'}
=A^{-1}u'^2-Aw'^2
=A^{-1}(u'^2-\lambda^2).
$$

Therefore

$$
\boxed{u'^2=\lambda^2+\kappa\left(1-\frac mu\right)}.
$$

If $\kappa=-\lambda^2$, then $u'^2=\lambda^2m/u$ and

$$
\frac{dw}{du}=\pm\frac{(u/m)^{3/2}}{u/m-1}.
$$

For $z>1$, define

$$
F(z)=\frac23z^{3/2}+2z^{1/2}
+\log\frac{\sqrt z-1}{\sqrt z+1};
$$

the hinted identity gives $F'(z)=z^{3/2}/(z-1)$. Hence $w=C\pm mF(u/m)$. Because $F(z)\to+\infty$ as $z\to\infty$, the prescribed limit selects the minus sign:

$$
\boxed{w(u)=C-m\left[
\frac23\left(\frac um\right)^{3/2}
+2\sqrt{\frac um}
+\log\frac{\sqrt{u/m}-1}{\sqrt{u/m}+1}
\right]}.
$$

As $u\downarrow m$, the logarithm tends to $-\infty$, so every such solution satisfies $\boxed{w\to+\infty}$.

## 16D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16d/solution">Solution</h3>

↑ **Parent:** [16D](#16d)

Multiply the [Gegenbauer differential equation](../../../analysis.md#gegenbauer-differential-equation) by

$$
w(x)=(1-x^2)^{\alpha-1/2}.
$$

It becomes the [Sturm-Liouville form](../../../analysis.md#sturm-liouville-form)

$$
\frac d{dx}\left((1-x^2)^{\alpha+1/2}y'\right)
+n(n+2\alpha)w(x)y=0.
$$

For two polynomial solutions of degrees $m\ne n$, multiply their equations crosswise, subtract, and integrate over $(-1,1)$. The boundary term vanishes because $\alpha>0$ and $(1-x^2)^{\alpha+1/2}\to0$. Since the eigenvalues $n(n+2\alpha)$ are distinct,

$$
\boxed{\int_{-1}^1C_m^\alpha(x)C_n^\alpha(x)(1-x^2)^{\alpha-1/2}\,dx=0}.
$$

Thus $a=-1$, $b=1$, and the displayed function is the weight.

Every interior root is simple: a solution and its derivative cannot both vanish at an ordinary point of a second-order linear differential equation unless the solution is identically zero. Let $x_1,\ldots,x_k$ be all interior roots and put $q(x)=\prod_i(x-x_i)$. If $k<n$, then $q$ has degree below $n$, so [orthogonality](../../../numerical-analysis.md#orthogonal-polynomial) gives

$$
\int_{-1}^1C_n^\alpha(x)q(x)w(x)\,dx=0.
$$

But $C_n^\alpha/q$ has no zero and constant sign on $(-1,1)$, whence the integrand $q(x)^2(C_n^\alpha(x)/q(x))w(x)$ has one strict sign except at finitely many points. Its integral cannot vanish, a contradiction. Therefore $k=n$: all $n$ roots are real, simple, and lie in $(-1,1)$.

## 17B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17b/solution">Solution</h3>

↑ **Parent:** [17B](#17b)

The total [angular momentum operator](../../../quantum-mechanics.md#angular-momentum-operator) is

$$
\mathbf L^2=L_x^2+L_y^2+L_z^2.
$$

Using the cyclic [orbital angular momentum commutation relations](../../../quantum-mechanics.md#orbital-angular-momentum-commutation-relations),

$$
[L_z,L_x^2]=i\hbar(L_yL_x+L_xL_y),
\qquad
[L_z,L_y^2]=-i\hbar(L_xL_y+L_yL_x),
$$

while $[L_z,L_z^2]=0$; hence $\boxed{[L_z,\mathbf L^2]=0}$. In Cartesian coordinates,

$$
\boxed{L_z=-i\hbar\left(x\frac{\partial}{\partial y}-y\frac{\partial}{\partial x}\right)}.
$$

Because $L_z(x+iy)=\hbar(x+iy)$ and it annihilates $z$ and every radial function,

$$
L_z[(x+iy)^mz^nf(r)]=m\hbar(x+iy)^mz^nf(r).
$$

Replacing $i$ by $-i$ gives eigenvalue $-m\hbar$.

The six-dimensional space splits into the five trace-free quadratic [spherical harmonics](../../../analysis.md#spherical-harmonic) with $\ell=2$ and one radial state with $\ell=0$. A simultaneous eigenbasis for $L_z$ and $\mathbf L^2$ is

$$
\begin{array}{c|c|c}
\text{state}&L_z&\mathbf L^2\\ \hline
(x+iy)^2f(r)&2\hbar&6\hbar^2\\
(x+iy)zf(r)&\hbar&6\hbar^2\\
(2z^2-x^2-y^2)f(r)&0&6\hbar^2\\
(x-iy)zf(r)&-\hbar&6\hbar^2\\
(x-iy)^2f(r)&-2\hbar&6\hbar^2\\
(r^2-3)f(r)&0&0
\end{array}
$$

where the eigenvalue $\ell(\ell+1)\hbar^2$ of $\mathbf L^2$ was used. Every displayed state is a complex [linear combination](../../../vector-space.md#linear-combination) of the original six energy eigenstates, so it is still an energy eigenstate at the same level.

## 18A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18a/solution">Solution</h3>

↑ **Parent:** [18A](#18a)

For a moving circuit, [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) states that the [electromotive force](../../../electromagnetism.md#electromotive-force)

$$
\mathcal E=\oint_C(\mathbf E+\mathbf v\times\mathbf B)\cdot d\boldsymbol\ell
$$

equals $-d\Phi_B/dt$, where $\Phi_B=\int_S\mathbf B\cdot d\mathbf S$ is the [magnetic flux](../../../electromagnetism.md#magnetic-flux) through any spanning surface. Choose the upward normal. The horizontal square has

$$
\Phi_B=(-2bz)(2a)^2=-8ba^2z,
$$

so [Ohm's law](../../../electromagnetism.md#ohm-s-law) gives the induced current

$$
\boxed{I=\frac{\mathcal E}{R}=\frac{8ba^2}{R}\dot z}
$$

with positive current taken counterclockwise from above.

On the edge $x=a$, $d\boldsymbol\ell=dy\,\mathbf e_y$. The [magnetic force on a current-carrying wire](../../../electromagnetism.md#magnetic-force-on-a-current-carrying-wire) is $d\mathbf F=I,d\boldsymbol\ell\times\mathbf B$, hence

$$
\mathbf F_{x=a}
=Ib\int_{-a}^a\mathbf e_y\times(a\mathbf e_x+y\mathbf e_y-2z\mathbf e_z)\,dy
=\boxed{-4abIz\,\mathbf e_x-2a^2bI\,\mathbf e_z}.
$$

The ratio of the horizontal to vertical magnitudes is $2|z|/a$, so the directed force makes angle $\tan^{-1}(2z/a)$ with the vertical, with the sign fixing the horizontal side.

The horizontal forces on opposite edges cancel, while all four vertical contributions add:

$$
\boxed{\mathbf F_{\rm em}=-8ba^2I\,\mathbf e_z
=-\frac{(8ba^2)^2}{R}\dot z\,\mathbf e_z}.
$$

This is an electromagnetic drag force opposing the motion, as required by [Lenz's law](../../../electromagnetism.md#lenz-s-law). Including gravity gives

$$
m\ddot z=-mg-\frac{(8ba^2)^2}{R}\dot z.
$$

At the [terminal velocity](../../../electromagnetism.md#terminal-speed-of-a-falling-conducting-loop), $\ddot z=0$, and the constant downward speed has magnitude

$$
\boxed{v_{\rm terminal}=\frac{Rmg}{(8ba^2)^2}}.
$$

## 19C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19c/solution">Solution</h3>

↑ **Parent:** [19C](#19c)

The [linear least-squares problem](../../../linear-algebra.md#linear-least-squares-problem) is to choose $x\in\mathbb R^n$ minimizing the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) of the residual:

$$
\boxed{\min_x\|Ax-b\|_2}.
$$

For a [QR decomposition](../../../linear-algebra.md#qr-decomposition) $A=QR$, orthogonality of $Q$ gives $\|Ax-b\|_2=\|Rx-Q^Tb\|_2$. If $A$ has full column rank and $R=\binom{R_1}{0}$ is in standard form with invertible upper-triangular $R_1\in\mathbb R^{n\times n}$, the minimizer solves $R_1x=(Q^Tb)_{1:n}$.

Applying the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) to the columns of the given matrix yields

$$
Q=\frac12\begin{pmatrix}
1&1&1&1\\
1&-1&1&-1\\
1&1&-1&-1\\
1&-1&-1&1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
2&1&1\\
0&1&0\\
0&0&1\\
0&0&0
\end{pmatrix}.
$$

Indeed, $Q$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) and $A=QR$. Moreover,

$$
Q^Tb=(6,-2,-3,1)^T.
$$

Back substitution in the leading triangular system gives

$$
x_2=-2,
\qquad x_3=-3,
\qquad 2x_1+x_2+x_3=6,
$$

so the unique least-squares solution is

$$
\boxed{x=(11/2,-2,-3)^T}.
$$

The unused final transformed residual component is $1$, so the minimum residual norm is $1$.

## 20H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="20h/a">a</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/a/solution">Solution</h4>

↑ **Parent:** [A](#20h/a)

Until the walk first reaches $B$, it is the [simple random walk](../../../markov-process.md#simple-random-walk) on a path of length $n$ with reflection at the endpoint $A$. If $h_i$ is the [expected hitting time](../../../markov-process.md#expected-hitting-time) of $B$ from the vertex at distance $i$ from $A$, then

$$
h_n=0,
\qquad h_0=1+h_1,
\qquad h_i=1+\frac12(h_{i-1}+h_{i+1})\quad(1\leq i<n).
$$

Solving this second-difference equation gives $h_i=n^2-i^2$. Therefore

$$
\boxed{\mathbb E_A[T_B]=n^2}.
$$

<h3 id="20h/b">b</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/b/solution">Solution</h4>

↑ **Parent:** [B](#20h/b)

A complete excursion from $B$ along any one arm and back to $B$ has mean length $L=2n$. This follows from the same path recurrence, or from [Kac's lemma](../../../probability-and-statistics.md#kac-s-lemma): the graph has $3n$ edges, the [stationary distribution](../../../markov-process.md#stationary-distribution) of simple random walk assigns mass $\deg(B)/(2|E|)=3/(6n)=1/(2n)$ to $B$, so its mean return time is $L=2n$.

Let $x$ be the mean time to hit $E$ starting at $B$. On each visit to $B$, the first step reaches $E$ with probability $1/3$; with probability $2/3$ it begins a wrong-arm excursion of mean duration $L$, after which the problem restarts. Thus

$$
x=\frac13+\frac23(L+x),
\qquad
x=1+2L=4n+1.
$$

The walk first takes mean time $n^2$ to reach $B$, so the requested time from $A$ is

$$
\boxed{\mathbb E_A[T_E]=n^2+4n+1=(n+2)^2-3}.
$$

<h3 id="20h/c">c</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/c/solution">Solution</h4>

↑ **Parent:** [C](#20h/c)

Let $v_i$ be the vertex $i$ steps from $B$ toward $C$, and let $x_i$ be the mean time to reach $v_{i+1}$ from $v_i$. Part (b) gives $x_0=4n+1$. For $1\leq i<n$, first-step analysis at $v_i$ gives

$$
x_i=\frac12\cdot1+\frac12(1+x_{i-1}+x_i),
$$

because a step to $v_{i-1}$ must be followed by a fresh passage of mean $x_{i-1}$ back to $v_i$ before trying again. Hence

$$
x_i=x_{i-1}+2=4n+1+2i.
$$

By the [Strong Markov property](../../../markov-process.md#strong-markov-property), the expected time from $B$ to $C$ is the sum of these successive passage times:

$$
\mathbb E_B[T_C]
=\sum_{i=0}^{n-1}x_i
=n(4n+1)+n(n-1)=5n^2.
$$

Adding the initial mean time $n^2$ from $A$ to $B$ gives

$$
\boxed{\mathbb E_A[T_C]=6n^2}.
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
