# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_1.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4G](#4g)
  - [Solution](#4g/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
  - [a](#5e/a)
    - [Solution](#5e/a/solution)
  - [b](#5e/b)
    - [Solution](#5e/b/solution)
- [6F](#6f)
  - [Solution](#6f/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10C](#10c)
  - [Solution](#10c/solution)
- [11B](#11b)
  - [Solution](#11b/solution)
- [12A](#12a)
  - [Solution](#12a/solution)
- [13F](#13f)
  - [Solution](#13f/solution)
- [14E](#14e)
  - [Solution](#14e/solution)
- [15G](#15g)
  - [Solution](#15g/solution)
- [16H](#16h)
  - [Solution](#16h/solution)
- [17E](#17e)
  - [Solution](#17e/solution)
- [18D](#18d)
  - [Solution](#18d/solution)
- [19D](#19d)
  - [Solution](#19d/solution)

## 1C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) $m_\beta(t)$ of the [linear map](../../../vector-space.md#linear-map) $\beta$ is the unique [monic polynomial](../../../polynomial.md#monic-polynomial) of smallest degree satisfying $m_\beta(\beta)=0$. An annihilating [polynomial](../../../polynomial.md) exists because the powers $I,\beta,\beta^2,\ldots$ lie in the finite-dimensional [vector space](../../../vector-space.md) $\operatorname{End}(V)$ and are therefore [linearly dependent](../../../vector-space.md#linear-dependence). If two monic annihilating [polynomials](../../../polynomial.md) had the same least degree, their difference would be an annihilating [polynomial](../../../polynomial.md) of smaller degree, so they coincide.

Write $m_\beta(t)=a_0+tq(t)$. If $a_0\ne0$, evaluation at the [linear map](../../../vector-space.md#linear-map) gives $\beta q(\beta)=-a_0I$. Since $\beta$ commutes with every [polynomial](../../../polynomial.md) in itself, this is a two-sided inverse:

$$
\boxed{\beta^{-1}=-\frac{q(\beta)}{a_0}}.
$$

Conversely, if $\beta$ is an [invertible linear map](../../../calculus.md#invertible-linear-map) and $a_0=0$, then $m_\beta(t)=tq(t)$ and multiplication of $\beta q(\beta)=0$ by $\beta^{-1}$ gives $q(\beta)=0$, contradicting the defining least degree. Thus **invertibility is equivalent to a nonzero constant term of the minimal polynomial**. In the zero-dimensional case the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is $1$ and the same conclusion holds.

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

The image is a [ring torus](../../../differential-geometry.md#ring-torus): a circle of radius $b$ is rotated about the vertical axis at distance $a$ from that axis. Put $r=\sqrt{x^2+y^2}$. Since $a>b$, every image point has $r>0$, and the image is precisely

$$
T=\{(x,y,z):(r-a)^2+z^2=b^2\}.
$$

Conversely, on this [level set](../../../topology.md#level-set) the pairs $((r-a)/b,z/b)$ and $(x/r,y/r)$ are unit vectors, so choosing their angles gives a preimage.

The specified angular rectangle removes two closed circles from the [torus](../../../topology.md#torus). More explicitly its image is

$$
U=T\setminus(C_u\cup C_v),\qquad
C_u=\{z=0,\ r=a+b\}\cap T,\quad
C_v=\{y=0,\ x>0\}\cap T.
$$

Here $C_u$ is the outer equatorial circle and $C_v$ is a meridian. The given openness property makes $U$ open in $T$. On $U$, the angles of $(r-a)+iz$ and $x+iy$ are uniquely chosen in $(0,2\pi)$; their continuous argument branches give the inverse $(x,y,z)\mapsto(u,v)$. Thus the restriction is a [homeomorphism](../../../topology.md#homeomorphism) onto $U$, and the inverse is locally [smooth](../../../analysis.md#smooth-function).

For the [immersion](../../../differential-geometry.md#immersion) condition, the two derivatives have [inner products](../../../linear-algebra.md#inner-product)

$$
\sigma_u\cdot\sigma_u=b^2,\qquad
\sigma_v\cdot\sigma_v=(a+b\cos u)^2,\qquad
\sigma_u\cdot\sigma_v=0.
$$

They are [linearly independent](../../../vector-space.md#linear-independence) everywhere, since $a+b\cos u\ge a-b>0$. Hence this is a smooth [embedded surface parametrization](../../../differential-geometry.md#embedded-surface-parametrization).

The angular cuts do not represent singularities of the [embedded torus of revolution](../../../topology.md#embedded-torus-of-revolution). To give a direct proof covering all points, define $F=(\sqrt{x^2+y^2}-a)^2+z^2-b^2$ on the open region $r>0$. On $T$,

$$
\nabla F=2\left((r-a)\frac{x}{r},(r-a)\frac{y}{r},z\right),\qquad
|\nabla F|=2b>0.
$$

The [implicit function theorem](../../../calculus.md#implicit-function-theorem) therefore describes $T$ near every point as a [smooth](../../../analysis.md#smooth-function) graph of two coordinates. **The whole torus is a smooth embedded surface.**

## 3F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

The [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) states that if $f$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on a neighborhood of a positively oriented simple closed contour $C$ and its interior, then for $w$ inside,

$$
f(w)=\frac1{2\pi i}\int_C\frac{f(z)}{z-w}\,dz.
$$

For the given counterclockwise circle, divide the rational function:

$$
\frac{z^3}{z^2+1}=z-\frac12\left(\frac1{z-i}+\frac1{z+i}\right).
$$

The [contour integral](../../../complex-analysis.md#contour-integral) of $z$ is zero because it has a primitive, while both points $\pm i$ lie inside the circle. Applying the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) to the constant function $1$ at each point gives

$$
\boxed{\int_{|z|=2}\frac{z^3}{z^2+1}\,dz=-2\pi i}.
$$

The sign reverses if the contour orientation is reversed.

## 4G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4g/solution">Solution</h3>

↑ **Parent:** [4G](#4g)

Use [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) coordinates $x^\mu=(ct,x,y,z)$ and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) of signature $(+,-,-,-)$. For a massive particle with three-velocity $\mathbf v=d\mathbf x/dt$ and $|\mathbf v|<c$, [proper time](../../../special-relativity.md#proper-time) satisfies

$$
c^2\,d\tau^2=c^2\,dt^2-|d\mathbf x|^2,\qquad
\frac{dt}{d\tau}=\gamma=\left(1-\frac{|\mathbf v|^2}{c^2}\right)^{-1/2}.
$$

Thus the [four-velocity](../../../special-relativity.md#four-velocity) components are

$$
\boxed{U^\mu=(\gamma c,\gamma v_x,\gamma v_y,\gamma v_z)}.
$$

Here upper indices indicate components in the chosen coordinates; lowering with the [Minkowski metric](../../../special-relativity.md#minkowski-metric) changes the signs of the spatial components. Its invariant product defined by the [Minkowski metric](../../../special-relativity.md#minkowski-metric) is

$$
U\cdot U=(U^0)^2-\sum_{j=1}^3(U^j)^2
=\gamma^2(c^2-|\mathbf v|^2)=c^2.
$$

The [four-momentum](../../../special-relativity.md#four-momentum) is $p^\mu=(E/c,\mathbf p)=mU^\mu$, so $E=\gamma mc^2$ and $\mathbf p=\gamma m\mathbf v$. The [Taylor expansion](../../../calculus.md#taylor-expansion) of the [Lorentz factor](../../../special-relativity.md#lorentz-factor) at small $|\mathbf v|/c$ is

$$
\gamma=1+\frac{|\mathbf v|^2}{2c^2}+O(|\mathbf v|^4/c^4).
$$

Consequently $\mathbf p=m\mathbf v+O(m|\mathbf v|^3/c^2)$, recovering ordinary [momentum](../../../classical-mechanics.md#momentum). At rest the [four-momentum](../../../special-relativity.md#four-momentum) has energy $E_0=mc^2$, so subtracting this [rest energy](../../../special-relativity.md#rest-energy) gives the [kinetic energy](../../../classical-mechanics.md#kinetic-energy)

$$
\boxed{K=E-E_0=(\gamma-1)mc^2
=\frac12m|\mathbf v|^2+O(m|\mathbf v|^4/c^2)}.
$$

Thus the nonrelativistic limit preserves the rest-energy offset as well as the usual [kinetic energy](../../../classical-mechanics.md#kinetic-energy).

## 5E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

For a two-dimensional [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) $\mathbf u=(u,v)$, the continuity equation is $u_x+v_y=0$. Locally, or globally on a [simply connected](../../../algebraic-topology.md#simply-connected-space) fluid region, this permits a [streamfunction](../../../fluid-mechanics.md#stream-function) with

$$
u=\psi_y,\qquad v=-\psi_x.
$$

Indeed, the one-form $-v\,dx+u\,dy$ is closed by incompressibility and hence is locally the differential of $\psi$. Conversely these expressions automatically give zero [divergence](../../../calculus.md#divergence) by equality of mixed derivatives.

A [streamline](../../../fluid-mechanics.md#streamline) at a fixed time is tangent to the instantaneous [velocity field](../../../fluid-mechanics.md#velocity-field). Along it,

$$
\frac{d\psi}{ds}=\nabla\psi\cdot\mathbf u
=\psi_x\psi_y-\psi_y\psi_x=0.
$$

Thus **streamlines are connected curves on which the streamfunction is constant**; wherever $\nabla\psi\ne0$, the [level curves](../../../topology.md#level-curve) have exactly the required tangent direction. At a [stagnation point](../../../fluid-mechanics.md#stagnation-point), the tangent is degenerate and distinct branches of a level set need not form a single streamline. For unsteady flow this argument fixes time: it does not identify [streamlines](../../../fluid-mechanics.md#streamline) with particle [pathlines](../../../fluid-mechanics.md#pathline).

<h3 id="5e/a">a</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/a/solution">Solution</h4>

↑ **Parent:** [A](#5e/a)

Integrating $\psi_y=x+\sin t$ and imposing $-\psi_x=-y$ gives the [streamfunction](../../../fluid-mechanics.md#stream-function)

$$
\boxed{\psi(x,y,t)=y(x+\sin t)}
$$

up to an arbitrary function of time. At the specified time, the [streamlines](../../../fluid-mechanics.md#streamline) are

$$
\boxed{y(x+1)=C}.
$$

For $C\ne0$, the connected branches are rectangular hyperbolas. The zero level consists of the lines $y=0$ and $x=-1$, with the [stagnation point](../../../fluid-mechanics.md#stagnation-point) $(-1,0)$ at their intersection; their half-lines and the stationary point are the distinct [streamlines](../../../fluid-mechanics.md#streamline).

<h3 id="5e/b">b</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/b/solution">Solution</h4>

↑ **Parent:** [B](#5e/b)

A particle [pathline](../../../fluid-mechanics.md#pathline) follows the time-dependent [velocity field](../../../fluid-mechanics.md#velocity-field), so its coordinates satisfy $\dot x-x=\sin t$ and $\dot y=-y$. The second equation and the initial data give $y=e^{-t}$. Using the [integrating factor](../../../differential-equation.md#integrating-factor) $e^{-t}$ in the first,

$$
e^{-t}x(t)=x_0+\int_0^t e^{-s}\sin s\,ds
=x_0+\frac12-\frac12e^{-t}(\sin t+\cos t).
$$

Therefore the complete [pathline](../../../fluid-mechanics.md#pathline) is

$$
\boxed{(x(t),y(t))
=\left((x_0+\tfrac12)e^t-\tfrac12(\sin t+\cos t),e^{-t}\right),\quad t\ge0}.
$$

If $x_0+\tfrac12\ne0$, its first coordinate grows without bound in magnitude. If $x_0=-\tfrac12$, the first coordinate remains bounded and periodic while $y\to0$. **The unique release coordinate giving a bounded particle path is $x_0=-1/2$.**

## 6F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6f/solution">Solution</h3>

↑ **Parent:** [6F](#6f)

For the [Cholesky decomposition](../../../linear-algebra.md#cholesky-decomposition) $A=LL^T$, choose $L$ lower triangular with positive diagonal whenever $A$ is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form). Successive entries are

$$
l_{11}=\sqrt2,\quad l_{21}=-2\sqrt2,\quad l_{31}=\sqrt2,\quad
l_{22}=\sqrt{\lambda+2}.
$$

The $(3,2)$ equation gives $l_{31}l_{21}+l_{32}l_{22}=2+3\lambda$, so $l_{32}=3\sqrt{\lambda+2}$. Finally,

$$
l_{33}^2=23+9\lambda-l_{31}^2-l_{32}^2=3.
$$

Thus for $\lambda>-2$,

$$
\boxed{L=\begin{pmatrix}
\sqrt2&0&0\\
-2\sqrt2&\sqrt{\lambda+2}&0\\
\sqrt2&3\sqrt{\lambda+2}&\sqrt3
\end{pmatrix}}.
$$

It is nonsingular, and for every nonzero vector $v$, $v^TAv=|L^Tv|^2>0$.

Necessity also follows from the leading principal determinants $2$, $2(\lambda+2)$ and $6(\lambda+2)$, or directly from the second elimination pivot. Hence

$$
\boxed{A\text{ is positive definite exactly when }\lambda>-2}.
$$

At $\lambda=-2$ the displayed limiting factor still satisfies $A=LL^T$, but has rank two and zero second diagonal entry: $A$ is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix), not [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form). For $\lambda<-2$, taking $v=(2,1,0)^T$ gives $v^TAv=\lambda+2<0$, so no real factor $LL^T$ exists.

## 7D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) of equal population probabilities, the three counts have a [multinomial distribution](../../../discrete-probability-distribution.md#multinomial-distribution) with probabilities $1/3$ and expected counts $100$ each. The [Pearson chi-squared goodness-of-fit test](../../../statistical-modelling.md#pearson-chi-squared-goodness-of-fit-test) uses

$$
X^2=\sum_{j=1}^3\frac{(O_j-100)^2}{100}
=\frac{(-8)^2+(-11)^2+19^2}{100}
=\boxed{5.46}.
$$

No probabilities have been estimated from the data, and the three counts sum to a fixed total. Hence the null reference [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) has $3-1=2$ [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom). The supplied $5\%$ upper critical value is $5.99$, and $5.46<5.99$. **At the 5% significance level there is insufficient evidence to reject equal popularity.**

The asymptotic [P-value](../../../statistical-modelling.md#p-value) is $\Pr(\chi_2^2\ge5.46)=e^{-5.46/2}\approx0.0652$. The expected counts are all large, so the approximation is appropriate if the sampled choices are independent and representative of this branch. The conclusion depends on the chosen [significance level](../../../statistical-modelling.md#significance-level); for instance, a $10\%$ test would reject. Nonrejection does not establish the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), and a survey at one branch does not by itself justify a population claim about every branch.

## 8D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Associate free real [dual variables](../../../mathematical-optimization.md#dual-variable) $u_i$ and $v_j$ with the row and column equality constraints. The [Lagrangian](../../../calculus-of-variations.md#lagrangian) for the [transportation problem](../../../mathematical-optimization.md#transportation-problem) is

$$
L(x,u,v)=\sum_i a_i u_i+\sum_j b_jv_j
+\sum_{i,j}(c_{ij}-u_i-v_j)x_{ij}.
$$

Its infimum over $x_{ij}\ge0$ is finite exactly when $u_i+v_j\le c_{ij}$ for every pair. The [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) therefore gives

$$
\boxed{\text{maximize }\sum_i a_i u_i+\sum_j b_jv_j
\quad\text{subject to }u_i+v_j\le c_{ij},\quad u_i,v_j\in\mathbb R}.
$$

The [dual variables](../../../mathematical-optimization.md#dual-variable) have no sign restrictions because the primal constraints are equalities.

A feasible shipment $x$ is optimal if and only if there exist feasible [transportation dual potentials](../../../mathematical-optimization.md#transportation-dual-potentials) satisfying [complementary slackness](../../../mathematical-optimization.md#complementary-slackness):

$$
\boxed{x_{ij}(c_{ij}-u_i-v_j)=0\quad\text{for every }i,j}.
$$

Thus every occupied route must have $u_i+v_j=c_{ij}$. To see sufficiency explicitly, the primal minus dual objective is

$$
\sum_{i,j}x_{ij}(c_{ij}-u_i-v_j)\ge0,
$$

and [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) makes it zero. This is the [weak duality](../../../mathematical-optimization.md#weak-duality) certificate. Necessity follows from [strong duality](../../../mathematical-optimization.md#strong-duality) for the feasible, bounded [linear program](../../../mathematical-optimization.md#linear-programming). If the total supply $M$ is positive, $x_{ij}=a_i b_j/M$ gives feasibility; if $M=0$, $x=0$ does. The feasible shipments form a closed bounded set, so the primal optimum is attained. This also covers zero supplies and demands. The one redundant equality merely leaves the dual gauge freedom $(u,v)\mapsto(u+t,v-t)$.

## 9C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

Let $\dim V=n$ and $\dim W=k$. Extend a [basis](../../../vector-space.md#basis) $w_1,\ldots,w_k$ of the [vector subspace](../../../vector-space.md#vector-subspace) $W$ to $w_1,\ldots,w_n$ of $V$, and let $f_1,\ldots,f_n$ be its [dual basis](../../../linear-algebra.md#dual-basis). Every [linear functional](../../../linear-algebra.md#linear-functional) is uniquely $\sum_i c_i f_i$. It vanishes on $W$ exactly when $c_1=\cdots=c_k=0$. Thus the [annihilator of a vector subspace](../../../linear-algebra.md#annihilator-of-a-vector-subspace) has [basis](../../../vector-space.md#basis) $f_{k+1},\ldots,f_n$, and

$$
\boxed{\dim\alpha(W)=n-k}.
$$

To apply this to a [matrix](../../../vector-space.md#matrix), regard its rows as elements of $(\mathbb R^n)^*$ and let $R$ be their linear span. Elementary invertible row and column operations reduce a rank-$r$ [matrix](../../../vector-space.md#matrix) to a block identity $\operatorname{diag}(I_r,0)$, showing that $\dim R=r$. The equations require that every functional in $R$ vanish on $x$. The canonical identification $\mathbb R^n\cong((\mathbb R^n)^*)^*$ sends $x$ to evaluation $f\mapsto f(x)$: it is injective because coordinate functionals separate points, and is bijective by equal dimensions. Consequently the solution [vector space](../../../vector-space.md) is the annihilator of $R$ under this identification. The dimension formula just proved gives

$$
\boxed{\dim\ker A=n-r}.
$$

A [basis](../../../vector-space.md#basis) of this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) consists of exactly $n-r$ [linearly independent](../../../vector-space.md#linear-independence) solutions, and every solution is their linear combination.

## 10C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10c/solution">Solution</h3>

↑ **Parent:** [10C](#10c)

Let $G$ act on its $n$ left [cosets](../../../group-theory.md#coset) by $g\cdot(xH)=gxH$. This is well-defined and gives a [group homomorphism](../../../group-theory.md#group-homomorphism) $\rho:G\to S_n$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $K$ is a [normal subgroup](../../../group-theory.md#normal-subgroup). An element lies in this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) exactly when it fixes every coset, so

$$
K=\bigcap_{x\in G}xHx^{-1}\subset H.
$$

This is the [normal core of a subgroup](../../../group-theory.md#core-group-theory). By the [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem), $G/K\cong\rho(G)$, a subgroup of $S_n$. The [Lagrange theorem](../../../group-theory.md#lagrange-s-theorem) therefore gives

$$
\boxed{[G:K]=|\rho(G)|\text{ divides }n!}.
$$

In particular $K$ has finite index even when $G$ is infinite.

Now let $H$ be generated by an element of order $q$ in a group of order $pq$. Then $|H|=q$ and $[G:H]=p$. The preceding result gives a normal $K\subset H$ with $[G:K]\mid p!$. Since $H$ has prime order, its subgroup $K$ is either $\{e\}$ or all of $H$. The first choice would imply $pq\mid p!$, which is impossible because the prime $q>p$ divides none of the factors of $p!$. Therefore $K=H$, proving that **every subgroup generated by an element of order $q$ is normal**. No classification of groups of order $pq$ is needed.

## 11B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11b/solution">Solution</h3>

↑ **Parent:** [11B](#11b)

Fix $x_0\in E$ and $\varepsilon>0$. By [uniform convergence](../../../real-analysis.md#uniform-convergence), choose $N$ so that $|f_N(x)-f(x)|<\varepsilon/3$ for every $x\in E$. By [continuity](../../../calculus.md#continuous-function) of $f_N$ relative to $E$, there is $\delta>0$ such that $x\in E$ and $|x-x_0|<\delta$ imply $|f_N(x)-f_N(x_0)|<\varepsilon/3$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
|f(x)-f(x_0)|
\le |f(x)-f_N(x)|+|f_N(x)-f_N(x_0)|+|f_N(x_0)-f(x_0)|
<\varepsilon.
$$

This proves the [uniform limit theorem](../../../real-analysis.md#uniform-limit-theorem) without requiring $E$ to be open or closed.

For the series, fix an arbitrary $x_0\in(0,1]$ and put $a=x_0/2>0$. On $[a,1]$ each summand $n^{-1-x}$ is [continuous](../../../calculus.md#continuous-function) and

$$
0<n^{-1-x}\le n^{-1-a},\qquad
\sum_{n=1}^\infty n^{-1-a}<\infty.
$$

The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) gives [uniform convergence](../../../real-analysis.md#uniform-convergence) of the series on $[a,1]$. Its partial sums are [continuous](../../../calculus.md#continuous-function), so the [uniform limit theorem](../../../real-analysis.md#uniform-limit-theorem) makes its sum [continuous](../../../calculus.md#continuous-function) on that interval, in particular at $x_0$ with the appropriate relative topology if $x_0=1$. Since $x_0$ was arbitrary, **the sum is continuous on $(0,1]$**.

This is local [uniform convergence](../../../real-analysis.md#uniform-convergence), not [uniform convergence](../../../real-analysis.md#uniform-convergence) on the entire half-open interval. Indeed, for any finite partial sum length $N$, its tail as $x\downarrow0$ is bounded below by arbitrarily long tails of the divergent harmonic series. There is no continuity claim at the excluded endpoint $0$.

## 12A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

The sum of the two [metrics](../../../topological-analysis.md#metric) is nonnegative and symmetric. It vanishes exactly when both coordinate distances vanish, hence exactly when the two points agree. Adding the two component [triangle inequalities](../../../topological-analysis.md#triangle-inequality) gives the [triangle inequality](../../../topological-analysis.md#triangle-inequality) on the [Cartesian product](../../../set-theory.md#cartesian-product), so the displayed function is a [metric](../../../topological-analysis.md#metric). Moreover,

$$
d_Y(\pi(x_1,y_1),\pi(x_2,y_2))\le d((x_1,y_1),(x_2,y_2)),
$$

so the [projection map](../../../function.md#projection-map) is $1$-[Lipschitz](../../../real-analysis.md#lipschitz-continuity) and therefore [continuous](../../../calculus.md#continuous-function).

To prove [sequential compactness](../../../geometry-and-topology.md#sequentially-compact-space) directly from [compactness](../../../topology.md#compact-space), take a sequence $(x_n)$ in $X$. If every point $x$ had a neighborhood containing sequence terms at only finitely many indices, these neighborhoods would form an open cover with a finite subcover, implying that only finitely many sequence terms exist, a contradiction. Thus some $x\in X$ has infinitely many indices in every neighborhood. Choose increasing indices $n_k$ with $d_X(x_{n_k},x)<1/k$; then $x_{n_k}\to x\in X$.

Now let $F\subset X\times Y$ be [closed](../../../topology.md#closed-set) and suppose $y_n\in\pi(F)$ converges to $y$. Choose $x_n$ such that $(x_n,y_n)\in F$. A [convergent subsequence](../../../real-analysis.md#convergent-subsequence) $x_{n_k}\to x$ exists by the preceding argument. In the product [metric](../../../topological-analysis.md#metric), $(x_{n_k},y_{n_k})\to(x,y)$, and the fact that $F$ is [closed](../../../topology.md#closed-set) gives $(x,y)\in F$. Thus $y\in\pi(F)$, proving that the [projection with a compact factor is closed](../../../topology.md#projection-with-a-compact-factor-is-closed). The sequential criterion for a [closed set](../../../topology.md#closed-set) in a [metric space](../../../topological-analysis.md#metric-space) follows by choosing points at distance less than $1/k$ from any point of its closure.

For a counterexample without a compact factor, take $X=Y=\mathbb R$ with their usual [metrics](../../../topological-analysis.md#metric) and

$$
F=\{(x,y):xy=1\}.
$$

The continuous product function makes $F$ [closed](../../../topology.md#closed-set), but $\pi(F)=\mathbb R\setminus\{0\}$ is not [closed](../../../topology.md#closed-set). Thus **compactness of the discarded factor is essential to the general conclusion**.

## 13F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13f/solution">Solution</h3>

↑ **Parent:** [13F](#13f)

Use the [Möbius transformation](../../../group-theory.md#mobius-transformation) $t=(z-1)/(z+1)$, the [principal square root](../../../analysis.md#principal-square-root-of-a-complex-number) $s=\sqrt t$ with $\Re s>0$, and then $w=(s-1)/(s+1)$. The resulting [conformal map](../../../geometry-and-topology.md#conformal-map) is

$$
\boxed{w(z)=\frac{\sqrt{(z-1)/(z+1)}-1}{\sqrt{(z-1)/(z+1)}+1}}.
$$

All branches here are single-valued: the inverse $z=(1+t)/(1-t)$ shows that the deleted segment corresponds to the nonpositive real axis. However, the exact first image is

$$
t(\mathbb C\setminus[-1,1])
=\bigl(\mathbb C\setminus(-\infty,0]\bigr)\setminus\{1\},
$$

since $t=1$ would require a source point at infinity. Thus the next image is $\{\Re s>0\}\setminus\{1\}$, and

$$
\boxed{w(\mathbb C\setminus[-1,1])=\{0<|w|<1\}}.
$$

The strict inequality $|w|<1$ follows from $|s+1|^2-|s-1|^2=4\Re s>0$. None of the component derivatives vanishes. For completeness the inverse on this punctured disk is

$$
z=-\frac12(w+w^{-1}).
$$

Given $0<|w|<1$, the inverse Cayley transform has positive real part, and reversing the three maps proves both injectivity and surjectivity onto this exact image.

This distinction matters for interpreting the printed request. The displayed function is a [conformal map](../../../geometry-and-topology.md#conformal-map) into the unit disk, but **no conformal bijection from the specified plane domain onto the full unit disk exists**. To prove the obstruction, the loop $z=2e^{i\theta}$ surrounds $0$, a point outside the domain, with [winding number](../../../complex-analysis.md#winding-number) $1$. A contraction within the source would remain in $\mathbb C\setminus\{0\}$ and preserve [winding number](../../../complex-analysis.md#winding-number), whereas a constant loop has [winding number](../../../complex-analysis.md#winding-number) $0$. Hence the source is not [simply connected](../../../algebraic-topology.md#simply-connected-space); a disk is [simply connected](../../../algebraic-topology.md#simply-connected-space), as straight-line contraction shows, and a conformal bijection is a [homeomorphism](../../../topology.md#homeomorphism).

The hinted construction becomes a bijection onto the full disk if the source is instead $\widehat{\mathbb C}\setminus[-1,1]$, including infinity on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). Near infinity, $w(z)=-1/(2z)+O(z^{-3})$, so the map extends with $w(\infty)=0$ and nonzero derivative in the coordinate $1/z$. This is the precise filled-in version of the [conformal map of a segment complement to a punctured disk](../../../geometry-and-topology.md#conformal-map-of-a-segment-complement-to-a-punctured-disk).

## 14E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14e/solution">Solution</h3>

↑ **Parent:** [14E](#14e)

The [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) satisfy $a_0=a_n=0$ and

$$
b_n=\frac1\pi\left(\int_0^\pi\sin(n\theta)\,d\theta-\int_\pi^{2\pi}\sin(n\theta)\,d\theta\right)
=\frac{2[1-(-1)^n]}{\pi n}.
$$

Thus the [square wave](../../../fourier-series.md#square-wave) has [Fourier series](../../../fourier-series.md)

$$
\boxed{f(\theta)\sim\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac{\sin(n\theta)}n}.
$$

It equals $f$ away from its [jump discontinuities](../../../calculus.md#jump-discontinuity), and converges to $0$ at the jumps. The assigned endpoint values do not affect its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient).

For the [Poisson equation](../../../partial-differential-equation.md#poisson-equation), use [separation of variables](../../../partial-differential-equation.md#separation-of-variables) $\phi=\sum_{n\text{ odd}}b_nR_n(r)\sin(n\theta)$. The radial equation is $r^2R_n''+rR_n'-n^2R_n=r^2$. Its bounded solution with zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) at $r=1$ is

$$
R_n(r)=\frac{r^n-r^2}{n^2-4}.
$$

Indeed the negative power is excluded at the centre, and the boundary fixes the coefficient of $r^n$. No resonance at $n=2$ occurs because only odd modes are forced. Therefore

$$
\boxed{\phi(r,\theta)=\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}
\frac{r^n-r^2}{n(n^2-4)}\sin(n\theta)}.
$$

This is a [Poisson equation on a disk with angular forcing](../../../partial-differential-equation.md#poisson-equation-on-a-disk-with-angular-forcing). The series converges uniformly on the closed disk: for $n\ge3$ each term is bounded by a constant times $n^{-3}$. Its first spatial derivatives also converge uniformly. For instance the radial derivative and $r^{-1}$ times the angular derivative of each term are bounded by constants times $n^{-2}$; the $n=1$ harmonic term is smooth in Cartesian coordinates. It defines a function with zero boundary data and the required [weak formulation](../../../partial-differential-equation.md#weak-formulation). Applying the [Laplacian](../../../calculus.md#laplacian) to finite partial sums gives the [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) of $f$, which converge in $L^2$; passing to the limit against smooth compactly supported test functions verifies the [Poisson equation](../../../partial-differential-equation.md#poisson-equation). It holds classically off the jump rays and the centre, where the forcing is locally constant. It cannot be interpreted as a global classical equation with continuous second derivatives for discontinuous forcing. Uniqueness follows from the zero-boundary [Dirichlet energy](../../../differential-geometry.md#dirichlet-energy) identity for the difference of two solutions.

Finally [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives $\int_0^{2\pi}f(\theta)\sin(n\theta)\,d\theta=\pi b_n$. The radial integral is

$$
\int_0^1R_n(r)r\,dr
=\frac{1}{n^2-4}\left(\frac1{n+2}-\frac14\right)
=-\frac1{4(n+2)^2}.
$$

Uniform convergence of $\phi$ and boundedness of $f$ justify integration term by term, so

$$
\boxed{\int_{r\le1}f\phi\,dA
=-\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac1{n^2(n+2)^2}}.
$$

The negative sign also agrees with $\int\phi\Delta\phi=-\int|\nabla\phi|^2$. The original PDF's radial denominator is $n^2-4$; the converted TeX's $n^2-1$ is a transcription error.

## 15G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15g/solution">Solution</h3>

↑ **Parent:** [15G](#15g)

Inside the [infinite square well](../../../quantum-mechanics.md#infinite-square-well), the time-independent [Schrödinger equation](../../../physics.md#schrodinger-equation) is $-\hbar^2u''/(2m)=Eu$ with $u(-a)=u(a)=0$. For $E<0$ the exponential solutions cannot satisfy both conditions except trivially, and for $E=0$ neither can a linear function. For $E>0$ put $k=\sqrt{2mE}/\hbar$. The first boundary condition selects $u=C\sin(k(x+a))$, and the second gives $\sin(2ak)=0$. Thus

$$
\boxed{u_n(x)=\frac1{\sqrt a}\sin\!\left(\frac{n\pi(x+a)}{2a}\right),\qquad
E_n=\frac{\hbar^2\pi^2n^2}{8ma^2},\quad n=1,2,\ldots}
$$

on $[-a,a]$, with $u_n=0$ outside. Their squared integrals are one, and the sine [orthogonality](../../../linear-algebra.md#orthogonal-vectors) identity gives an [orthonormal set](../../../linear-algebra.md#orthonormal-set). The sine [Fourier basis](../../../fourier-series.md#fourier-basis) on the interval is complete: odd extension to an interval of length $4a$ reduces this to completeness of the [Fourier series](../../../fourier-series.md) basis. Hence these are a complete set of normalized [energy eigenstates](../../../quantum-mechanics.md#energy-eigenstate).

Choosing the harmless sign of the second [energy eigenstate](../../../quantum-mechanics.md#energy-eigenstate) so that $v_1=a^{-1/2}\cos(\pi x/(2a))$ and $v_2=a^{-1/2}\sin(\pi x/a)$, the specified [wave function](../../../quantum-mechanics.md#wave-function) is $v_1/\sqrt5+2v_2/\sqrt5$. The [Born rule](../../../quantum-mechanics.md#born-rule) therefore gives

$$
\boxed{\Pr(E=E_1)=\frac15,\qquad\Pr(E=E_2)=\frac45},
$$

with no other possible measured energies. The two [energy eigenvalues](../../../quantum-mechanics.md#energy-eigenvalue) are $E_1=\hbar^2\pi^2/(8ma^2)$ and $E_2=4E_1$.

After the first measurement gives the [ground state](../../../quantum-mechanics.md#ground-state), the old state is $v_1$. Doubling the width puts the walls at $\pm2a$, and the new normalized [ground state](../../../quantum-mechanics.md#ground-state) is $w_1=(2a)^{-1/2}\cos(\pi x/(4a))$. The stipulated unchanged state is zero outside the original interval, so the [probability amplitude](../../../quantum-mechanics.md#probability-amplitude) is

$$
\langle w_1,v_1\rangle
=\frac1{\sqrt2\,a}\int_{-a}^a
\cos\!\left(\frac{\pi x}{4a}\right)\cos\!\left(\frac{\pi x}{2a}\right)\,dx
=\frac8{3\pi}.
$$

Squaring gives

$$
\boxed{\Pr(\text{new ground state}\mid\text{old ground state})=\frac{64}{9\pi^2}}.
$$

The [ground-state overlap after sudden expansion of a square well](../../../quantum-mechanics.md#ground-state-overlap-after-sudden-expansion-of-a-square-well) stays unchanged during subsequent evolution in the fixed new well, because the energy-basis coefficients acquire only phases. The answer is conditional on the already observed old [ground state](../../../quantum-mechanics.md#ground-state); its earlier probability $1/5$ is not another factor in this conditional question.

## 16H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16h/solution">Solution</h3>

↑ **Parent:** [16H](#16h)

Fix the [electric potential](../../../electromagnetism.md#electric-potential) to vanish at infinity and assume a localized, nonsingular [charge density](../../../electromagnetism.md#charge-density) of finite [electrostatic energy](../../../electromagnetism.md#electrostatic-energy). Assemble the charge by scaling $\rho_s=s\rho$ from $s=0$ to $1$. Linearity gives $\phi_s=s\phi$, so the work is

$$
U=\int_0^1ds\int\phi_s\rho\,d^3x
=\frac12\int\rho\phi\,d^3x.
$$

The factor $1/2$ prevents double counting of pair interactions. Using [Gauss law](../../../electromagnetism.md#gauss-s-law), $\rho=-\epsilon_0\Delta\phi$, and [integration by parts](../../../calculus.md#integration-by-parts),

$$
U=-\frac{\epsilon_0}2\int\phi\Delta\phi\,d^3x
=\boxed{\frac{\epsilon_0}2\int|\nabla\phi|^2\,d^3x
=\frac{\epsilon_0}2\int|\mathbf E|^2\,d^3x}.
$$

The boundary integral at infinity vanishes for a localized distribution since $\phi=O(r^{-1})$ and $\partial_r\phi=O(r^{-2})$. Singular point-charge self-energies require a separate regularization and are not finite instances of this identity.

For the uniform solid sphere, spherical symmetry and [Gauss law](../../../electromagnetism.md#gauss-s-law) give

$$
\boxed{\mathbf E(r)=
\begin{cases}
\dfrac{\rho r}{3\epsilon_0}\,\widehat{\mathbf r},&0\le r\le R,\\[2pt]
\dfrac{\rho R^3}{3\epsilon_0r^2}\,\widehat{\mathbf r},&r\ge R.
\end{cases}}
$$

Integrating inward from infinity and matching the continuous [electric potential](../../../electromagnetism.md#electric-potential) at $R$ gives

$$
\boxed{\phi(r)=
\begin{cases}
\dfrac{\rho}{6\epsilon_0}(3R^2-r^2),&r\le R,\\[2pt]
\dfrac{\rho R^3}{3\epsilon_0r},&r\ge R.
\end{cases}}
$$

The value of the [electric field](../../../electromagnetism.md#electric-field) at the centre is the zero vector.

Writing $Q=4\pi\rho R^3/3$, the [electrostatic energy of a uniformly charged solid sphere](../../../electromagnetism.md#electrostatic-energy-of-a-uniformly-charged-solid-sphere) follows either from the charge-potential integral or from the field integral including the exterior:

$$
U=\frac12\,4\pi\rho\int_0^R\phi(r)r^2\,dr
=\boxed{\frac{4\pi\rho^2R^5}{15\epsilon_0}
=\frac{3Q^2}{20\pi\epsilon_0R}}.
$$

For the nuclear scaling, $Q=Ze$ while constant volume per proton gives $R\propto Z^{1/3}$. Therefore **the electric contribution scales as $Q^2/R\propto Z^{5/3}$** in this uniform-density model.

## 17E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17e/solution">Solution</h3>

↑ **Parent:** [17E](#17e)

For [potential flow](../../../fluid-mechanics.md#potential-flow) $\mathbf u=\nabla\varphi$ in an inviscid fluid of constant density under the [conservative force](../../../classical-mechanics.md#conservative-force) per unit mass $-\nabla\chi$, the unsteady [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) is

$$
\frac p\rho+\partial_t\varphi+\frac12|\nabla\varphi|^2+\chi=C(t).
$$

It follows by inserting the [velocity potential](../../../fluid-mechanics.md#velocity-potential) into the [Euler equations](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) and integrating the resulting spatial gradient. A time-only change of the [velocity potential](../../../fluid-mechanics.md#velocity-potential) changes $C(t)$ without altering the [velocity field](../../../fluid-mechanics.md#velocity-field).

For spherical motion in an unbounded liquid, incompressibility gives $r^2u_r=A(t)$; the kinematic condition $u_r(R)=\dot R$ gives $A=R^2\dot R$. Choose $\varphi=-R^2\dot R/r$, vanishing at infinity. To obtain the displayed bubble relation, take no spatial body-force contribution, neglect [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) and [surface tension](../../../fluid-mechanics.md#surface-tension), and equate the liquid-side interface pressure to $p_b$. With the far-field pressure $p_\infty$, [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) evaluated at the surface uses the partial derivative at fixed $r$:

$$
\left.\partial_t\varphi\right|_{r=R}
=-2\dot R^2-R\ddot R,\qquad
\left.|\mathbf u|^2\right|_{r=R}=\dot R^2.
$$

Hence the [Rayleigh equation for an inviscid spherical bubble](../../../fluid-mechanics.md#rayleigh-equation-for-an-inviscid-spherical-bubble) is

$$
\boxed{p_b-p_\infty=\rho\left(R\ddot R+\frac32\dot R^2\right)}.
$$

The exterior [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is

$$
K=\frac\rho2\int_R^\infty4\pi r^2\frac{R^4\dot R^2}{r^4}\,dr
=\boxed{2\pi\rho R^3\dot R^2}.
$$

Differentiating it and using $\dot V=4\pi R^2\dot R$ gives the [pressure-work energy balance for a spherical bubble](../../../fluid-mechanics.md#pressure-work-energy-balance-for-a-spherical-bubble):

$$
\dot K=4\pi\rho R^2\dot R\left(R\ddot R+\frac32\dot R^2\right)
=\boxed{(p_b-p_\infty)\dot V}.
$$

This derivation also holds at a turning point $\dot R=0$, without dividing by $\dot R$.

For constant $p_\infty$ and the stated inverse-volume bubble pressure, integrate this exact time derivative:

$$
K-K_0=p_\infty\int_{V_0}^V\left(\frac{V_0}{s}-1\right)\,ds
=\boxed{p_\infty\left[V_0\log\!\left(\frac V{V_0}\right)-V+V_0\right]}.
$$

The relation is valid on physically accessible portions of the motion, where the resulting [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is nonnegative. In particular $\log q\le q-1$ makes the bracket nonpositive, as expected for the restoring pressure about $V_0$.

## 18D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18d/solution">Solution</h3>

↑ **Parent:** [18D](#18d)

A [simple hypothesis](../../../statistical-modelling.md#simple-hypothesis) specifies the entire probability distribution. A [critical region](../../../statistical-modelling.md#rejection-region) $C$ is the set of observations for which the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) is rejected. The [size of a statistical test](../../../statistical-modelling.md#size-of-a-statistical-test) is $\sup_{\theta\in H_0}\Pr_\theta(X\in C)$, which reduces to $\Pr_0(C)$ for a [simple hypothesis](../../../statistical-modelling.md#simple-hypothesis). The [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) is $\Pr_\theta(C)$ as a function of the true parameter or distribution. At a specified alternative, the [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) probability is $\Pr_\theta(C^c)=1-\Pr_\theta(C)$, the chance of failing to reject a false [null hypothesis](../../../statistical-modelling.md#null-hypothesis). The [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) probability is the corresponding rejection probability under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis).

The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) says that, for two [simple hypotheses](../../../statistical-modelling.md#simple-hypothesis), a test rejecting where $f_1>kf_0$, accepting where $f_1<kf_0$, and if necessary randomizing on equality to achieve prescribed size $\alpha$, has maximal [statistical power](../../../probability-and-statistics.md#statistical-power) among tests of size at most $\alpha$. Conversely a most powerful test can be taken in this [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) form, up to equality sets and null sets.

Here the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) for $x\ne0$ is

$$
\frac{f_1(x)}{f_0(x)}=\sqrt{\frac2\pi}\frac1{|x|}.
$$

Its value is infinite at $0$, which has probability zero under both continuous distributions. Large [likelihood ratios](../../../statistical-modelling.md#likelihood-ratio) correspond to small $|x|$. Thus the best [critical region](../../../statistical-modelling.md#rejection-region) is $|X|<c_\alpha$, where

$$
\alpha=\int_{-c_\alpha}^{c_\alpha}\frac12|x|e^{-x^2/2}\,dx
=1-e^{-c_\alpha^2/2}.
$$

There is no boundary randomization to worry about. The complete answer is

$$
\boxed{\text{reject if }|X|<\sqrt{-2\log(1-\alpha)},\qquad
\text{power}=2\Phi\!\left(\sqrt{-2\log(1-\alpha)}\right)-1}.
$$

For the [minimum sum of errors in a simple hypothesis test](../../../statistical-modelling.md#minimum-sum-of-errors-in-a-simple-hypothesis-test), write the error sum as $\int_Cf_0+\int_{C^c}f_1$. At each observation its smaller contribution is obtained by rejecting exactly where $f_1>f_0$. This proves optimality over all tests, including randomized ones, rather than just optimizing within an assumed family. Here it gives $c_*=\sqrt{2/\pi}$, and therefore

$$
\boxed{\alpha_*=1-e^{-1/\pi}\approx0.2726}.
$$

The minimum error sum is $1-e^{-1/\pi}+2[1-\Phi(\sqrt{2/\pi})]$. This criterion weights the two error probabilities equally; it does not impose a conventional $5\%$ [significance level](../../../statistical-modelling.md#significance-level).

## 19D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19d/solution">Solution</h3>

↑ **Parent:** [19D](#19d)

Let $D_n\in\{1,2,3\}$ be the shorter circular separation after $n$ swaps, so $D_0=1$. There are $\binom62=15$ equally likely unordered swaps. Six swap only guests, one swaps the distinguished pair, and eight swap one distinguished diner with a guest. Rotations, reflections and exchangeability of the guests ensure that the next-separation probabilities depend only on $D_n$. Thus this is the [separation chain for two labels in a circular transposition shuffle](../../../markov-process.md#separation-chain-for-two-labels-in-a-circular-transposition-shuffle), a [lumped Markov chain](../../../markov-process.md#lumped-markov-chain).

Counting all swaps gives the [transition matrix](../../../markov-process.md#stochastic-matrix)

$$
P=\frac1{15}\begin{pmatrix}9&4&2\\4&9&2\\4&4&7\end{pmatrix},
$$

with states ordered $1,2,3$. To verify the counts, fix one distinguished diner at seat $0$ and the other at seat $d$. For $d=1$, swaps moving the diner at $0$ to seats $2,3,4,5$ give separations $1,2,3,2$; swaps moving the diner at $1$ to those seats give $2,3,2,1$. Along with the seven separation-preserving swaps this gives $(9,4,2)$. For $d=2$, moving the first diner to seats $1,3,4,5$ gives $1,1,2,3$, while moving the second gives $1,3,2,1$; the total is $(4,9,2)$. For $d=3$, each distinguished diner has two moves to separation $1$ and two to separation $2$, giving $(4,4,7)$.

If $r_n=\Pr(D_n=3)$, the last column yields

$$
r_{n+1}=\frac2{15}(1-r_n)+\frac7{15}r_n
=\frac2{15}+\frac13r_n,\qquad r_0=0.
$$

Subtracting the fixed point $1/5$ and iterating solves the [affine recurrence](../../../algebra.md#affine-recurrence):

$$
\boxed{\Pr(\text{opposite on night }n+1)=r_n=\frac15(1-3^{-n})}.
$$

For one swap this gives $2/15$, agreeing with direct counting. The limit $1/5$ also agrees with the [stationary distribution](../../../markov-process.md#stationary-distribution) $(2/5,2/5,1/5)$ of the separation [Markov chain](../../../markov-process.md#markov-chain): given one diner's seat, one of the five remaining seats is opposite. The complete permutation shuffle alternates parity, but that does not prevent this lumped separation probability from converging.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
