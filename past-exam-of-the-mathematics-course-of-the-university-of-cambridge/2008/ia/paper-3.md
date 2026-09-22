# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_3.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3C](#3c)
  - [i](#3c/i)
    - [Solution](#3c/i/solution)
  - [ii](#3c/ii)
    - [Solution](#3c/ii/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
  - [i](#5e/i)
    - [Solution](#5e/i/solution)
  - [ii](#5e/ii)
    - [Solution](#5e/ii/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
  - [i](#7e/i)
    - [Solution](#7e/i/solution)
  - [ii](#7e/ii)
    - [Solution](#7e/ii/solution)
  - [iii](#7e/iii)
    - [Solution](#7e/iii/solution)
- [8E](#8e)
  - [Solution](#8e/solution)
- [9C](#9c)
  - [i](#9c/i)
    - [Solution](#9c/i/solution)
  - [ii](#9c/ii)
    - [Solution](#9c/ii/solution)
- [10C](#10c)
  - [Solution](#10c/solution)
  - [i](#10c/i)
    - [Solution](#10c/i/solution)
  - [ii](#10c/ii)
    - [Solution](#10c/ii/solution)
  - [iii](#10c/iii)
    - [Solution](#10c/iii/solution)
- [11C](#11c)
  - [a](#11c/a)
    - [Solution](#11c/a/solution)
  - [b](#11c/b)
    - [i](#11c/b/i)
      - [Solution](#11c/b/i/solution)
    - [ii](#11c/b/ii)
      - [Solution](#11c/b/ii/solution)
    - [iii](#11c/b/iii)
      - [Solution](#11c/b/iii/solution)
- [12C](#12c)
  - [i](#12c/i)
    - [Solution](#12c/i/solution)
  - [ii](#12c/ii)
    - [Solution](#12c/ii/solution)
  - [iii](#12c/iii)
    - [Solution](#12c/iii/solution)

## 1E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

For a [permutation](../../../combinatorics.md#permutation) $\sigma\in S_n$, let $P_\sigma$ be its [permutation matrix](../../../vector-space.md#permutation-matrix), defined by $P_\sigma e_j=e_{\sigma(j)}$. Define the [signature of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) by $\epsilon(\sigma)=\det P_\sigma$. A [permutation matrix](../../../vector-space.md#permutation-matrix) is orthogonal, so $(\det P_\sigma)^2=1$ and its [permutation sign](../../../finite-group-theory.md#sign-of-a-permutation) lies in $\{1,-1\}$. A [transposition](../../../combinatorics.md#transposition-permutation) exchanges two columns of the identity and therefore has [determinant](../../../linear-algebra.md#determinant) $-1$. Every [permutation](../../../combinatorics.md#permutation) is a product of [transpositions](../../../combinatorics.md#transposition-permutation), by decomposing each [permutation cycle](../../../finite-group-theory.md#permutation-cycle) as

$$
(a_1\,a_2\,\ldots,a_r)=(a_1\,a_r)(a_1\,a_{r-1})\cdots(a_1\,a_2).
$$

Hence $\epsilon(\sigma)=(-1)^m$ for any expression as $m$ [transpositions](../../../combinatorics.md#transposition-permutation); the [determinant](../../../linear-algebra.md#determinant) definition proves that this [parity of a permutation](../../../finite-group-theory.md#parity-of-a-permutation) is independent of the expression. Equivalently the [permutation sign](../../../finite-group-theory.md#sign-of-a-permutation) is positive for an [even permutation](../../../finite-group-theory.md#even-permutation) and negative for an [odd permutation](../../../finite-group-theory.md#odd-permutation).

Composition is taken rightmost first. Since $P_{\sigma\tau}e_j=e_{\sigma(\tau(j))}=P_\sigma P_\tau e_j$, we have $P_{\sigma\tau}=P_\sigma P_\tau$. Multiplicativity of the [determinant](../../../linear-algebra.md#determinant) therefore proves the [sign homomorphism](../../../finite-group-theory.md#sign-homomorphism) identity

$$
\boxed{\epsilon(\sigma\tau)=\epsilon(\sigma)\epsilon(\tau).}
$$

The [alternating group](../../../finite-group-theory.md#alternating-group) consists of the [even permutations](../../../finite-group-theory.md#even-permutation):

$$
\boxed{A_n=\{\sigma\in S_n:\epsilon(\sigma)=1\}=\ker\epsilon.}
$$

It contains the identity. If $\sigma,\tau\in A_n$, their product has [permutation sign](../../../finite-group-theory.md#sign-of-a-permutation) $1$, and $\epsilon(\sigma^{-1})=\epsilon(\sigma)^{-1}=1$, so their inverses also belong to $A_n$. This proves it is a [subgroup](../../../group.md#subgroup). Finally, for every $g\in S_n$ and $a\in A_n$,

$$
\epsilon(gag^{-1})=\epsilon(g)\epsilon(a)\epsilon(g)^{-1}=1.
$$

Thus **$A_n$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) of $S_n$**. This also exhibits directly why a [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is normal.

## 2E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

The real [orthogonal group](../../../linear-algebra.md#orthogonal-group) and [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) are, under [matrix](../../../vector-space.md#matrix) multiplication,

$$
\boxed{O(n)=\{Q\in M_n(\mathbb R):Q^TQ=I\},\qquad
SO(n)=\{Q\in O(n):\det Q=1\}.}
$$

An [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) preserves Euclidean [inner products](../../../linear-algebra.md#inner-product); taking [determinants](../../../linear-algebra.md#determinant) of $Q^TQ=I$ shows that its [determinant](../../../linear-algebra.md#determinant) is $1$ or $-1$. Its inverse is $Q^T$, so $QQ^T=I$ as well.

For $Q\in SO(3)$, use $Q-I=Q(I-Q^T)$. The [determinant](../../../linear-algebra.md#determinant) then satisfies

$$
\det(Q-I)=\det Q\det(I-Q^T)=\det(I-Q)=(-1)^3\det(Q-I).
$$

It follows that $\det(Q-I)=0$. Thus the real [matrix](../../../vector-space.md#matrix) $Q-I$ has a nonzero [vector](../../../vector-space.md#vector) in its [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map), yielding

$$
\boxed{Qv=v\quad\text{for some }v\ne0.}
$$

This is the three-dimensional case of [odd-dimensional special orthogonal transformation has a fixed vector](../../../linear-algebra.md#odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector); geometrically it supplies the fixed [rotation](../../../riemannian-geometry.md#rotation-mathematics) axis, unless the transformation is the identity and every direction is fixed.

The claim is **false for $O(3)$**. The [matrix](../../../vector-space.md#matrix) $Q=-I_3$ is orthogonal with [determinant](../../../linear-algebra.md#determinant) $-1$ and has only the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-1$. It therefore has no nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$.

## 3C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3c/i">i</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/i/solution">Solution</h4>

↑ **Parent:** [I](#3c/i)

Differentiate the parametrized [curve](../../../topology.md#curve) to obtain $\boldsymbol x'(t)=(1-t^2,2t,1+t^2)$. Its [speed](../../../classical-mechanics.md#speed) obeys

$$
|\boldsymbol x'(t)|^2=(1-t^2)^2+4t^2+(1+t^2)^2=2(1+t^2)^2.
$$

Since $1+t^2>0$, the [arc length](../../../riemannian-geometry.md#arc-length) is

$$
\boxed{L=\int_0^1\sqrt2(1+t^2)\,dt=\frac{4\sqrt2}{3}.}
$$

<h3 id="3c/ii">ii</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3c/ii)

Divide the velocity by the [speed](../../../classical-mechanics.md#speed) calculated above. The [unit tangent vector](../../../differential-geometry.md#unit-tangent-vector) is

$$
\boxed{T(t)=\frac1{\sqrt2}\left(\frac{1-t^2}{1+t^2},\frac{2t}{1+t^2},1\right).}
$$

Its derivative is

$$
T'(t)=\frac1{\sqrt2(1+t^2)^2}\bigl(-4t,2(1-t^2),0\bigr),
\qquad |T'(t)|=\frac{\sqrt2}{1+t^2}>0.
$$

Because $ds/dt=\sqrt2(1+t^2)>0$, the [principal normal vector](../../../differential-geometry.md#principal-normal-vector) has the direction of $T'(t)$, giving

$$
\boxed{N(t)=\left(-\frac{2t}{1+t^2},\frac{1-t^2}{1+t^2},0\right).}
$$

This is a [unit vector](../../../vector-space.md#unit-vector), and $N\cdot e_z=0$ for every real $t$. The [curvature of a space curve](../../../differential-geometry.md#curvature-of-a-space-curve) is $|T'|/(ds/dt)=1/(1+t^2)^2>0$, so the [principal normal vector](../../../differential-geometry.md#principal-normal-vector) is defined everywhere on this [curve](../../../topology.md#curve). The same perpendicularity follows from [constant tangent component forces perpendicular principal normals](../../../differential-geometry.md#constant-tangent-component-forces-perpendicular-principal-normals): $T\cdot e_z=1/\sqrt2$ is constant, and differentiating this identity forces the normal component along $e_z$ to vanish.

## 4C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

For a constant orthogonal Cartesian coordinate change $x'_i=R_{ij}x_j$, a [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor) has components satisfying

$$
\boxed{T'_{ij}(x')=R_{ik}R_{jl}T_{kl}(x).}
$$

Both indices transform by the coordinate-change [matrix](../../../vector-space.md#matrix); summation over repeated indices is understood by the [Einstein summation convention](../../../linear-algebra.md#einstein-notation). A [vector](../../../vector-space.md#vector) would have the one-index rule $U'_i=R_{ik}U_k$.

Define $U_i=\partial T_{ij}/\partial x_j$. Since $x_m=R_{jm}x'_j$, the [chain rule](../../../calculus.md#chain-rule) gives $\partial/\partial x'_j=R_{jm}\partial/\partial x_m$. The [rotation](../../../riemannian-geometry.md#rotation-mathematics) coefficients are constant, so

$$
\begin{aligned}
U'_i&=\frac{\partial T'_{ij}}{\partial x'_j}
=R_{jm}R_{ik}R_{jl}\frac{\partial T_{kl}}{\partial x_m}\\
&=R_{ik}\delta_{ml}\frac{\partial T_{kl}}{\partial x_m}
=R_{ik}\frac{\partial T_{kl}}{\partial x_l}=R_{ik}U_k.
\end{aligned}
$$

The identity $R_{jm}R_{jl}=\delta_{ml}$ follows from orthogonality. Hence **the contracted derivative transforms as a [vector](../../../vector-space.md#vector)**. This proves the [divergence of a Cartesian second-rank tensor](../../../linear-algebra.md#divergence-of-a-cartesian-second-rank-tensor) rule for global Cartesian [rotations](../../../riemannian-geometry.md#rotation-mathematics). In curvilinear coordinates the corresponding construction uses a [covariant derivative](../../../general-relativity.md#covariant-derivative); ordinary partial derivatives alone would not have the stated tensorial transformation law.

## 5E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

For a [normal subgroup](../../../group-theory.md#normal-subgroup) $H\trianglelefteq G$, define multiplication of left [cosets](../../../group-theory.md#coset) by

$$
\boxed{(gH)(kH)=(gk)H.}
$$

To check that this is well-defined, replace $g,k$ by $gh_1,kh_2$ with $h_1,h_2\in H$. Their product is $gh_1kh_2=gk(k^{-1}h_1k)h_2$, and normality puts $(k^{-1}h_1k)h_2$ in $H$. Thus the product [coset](../../../group-theory.md#coset) is independent of the representatives. [Associativity](../../../group.md#associative-property) follows from multiplication in $G$, the identity is $H$, and the inverse of $gH$ is $g^{-1}H$. These operations form the [quotient group](../../../group-theory.md#quotient-group) $G/H$.

For the unheaded finite-index conclusion, let $G$ act on the $n$ left [cosets](../../../group-theory.md#coset) of its proper [subgroup](../../../group.md#subgroup) $H$ by $g\cdot(xH)=gxH$. This is well-defined even if $H$ is not normal: replacing $x$ by $xh$ leaves $gxH$ unchanged. The maps are bijections with inverses supplied by $g^{-1}$, and their compositions give a [group homomorphism](../../../group-theory.md#group-homomorphism) $\varphi:G\to S_n$. Its [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) $N$ is normal, by the calculation in part (ii).

The action is not trivial, because some $g\notin H$ sends the [coset](../../../group-theory.md#coset) $H$ to $gH\ne H$; hence $N\ne G$. If $N$ were trivial, $\varphi$ would be [injective](../../../algebra.md#injective-function), implying $|G|\leq|S_n|=n!$. Under the given strict inequality this is impossible. Thus $N$ is a nontrivial proper [normal subgroup](../../../group-theory.md#normal-subgroup), and

$$
\boxed{|G|>n!\ \Longrightarrow\ G\text{ is not simple}.}
$$

More precisely, $N=\bigcap_{x\in G}xHx^{-1}$ is the [subgroup core](../../../group-theory.md#core-group-theory): $g$ fixes every [coset](../../../group-theory.md#coset) if and only if $x^{-1}gx\in H$ for every $x$. This identifies the [normal subgroup](../../../group-theory.md#normal-subgroup) produced by the [coset action](../../../group-theory.md#coset-action).

<h3 id="5e/i">i</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/i/solution">Solution</h4>

↑ **Parent:** [I](#5e/i)

Assume $H$ is a [normal subgroup](../../../group-theory.md#normal-subgroup). Take the [quotient group](../../../group-theory.md#quotient-group) $K=G/H$ and the natural projection $\theta(g)=gH$. The well-defined multiplication constructed above gives $\theta(gk)=\theta(g)\theta(k)$, so this is a [group homomorphism](../../../group-theory.md#group-homomorphism). Its identity is the [coset](../../../group-theory.md#coset) $H$, and $\theta(g)=H$ exactly when $g\in H$. Therefore

$$
\boxed{\ker\theta=H,}
$$

which proves the implication from normality to being the [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism).

<h3 id="5e/ii">ii</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5e/ii)

Assume $H=\ker\theta$ for a [group homomorphism](../../../group-theory.md#group-homomorphism) $\theta:G\to K$. For $h\in H$ and $g\in G$,

$$
\theta(ghg^{-1})=\theta(g)\theta(h)\theta(g)^{-1}=e_K.
$$

Thus $gHg^{-1}\subseteq H$. Apply the same inclusion with $g^{-1}$ to obtain the reverse inclusion, giving $gHg^{-1}=H$. Hence **every kernel is a [normal subgroup](../../../group-theory.md#normal-subgroup)**, proving the reverse implication and the required equivalence.

## 6E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

For any [permutation](../../../combinatorics.md#permutation) $\tau$, conjugating a [permutation cycle](../../../finite-group-theory.md#permutation-cycle) relabels its entries:

$$
\tau(a_1\,a_2\,\ldots,a_r)\tau^{-1}=(\tau(a_1)\,\tau(a_2)\,\ldots,\tau(a_r)).
$$

Indeed, the conjugate sends $\tau(a_j)$ to $\tau(a_{j+1})$ and fixes the other relabeled entries exactly as the original [permutation cycle](../../../finite-group-theory.md#permutation-cycle) does. Therefore [conjugation](../../../group-theory.md#conjugation) preserves the multiset of [permutation cycle](../../../finite-group-theory.md#permutation-cycle) lengths. Conversely, if two [permutations](../../../combinatorics.md#permutation) have the same [cycle type](../../../finite-group-theory.md#cycle-type), pair their [permutation cycles](../../../finite-group-theory.md#permutation-cycle) of each length and let $\tau$ carry the $j$th entry of each first [permutation cycle](../../../finite-group-theory.md#permutation-cycle) to the $j$th entry of its partner. Include one-cycles for fixed points. This defines a [bijection](../../../function.md#bijection) of all labels, and the displayed relabeling identity makes the [permutations](../../../combinatorics.md#permutation) conjugate. Thus

$$
\boxed{\sigma\sim_{S_n}\rho\quad\Longleftrightarrow\quad\sigma,\rho\text{ have the same cycle type}.}
$$

For $n\geq2$, the [alternating conjugacy class splitting criterion](../../../group-theory.md#alternating-conjugacy-class-splitting-criterion) says that an even [permutation](../../../combinatorics.md#permutation) has the same class in $A_n$ and $S_n$ precisely when its type is not a collection of pairwise distinct odd lengths. Equivalently, **there is an even-length [permutation cycle](../../../finite-group-theory.md#permutation-cycle) or a repeated [permutation cycle](../../../finite-group-theory.md#permutation-cycle) length**, counting each fixed point as a length-one [permutation cycle](../../../finite-group-theory.md#permutation-cycle). Distinct odd lengths instead give two alternating-group classes. For $n=1$, $A_1=S_1$ and the sole class is the same; the index-two splitting criterion is not applicable.

Squaring an odd-length [permutation cycle](../../../finite-group-theory.md#permutation-cycle) keeps one [permutation cycle](../../../finite-group-theory.md#permutation-cycle) of that length, since advancing by two visits all of its entries. Squaring an even-length [permutation cycle](../../../finite-group-theory.md#permutation-cycle) splits it into two [permutation cycles](../../../finite-group-theory.md#permutation-cycle), each of half that length. Thus any even-length [permutation cycle](../../../finite-group-theory.md#permutation-cycle) strictly increases the total [permutation cycle](../../../finite-group-theory.md#permutation-cycle) count on squaring, while odd [permutation cycles](../../../finite-group-theory.md#permutation-cycle) leave that count unchanged. The [cycle type](../../../finite-group-theory.md#cycle-type) can agree with its square exactly when every length is odd. This proves [permutation conjugate to its square](../../../finite-group-theory.md#permutation-conjugate-to-its-square):

$$
\boxed{\sigma\sim_{S_n}\sigma^2\quad\Longleftrightarrow\quad\text{every cycle length is odd}
\quad\Longleftrightarrow\quad\operatorname{ord}(\sigma)\text{ is odd}.}
$$

The final equivalence follows because the [order of a group element](../../../group-theory.md#order-of-a-group-element) that is a [permutation](../../../combinatorics.md#permutation) is the [least common multiple](../../../number-theory.md#least-common-multiple) of its [permutation cycle](../../../finite-group-theory.md#permutation-cycle) lengths.

The possible even types on five labels are the identity, a three-cycle, a product of two disjoint [transpositions](../../../combinatorics.md#transposition-permutation) and a five-cycle. The identity and the double [transpositions](../../../combinatorics.md#transposition-permutation) are their own inverses. For a three-cycle $(a\,b\,c)$ with unused labels $d,e$, the even [permutation](../../../combinatorics.md#permutation) $(b\,c)(d\,e)$ conjugates it to its inverse. For a five-cycle $(a\,b\,c\,d\,e)$, the even [permutation](../../../combinatorics.md#permutation) $(b\,e)(c\,d)$ reverses its order. Therefore **every element of $A_5$ is conjugate to its inverse within $A_5$**. Inverting a five-cycle uses two [transpositions](../../../combinatorics.md#transposition-permutation), in agreement with [inversion of an odd cycle in an alternating group](../../../group-theory.md#inversion-of-an-odd-cycle-in-an-alternating-group).

A small counterexample elsewhere is

$$
\boxed{n=3,\qquad\sigma=(1\,2\,3).}
$$

The [alternating group](../../../finite-group-theory.md#alternating-group) $A_3=\{e,(1\,2\,3),(1\,3\,2)\}$ is cyclic and therefore abelian. Every [conjugacy class](../../../group-theory.md#conjugacy-class) in an [abelian group](../../../group.md#abelian-group) is a singleton, while $\sigma\ne\sigma^{-1}$. Thus these two elements are not conjugate in $A_3$.

## 7E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

Write a [Möbius transformation](../../../group-theory.md#mobius-transformation) as $M(z)=(az+b)/(cz+d)$ with $ad-bc\ne0$, interpreted on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). Let $T_u(z)=z+u$, $D_\lambda(z)=\lambda z$ with $\lambda\ne0$, and $I(z)=1/z$.

If $c=0$, then $a,d\ne0$ and $M(z)=(a/d)z+b/d=T_{b/d}\circ D_{a/d}(z)$. If $c\ne0$, algebraic division gives

$$
M(z)=\frac ac+\frac{bc-ad}{c^2}\frac1{z+d/c}.
$$

Consequently

$$
\boxed{M=T_{a/c}\circ D_{(bc-ad)/c^2}\circ I\circ T_{d/c}.}
$$

The scaling coefficient is nonzero because $ad-bc\ne0$. Thus translations, nonzero complex scalings and reciprocal inversion generate every [Möbius map](../../../group-theory.md#mobius-transformation). The formulas extend over their poles and infinity by the sphere interpretation.

<h3 id="7e/i">i</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/i/solution">Solution</h4>

↑ **Parent:** [I](#7e/i)

The assertion is **true**. A [Möbius map](../../../group-theory.md#mobius-transformation) fixes infinity if and only if $c=0$: if $c\ne0$, its value there is the finite number $a/c$. For $c=0$, the decomposition above uses only a nonzero complex scaling and a translation. These maps form the [Affine subgroup of the Möbius group](../../../group-theory.md#affine-subgroup-of-the-mobius-group).

<h3 id="7e/ii">ii</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7e/ii)

The assertion is **false**. Let $D_\lambda(z)=\lambda z$ and $I(z)=1/z$. Their relations are

$$
I^2=\operatorname{id},\qquad ID_\lambda=D_{\lambda^{-1}}I.
$$

Moving each inversion to the right reduces every word to $D_\lambda I^\epsilon$ with $\epsilon=0$ or $1$. Thus the [subgroup generated by complex scalings and reciprocal inversion](../../../group-theory.md#subgroup-generated-by-complex-scalings-and-reciprocal-inversion) consists only of $z\mapsto\lambda z$ and $z\mapsto\lambda/z$. Of these, only the first form fixes zero.

The [Möbius transformation](../../../group-theory.md#mobius-transformation)

$$
\boxed{M(z)=\frac z{z+1}}
$$

fixes zero but is not a scaling: it sends infinity to $1$ instead of infinity. It therefore cannot belong to the [subgroup](../../../group.md#subgroup) generated by scalings and reciprocal inversion.

<h3 id="7e/iii">iii</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7e/iii)

The assertion is **true** over the complex numbers. It suffices to generate every nonzero scaling using translations and $I(z)=1/z$, since these together with scalings already generate the [Möbius group](../../../group-theory.md#mobius-group).

For $s\ne0$, compose the maps rightmost first. Away from the intermediate poles, the successive values are

$$
z\longmapsto\frac1z\longmapsto\frac{1+sz}{z}\longmapsto\frac z{1+sz}
\longmapsto-\frac1{s(1+sz)}\longmapsto-s(1+sz)\longmapsto-s^2z.
$$

Hence

$$
\boxed{T_s\circ I\circ T_{-1/s}\circ I\circ T_s\circ I=D_{-s^2}.}
$$

For every $\lambda\ne0$, choose a complex square root $s$ with $s^2=-\lambda$. This gives $D_\lambda$ and proves [Möbius scaling generated by translations and reciprocal inversion](../../../group-theory.md#mobius-scaling-generated-by-translations-and-reciprocal-inversion). Equality of the rational maps extends the identity to all points of the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), including the intermediate exceptional values.

## 8E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8e/solution">Solution</h3>

↑ **Parent:** [8E](#8e)

Let a finite [group](../../../group.md) $G$ act on a set $X$. For $x\in X$, define its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) $G_x=\{g:g\cdot x=x\}$ and its [group orbit](../../../group-theory.md#orbit-of-a-group-action) $Gx=\{g\cdot x:g\in G\}$. The map

$$
gG_x\longmapsto g\cdot x
$$

is well-defined, because multiplying $g$ on the right by an element fixing $x$ does not change its image. It is onto by the definition of the orbit. If $g\cdot x=h\cdot x$, then $h^{-1}g\in G_x$, so $gG_x=hG_x$; hence it is one-to-one. Every [coset](../../../group-theory.md#coset) has $|G_x|$ elements and the [cosets](../../../group-theory.md#coset) partition $G$. This proves the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem):

$$
\boxed{|G|=|Gx|\,|G_x|.}
$$

For a [group](../../../group.md) element $x$, its [cyclic subgroup](../../../group.md#cyclic-subgroup) $H=\langle x\rangle$ has $\operatorname{ord}(x)$ elements. Apply the theorem to the action of $G$ on its left [cosets](../../../group-theory.md#coset) $G/H$, whose stabilizer at $H$ is $H$. It follows that

$$
\boxed{\operatorname{ord}(x)=|H|\text{ divides }|G|.}
$$

This is the needed case of [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), obtained directly from the action.

To prove [Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups), let $p$ be a prime divisor of $|G|$ and consider

$$
\mathcal X=\{(g_1,\ldots,g_p)\in G^p:g_1\cdots g_p=e\}.
$$

The first $p-1$ entries are arbitrary and determine the last, so $|\mathcal X|=|G|^{p-1}$ is divisible by $p$. Cyclically rotate the entries. This preserves the product constraint even if $G$ is nonabelian, since

$$
g_2\cdots g_pg_1=g_1^{-1}(g_1\cdots g_p)g_1=e.
$$

Thus a [cyclic group](../../../group.md#cyclic-group) of order $p$ acts on $\mathcal X$. By the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem), its orbits have size one or $p$. Its fixed tuples are exactly $(g,\ldots,g)$ with $g^p=e$. If $m$ is their number, counting the remaining size-$p$ orbits gives $m\equiv|\mathcal X|\equiv0\pmod p$. The identity provides one fixed tuple, so $m\geq p$ and a nonidentity $g$ with $g^p=e$ exists. The order of this $g$ divides $p$: division of $p$ by its order and minimality of that order prove this directly. Since $p$ is prime and $g\ne e$, the order is exactly $p$. This is the [cyclic-tuple proof of Cauchy theorem](../../../finite-group-theory.md#cyclic-tuple-proof-of-cauchy-theorem).

Now suppose every nonidentity element has order two. Then every element equals its inverse, and for any $a,b\in G$,

$$
ab=(ab)^{-1}=b^{-1}a^{-1}=ba.
$$

Thus [group of exponent two is abelian](../../../group.md#group-of-exponent-two-is-abelian) applies. Starting from the identity [subgroup](../../../group.md#subgroup), choose an element outside the [subgroup](../../../group.md#subgroup) already generated. Because the [group](../../../group.md) is abelian and that element squares to the identity, adjoining it doubles the [subgroup](../../../group.md#subgroup): it is the disjoint union of the old [subgroup](../../../group.md#subgroup) and its translate by the new element. Repeating until the [finite group](../../../group.md#finite-group) is exhausted shows $|G|=2^r$. Conversely the [direct product of groups](../../../group-theory.md#direct-product-of-groups) $C_2^r$ has order $2^r$ and every nonidentity element has order two. Therefore

$$
\boxed{n=2^r\quad(r=0,1,2,\ldots).}
$$

The case $r=0$ is the trivial [group](../../../group.md) and satisfies the condition vacuously. These finite examples are [elementary abelian groups](../../../group.md#elementary-abelian-group) of exponent two.

An infinite example is the [group](../../../group.md) of all binary sequences, with coordinatewise addition modulo two:

$$
\boxed{G=\prod_{j=1}^\infty\mathbb Z/2\mathbb Z.}
$$

Every sequence added to itself is zero, so every nonzero sequence has order exactly two. The sequences having a single $1$ in coordinate $j$ are all distinct, proving that the [group](../../../group.md) is infinite.

## 9C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9c/i">i</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/i/solution">Solution</h4>

↑ **Parent:** [I](#9c/i)

The [vector triple product](../../../calculus.md#vector-triple-product) removes the nested [cross products](../../../vector-space.md#cross-product):

$$
F_i=\omega_i\omega_jx_j-|\boldsymbol\omega|^2x_i.
$$

Since $\boldsymbol\omega$ is constant, the [divergence](../../../calculus.md#divergence) is

$$
\partial_iF_i=\omega_i\omega_i-3|\boldsymbol\omega|^2=-2|\boldsymbol\omega|^2.
$$

The cube has [volume](../../../geometry-and-topology.md#volume) $2^3=8$. With the outward [unit normal](../../../differential-geometry.md#unit-normal), the [divergence theorem](../../../calculus.md#divergence-theorem) therefore gives

$$
\boxed{\int_S\mathbf F\cdot d\mathbf S=-16|\boldsymbol\omega|^2.}
$$

<h3 id="9c/ii">ii</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9c/ii)

The derivative [matrix](../../../vector-space.md#matrix)

$$
\partial_jF_k=\omega_k\omega_j-|\boldsymbol\omega|^2\delta_{kj}
$$

is symmetric in $j,k$. Contracting it with the antisymmetric [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) gives the [curl](../../../calculus.md#curl)

$$
(\nabla\times\mathbf F)_i=\epsilon_{ijk}(\omega_k\omega_j-|\boldsymbol\omega|^2\delta_{kj})=0.
$$

Direct differentiation of the [scalar potential](../../../quantum-field-theory.md#scalar-potential) gives

$$
\partial_i\phi=\omega_i(\boldsymbol\omega\cdot\mathbf x)-|\boldsymbol\omega|^2x_i=F_i,
$$

so **$\mathbf F=\nabla\phi$**. To identify the [level sets](../../../topology.md#level-set), use the [cross product](../../../vector-space.md#cross-product) identity

$$
\phi=-\tfrac12|\boldsymbol\omega\times\mathbf x|^2.
$$

If $\boldsymbol\omega\ne0$, write $\mathbf x=\mathbf x_{\parallel}+\mathbf x_{\perp}$ relative to its direction. Then $\phi=-|\boldsymbol\omega|^2|\mathbf x_{\perp}|^2/2$. Thus **each negative level $\phi=c$ is a [circular cylinder](../../../differential-geometry.md#circular-cylinder) with axis $\mathbb R\boldsymbol\omega$ and radius $\sqrt{-2c}/|\boldsymbol\omega|$**. The zero level is the axis itself; positive levels are empty. If $\boldsymbol\omega=0$, the [scalar potential](../../../quantum-field-theory.md#scalar-potential) is identically zero, so its zero level is all of space and every other level is empty.

## 10C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10c/solution">Solution</h3>

↑ **Parent:** [10C](#10c)

Use the right-handed [rotation matrix](../../../linear-algebra.md#rotation-matrix) which sends the positive $x$ direction to the positive $y$ direction:

$$
R=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}.
$$

The [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor) transformation law gives

$$
S'=RSR^{\mathsf T}=\begin{pmatrix}
S_{22}&-S_{21}&-S_{23}\\
-S_{12}&S_{11}&S_{13}\\
-S_{32}&S_{31}&S_{33}
\end{pmatrix}.
$$

Here [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) means invariant under every proper [rotation](../../../riemannian-geometry.md#rotation-mathematics), as is needed for the rank-three assertion involving the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol). A passive coordinate [rotation](../../../riemannian-geometry.md#rotation-mathematics) through the same angle uses $R^{\mathsf T}$ instead; the invariance conclusions are identical.

Setting $S'=S$ forces $S_{11}=S_{22}$, $S_{12}=-S_{21}$, and $S_{13}=S_{23}=S_{31}=S_{32}=0$. No symmetry assumption on $S$ has been made: it now has the form

$$
S=\begin{pmatrix}a&b&0\\-b&a&0\\0&0&c\end{pmatrix}.
$$

Invariance under a right-handed quarter-turn about the $x$ axis next gives $S_{22}=S_{33}$ and $S_{12}=-S_{13}$, hence $a=c$ and $b=0$. Conversely $R(\lambda I)R^{\mathsf T}=\lambda I$ for every [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix). The general [isotropic second-rank tensor](../../../linear-algebra.md#isotropic-second-rank-tensor) is therefore **$S_{ij}=\lambda\delta_{ij}$**.

An isotropic [vector](../../../vector-space.md#vector) must be fixed by the half-turn about the $z$ axis, so its first two components vanish. The half-turn about the $x$ axis then forces its third component to vanish. Thus **the only isotropic [vector](../../../vector-space.md#vector) is zero**. The general [isotropic third-rank tensor](../../../linear-algebra.md#isotropic-third-rank-tensor) under proper [rotations](../../../riemannian-geometry.md#rotation-mathematics) is **$A_{ijk}=\lambda\epsilon_{ijk}$**. If invariance under the whole [orthogonal group](../../../linear-algebra.md#orthogonal-group) were required of an ordinary rank-three [tensor](../../../linear-algebra.md#tensor), inversion $R=-I$ would send $A$ to $-A$, forcing $A=0$ instead.

<h3 id="10c/i">i</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/i/solution">Solution</h4>

↑ **Parent:** [I](#10c/i)

Both the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and $T$ are invariant under proper [rotations](../../../riemannian-geometry.md#rotation-mathematics). Their [tensor contraction](../../../linear-algebra.md#tensor-contraction)

$$
A_l=\epsilon_{ijk}T_{ijkl}
$$

is consequently an isotropic [vector](../../../vector-space.md#vector). The introductory proof shows that it must vanish, so **$\epsilon_{ijk}T_{ijkl}=0$**.

For the displayed combination of [Kronecker deltas](../../../linear-algebra.md#kronecker-delta), the three terms are

$$
\alpha\epsilon_{ijk}\delta_{ij}\delta_{kl},\qquad
\beta\epsilon_{ijk}\delta_{ik}\delta_{jl},\qquad
\gamma\epsilon_{ijk}\delta_{il}\delta_{jk}.
$$

In each term the [tensor contraction](../../../linear-algebra.md#tensor-contraction) repeats two indices of the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol); each term is zero. This verifies the identity for arbitrary $\alpha,\beta,\gamma$.

<h3 id="10c/ii">ii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10c/ii)

The [tensor contraction](../../../linear-algebra.md#tensor-contraction) $B_{kl}=\delta_{ij}T_{ijkl}$ is an [isotropic second-rank tensor](../../../linear-algebra.md#isotropic-second-rank-tensor), because the [Kronecker delta](../../../linear-algebra.md#kronecker-delta) and $T$ are invariant under [rotations](../../../riemannian-geometry.md#rotation-mathematics). The classification proved above yields **$B_{kl}=\mu\delta_{kl}$** for some scalar $\mu$.

For the given three-term [tensor](../../../linear-algebra.md#tensor), contraction over $i,j$ gives

$$
\delta_{ij}T_{ijkl}=\alpha\delta_{ii}\delta_{kl}+\beta\delta_{kl}+\gamma\delta_{kl}
=\boxed{(3\alpha+\beta+\gamma)\delta_{kl}}.
$$

Thus **$\mu=3\alpha+\beta+\gamma$**.

<h3 id="10c/iii">iii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10c/iii)

The [tensor contraction](../../../linear-algebra.md#tensor-contraction) $C_{mkl}=\epsilon_{ijm}T_{ijkl}$ is an [isotropic third-rank tensor](../../../linear-algebra.md#isotropic-third-rank-tensor) under proper [rotations](../../../riemannian-geometry.md#rotation-mathematics). It therefore equals $\nu\epsilon_{mkl}$. Cyclically permuting three indices is even, so $\epsilon_{mkl}=\epsilon_{klm}$ and **$\epsilon_{ijm}T_{ijkl}=\nu\epsilon_{klm}$**.

For the given [Kronecker delta](../../../linear-algebra.md#kronecker-delta) expression, the $\alpha$ term vanishes by antisymmetry, while the $\beta$ and $\gamma$ terms give respectively $\beta\epsilon_{klm}$ and $\gamma\epsilon_{lkm}=-\gamma\epsilon_{klm}$. Hence

$$
\boxed{\epsilon_{ijm}T_{ijkl}=(\beta-\gamma)\epsilon_{klm},\qquad \nu=\beta-\gamma.}
$$

These computations also illustrate [isotropic contractions of a fourth-rank tensor](../../../linear-algebra.md#isotropic-contractions-of-a-fourth-rank-tensor).

## 11C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11c/a">a</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/a/solution">Solution</h4>

↑ **Parent:** [A](#11c/a)

The [product rule](../../../calculus.md#product-rule) gives

$$
\nabla\cdot(f\nabla g)=\nabla f\cdot\nabla g+f\nabla^2g.
$$

Apply the [divergence theorem](../../../calculus.md#divergence-theorem), with outward [unit normal](../../../differential-geometry.md#unit-normal) $\mathbf n$, and use the vanishing [Laplacian](../../../calculus.md#laplacian) of the [harmonic function](../../../partial-differential-equation.md#harmonic-function) $g$:

$$
\int_V\nabla f\cdot\nabla g\,dV=\int_S f\nabla g\cdot\mathbf n\,dS.
$$

The boundary value of $f$ is one. Another application of the [divergence theorem](../../../calculus.md#divergence-theorem) therefore gives

$$
\int_S f\nabla g\cdot\mathbf n\,dS=\int_S\nabla g\cdot\mathbf n\,dS=\int_V\nabla^2g\,dV=\boxed{0}.
$$

This is the [gradient pairing with a boundary-constant function and a harmonic function](../../../partial-differential-equation.md#gradient-pairing-with-a-boundary-constant-function-and-a-harmonic-function), obtained directly from [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity). The [harmonic function](../../../partial-differential-equation.md#harmonic-function) must be regular throughout the volume; an interior singularity can supply an additional boundary flux.

<h3 id="11c/b">b</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/b/i">i</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11c/b/i)

Here $v=z$, so $\nabla v=\mathbf e_z$, while $\nabla u=\widehat{\mathbf r}$ away from the origin. Their [inner product](../../../linear-algebra.md#inner-product) is $\cos\theta$. The [spherical coordinates](../../../calculus.md#spherical-coordinate-system) volume element gives

$$
\int_V\nabla u\cdot\nabla v\,dV=\int_0^a r^2\,dr\int_0^\pi\cos\theta\sin\theta\,d\theta\int_0^{2\pi}d\varphi=\boxed{0}.
$$

This agrees with the boundary-constant [gradient pairing with a boundary-constant function and a harmonic function](../../../partial-differential-equation.md#gradient-pairing-with-a-boundary-constant-function-and-a-harmonic-function): $u$ has constant boundary value $a$ and $v=z$ is a regular [harmonic function](../../../partial-differential-equation.md#harmonic-function). For comparison with the boundary value one in part (a), use $u/a$ and multiply back by $a$. Strictly, $u=r$ is not differentiable at the origin. Excising a ball of radius $\varepsilon$ resolves this: the inner boundary term $u\partial_n v=-\varepsilon\cos\theta$ has zero angular integral, so it contributes nothing in the limit. Thus the improper [volume integral](../../../calculus.md#volume-integral) has the same zero value.

<h4 id="11c/b/ii">ii</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11c/b/ii)

Now $v=z^2$ and $\nabla v=2z\mathbf e_z$. Since $\nabla u=\widehat{\mathbf r}/a$, their [inner product](../../../linear-algebra.md#inner-product) is $2r\cos^2\theta/a$. Consequently

$$
\int_V\nabla u\cdot\nabla v\,dV=\frac2a\int_0^a r^3\,dr\int_0^\pi\cos^2\theta\sin\theta\,d\theta\int_0^{2\pi}d\varphi
=\frac2a\frac{a^4}{4}\frac23(2\pi)=\boxed{\frac{2\pi a^3}{3}}.
$$

Although $u=1$ on the boundary, the [Laplacian](../../../calculus.md#laplacian) is $\nabla^2v=2$, so $v$ is not a [harmonic function](../../../partial-differential-equation.md#harmonic-function). There is no contradiction with part (a). The origin singularity in the derivative of $u$ is harmless for this integral: its inner boundary contribution is of order $\varepsilon^4/a$ and tends to zero. More explicitly, [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) on the punctured ball gives outer flux $8\pi a^3/3$ and volume term $\int_V2r/a\,dV=2\pi a^3$, whose difference is the displayed answer.

<h4 id="11c/b/iii">iii</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#11c/b/iii)

Away from the origin the [gradients](../../../calculus.md#gradient) are $\nabla u=\widehat{\mathbf r}/a$ and $\nabla v=-\widehat{\mathbf r}/r^2$. The improper [volume integral](../../../calculus.md#volume-integral) is therefore

$$
\lim_{\varepsilon\downarrow0}\int_{\varepsilon<r<a}-\frac{1}{ar^2}\,dV
=-\frac{4\pi}{a}\lim_{\varepsilon\downarrow0}\int_\varepsilon^a dr=\boxed{-4\pi}.
$$

The function $v=1/r$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) only off the origin. It is singular inside the integration volume, so it does not meet part (a)'s regularity hypothesis. On the punctured ball, [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) has outer flux $-4\pi$ and inner flux $4\pi\varepsilon/a$: the inner outward [unit normal](../../../differential-geometry.md#unit-normal) is $-\widehat{\mathbf r}$, so $u\partial_n v=(\varepsilon/a)/\varepsilon^2$. Their sum is $-4\pi+4\pi\varepsilon/a$, exactly the integral before taking the limit. Equivalently the distributional [Laplacian](../../../calculus.md#laplacian) of $1/r$ is $-4\pi\delta_0$, rather than zero throughout the ball. This is [boundary flux from a singular harmonic potential](../../../partial-differential-equation.md#boundary-flux-from-a-singular-harmonic-potential); it explains why applying part (a) across the origin would be invalid.

## 12C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12c/i">i</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/i/solution">Solution</h4>

↑ **Parent:** [I](#12c/i)

The inequalities $y\le x\le2y$ force $y\ge0$, and the reciprocal bounds exclude zero. Thus the whole region lies in the positive quadrant. Introduce [ratio-product coordinates](../../../calculus.md#ratio-product-coordinates)

$$
u=\frac{x}{y},\qquad v=xy.
$$

The region becomes the rectangle $1\le u\le2$, $1\le v\le2$. The inverse map and its [Jacobian determinant](../../../calculus.md#jacobian-determinant) are

$$
x=\sqrt{uv},\qquad y=\sqrt{v/u},\qquad
\frac{\partial(x,y)}{\partial(u,v)}=\begin{vmatrix}x/(2u)&x/(2v)\\-y/(2u)&y/(2v)\end{vmatrix}=\frac{xy}{2uv}=\frac1{2u}>0.
$$

The [change of variables formula](../../../calculus.md#change-of-variables-formula) then gives

$$
\int_A\frac{x}{y}\,dx\,dy=\int_1^2\int_1^2u\frac1{2u}\,dv\,du=\boxed{\frac12}.
$$

<h3 id="12c/ii">ii</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12c/ii)

Take the usual positive, counterclockwise [boundary orientation](../../../differential-geometry.md#boundary-orientation); the printed question does not specify one, and reversing it negates the answer. Write the successive corner points as $P=(1,1)$, $Q=(\sqrt2,1/\sqrt2)$, $R=(2,1)$, $S=(\sqrt2,\sqrt2)$. Traverse $P\to Q\to R\to S\to P$, keeping the region on the left.

<a id="12c/ii/image-counterclockwise-boundary-of-the-region-between-two-rays-and-two-hyperbolas"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3-region.png)

**[Figure 1](#12c/ii/image-counterclockwise-boundary-of-the-region-between-two-rays-and-two-hyperbolas). Counterclockwise boundary of the region between two rays and two hyperbolas**.

On $PQ$, use $y=1/x$ with $1\le x\le\sqrt2$. Here $dy=-dx/x^2$, so the [line integral](../../../calculus.md#line-integral) is

$$
I_{PQ}=\int_1^{\sqrt2}\left(-\frac{x}{2}-1\right)dx=\frac34-\sqrt2.
$$

On $QR$, use $y=x/2$ with $\sqrt2\le x\le2$:

$$
I_{QR}=\int_{\sqrt2}^{2}\left(\frac{x}{2}-1\right)dx=\sqrt2-\frac32.
$$

On $RS$, use $y=2/x$ with $x$ decreasing from $2$ to $\sqrt2$:

$$
I_{RS}=\int_2^{\sqrt2}\left(-\frac{x}{2}-1\right)dx=\frac52-\sqrt2.
$$

Finally, on $SP$, use $y=x$ with $x$ decreasing from $\sqrt2$ to $1$:

$$
I_{SP}=\int_{\sqrt2}^{1}\left(\frac{x}{2}-1\right)dx=\sqrt2-\frac54.
$$

Adding all four [line integrals](../../../calculus.md#line-integral) gives **$\oint_C(x^2/(2y))\,dy-dx=1/2$** for the positive orientation, or **$-1/2$** for the reverse orientation.

<h3 id="12c/iii">iii</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12c/iii)

The equality with part (i) follows from [Green's theorem](../../../calculus.md#green-theorem). For the coefficients $P=-1$ and $Q=x^2/(2y)$,

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=\frac{x}{y}.
$$

They are smooth on a neighborhood of this region, since $y>0$. Thus for the positively oriented boundary,

$$
\boxed{\oint_C P\,dx+Q\,dy=\int_A\frac{x}{y}\,dx\,dy=\frac12.}
$$

The term $-dx$ itself has zero [line integral](../../../calculus.md#line-integral) around the closed [curve](../../../topology.md#curve), although it contributes to the four individual edge integrals.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
