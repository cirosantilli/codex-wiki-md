# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2006/PaperIB_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2006/PaperIB_1.pdf)

**Table of contents**

- [1H](#1h)
  - [Solution](#1h/solution)
- [2H](#2h)
  - [Solution](#2h/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5A](#5a)
  - [Solution](#5a/solution)
- [6D](#6d)
  - [a](#6d/a)
    - [Solution](#6d/a/solution)
  - [b](#6d/b)
    - [Solution](#6d/b/solution)
- [7C](#7c)
  - [Solution](#7c/solution)
- [8C](#8c)
  - [Solution](#8c/solution)
- [9H](#9h)
  - [Solution](#9h/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12F](#12f)
  - [i](#12f/i)
    - [Solution](#12f/i/solution)
  - [ii](#12f/ii)
    - [Solution](#12f/ii/solution)
- [13D](#13d)
  - [Solution](#13d/solution)
- [14A](#14a)
  - [Solution](#14a/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16G](#16g)
  - [Solution](#16g/solution)
- [17A](#17a)
  - [Solution](#17a/solution)
- [18C](#18c)
  - [Solution](#18c/solution)
- [19C](#19c)
  - [Solution](#19c/solution)

## 1H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1h/solution">Solution</h3>

↑ **Parent:** [1H](#1h)

The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) $m_A$ is the [monic polynomial](../../../polynomial.md#monic-polynomial) of smallest degree satisfying $m_A(A)=0$. An annihilating [polynomial](../../../polynomial.md) exists, for example because $I,A,\ldots,A^{n^2}$ are linearly dependent in the $n^2$-dimensional space of [matrices](../../../vector-space.md#matrix). A nonzero constant cannot annihilate $A$, so the minimal degree is positive.

If $p$ and $q$ are two such [monic polynomials](../../../polynomial.md#monic-polynomial) of minimal degree $d$, then $(p-q)(A)=0$ and $\deg(p-q)<d$ unless $p=q$. Minimality therefore forces $p=q$. [Polynomial](../../../polynomial.md) division also shows that $m_A$ divides every annihilating [polynomial](../../../polynomial.md): the remainder after division would otherwise be an annihilator of smaller degree. This proves uniqueness rather than merely choosing one of several minimal-degree [polynomials](../../../polynomial.md).

If $A$ is real, coefficientwise [complex conjugation](../../../complex-analysis.md#complex-conjugation) of $m_A(A)=0$ gives $\overline{m_A}(A)=0$. The conjugated [polynomial](../../../polynomial.md) is monic of the same degree, hence uniqueness gives $\overline{m_A}=m_A$. **The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) of a real [matrix](../../../vector-space.md#matrix) has real coefficients.**

For $n\ge3$, use the [block diagonal matrix](../../../vector-space.md#block-diagonal-matrix)

$$
\boxed{A=\begin{pmatrix}1&1\\0&1\end{pmatrix}\oplus(-1)\oplus I_{n-3}.}
$$

The two-dimensional [Jordan block](../../../linear-operator-theory.md#jordan-block) is annihilated by $(t-1)^2$ but not by $t-1$, while the scalar block requires the factor $t+1$. A [polynomial](../../../polynomial.md) annihilates the [direct sum](../../../vector-space.md#direct-sum) exactly when it annihilates every block. Thus its [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is the [least common multiple](../../../number-theory.md#least-common-multiple) $(t-1)^2(t+1)$. For $n=3$ the final identity block is omitted.

## 2H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2h/solution">Solution</h3>

↑ **Parent:** [2H](#2h)

In the [upper half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model) $H=\{(x,y):y>0\}$ the [hyperbolic metric](../../../geometry-and-topology.md#hyperbolic-metric) is

$$
ds^2=\frac{dx^2+dy^2}{y^2}.
$$

The length of a differentiable curve is $\int\sqrt{\dot x^2+\dot y^2}\,dt/y$. The area element is the square root of the metric determinant times $dx\,dy$, so the [hyperbolic area](../../../geometry-and-topology.md#hyperbolic-area) of a measurable region $S$ is $\int_S y^{-2}\,dx\,dy$.

The [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) for a [geodesic](../../../riemannian-geometry.md#geodesic) [hyperbolic triangle](../../../geometry-and-topology.md#hyperbolic-triangle) of angles $\alpha,\beta,\gamma$ in [curvature](../../../differential-geometry.md#curvature) $-1$ gives **area $\pi-\alpha-\beta-\gamma$**; an ideal vertex has angle zero. The horizontal edge in the present region is not a [geodesic](../../../riemannian-geometry.md#geodesic), so it is simpler to use the area element directly:

$$
\operatorname{Area}_H(R)=\int_0^{1/2}\int_{\sqrt{1-x^2}}^1\frac{dy\,dx}{y^2}
=\int_0^{1/2}\left(\frac1{\sqrt{1-x^2}}-1\right)dx
=\boxed{\frac\pi6-\frac12}.
$$

The open boundary does not affect the [integral](../../../calculus.md#integral) because its area is zero.

## 3D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

Write the [holomorphic function](../../../complex-analysis.md#holomorphic-function) as $f=u+iv$. Analyticity gives smooth real and imaginary parts satisfying the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) $u_x=v_y$, $u_y=-v_x$. Differentiating these identities shows

$$
\Delta u=v_{yx}-v_{xy}=0,\qquad \Delta v=-u_{yx}+u_{xy}=0.
$$

Thus both parts are [harmonic functions](../../../partial-differential-equation.md#harmonic-function). The [product rule](../../../calculus.md#product-rule) then gives

$$
\Delta|f|^2=\Delta(u^2+v^2)
=2(u_x^2+u_y^2+v_x^2+v_y^2)+2u\Delta u+2v\Delta v
=4(u_x^2+v_x^2).
$$

Since $f'=u_x+iv_x$, this proves the [Laplacian identity for the squared modulus of a holomorphic function](../../../partial-differential-equation.md#laplacian-identity-for-the-squared-modulus-of-a-holomorphic-function),

$$
\boxed{\Delta|f(z)|^2=4|f'(z)|^2.}
$$

## 4B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

Interpret $m$ as the [rest mass](../../../special-relativity.md#invariant-mass) of each initial ball and assume that no energy or [momentum](../../../classical-mechanics.md#momentum) escapes the collision. Let $\gamma=(1-v^2/c^2)^{-1/2}$ be its [Lorentz factor](../../../special-relativity.md#lorentz-factor). The total initial energy and [momentum](../../../classical-mechanics.md#momentum) are

$$
E=mc^2(\gamma+1),\qquad P=\gamma mv.
$$

Their conservation determines the final [four-momentum](../../../special-relativity.md#four-momentum). For a single lump, $P=\gamma'm'v'$ and $E=\gamma'm'c^2$, hence

$$
\boxed{v'=\frac{Pc^2}{E}=\frac{\gamma v}{\gamma+1}.}
$$

The final [invariant mass](../../../special-relativity.md#invariant-mass) follows from $m'^2c^4=E^2-c^2P^2$:

$$
m'^2=m^2\left[(\gamma+1)^2-\gamma^2\frac{v^2}{c^2}\right]
=m^2(2+2\gamma),\qquad
\boxed{m'=m\sqrt{2(1+\gamma)}.}
$$

This is the [rest mass of a coalescing relativistic collision](../../../special-relativity.md#rest-mass-of-a-coalescing-relativistic-collision). For $v>0$, $m'>2m$: some [kinetic energy](../../../classical-mechanics.md#kinetic-energy) becomes [internal energy](../../../thermodynamics.md#internal-energy) in the final rest frame. Setting $m'=2m$ would discard that energy and contradict conservation. At small speeds $v'\sim v/2$, while $v=0$ gives $m'=2m$.

## 5A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5a/solution">Solution</h3>

↑ **Parent:** [5A](#5a)

The displayed evolution law uses the usual assumptions of [incompressible flow](../../../fluid-mechanics.md#incompressible-flow), constant [density](../../../fluid-mechanics.md#density) and conservative body force. With $\boldsymbol\omega=\nabla\times\mathbf u$, the [Euler equation](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) is

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+\Phi).
$$

Use $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$ and take a [curl](../../../calculus.md#curl). [Gradients](../../../calculus.md#gradient) have zero [curl](../../../calculus.md#curl), and

$$
\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega)
=(\boldsymbol\omega\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\boldsymbol\omega
+\mathbf u\nabla\cdot\boldsymbol\omega-\boldsymbol\omega\nabla\cdot\mathbf u.
$$

Here $\nabla\cdot\boldsymbol\omega=0$ because it is a [curl](../../../calculus.md#curl), and $\nabla\cdot\mathbf u=0$ by incompressibility. The [vorticity equation](../../../physics.md#vorticity-equation) is therefore

$$
\boxed{\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

The [material derivative](../../../continuum-mechanics.md#material-derivative) combines local change with advection by fluid particles. The right-hand side is [vortex stretching](../../../physics.md#vortex-stretching) and tilting: spatial variation of velocity along a vortex line changes its strength and direction. Along each particle path this is a homogeneous linear equation for [vorticity](../../../fluid-mechanics.md#vorticity). For a smooth velocity field its solution with zero initial [vorticity](../../../fluid-mechanics.md#vorticity) remains zero by uniqueness. Thus an initially [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) remains irrotational while these assumptions and smoothness hold.

For a plane flow $\mathbf u=(u(x,y,t),v(x,y,t),0)$, the [vorticity](../../../fluid-mechanics.md#vorticity) is $\boldsymbol\omega=(0,0,\zeta)$ and $(\boldsymbol\omega\cdot\nabla)\mathbf u=\zeta\partial_z\mathbf u=0$. Hence $D\zeta/Dt=0$. Every particle retains its initial value, so an initially uniform value gives

$$
\boxed{\boldsymbol\omega(x,y,t)=\boldsymbol\omega_0\quad\text{for all later times}.}
$$

Inviscid motion alone is insufficient for the printed simplified law: compressible variable-density motion generally adds $-\boldsymbol\omega\nabla\cdot\mathbf u+\nabla\rho\times\nabla p/\rho^2$. Those terms vanish under the assumptions used above.

## 6D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6d/a">a</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/a/solution">Solution</h4>

↑ **Parent:** [A](#6d/a)

Use [columnwise partial pivoting](../../../numerical-analysis.md#columnwise-partial-pivoting): select the largest absolute entry in the current column and interchange rows. In the first column the pivot is $4$, so interchange rows 1 and 2. The multipliers are $1/2$ and $-1/2$, and elimination gives

$$
\begin{pmatrix}4&1&0\\0&1/2&1\\0&5/2&1\end{pmatrix}.
$$

The second pivot is $5/2$, so interchange the two remaining rows. Their previously stored first-column multipliers must also be interchanged. The final multiplier is $(1/2)/(5/2)=1/5$, giving the [LU decomposition](../../../numerical-analysis.md#lu-decomposition)

$$
\boxed{PA=LU,\qquad
P=\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix},\quad
L=\begin{pmatrix}1&0&0\\-1/2&1&0\\1/2&1/5&1\end{pmatrix},\quad
U=\begin{pmatrix}4&1&0\\0&5/2&1\\0&0&4/5\end{pmatrix}.}
$$

The [permutation matrix](../../../vector-space.md#permutation-matrix) orders the original rows as $2,3,1$. Multiplication verifies the displayed identity.

If “column pivoting” instead denotes interchanging columns rather than searching within a column, that convention gives $AQ=\widetilde L\widetilde U$ with

$$
Q=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix},\quad
\widetilde L=\begin{pmatrix}1&0&0\\2&1&0\\-1&-1&1\end{pmatrix},\quad
\widetilde U=\begin{pmatrix}2&1&1\\0&-2&-1\\0&0&2\end{pmatrix}.
$$

This second identity uses a different pivot convention; it does not change the row-pivoted answer above.

<h3 id="6d/b">b</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/b/solution">Solution</h4>

↑ **Parent:** [B](#6d/b)

At the first step of [Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination), the first column of a nonsingular [matrix](../../../vector-space.md#matrix) cannot be zero. Choose a nonzero pivot there using a row interchange and eliminate below it. The resulting [matrix](../../../vector-space.md#matrix) has block form

$$
\begin{pmatrix}p&r\\0&B\end{pmatrix},\qquad p\ne0.
$$

Elementary elimination and row [permutations](../../../combinatorics.md#permutation) preserve nonsingularity, so $p\det B\ne0$ and the trailing [matrix](../../../vector-space.md#matrix) $B$ is nonsingular. Its first column again has a nonzero entry. Repeating this argument inductively provides a nonzero pivot at every step and produces an upper-triangular factor. The recorded elimination multipliers, with previous entries permuted when necessary, form the unit lower-triangular factor. **Every nonsingular square [matrix](../../../vector-space.md#matrix) admits $PA=LU$ under [columnwise partial pivoting](../../../numerical-analysis.md#columnwise-partial-pivoting).**

For the column-interchange convention from part (a), use the same induction with a nonzero entry in the first row of each nonsingular trailing [matrix](../../../vector-space.md#matrix). Column interchanges put it in the pivot position, and elimination gives $AQ=LU$. These existence statements are in exact arithmetic; they do not assert that all choices have equally good numerical stability.

## 7C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

For the independent [normal distribution](../../../probability-theory.md#normal-distribution) observations, the log [likelihood](../../../statistical-modelling.md#likelihood-function) is

$$
\ell(\theta)=-\frac n2\log(2\pi)-\frac12\sum_{i=1}^n(X_i-\theta)^2.
$$

Its [derivative](../../../calculus.md#derivative) is $\sum_i(X_i-\theta)$ and its second [derivative](../../../calculus.md#derivative) is $-n<0$, so the unique [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) is

$$
\boxed{\widehat\theta_M=\overline X=\frac1n\sum_iX_i.}
$$

For the prior $\theta\sim N(\mu,\tau^{-1})$ with $\tau>0$, multiplying prior [density](../../../fluid-mechanics.md#density) by [likelihood](../../../statistical-modelling.md#likelihood-function) and completing the square gives

$$
\sum_i(X_i-\theta)^2+\tau(\theta-\mu)^2
=(n+\tau)\left(\theta-\frac{n\overline X+\tau\mu}{n+\tau}\right)^2+\text{a term independent of }\theta.
$$

Thus [normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives the [posterior distribution](../../../statistical-inference.md#bayesian-posterior)

$$
\theta\mid X\sim N\!\left(\frac{n\overline X+\tau\mu}{n+\tau},\frac1{n+\tau}\right).
$$

For [quadratic loss](../../../statistical-inference.md#squared-error-loss), the conditional expected loss of action $a$ is the [posterior variance](../../../statistical-inference.md#posterior-variance) plus $(a-\mathbb E[\theta\mid X])^2$. Its unique minimizer is the [posterior mean](../../../statistical-inference.md#posterior-mean), so the [Bayes estimator](../../../statistical-inference.md#bayes-estimator) is

$$
\boxed{\widehat\theta_B=\frac{n\overline X+\tau\mu}{n+\tau}.}
$$

This weights the sample and prior [means](../../../probability-theory.md#expected-value) by their respective precisions.

## 8C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8c/solution">Solution</h3>

↑ **Parent:** [8C](#8c)

For maximization of $f(x)$ subject to $g_j(x)\le0$ and $h_k(x)=0$, the [Lagrangian sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem) says: if a feasible $x^*$ globally maximizes $L(x)=f(x)-\sum_j\lambda_jg_j(x)+\sum_k\nu_kh_k(x)$, where $\lambda_j\ge0$, and $\lambda_jg_j(x^*)=0$, then $x^*$ globally maximizes $f$ over the feasible set. Indeed, at every feasible $x$,

$$
f(x)\le L(x)\le L(x^*)=f(x^*).
$$

This requires a global maximum of the [optimization Lagrangian](../../../mathematical-optimization.md#optimization-lagrangian); a stationary point alone is not sufficient without additional concavity or another justification.

Put $q=p/(p-1)$ and $C=(\sum_i|a_i|^q)^{1/q}$. If every $a_i=0$, **the maximum is zero and every feasible vector is optimal**. Otherwise set

$$
x_i^*=\frac{\operatorname{sgn}(a_i)|a_i|^{q-1}}{C^{q-1}},\qquad \lambda=\frac Cp.
$$

Since $p(q-1)=q$, $\sum_i|x_i^*|^p=1$. For $g(x)=\sum_i|x_i|^p-1$, the [optimization Lagrangian](../../../mathematical-optimization.md#optimization-lagrangian) is $L(x)=\sum_i a_ix_i-\lambda g(x)$. Its [gradient](../../../calculus.md#gradient) vanishes at $x^*$ because

$$
\lambda p\operatorname{sgn}(x_i^*)|x_i^*|^{p-1}=a_i.
$$

The function $\sum_i|x_i|^p$ is a [strictly convex function](../../../real-analysis.md#strictly-convex-function) for $p>1$, so $L$ is a [strictly concave function](../../../real-analysis.md#strictly-concave-function). Its supporting-hyperplane inequality proves that this stationary point is its global maximum. [Complementary slackness](../../../mathematical-optimization.md#complementary-slackness) and feasibility hold, so the sufficiency theorem applies. Substitution gives

$$
\boxed{\max_{\sum_i|x_i|^p\le1}\sum_i a_ix_i=C=\left(\sum_i|a_i|^{p/(p-1)}\right)^{(p-1)/p}.}
$$

The maximizing vector is unique when $a\ne0$. It is the [norming vector for Holder inequality](../../../functional-analysis.md#norming-vector-for-holder-inequality), and the value is the corresponding [dual norm](../../../functional-analysis.md#dual-norm).

## 9H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9h/solution">Solution</h3>

↑ **Parent:** [9H](#9h)

For a [linear map](../../../vector-space.md#linear-map) $\theta:U\to V$, its [rank of a linear map](../../../vector-space.md#rank-of-a-linear-map) is $r(\theta)=\dim\operatorname{im}\theta$, and its [nullity](../../../linear-algebra.md#nullity-of-a-linear-map) is $n(\theta)=\dim\ker\theta$. Choose a [basis](../../../vector-space.md#basis) $e_1,\ldots,e_s$ of its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and extend it to a [basis](../../../vector-space.md#basis) $e_1,\ldots,e_d$ of $U$. Then $\theta e_{s+1},\ldots,\theta e_d$ span its image. They are linearly independent: a linear combination mapped to zero would belong to the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map), contradicting independence of the extended [basis](../../../vector-space.md#basis) unless all its coefficients vanish. Hence $r(\theta)=d-s$, proving

$$
\boxed{r(\theta)+n(\theta)=\dim U.}
$$

For [endomorphisms](../../../algebra.md#endomorphism) of $U$, define $(\theta+\phi)(u)=\theta(u)+\phi(u)$ and $(\theta\phi)(u)=\theta(\phi(u))$. The image of the sum lies in the sum of the two images. Thus

$$
r(\theta+\phi)\le\dim(\operatorname{im}\theta+\operatorname{im}\phi)
\le r(\theta)+r(\phi).
$$

To prove the product inequality, restrict $\phi$ to $K=\ker(\theta\phi)$. This map has [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $\ker\phi$ and image $\operatorname{im}\phi\cap\ker\theta$: every vector in the intersection has a preimage in $K$. Applying the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) to the restricted map gives

$$
n(\theta\phi)=n(\phi)+\dim(\operatorname{im}\phi\cap\ker\theta)
\le n(\phi)+n(\theta).
$$

Now put $d=\dim U$ and $s=r(\theta)+r(\phi)$. If both equalities hold, $r(\theta+\phi)=s\le d$, while $n(\theta\phi)=2d-s\le d$ forces $s\ge d$. Therefore $s=d$, the sum has full [rank](../../../linear-algebra.md#rank-one-quadratic-form), and the product has [nullity](../../../linear-algebra.md#nullity-of-a-linear-map) $d$. The sum is an [isomorphism](../../../algebra.md#isomorphism) and the product is zero.

Conversely, if $\theta\phi=0$, then $\operatorname{im}\phi\subseteq\ker\theta$, giving $s\le d$. If the sum is also an [isomorphism](../../../algebra.md#isomorphism), its [rank](../../../linear-algebra.md#rank-one-quadratic-form) is $d\le s$. Thus $s=d$, and the two inequalities become equalities. This proves the [equality in the rank-sum and nullity-product inequalities](../../../linear-algebra.md#equality-in-the-rank-sum-and-nullity-product-inequalities) in both directions.

## 10E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

Use the following standard facts: $A_5$ has order $60$ and is a nonabelian [simple group](../../../finite-group-theory.md#simple-group); the [coset action](../../../group-theory.md#coset-action) on the cosets of an index-$j$ [subgroup](../../../group.md#subgroup) is a transitive [homomorphism](../../../algebra.md#homomorphism) into $S_j$. If $H<A_5$ has index $j>1$, that action is nontrivial. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is a [normal subgroup](../../../group-theory.md#normal-subgroup), hence is trivial by simplicity. It would therefore embed $A_5$ in $S_j$. For $j=2,3,4$ this is impossible since $j!<60$. **There are no [subgroups](../../../group.md#subgroup) of indices 2, 3 or 4.**

An index-5 [subgroup](../../../group.md#subgroup) has order $12$ by [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). Consider its natural action on the five letters. It cannot be transitive, since an orbit of size 5 would divide its order by the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem). If it had no fixed letter, its orbits would have sizes 2 and 3. It would then be a [subgroup](../../../group.md#subgroup) of the [permutations](../../../combinatorics.md#permutation) preserving that partition, namely $S_2\times S_3$. Exactly half of those 12 [permutations](../../../combinatorics.md#permutation) are even, so $(S_2\times S_3)\cap A_5$ has order 6, too small to contain $H$.

Thus $H$ fixes a letter $i$. The stabilizer of $i$ in $A_5$ is the copy of $A_4$ consisting of even [permutations](../../../combinatorics.md#permutation) of the other four letters; it has order 12. Containment and equality of orders force $H$ to equal that stabilizer. Conversely each such stabilizer has index 5. Consequently

$$
\boxed{\text{The index-5 subgroups are precisely }\operatorname{Stab}_{A_5}(i),\quad i=1,\ldots,5.}
$$

These five [subgroups](../../../group.md#subgroup) are distinct: for $i\ne j$, a [three-cycle](../../../finite-group-theory.md#three-cycle) on letters other than $i$ can move $j$, so it belongs to the stabilizer of $i$ but not that of $j$.

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

Let $S_N(x)=\sum_{n=1}^N[a_n\cos(nx)+b_n\sin(nx)]$. Under the first coefficient bounds,

$$
\sup_{x\in\mathbb R}|S_M(x)-S_N(x)|\le2c\sum_{n>N}n^{-1-\varepsilon}\longrightarrow0.
$$

This proves the uniform Cauchy condition on the whole [real line](../../../real-analysis.md#real-line) and hence [uniform convergence](../../../real-analysis.md#uniform-convergence) to $f$. It is the [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) applied with the summable majorant $2cn^{-1-\varepsilon}$. Every partial sum is continuous. To see continuity of the limit explicitly, at a chosen $x_0$ first choose $N$ with small uniform error; then make $|S_N(x)-S_N(x_0)|$ small by continuity. The inequality

$$
|f(x)-f(x_0)|\le|f(x)-S_N(x)|+|S_N(x)-S_N(x_0)|+|S_N(x_0)-f(x_0)|
$$

proves continuity. Also $S_N(x+2\pi)=S_N(x)$ for every $N$, so taking limits gives **$f(x+2\pi)=f(x)$**.

Under the stronger coefficient bounds, the [derivative](../../../calculus.md#derivative) series has summable uniform majorant $2cn^{-1-\varepsilon}$. Thus $S_N'$ converges uniformly to a continuous function $g$ given by that series. The original series also converges uniformly. On any finite interval, the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives $S_N(x)-S_N(0)=\int_0^x S_N'(t)dt$. [Uniform convergence](../../../real-analysis.md#uniform-convergence) permits passage to the limit inside this finite [integral](../../../calculus.md#integral), since the error is at most $|x|\|S_N'-g\|_\infty$. Therefore $f(x)-f(0)=\int_0^x g(t)dt$, and continuity of $g$ gives $f'=g$. This justifies [Termwise differentiation of a Fourier series](../../../fourier-series.md#termwise-differentiation-of-a-fourier-series) rather than assuming it:

$$
\boxed{f'(x)=-\sum_{n\ge1}na_n\sin(nx)+\sum_{n\ge1}nb_n\cos(nx).}
$$

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/i">i</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/i/solution">Solution</h4>

↑ **Parent:** [I](#12f/i)

The [product topology](../../../geometry-and-topology.md#product-topology) on $X\times Y$ consists of arbitrary unions of rectangles $U\times V$, with $U$ open in $X$ and $V$ open in $Y$. Equivalently, these rectangles form a [basis](../../../vector-space.md#basis).

The empty set is the empty union, and $X\times Y$ is itself an allowed rectangle. An arbitrary union of sets of this form is still a union of allowed rectangles. Finally,

$$
(U_1\times V_1)\cap(U_2\times V_2)=(U_1\cap U_2)\times(V_1\cap V_2),
$$

which is an allowed rectangle because the factor topologies are closed under finite intersections. Distributing intersection over unions shows that the intersection of any two product-open sets is product-open; induction handles all finite intersections. These verify every [topology axiom](../../../topology.md#topology-axiom). Rectangles alone are generally not a topology, which is why their arbitrary unions are included.

<h3 id="12f/ii">ii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12f/ii)

Parametrize the [logarithmic spiral](../../../topology.md#logarithmic-spiral) by

$$
h:\mathbb R\longrightarrow X,\qquad h(t)=(e^t\cos t,e^t\sin t).
$$

The map is continuous into the ambient plane, hence into $X$ with its [subspace topology](../../../topology.md#subspace-topology), and it is onto by the definition of the spiral. It is injective because its radius $|h(t)|=e^t$ determines $t$ uniquely, even when the angular coordinate winds through repeated turns.

Every point of $X$ is nonzero. The inverse is therefore

$$
\boxed{h^{-1}(x,y)=\log\sqrt{x^2+y^2},}
$$

the restriction of a continuous function on the punctured plane. Hence $h$ is a [homeomorphism](../../../topology.md#homeomorphism) and **the spiral is homeomorphic to the [real line](../../../real-analysis.md#real-line)**. Its accumulation at the origin causes no failure of this argument: the origin is not included in $X$.

## 13D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13d/solution">Solution</h3>

↑ **Parent:** [13D](#13d)

Let $F(z)=e^{az}/(1+e^z)$ and integrate counterclockwise around the rectangle with vertices $-R,R,R+2\pi i,-R+2\pi i$. It contains a single [simple pole](../../../isolated-singularity.md#simple-pole) at $z=\pi i$, with [residue](../../../analysis.md#residue)

$$
\operatorname{Res}_{z=\pi i}F=\frac{e^{a\pi i}}{e^{\pi i}}=-e^{a\pi i}.
$$

On the top edge $F(x+2\pi i)=e^{2\pi ia}F(x)$, and its orientation reverses that of the bottom edge. On the right edge $|F|\le e^{aR}/(e^R-1)$, so its [integral](../../../calculus.md#integral) tends to zero for $a<1$. On the left $|F|\le e^{-aR}/(1-e^{-R})$, which tends to zero for $a>0$. The [residue theorem](../../../analysis.md#residue-theorem) therefore gives

$$
(1-e^{2\pi ia})\int_{-\infty}^{\infty}\frac{e^{ax}}{1+e^x}\,dx=-2\pi i e^{a\pi i}.
$$

Since $1-e^{2\pi ia}=-2ie^{\pi ia}\sin(\pi a)$,

$$
\boxed{\int_{-\infty}^{\infty}\frac{e^{ax}}{1+e^x}\,dx=\frac\pi{\sin(\pi a)}.}
$$

The restriction is also necessary for ordinary convergence: at $-\infty$ the integrand behaves as $e^{ax}$, requiring $a>0$, while at $+\infty$ it behaves as $e^{(a-1)x}$, requiring $a<1$. At either endpoint one tail approaches a nonzero constant; outside this range one tail grows. There is no cancellation because the real integrand is positive.

## 14A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14a/solution">Solution</h3>

↑ **Parent:** [14A](#14a)

In orthonormal Cartesian coordinates, a second-rank [tensor](../../../linear-algebra.md#tensor) has components transforming under a change of axes $Q$ as $M'_{ij}=Q_{ik}Q_{j\ell}M_{k\ell}$, where $QQ^T=I$. Its contraction is invariant:

$$
M'_{ii}=Q_{ik}Q_{i\ell}M_{k\ell}=\delta_{k\ell}M_{k\ell}=M_{kk}.
$$

Thus **$M_{ii}$ is a scalar**. This is [tensor contraction](../../../linear-algebra.md#tensor-contraction) with the [Euclidean metric](../../../differential-geometry.md#euclidean-metric). In general nonorthonormal coordinates the invariant expression is $g^{ij}M_{ij}$, not an unweighted sum of diagonal covariant components.

For the planar plate, every mass element has $z=0$. The [inertia tensor](../../../classical-mechanics.md#inertia-tensor) is consequently

$$
M=\begin{pmatrix}
\int_Dy^2\rho\,dS&-\int_Dxy\rho\,dS&0\\
-\int_Dxy\rho\,dS&\int_Dx^2\rho\,dS&0\\
0&0&\int_D(x^2+y^2)\rho\,dS
\end{pmatrix}.
$$

It follows directly that $\mathbf e_z$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) and

$$
\boxed{M_\perp=\int_D(x^2+y^2)\rho\,dS.}
$$

The real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) has three real [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Its [trace](../../../linear-algebra.md#matrix-trace) is $2\int_D(x^2+y^2)\rho\,dS=2M_\perp$, so $M_1+M_2+M_\perp=2M_\perp$. Hence the [perpendicular axis theorem](../../../classical-mechanics.md#perpendicular-axis-theorem) gives **$M_\perp=M_1+M_2$**.

For a disc of constant areal [density](../../../fluid-mechanics.md#density) $\rho_0$, symmetry gives $\int_Dxy\,dS=0$, and polar integration gives $\int_Dx^2\,dS=\int_Dy^2\,dS=\pi a^4/4$. Therefore

$$
\boxed{M=\frac{\pi\rho_0a^4}{4}\operatorname{diag}(1,1,2)
=\frac{Ma^2}{4}\operatorname{diag}(1,1,2),\qquad M=\pi\rho_0a^2,}
$$

where the scalar $M$ in the last expression denotes the total mass rather than the [tensor](../../../linear-algebra.md#tensor).

## 15B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

**No: ordering the attractive potentials does not impose the proposed ordering of reflection probabilities.** Take $k=\pi/(4a)$ and let $M$ denote the particle mass. Choose $V_2=0$ everywhere and

$$
V_1(x)=\begin{cases}-4\hbar^2k^2/M,&|x|<a,\\0,&|x|\ge a.\end{cases}
$$

These satisfy every stated ordering and support condition. The incoming energy is $\hbar^2k^2/(2M)$; the interior [wavenumber](../../../wave-equation.md#wavenumber) in the [finite square well](../../../quantum-mechanics.md#finite-square-well) is $q=\sqrt{k^2-2MV_1/\hbar^2}=3k$.

Here is an explicit matching calculation. For a general well of width $L=2a$, take exterior waves $e^{ik(x+a)}+re^{-ik(x+a)}$ on the left and $te^{ik(x-a)}$ on the right. Shifting the incident phase in this way does not change the [reflection probability](../../../quantum-mechanics.md#quantum-reflection-probability). Continuity of the [wavefunction](../../../quantum-mechanics.md#wave-function) and its first [derivative](../../../calculus.md#derivative) gives the propagation relation

$$
\begin{pmatrix}t\\ikt\end{pmatrix}
=\begin{pmatrix}\cos(qL)&\sin(qL)/q\\-q\sin(qL)&\cos(qL)\end{pmatrix}
\begin{pmatrix}1+r\\ik(1-r)\end{pmatrix}.
$$

Inverting it and adding the two equations after dividing the [derivative](../../../calculus.md#derivative) equation by $ik$ yields

$$
t=\frac2{2\cos(qL)-i(k/q+q/k)\sin(qL)},\qquad
r=\frac{i(q/k-k/q)\sin(qL)}{2\cos(qL)-i(k/q+q/k)\sin(qL)}.
$$

The incident and reflected exterior waves have the same speed, so their [flux](../../../physics.md#flux) ratio is

$$
p_1=|r|^2=\frac{(q^2-k^2)^2\sin^2(qL)}{4k^2q^2+(q^2-k^2)^2\sin^2(qL)}.
$$

For the chosen parameters $qL=3\pi/2$ and $(q^2-k^2)^2/(4k^2q^2)=16/9$. Thus

$$
\boxed{p_1=\frac{16}{25},\qquad p_2=0.}
$$

The zero potential has no reflected component. This proves the failure with explicit probabilities. More generally the same expression vanishes at $qL\in\pi\mathbb Z$, explaining [resonant transmission through a square well](../../../quantum-mechanics.md#resonant-transmission-through-a-square-well) and why increasing attractive well depth does not monotonically control reflection.

## 16G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16g/solution">Solution</h3>

↑ **Parent:** [16G](#16g)

Take zero [electric potential](../../../electromagnetism.md#electric-potential) at infinity and put $K=(4\pi\varepsilon_0)^{-1}$. By [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) and [Gauss's law](../../../electromagnetism.md#gauss-s-law), the [electric field](../../../electromagnetism.md#electric-field) is radial, with magnitude determined by the total enclosed [electric charge](../../../electromagnetism.md#electric-charge). Thus, away from the idealized shell surfaces,

$$
\boxed{\mathbf E(r)=Kq\begin{cases}
0,&0\le r<a,\\
\mathbf e_r/r^2,&a<r<b,\\
-\mathbf e_r/r^2,&b<r<c,\\
2\mathbf e_r/r^2,&r>c.
\end{cases}}
$$

Integrating $E_r=-d\Phi/dr$ from infinity, or adding the three spherical-shell potentials, gives

$$
\boxed{\Phi(r)=Kq\begin{cases}
a^{-1}-2b^{-1}+3c^{-1},&r\le a,\\
r^{-1}-2b^{-1}+3c^{-1},&a\le r\le b,\\
-r^{-1}+3c^{-1},&b\le r\le c,\\
2r^{-1},&r\ge c.
\end{cases}}
$$

The expressions agree at each interface, so the potential is continuous everywhere, including the origin. The [electric field](../../../electromagnetism.md#electric-field) has different interior and exterior limits at each infinitely thin charged surface, with jump equal to [surface charge density](../../../electromagnetism.md#surface-charge-density) divided by $\varepsilon_0$. An ideal sheet has no single classical field value on the sheet itself; the displayed adjacent limits specify the field there. In conducting material of nonzero thickness the internal field is zero.

The [electrostatic energy](../../../electromagnetism.md#electrostatic-energy) is the [integral](../../../calculus.md#integral) of $\varepsilon_0|\mathbf E|^2/2$. There is no contribution from $r<a$, and spherical integration gives

$$
U=\frac{q^2}{8\pi\varepsilon_0}\left[\int_a^b\frac{dr}{r^2}+\int_b^c\frac{dr}{r^2}+4\int_c^\infty\frac{dr}{r^2}\right]
=\boxed{\frac{q^2}{8\pi\varepsilon_0}\left(\frac1a+\frac3c\right).}
$$

The dependence on $b$ cancels because the magnitude of enclosed [electric charge](../../../electromagnetism.md#electric-charge) is $|q|$ on both sides of the middle shell, even though the field direction changes.

## 17A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17a/solution">Solution</h3>

↑ **Parent:** [17A](#17a)

Define source strength $m$ here as the volume [flux](../../../physics.md#flux) through a small sphere around the source. For incompressible [potential flow](../../../fluid-mechanics.md#potential-flow), $\mathbf u=\nabla\phi$ and the governing conditions are

$$
\Delta\phi=m\delta(\mathbf x-\mathbf x_s),\qquad
\partial_z\phi=0\text{ on }z=0,\qquad \phi\to0\text{ at infinity}.
$$

Equivalently the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) holds away from the source, with local behavior $\phi\sim-m/(4\pi|\mathbf x-\mathbf x_s|)$. The boundary condition expresses impermeability. The [method of images](../../../mathematics.md#method-of-images) uses an equal source below the plane:

$$
\boxed{\phi(\mathbf x)=-\frac m{4\pi}\left(\frac1{\sqrt{x^2+y^2+(z-a)^2}}+\frac1{\sqrt{x^2+y^2+(z+a)^2}}\right).}
$$

The image singularity lies outside the fluid, the two vertical [derivatives](../../../calculus.md#derivative) cancel on the wall, and the source has the specified outward [flux](../../../physics.md#flux).

Let $s=\sqrt{x^2+y^2}$. On the wall $u_z=0$ and the tangential radial velocity is $u_s=ms/[2\pi(s^2+a^2)^{3/2}]$. With ambient [pressure](../../../thermodynamics.md#pressure) $p_\infty$, the steady [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) in this [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) gives

$$
\boxed{p(s,0)=p_\infty-\frac{\rho m^2s^2}{8\pi^2(s^2+a^2)^3}.}
$$

The fluid [pressure](../../../thermodynamics.md#pressure) is reduced everywhere on the wall except at its axis and in the infinite-distance limit. The finite hydrodynamic force is the excess over the uniform ambient-pressure force. Integrating its magnitude over the plane yields

$$
F=2\pi\int_0^\infty[p_\infty-p(s,0)]s\,ds
=\frac{\rho m^2}{4\pi}\int_0^\infty\frac{s^3\,ds}{(s^2+a^2)^3}.
$$

Putting $u=s^2$ gives the last [integral](../../../calculus.md#integral) as $\tfrac12\int_0^\infty u(u+a^2)^{-3}du=1/(4a^2)$. Hence

$$
\boxed{F=\frac{\rho m^2}{16\pi a^2},\qquad \mathbf F=F\mathbf e_z.}
$$

Relative to ambient [pressure](../../../thermodynamics.md#pressure) on the other side, the boundary is **attracted toward the source**. This is the [hydrodynamic attraction of a plane wall to a point source](../../../fluid-mechanics.md#hydrodynamic-attraction-of-a-plane-wall-to-a-point-source).

There is an alternative source-strength convention: if $m$ denotes the coefficient in $u_r=m/r^2$ rather than total volume [flux](../../../physics.md#flux), replace the [flux](../../../physics.md#flux) above by $4\pi m$. Then $\phi=-m(1/r_++1/r_-)$, $p-p_\infty=-2\rho m^2s^2/(s^2+a^2)^3$, and $F=\pi\rho m^2/a^2$. The physical result is identical once the normalization is fixed.

## 18C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18c/solution">Solution</h3>

↑ **Parent:** [18C](#18c)

A [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic) $T(X)$ for $\theta$ is a function of the observations whose conditional distribution of $X$ given $T(X)$ does not depend on $\theta$, whenever that conditioning event is possible. It retains all parameter dependence of the [likelihood](../../../statistical-modelling.md#likelihood-function).

In the discrete case the [Fisher-Neyman factorization theorem](../../../probability-and-statistics.md#fisher-neyman-factorization-theorem) provides a direct criterion: $f(x\mid\theta)=g(T(x),\theta)h(x)$, where $h$ is independent of the parameter. To justify sufficiency, for a value $t$ with positive probability, sum this expression over its fiber and divide:

$$
\mathbb P_\theta(X=x\mid T=t)=\frac{h(x)}{\sum_{y:T(y)=t}h(y)},\qquad T(x)=t.
$$

The parameter-dependent factor cancels. Conversely, parameter-independent conditional probabilities $h_t(x)$ give the factorization $f(x\mid\theta)=\mathbb P_\theta(T=t)h_t(x)$ with $t=T(x)$. Thus the criterion is both necessary and sufficient, with conditional laws only required on fibers of positive probability.

For the shifted exponential sample the [likelihood](../../../statistical-modelling.md#likelihood-function) is

$$
f(x\mid\theta)=\lambda^n e^{-\lambda\sum_i x_i}e^{n\lambda\theta}\mathbf1_{\{\theta\le\min_i x_i\}},\qquad\theta\ge0.
$$

It factors through $T=X_{(1)}=\min_iX_i$, so **the sample minimum is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic)**. Writing $Y_i=X_i-\theta$, independence gives for $t\ge0$

$$
\mathbb P(T-\theta>t)=\prod_i\mathbb P(Y_i>t)=e^{-n\lambda t}.
$$

Therefore $T-\theta$ is exponential with rate $n\lambda$. Its [mean](../../../probability-theory.md#expected-value) is $(n\lambda)^{-1}$ and its [variance](../../../variance.md) is $(n\lambda)^{-2}$. The [unbiased endpoint estimator for a shifted exponential sample](../../../statistical-modelling.md#unbiased-endpoint-estimator-for-a-shifted-exponential-sample) is consequently

$$
\boxed{\widehat\theta=X_{(1)}-\frac1{n\lambda},\quad
\mathbb E_\theta[\widehat\theta]=\theta,\quad
\operatorname{Var}_\theta(\widehat\theta)=\frac1{(n\lambda)^2}.}
$$

Although the parameter is nonnegative, this [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) can be negative. Truncating it at zero would change its expectation and lose the requested property of an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator).

## 19C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19c/solution">Solution</h3>

↑ **Parent:** [19C](#19c)

For the natural [filtration](../../../stochastic-process.md#filtration-probability-theory) $\mathcal F_n=\sigma(X_0,\ldots,X_n)$, a [stopping time](../../../martingale.md#stopping-time) $T$ takes values in $\{0,1,\ldots\}\cup\{\infty\}$ and satisfies $\{T\le n\}\in\mathcal F_n$ for each $n$. Whether it has occurred by time $n$ can be decided from the observations through that time.

The [Strong Markov property](../../../markov-process.md#strong-markov-property) for a time-homogeneous [Markov chain](../../../markov-process.md#markov-chain) says that, on $\{T<\infty\}$, conditional on $\mathcal F_T$, the process $(X_{T+r})_{r\ge0}$ has the law of a fresh chain started at $X_T$. In particular its future conditional law depends on the past only through $X_T$. For example $\mathbb P(X_{T+r}=j\mid\mathcal F_T)=(P^r)_{X_Tj}$ on that event, and the corresponding statement holds for every finite future path.

Start at $i$ and let $T_0=0$, $T_{r+1}=\inf\{n>T_r:X_n=i\}$, with $\inf\varnothing=\infty$. These are [stopping times](../../../martingale.md#stopping-time). Put $f=\mathbb P_i(T_1<\infty)$. Each finite return restarts the chain at $i$, so the [Strong Markov property](../../../markov-process.md#strong-markov-property) gives inductively

$$
\mathbb P_i(T_r<\infty)=f^r.
$$

The events decrease as $r$ increases; infinitely many visits occur exactly when every return time is finite. Continuity of probability therefore gives

$$
\boxed{\mathbb P_i(\text{infinitely many visits to }i)=\lim_{r\to\infty}f^r
=\begin{cases}0,&f<1,\\1,&f=1.\end{cases}}
$$

No irreducibility assumption is needed for this zero-one conclusion at the starting state.

Let $N=\sum_{n\ge0}\mathbf1_{\{X_n=i\}}$, counting the initial visit. Summing nonnegative random variables and then using the tail-sum identity gives

$$
\sum_{n\ge0}\mathbb P_i(X_n=i)=\mathbb E_iN
=\sum_{r\ge0}\mathbb P_i(N\ge r+1)=\sum_{r\ge0}f^r.
$$

If $f<1$, this is $1/(1-f)<\infty$. Thus [divergence](../../../calculus.md#divergence) of the given sum forces $f=1$, and **infinitely many visits then occur with probability one**. This proves the [recurrence criterion by return probabilities](../../../markov-process.md#recurrence-criterion-by-return-probabilities) directly from the regeneration at return times; divergent probability sums alone would not suffice for arbitrary dependent events.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
