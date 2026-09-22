# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_3.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
  - [i](#3b/i)
    - [Solution](#3b/i/solution)
  - [ii](#3b/ii)
    - [Solution](#3b/ii/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5F](#5f)
  - [Solution](#5f/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7G](#7g)
  - [Solution](#7g/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9D](#9d)
  - [Solution](#9d/solution)
- [10B](#10b)
  - [Solution](#10b/solution)
- [11C](#11c)
  - [i](#11c/i)
    - [Solution](#11c/i/solution)
  - [ii](#11c/ii)
    - [Solution](#11c/ii/solution)
- [12A](#12a)
  - [Solution](#12a/solution)
- [13B](#13b)
  - [Solution](#13b/solution)
- [14A](#14a)
  - [Solution](#14a/solution)
- [15H](#15h)
  - [Solution](#15h/solution)
- [16G](#16g)
  - [Solution](#16g/solution)
- [17H](#17h)
  - [Solution](#17h/solution)
- [18E](#18e)
  - [Solution](#18e/solution)
- [19F](#19f)
  - [Solution](#19f/solution)
- [20D](#20d)
  - [a](#20d/a)
    - [Solution](#20d/a/solution)
  - [b](#20d/b)
    - [Solution](#20d/b/solution)
  - [c](#20d/c)
    - [Solution](#20d/c/solution)

## 1C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

The [conjugate group elements](../../../group-theory.md#conjugate-group-elements) relation is $x\sim y$ when $y=gxg^{-1}$ for some $g\in G$. It is reflexive by taking the identity, symmetric because $x=g^{-1}yg$, and transitive because $y=gxg^{-1}$ and $z=hyh^{-1}$ imply $z=(hg)x(hg)^{-1}$. Hence it is an [equivalence relation](../../../set-theory.md#equivalence-relation).

For a finite [group](../../../group.md), the [centralizer](../../../group-theory.md#centralizer) $C_G(x)=\{g:gx=xg\}$ is a subgroup. The map $g\mapsto gxg^{-1}$ has equal values at $g,h$ exactly when $h^{-1}g\in C_G(x)$. Its fibers are therefore the left cosets of $C_G(x)$, giving

$$
\boxed{|\operatorname{Cl}(x)|=[G:C_G(x)]=\frac{|G|}{|C_G(x)|}}.
$$

By [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), this index divides $|G|$. This is also the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) for the conjugation action, with the centralizer as stabilizer.

## 2A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

For curvature $-1$, the [Poincare disc model](../../../geometry-and-topology.md#poincare-disk-model) has metric and area element

$$
\boxed{ds^2=\frac{4(dx^2+dy^2)}{(1-x^2-y^2)^2}},\qquad dA=\frac{4r\,dr\,d\theta}{(1-r^2)^2}.
$$

The given minimizing-diameter property makes the distance from zero to Euclidean radius $R$ equal to

$$
\rho=\int_0^R\frac{2\,dr}{1-r^2}=\log\frac{1+R}{1-R},\qquad\boxed{R=\tanh(\rho/2)}.
$$

Radial symmetry therefore identifies the whole [hyperbolic circle in the Poincare disc](../../../geometry-and-topology.md#hyperbolic-circle-in-the-poincare-disc). Integrating its enclosed [hyperbolic area](../../../geometry-and-topology.md#hyperbolic-area) gives

$$
A=\int_0^{2\pi}\int_0^R\frac{4r}{(1-r^2)^2}\,dr\,d\theta=4\pi\left(\frac1{1-R^2}-1\right)=\boxed{2\pi(\cosh\rho-1)}.
$$

For a geodesic [hyperbolic triangle](../../../geometry-and-topology.md#hyperbolic-triangle) with angles $\alpha,\beta,\gamma$, the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) states $A=\pi-(\alpha+\beta+\gamma)$, in particular $A\leq\pi$, with strict inequality for ordinary finite vertices. Let $d$ be the distance of the interior point $P$ to the nearest side. The open disc of radius $d$ about $P$ is contained in the triangle: a path from $P$ to an exterior point must first cross the boundary at distance at least $d$. A hyperbolic isometry carries its center to zero, so its area is the area already calculated. Consequently

$$
2\pi(\cosh d-1)\leq A\leq\pi,\qquad\boxed{d\leq\operatorname{arcosh}(3/2)}.
$$

This uses [hyperbolic area bounds an inscribed disc](../../../geometry-and-topology.md#hyperbolic-area-bounds-an-inscribed-disc) and establishes the requested bound without assuming that $P$ is an incenter. A sharper universal triangle bound is possible, but is not needed here.

## 3B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

A function is a [differentiable function](../../../analysis.md#differentiable-function) at $a_0=(a,b)$ if there is a [linear map](../../../vector-space.md#linear-map) $L:\mathbb R^2\to\mathbb R$ with

$$
f(a_0+h)=f(a_0)+Lh+r(h),\qquad\frac{r(h)}{\|h\|}\longrightarrow0\quad(h\to0).
$$

The map $L=Df_{a_0}$ is its derivative; equivalently $L(h_1,h_2)=Ah_1+Bh_2$ for fixed constants. Since every such linear map is bounded, $|f(a_0+h)-f(a_0)|\leq\|L\|\|h\|+|r(h)|\to0$. This proves **[differentiability implies continuity](../../../analysis.md#differentiability-implies-continuity)**, not merely continuity along each coordinate axis.

<h3 id="3b/i">i</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/i/solution">Solution</h4>

↑ **Parent:** [I](#3b/i)

Put $r=(x^2+y^2)^{1/2}$. Since $x^2y^2\leq(x^2+y^2)^2/4$, the nonzero-point expression satisfies

$$
0\leq |f(x,y)|\leq\frac{r^2}{4},\qquad\frac{|f(x,y)-f(0,0)|}{r}\leq\frac r4\longrightarrow0.
$$

Thus the defining remainder condition for [differentiability](../../../analysis.md#differentiability) holds with the zero [linear map](../../../vector-space.md#linear-map):

$$
\boxed{Df_{(0,0)}=0.}
$$

The estimate controls every approach direction at once, which is stronger than merely finding the two zero partial derivatives.

<h3 id="3b/ii">ii</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3b/ii)

On the nonzero $x$ axis the function equals one, whereas its assigned value at the origin is zero. Therefore $f(x,0)$ does not tend to $f(0,0)$ as $x\to0$. It is not a [continuous function](../../../calculus.md#continuous-function) there, and [differentiability implies continuity](../../../analysis.md#differentiability-implies-continuity) shows

$$
\boxed{f\text{ is not differentiable at }(0,0).}
$$

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Include the empty set, and take all unions of intervals $[a,b)$ with $a<b$. These intervals cover the real line, and the intersection of two is either empty or $[\max(a,c),\min(b,d))$. Distributing intersections over unions therefore makes finite intersections of open sets open; arbitrary unions are open by construction. The whole line is open, so the axioms of a [topology](../../../topology.md) hold. This is the [lower limit topology](../../../topology.md#lower-limit-topology), whose space is the [Sorgenfrey line](../../../topology.md#lower-limit-topology).

If $x<y$, the neighborhoods $[x,y)$ and $[y,y+1)$ are disjoint. Hence $\boxed{(\mathbb R,\tau_1)\text{ is Hausdorff}}$.

For the identity into the [cofinite topology](../../../topology.md#cofinite-topology), an inverse image is the same subset of $\mathbb R$. Let $F$ be finite and $x\notin F$. If $F$ has a point greater than $x$, choose $b$ to be its least such point; otherwise take $b=x+1$. Then $[x,b)$ avoids every point of $F$, including $b$ itself. Taking these intervals over all $x\notin F$ writes $\mathbb R\setminus F$ as a $\tau_1$-open set. The inverse image of every cofinite open set, and of the empty set, is open. **The identity map is continuous**, because $\tau_2\subseteq\tau_1$.

## 5F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5f/solution">Solution</h3>

↑ **Parent:** [5F](#5f)

A real [harmonic function](../../../partial-differential-equation.md#harmonic-function) on a planar open set is a twice continuously differentiable function satisfying $f_{xx}+f_{yy}=0$. The ordered pair $(f,g)$ consists of [harmonic conjugates](../../../partial-differential-equation.md#harmonic-conjugate) when $f+ig$ is holomorphic; the corresponding [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) are $f_x=g_y$ and $f_y=-g_x$.

To prove [composition of harmonic conjugate pairs](../../../partial-differential-equation.md#composition-of-harmonic-conjugate-pairs), denote $P=p(u,v)$ and $Q=q(u,v)$, and assume the inner pair's image lies in the outer pair's domain. Their equations are $u_x=v_y$, $u_y=-v_x$, $p_u=q_v$ and $p_v=-q_u$. The [chain rule](../../../calculus.md#chain-rule) gives

$$
P_x=p_uu_x+p_vv_x=p_uu_x-q_uv_x=Q_y,
$$



$$
P_y=p_uu_y+p_vv_y=-p_uv_x-q_uu_x=-Q_x.
$$

Thus the composite satisfies the Cauchy-Riemann equations. Its components are $C^2$, and differentiating gives $P_{xx}+P_{yy}=Q_{yx}-Q_{xy}=0$ and similarly $Q_{xx}+Q_{yy}=0$. **The composite pair is harmonic conjugate**, including when the inner map has a critical point.

## 6E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

At a regular point of the constraint curve, $\nabla g\ne0$. A constrained stationary point has $Df$ zero on every tangent vector annihilated by $Dg$, so its gradient is normal to the curve. The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations are therefore $\nabla f=\lambda\nabla g$ together with $g=0$. Singular constraint points require separate examination.

Assume $a,b>0$. For the ellipse, the equations are

$$
y=\frac{2\lambda x}{a^2},\qquad x=\frac{2\lambda y}{b^2},\qquad\frac{x^2}{a^2}+\frac{y^2}{b^2}=1.
$$

Neither coordinate can vanish at a stationary point, because the first two equations would then force both to vanish. Multiplication gives $4\lambda^2=a^2b^2$. Therefore $y=\pm(b/a)x$, and the constraint gives $x^2=a^2/2$, $y^2=b^2/2$. The stationary values are

$$
\boxed{xy=ab/2\text{ at }(a/\sqrt2,b/\sqrt2),(-a/\sqrt2,-b/\sqrt2),}
$$



$$
\boxed{xy=-ab/2\text{ at }(a/\sqrt2,-b/\sqrt2),(-a/\sqrt2,b/\sqrt2).}
$$

The compact ellipse has global extrema, all its points are regular, and these are all stationary points. Hence the first value is the global maximum and the second the global minimum.

## 7G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7g/solution">Solution</h3>

↑ **Parent:** [7G](#7g)

For a state in the domain of the operator, its [expectation value](../../../quantum-mechanics.md#expectation-value) is

$$
\langle\mathcal O\rangle=\frac{\int\Psi^*(x,t)(\mathcal O\Psi)(x,t)\,dx}{\int|\Psi(x,t)|^2dx}.
$$

For a normalized state the denominator is one. Use an orthonormal [energy eigenstate](../../../quantum-mechanics.md#energy-eigenstate) basis, choosing orthogonal vectors within degenerate eigenspaces. Inserting an expansion into the time-dependent [Schrödinger equation](../../../physics.md#schrodinger-equation) gives $i\hbar\dot a_n(t)=E_na_n(t)$. Consequently

$$
\boxed{\Psi(x,t)=\sum_n a_n e^{-iE_nt/\hbar}u_n(x)}.
$$

The phases preserve normalization. Projection onto a specified basis eigenstate gives probability $\boxed{|a_p|^2}$, independent of time. If the measurement distinguishes only the energy and $E_p$ is degenerate, sum $|a_n|^2$ over all $n$ with $E_n=E_p$.

Using orthonormality to eliminate all cross terms,

$$
\boxed{\langle H\rangle=\sum_n|a_n|^2E_n}.
$$

This is time independent whenever the expectation is defined. The time-independent Hamiltonian changes only relative phases, not the energy probabilities.

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Write $Q=\sum_i(X_i-\bar X)^2$ and $Q_0=\sum_i(X_i-\mu_0)^2=Q+n(\bar X-\mu_0)^2$. The normal-sample likelihood is

$$
L(\mu,\sigma^2)=(2\pi\sigma^2)^{-n/2}\exp\left[-\frac{\sum_i(X_i-\mu)^2}{2\sigma^2}\right].
$$

Without the mean restriction, its maximum has $\widehat\mu=\bar X$ and $\widehat\sigma^2=Q/n$. Under the null, the maximizing variance is $Q_0/n$. Substituting them gives the [generalized likelihood-ratio test](../../../statistical-modelling.md#generalized-likelihood-ratio-test) statistic

$$
\Lambda=\frac{\sup_{H_0}L}{\sup L}=\left(\frac Q{Q_0}\right)^{n/2}=\boxed{\left(1+\frac{T^2}{n-1}\right)^{-n/2}},
$$

where $S^2=Q/(n-1)$ and $T=\sqrt n(\bar X-\mu_0)/S$. Assume $n\geq2$; $Q>0$ almost surely for positive population variance.

The ratio decreases strictly as $|T|$ increases, so rejecting for small $\Lambda$ is equivalent to rejecting for large $|T|$. Under $H_0$, $T$ has [Student's t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ degrees of freedom. Therefore the exact size-$\alpha$ rule is

$$
\boxed{|T|>t_{n-1,\,1-\alpha/2}}.
$$

This is the two-sided [Student's t-test](../../../statistical-modelling.md#student-s-t-test). Equivalently reject when $\Lambda<(1+t_{n-1,1-\alpha/2}^2/(n-1))^{-n/2}$. No large-sample chi-squared approximation is needed for this [normal-mean likelihood ratio with unknown variance](../../../statistical-modelling.md#normal-mean-likelihood-ratio-with-unknown-variance).

## 9D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9d/solution">Solution</h3>

↑ **Parent:** [9D](#9d)

For a state $i$, let $N_i=\{n\geq1:P^n_{ii}>0\}$ and $d_i=\gcd N_i$. If distinct states $i,j$ communicate, choose positive-probability paths $i\to j$ and $j\to i$ of lengths $r,s$. Then $r+s$ is a return time to each. For every $n\in N_i$, concatenate $j\to i$, the $i$-return loop, and $i\to j$ to see that $s+n+r\in N_j$. Since $d_j$ divides this and $s+r$, it divides $n$. Thus $d_j\mid d_i$, and interchanging the states gives $d_i\mid d_j$. This proves **[period is constant on a communicating class](../../../markov-process.md#period-is-constant-on-a-communicating-class)**.

Read the transition matrix from the original PDF; the converted TeX loses the location of the second row's final entry. The [communicating classes](../../../markov-process.md#communicating-class) are

$$
\boxed{\{1,3,4\},\quad\{2,7\},\quad\{6\},\quad\{5\}}.
$$

Within $\{1,3,4\}$ the only internal cycle is $1\to3\to4\to1$. Return lengths are multiples of three, and length three has positive probability, so its period is three. This class is open because it has exits to other classes. The class $\{2,7\}$ is the closed deterministic two-cycle, of period two. The absorbing class $\{6\}$ is closed and has period one.

State 5 has outgoing transitions but no incoming transition at all, so it is an open singleton class and $N_5=\varnothing$. For this [return-free state in a Markov chain](../../../markov-process.md#return-free-state-in-a-markov-chain), the convention $\gcd\varnothing=0$ gives **period zero**; if period is defined only when positive return times exist, it is undefined instead. In particular, this singleton is not aperiodic: aperiodicity would require period one.

## 10B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10b/solution">Solution</h3>

↑ **Parent:** [10B](#10b)

On the smooth-function space, the product rule gives $ABf=(xf)'=f+xf'$ while $BAf=xf'$. Hence $\boxed{[A,B]=I}$, and both maps preserve the stated smooth space.

For general operators with this [commutator](../../../lie-algebra.md#commutator) relation, use $[A,BC]=[A,B]C+B[A,C]$. Induction gives $[A,B^i]=iB^{i-1}$ for $i\geq1$. Since $Ay=0$,

$$
\boxed{A(By)=y,\qquad A(B^iy)=iB^{i-1}y\ (i\geq1),\qquad Ay=0.}
$$

Every displayed vector lies in $W$, so $W$ is invariant under $A$, as well as under $B$. Iterating the lowering formula gives $A^kB^iy=i!B^{i-k}y/(i-k)!$ for $k\leq i$, and zero for $k>i$.

Suppose a nontrivial finite [linear dependence](../../../vector-space.md#linear-dependence) has highest nonzero term $c_nB^ny$. Applying $A^n$ kills all lower terms and yields $c_nn!y=0$. The field is real, $n!\ne0$, and $y\ne0$, so this contradicts $c_n\ne0$. Thus **the entire sequence is linearly independent**. This [identity commutator cyclic ladder](../../../lie-algebra.md#identity-commutator-cyclic-ladder) also proves that such a representation with a nonzero vector in the kernel of $A$ cannot be finite dimensional.

## 11C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11c/i">i</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/i/solution">Solution</h4>

↑ **Parent:** [I](#11c/i)

A nonzero [primitive polynomial](../../../commutative-algebra.md#primitive-polynomial) in $\mathbb Z[x]$ has greatest common divisor of its coefficients equal to one. Suppose primitive polynomials $f,g$ had a product whose coefficients were all divisible by some prime $p$. Their reductions in $\mathbb F_p[x]$ are both nonzero, because neither polynomial has every coefficient divisible by $p$. A polynomial ring over a field is an [integral domain](../../../commutative-algebra.md#integral-domain), so their product is nonzero modulo $p$, a contradiction. Hence **the product of primitive polynomials is primitive**.

To deduce unique factorization, write any nonzero integer polynomial as its positive [polynomial content](../../../commutative-algebra.md#polynomial-content) times a primitive polynomial, with its sign treated as a unit. The preceding result gives multiplicativity of content. Factor the primitive part over the Euclidean polynomial ring $\mathbb Q[x]$, and rescale every irreducible rational factor to a primitive integer polynomial. If $f=q\prod_if_i$ with all polynomials primitive and $q=a/b$ in lowest terms, the equality $bf=a\prod_if_i$ has contents $b$ and $|a|$. Thus $b=|a|$, forcing $q=\pm1$. The rational factorization therefore lifts to an integer factorization.

A primitive integer polynomial is irreducible over $\mathbb Z$ exactly when it is irreducible over $\mathbb Q$: an integer factorization gives a rational one, and a rational factorization lifts by the same primitive-content argument. Factor the content into integer primes. Existence and uniqueness over the integers and over $\mathbb Q[x]$ now give existence and uniqueness of the resulting factorization into constant prime factors and primitive irreducible polynomial factors, up to order and signs. Therefore $\boxed{\mathbb Z[x]\text{ is a unique factorization domain}}$. This is the full lifting step in [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials).

<h3 id="11c/ii">ii</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11c/ii)

The polynomial $p=x^5-4x+2$ satisfies the [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) at the prime two: every nonleading coefficient is even, the leading coefficient is not, and the constant term is not divisible by four. Hence it is irreducible over $\mathbb Q$. Its ideal is maximal in $\mathbb Q[x]$; explicitly, for any polynomial not divisible by $p$, the Euclidean algorithm gives $ag+bp=1$, furnishing the inverse of its residue class. Thus

$$
\boxed{\mathbb Q[x]/(p)\text{ is a field}.}
$$

For the integer quotient, division by the monic polynomial $p$ gives a unique remainder of degree below five with integer coefficients. If an integer polynomial becomes zero in the rational quotient, its integer remainder is still divisible by $p$ over $\mathbb Q$, so must be zero. This gives an injective ring map $\mathbb Z[x]/(p)\to\mathbb Q[x]/(p)$, proving the [monic irreducible integer-polynomial quotient is a domain](../../../polynomial.md#monic-irreducible-integer-polynomial-quotient-is-a-domain).

The same unique-remainder argument makes the integer quotient a free abelian group with basis $1,x,x^2,x^3,x^4$. The class of two is nonzero and cannot have an inverse: twice an integer remainder cannot equal the remainder one. Consequently

$$
\boxed{\mathbb Z[x]/(p)\text{ is an integral domain but not a field}.}
$$

## 12A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

Project from the north pole $N=(0,0,1)$ along the line through a sphere point onto the equatorial plane $Z=0$, identified with $\mathbb C$. Parameterizing this line gives

$$
\boxed{\pi(X,Y,Z)=\frac{X+iY}{1-Z},\qquad\pi(N)=\infty}.
$$

The inverse [stereographic projection](../../../complex-analysis.md#stereographic-projection) is

$$
(X,Y,Z)=\frac{(2\operatorname{Re}z,2\operatorname{Im}z,|z|^2-1)}{1+|z|^2}.
$$

Negating the three sphere coordinates consequently sends $z$ to $-1/\bar z$, with $0,\infty$ interchanged. This proves the [antipodal stereographic coordinate relation](../../../complex-analysis.md#antipodal-stereographic-coordinate-relation).

A nonidentity [Möbius transformation](../../../group-theory.md#mobius-transformation) $T(z)=(az+b)/(cz+d)$ has $ad-bc\ne0$. For $c\ne0$, its fixed points are the roots of $cz^2+(d-a)z-b=0$, giving one or two distinct points. If $c=0$ and $a\ne d$, there is one finite root and the fixed point infinity. If $c=0$, $a=d$, and $b\ne0$, it is a translation and only infinity is fixed. The remaining case is the identity, already excluded. Thus the claim includes fixed points at infinity, not just finite solutions of the quadratic.

A nontrivial rotation of the sphere fixes exactly the two poles on its axis, which are antipodal. It therefore gives exactly two fixed stereographic points with $z_2=-1/\bar z_1$. Here the nonzero rotation angle is understood modulo $2\pi$; an angle that is a whole multiple of $2\pi$ would be the identity.

Conversely, use a sphere rotation whose Möbius map $S$ sends the two antipodal fixed points to $0,\infty$. The conjugate $STS^{-1}$ fixes both, hence equals $z\mapsto az$ for some $a\ne0$. If $|a|=1$, write $a=e^{i\theta}$; the inverse stereographic formula shows that this rotates $X+iY$ while leaving $Z$ fixed. Conjugating back by the rotation $S$ gives a sphere rotation. If $|a|<1$, $a^nz\to0$ for every finite $z$. If $|a|>1$, $a^nz\to\infty$ for every $z\ne0$, in the sphere topology. Pulling these conclusions back proves the [antipodal fixed-point classification of Möbius transformations](../../../group-theory.md#antipodal-fixed-point-classification-of-mobius-transformations): **either the map is a sphere rotation or one fixed point attracts every point except the other fixed point**.

## 13B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13b/solution">Solution</h3>

↑ **Parent:** [13B](#13b)

For a [homogeneous function](../../../real-analysis.md#homogeneous-function), fix $x\in U$ and differentiate $f(\lambda x)=\lambda^cf(x)$ at $\lambda=1$. The [chain rule](../../../calculus.md#chain-rule) gives

$$
\boxed{Df_x(x)=cf(x)}.
$$

Conversely, assume this derivative identity throughout $U$. Along a positive ray define $h(\lambda)=\lambda^{-c}f(\lambda x)$. The ray stays in $U$ by hypothesis, and linearity of the derivative gives

$$
h'(\lambda)=\lambda^{-c-1}\{Df_{\lambda x}(\lambda x)-cf(\lambda x)\}=0.
$$

Therefore $h$ is constant on the connected interval $(0,\infty)$ and equals $h(1)=f(x)$. Hence $\boxed{f(\lambda x)=\lambda^cf(x)}$ for every positive $\lambda$. This proves [Euler differential identity characterizes homogeneity](../../../real-analysis.md#euler-differential-identity-characterizes-homogeneity); no connectedness assumption on the whole domain is needed.

## 14A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14a/solution">Solution</h3>

↑ **Parent:** [14A](#14a)

For a function holomorphic on and inside a positively oriented simple closed contour $C$, the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) gives

$$
f(z)=\frac1{2\pi i}\int_C\frac{f(\zeta)}{\zeta-z}\,d\zeta,\qquad f^{(m)}(z)=\frac{m!}{2\pi i}\int_C\frac{f(\zeta)}{(\zeta-z)^{m+1}}\,d\zeta.
$$

If an [entire function](../../../complex-analysis.md#entire-function) is bounded by $M$, apply the derivative formula on a radius-$R$ circle about any $z$ to obtain $|f'(z)|\leq M/R$. Letting $R\to\infty$ makes every derivative $f'(z)$ zero, so $f$ is constant. This proves [Liouville theorem](../../../complex-analysis.md#liouville-theorem) directly.

For the given [meromorphic function](../../../isolated-singularity.md#meromorphic-function), the growth bound excludes poles outside the bounding disc. Its poles inside are finite in number, since poles cannot accumulate at a finite point of a meromorphic function. Subtract all their finite [principal parts](../../../complex-geometry.md#principal-part-of-a-meromorphic-function):

$$
g(z)=f(z)-\sum_p\sum_{j=1}^{m_p}\frac{a_{p,-j}}{(z-p)^j}.
$$

The remainder is entire. The rational sum is $O(1/|z|)$ at infinity. If $n\geq0$, this makes $g(z)=O(|z|^n)$; the [Cauchy estimates](../../../analysis.md#cauchy-estimate) at zero give $|g^{(m)}(0)|\leq m!\,O(R^{n-m})$ for $m>n$, hence these derivatives vanish. Its Taylor series is a polynomial of degree at most $n$. If $n<0$, then $g\to0$ at infinity, so it is bounded and equals zero by Liouville. In both cases, adding back the principal parts proves

$$
\boxed{f\text{ is a rational function}.}
$$

This proof of [polynomial growth forces a meromorphic function to be rational](../../../isolated-singularity.md#polynomial-growth-forces-a-meromorphic-function-to-be-rational) includes negative integers $n$, not only the polynomial-growth case $n\geq0$.

## 15H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15h/solution">Solution</h3>

↑ **Parent:** [15H](#15h)

Write $y(t)=\sum_{k\geq0}a_kt^k$ at the ordinary point zero. Substituting into the [Legendre differential equation](../../../differential-equation.md#legendre-differential-equation) and comparing coefficients gives

$$
\boxed{a_{k+2}=\frac{k(k+1)-\lambda}{(k+1)(k+2)}a_k\quad(k\geq0).}
$$

The two arbitrary coefficients $a_0,a_1$ generate the even and odd series separately, convergent at least for $|t|<1$. A nonzero polynomial of degree $n$ has top coefficient satisfying $[\lambda-n(n+1)]a_n=0$, so $\lambda=n(n+1)$ is necessary. For this value the recurrence in parity $n$ terminates at degree $n$, while the other parity cannot terminate unless its initial coefficient is zero. Thus a polynomial solution exists and is unique up to scale, with $\boxed{P_n(-t)=(-1)^nP_n(t)}$.

For [Orthogonality of Legendre polynomials](../../../differential-equation.md#orthogonality-of-legendre-polynomials), write the equation in self-adjoint form $[(1-t^2)P_n']'+n(n+1)P_n=0$. Multiply it by $P_m$, subtract the equation for $P_m$ multiplied by $P_n$, and integrate. The boundary term is $[(1-t^2)(P_mP_n'-P_nP_m')]_{-1}^1=0$, because the functions are polynomials. For $m\ne n$ the eigenvalues differ, giving $\int_{-1}^1P_nP_m=0$. For $m=n$, the integral of the square is positive. Hence $\int P_nP_m=k_n\delta_{nm}$ with $k_n>0$.

Let $G(x,t)=(1-2xt+x^2)^{-1/2}$. The supplied operator $x\partial_x^2x$ means $x\partial_x^2(xG)$, which equals $\partial_x(x^2\partial_xG)$. Expand $G=\sum_na_n(x)P_n(t)$ in the given identity and use the Legendre equation. Each coefficient satisfies

$$
x^2a_n''+2xa_n'-n(n+1)a_n=0,
$$

whose solutions are $a_n=A_nx^n+B_nx^{-n-1}$. Regularity at $x=0$ removes $B_n$. At $t=1$, normalization $P_n(1)=1$ and $G(x,1)=1/(1-x)$ give $\sum_nA_nx^n=\sum_nx^n$, so $A_n=1$. Thus

$$
\boxed{G(x,t)=\sum_{n=0}^\infty x^nP_n(t),\qquad |x|<1.}
$$

A rigorous justification for the expansion and operations is to begin with the Taylor series of $G$ in $x$. It converges uniformly for $|x|\leq r<1$, $-1\leq t\leq1$. Its $x^n$ coefficient is a degree-$n$ polynomial in $t$, and the differential identity makes that coefficient solve the degree-$n$ Legendre equation. Its value at one is one, so it is exactly $P_n$. This avoids assuming an unjustified endpoint convergence of an arbitrary orthogonal expansion.

Square the generating series and integrate, using uniform convergence and orthogonality:

$$
\sum_{n\geq0}k_nx^{2n}=\int_{-1}^1\frac{dt}{1-2xt+x^2}=\frac1x\log\frac{1+x}{1-x}=2\sum_{n\geq0}\frac{x^{2n}}{2n+1}.
$$

Comparing coefficients proves the [generating function and norm of Legendre polynomials](../../../differential-equation.md#generating-function-and-norm-of-legendre-polynomials) result

$$
\boxed{k_n=\frac2{2n+1}}.
$$

## 16G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16g/solution">Solution</h3>

↑ **Parent:** [16G](#16g)

For an axisymmetric potential, insert $\Psi(r,\phi)=R(r)\Phi(\phi)$ into the time-independent [Schrödinger equation](../../../physics.md#schrodinger-equation) and divide by $R\Phi$. The polar [Laplacian](../../../calculus.md#laplacian) separates the angular equation $\Phi''+m^2\Phi=0$ from

$$
R''+\frac1rR'+\left[\frac{2\mu(E-V(r))}{\hbar^2}-\frac{m^2}{r^2}\right]R=0.
$$

Single-valuedness under $\phi\mapsto\phi+2\pi$ gives $m\in\mathbb Z$, with an angular eigenbasis $\boxed{\Phi=e^{im\phi}}$. Linear combinations of the degenerate $m,-m$ modes are also possible.

Inside the [circular infinite quantum well](../../../quantum-mechanics.md#circular-infinite-quantum-well), put $\rho=r\sqrt{2\mu E/\hbar^2}$. The equation becomes

$$
\boxed{R_{\rho\rho}+\rho^{-1}R_\rho+(1-m^2/\rho^2)R=0}.
$$

The physical solution must be regular at the origin, behaving as $r^{|m|}$ for $m\ne0$, or with finite value and zero radial derivative for $m=0$. At the infinite wall impose $R(r=a)=0$. The printed question's boundary phrase uses capital $R=a$; it means the radial position $r=a$, not a value imposed on the radial wavefunction. The singular [Bessel function of the second kind](../../../analysis.md#bessel-function-of-the-second-kind) is excluded; mere square-integrability of its logarithmic $m=0$ singularity would not put it in the ordinary finite-energy Hamiltonian domain.

For $m=0$, multiply the equation by $\rho^2$ and insert $R=\sum_{k\geq0}A_k\rho^k$. The coefficient of $\rho$ gives $A_1=0$, and subsequent coefficients give

$$
\boxed{A_{k+2}=-\frac{A_k}{(k+2)^2}}.
$$

All odd coefficients vanish, $A_2=-A_0/4$, and $A_4=A_0/64$. The regular solution is a multiple of the [Bessel function of the first kind](../../../analysis.md#bessel-function-of-the-first-kind) $J_0$. Its requested fourth-order estimate is

$$
R(\rho)\approx A_0(1-\rho^2/4+\rho^4/64)=A_0(1-\rho^2/8)^2.
$$

Therefore the first positive zero of this truncation is $\boxed{\rho\approx\sqrt8}$, giving

$$
\boxed{E_0\approx\frac{\hbar^2(\sqrt8)^2}{2\mu a^2}=\frac{4\hbar^2}{\mu a^2}}.
$$

The ground state is in the $m=0$ sector because nonzero angular modes add nonnegative centrifugal kinetic energy to the radial energy form. This [quartic truncation of the Bessel function J0](../../../analysis.md#quartic-truncation-of-the-bessel-function-j0) is only a rough local-series estimate, not an exact eigenvalue or a certified variational bound; its double zero warns that the truncation does not reproduce the simple zero of the full function.

## 17H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17h/solution">Solution</h3>

↑ **Parent:** [17H](#17h)

In vacuum without sources, [Maxwell equations](../../../electromagnetism.md#maxwell-equations) are $\nabla\cdot E=\nabla\cdot B=0$, $\nabla\times E=-\dot B$, and $\nabla\times B=\dot E/c^2$. For $E'=cB$, $B'=-E/c$, both divergences remain zero, and

$$
\nabla\times E'=c\nabla\times B=\dot E/c=-\dot B',\qquad\nabla\times B'=-\nabla\times E/c=\dot B/c=\dot E'/c^2.
$$

This proves the quarter-turn [electromagnetic duality](../../../electromagnetism.md#electromagnetic-duality) transformation.

A [perfect conductor](../../../electromagnetism.md#perfect-conductor) has zero electric field in its bulk. Continuity of tangential electric field therefore gives $n\times E=0$ at its surface. Faraday's law makes a nonzero-frequency magnetic field vanish in that bulk, and continuity of its normal component gives $n\cdot B=0$ for the wave field. An independently trapped static magnetic flux is not excluded by perfect conductivity alone; the stated condition applies to the oscillating field under consideration.

For amplitudes with dependence $e^{i(kz-\omega t)}$, let $\gamma^2=\omega^2/c^2-k^2$ and suppose $(\Delta_\perp+\gamma^2)\psi=0$. With $k\ne0$ and $\omega\ne0$, define the transverse-magnetic family of [scalar-potential conducting waveguide modes](../../../electromagnetism.md#scalar-potential-conducting-waveguide-modes) by

$$
\boxed{e_\perp=\nabla_\perp\psi,\quad e_z=-\frac{i\gamma^2}{k}\psi=i\left(k-\frac{\omega^2}{kc^2}\right)\psi,\quad b_\perp=\frac\omega{kc^2}\widehat z\times\nabla_\perp\psi,\quad b_z=0.}
$$

The electric divergence is $\Delta_\perp\psi+ike_z=0$; the magnetic divergence is zero because the transverse field is a rotated gradient. Direct differentiation gives $\nabla\times e=i\omega b$ and $\nabla\times b=-i\omega e/c^2$, where longitudinal differentiation means multiplication by $ik$. Thus all vacuum equations hold, with $\boxed{\gamma^2=\omega^2/c^2-k^2}$.

On a wall parallel to $z$, $\psi=0$ makes both $e_z$ and the boundary-tangential derivative of $\psi$ vanish. It also makes $n\cdot b$ proportional to that tangential derivative, hence zero. This proves the [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) supplies both conductor conditions.

For a transverse-electric family, use duality and rescale the potential, or check directly that

$$
\boxed{e_\perp=\widehat z\times\nabla_\perp\psi,\quad e_z=0,\quad b_\perp=-\frac k\omega\nabla_\perp\psi,\quad b_z=\frac{i\gamma^2}{\omega}\psi}
$$

satisfies the same equations. If $t=\widehat z\times n$ is the cross-sectional wall tangent, then $t\cdot e=n\cdot\nabla_\perp\psi$ and $n\cdot b=-(k/\omega)n\cdot\nabla_\perp\psi$. Consequently $\boxed{\partial_n\psi=0}$, a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition), supplies both wall conditions. Duality exchanges the field constructions, but does not preserve electric-conductor boundary conditions without this new boundary test.

## 18E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18e/solution">Solution</h3>

↑ **Parent:** [18E](#18e)

Differentiate the [velocity potential](../../../fluid-mechanics.md#velocity-potential) in polar coordinates:

$$
\boxed{u_r=U(1-a^2/r^2)\cos\theta,\qquad u_\theta=-U(1+a^2/r^2)\sin\theta+\frac\kappa{2\pi r}}.
$$

At $r=a$ the normal velocity is zero. At large radius these components tend to $U\cos\theta,-U\sin\theta$, the polar components of uniform flow in the positive $x$ direction. The circulation around any concentric circle is $\int_0^{2\pi}u_\theta r\,d\theta=\kappa$. Although the potential's circulation term is multivalued, its velocity is single-valued and irrotational away from the excluded axis.

For steady inviscid constant-density flow, [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) gives $p+\rho|u|^2/2=p_\infty+\rho U^2/2$. On the cylinder, $u_\theta=-2U\sin\theta+\kappa/(2\pi a)$, so

$$
\boxed{p(a,\theta)=p_\infty+\frac\rho2\left[U^2-\left(-2U\sin\theta+\frac\kappa{2\pi a}\right)^2\right]}.
$$

In the displayed force integral, every constant or $\sin^2\theta$ term has zero cosine and sine first moments. The cross term in pressure is $\rho U\kappa\sin\theta/(\pi a)$. Therefore, using exactly the positive-sign convention printed,

$$
\boxed{F_x=0,\qquad F_y=\rho U\kappa}
$$

per unit axial length, since $\int_0^{2\pi}\sin^2\theta\,d\theta=\pi$.

With the usual normal directed outward from the cylinder into the fluid, pressure exerts traction $-pn$, so the physical force of the fluid on the cylinder is instead $\boxed{(0,-\rho U\kappa)}$. The positive integral printed in the question has the opposite sign. This makes the convention explicit and is consistent with the [Kutta–Joukowski theorem](../../../fluid-mechanics.md#kutta-joukowski-theorem) for positive counterclockwise circulation.

## 19F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19f/solution">Solution</h3>

↑ **Parent:** [19F](#19f)

Split $A=D+L+U$ with $D=\mu^{-1}I$, $L$ the negative unit subdiagonal and $U$ the positive unit superdiagonal. The [Jacobi method](../../../numerical-analysis.md#jacobi-method) uses $x^{(r+1)}=-D^{-1}(L+U)x^{(r)}+D^{-1}b$, so

$$
\boxed{T_J=\begin{pmatrix}0&-\mu&0&0\\\mu&0&-\mu&0\\0&\mu&0&-\mu\\0&0&\mu&0\end{pmatrix}}.
$$

The [Gauss-Seidel method](../../../numerical-analysis.md#gauss-seidel-method) uses $(D+L)x^{(r+1)}=b-Ux^{(r)}$, giving by forward substitution

$$
\boxed{T_{GS}=\begin{pmatrix}0&-\mu&0&0\\0&-\mu^2&-\mu&0\\0&-\mu^3&-\mu^2&-\mu\\0&-\mu^4&-\mu^3&-\mu^2\end{pmatrix}}.
$$

Both iterations converge for every initial error exactly when their [spectral radius](../../../analysis.md#spectral-radius) is below one, since the error evolves as powers of the iteration matrix.

For Jacobi, the leading tridiagonal determinant recurrence is $p_j(\lambda)=\lambda p_{j-1}(\lambda)+\mu^2p_{j-2}(\lambda)$, with $p_0=1,p_1=\lambda$. Thus

$$
p_4=\lambda^4+3\mu^2\lambda^2+\mu^4.
$$

Its roots are $\lambda=\pm i\mu\sqrt{(3+\sqrt5)/2}$ and $\pm i\mu\sqrt{(3-\sqrt5)/2}$. Expanding the Gauss-Seidel determinant gives

$$
\det(\lambda I-T_{GS})=\lambda^2(\lambda^2+3\mu^2\lambda+\mu^4),
$$

so its nonzero eigenvalues are $-\mu^2(3\pm\sqrt5)/2$. Therefore

$$
\rho(T_J)=\frac{1+\sqrt5}{2}|\mu|,\qquad\rho(T_{GS})=\frac{3+\sqrt5}{2}\mu^2=\rho(T_J)^2.
$$

The [skew-tridiagonal Jacobi and Gauss-Seidel iterations](../../../numerical-analysis.md#skew-tridiagonal-jacobi-and-gauss-seidel-iterations) consequently have the same convergence range:

$$
\boxed{0<|\mu|<\frac{\sqrt5-1}{2}}.
$$

Equality fails the every-start convergence condition, and larger magnitudes have unstable modes. The nonsymmetric matrix does not permit an unexamined positive-definite-matrix convergence argument.

## 20D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="20d/a">a</h3>

↑ **Parent:** [20D](#20d)

<h4 id="20d/a/solution">Solution</h4>

↑ **Parent:** [A](#20d/a)

Continue the [simplex algorithm](../../../numerical-analysis.md#simplex-algorithm) using dictionaries, with nonbasic variables zero at the current vertex. The given basis has payoff

$$
f=\frac{116}{9}+\frac{17}{9}x_2-\frac{121}{9}x_3-\frac49z_3.
$$

Thus $x_2$ enters. Its positive row coefficients give ratios $11$ for $z_1$ and $77/4$ for $z_2$; the $x_1$ row does not restrict this increase. Therefore $z_1$ leaves. After that pivot,

$$
\begin{aligned}x_2&=11+11x_3-z_1,\\z_2&=11-11x_3+\tfrac43z_1-\tfrac13z_3,\\x_1&=\tfrac{17}3+\tfrac43x_3-\tfrac29z_1-\tfrac19z_3,\\f&=\tfrac{101}3+\tfrac{22}3x_3-\tfrac{17}9z_1-\tfrac49z_3.\end{aligned}
$$

Now $x_3$ enters. Only the $z_2$ row decreases along this move, and its ratio is $11/11=1$, so $z_2$ leaves. The final dictionary is

$$
\boxed{\begin{aligned}x_1&=7-\tfrac2{33}z_1-\tfrac4{33}z_2-\tfrac5{33}z_3,\\x_2&=22+\tfrac13z_1-z_2-\tfrac13z_3,\\x_3&=1+\tfrac4{33}z_1-\tfrac1{11}z_2-\tfrac1{33}z_3,\\f&=41-z_1-\tfrac23z_2-\tfrac23z_3.\end{aligned}}
$$

All reduced payoff coefficients are nonpositive. Since the slacks must be nonnegative, $f\leq41$, attained with $z=0$. Hence $\boxed{x^*=(7,22,1),\quad f^*=41}$. Direct substitution makes all three original constraints equalities. The final dictionary is the optimal tableau expressed with basic variables on the left, not just a proposed feasible vertex.

<h3 id="20d/b">b</h3>

↑ **Parent:** [20D](#20d)

<h4 id="20d/b/solution">Solution</h4>

↑ **Parent:** [B](#20d/b)

The [dual linear program](../../../mathematical-optimization.md#dual-linear-program) is

$$
\boxed{\begin{aligned}\text{minimize }&11y_1+16y_2+29y_3,\\\text{subject to }&-3y_2+9y_3\geq4,\\&y_1+2y_2-2y_3\geq1,\\&-11y_1-7y_2+10y_3\geq-9,\\&y_1,y_2,y_3\geq0.\end{aligned}}
$$

The negatives of the final slack payoff coefficients give $\boxed{y^*=(1,2/3,2/3)}$. Its three dual constraints are equalities, and its objective is $11+32/3+58/3=41$. Equality with the primal objective proves optimality by [weak duality](../../../mathematical-optimization.md#weak-duality), independently of tableau sign conventions. It is also the [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) certificate, with all primal variables and all dual variables strictly positive.

<h3 id="20d/c">c</h3>

↑ **Parent:** [20D](#20d)

<h4 id="20d/c/solution">Solution</h4>

↑ **Parent:** [C](#20d/c)

The dual constraints and objective coefficients on $x$ are unchanged, so $y^*$ remains dual feasible. Since every component of $y^*$ is positive, complementary slackness forces every constraint of any primal optimum paired with it to bind. Let $A$ be the original three-by-three constraint matrix and $b'=b+\epsilon$. It is invertible, and the only possible paired primal point is

$$
x'=A^{-1}b'=\begin{pmatrix}7+(2\epsilon_1+4\epsilon_2+5\epsilon_3)/33\\22-\epsilon_1/3+\epsilon_2+\epsilon_3/3\\1+(-4\epsilon_1+3\epsilon_2+\epsilon_3)/33\end{pmatrix}.
$$

If this point is nonnegative, it is primal feasible with zero slacks and $c^Tx'=y^{*T}b'$, proving $y^*$ optimal. Conversely, if $y^*$ is optimal, [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) supplies a paired primal optimum, and complementary slackness forces it to be exactly this point. This proves the [strictly positive dual certificate and right-hand-side sensitivity](../../../mathematical-optimization.md#strictly-positive-dual-certificate-and-right-hand-side-sensitivity) criterion:

$$
\boxed{\begin{aligned}2\epsilon_1+4\epsilon_2+5\epsilon_3&\geq-231,\\-\epsilon_1+3\epsilon_2+\epsilon_3&\geq-66,\\-4\epsilon_1+3\epsilon_2+\epsilon_3&\geq-33.\end{aligned}}
$$

Non-strict inequalities are essential: boundary cases can be degenerate but retain the same optimal dual vector. This is the complete range, not just a small-perturbation sufficient condition for [linear programming sensitivity within a fixed optimal basis](../../../mathematical-optimization.md#linear-programming-sensitivity-within-a-fixed-optimal-basis).

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
