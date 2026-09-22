# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper7.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

In a unital [Banach algebra](../../../banach-algebra.md), the [Neumann series](../../../banach-algebra.md#neumann-series) gives $(1-u)^{-1}=\sum_{k=0}^\infty u^k$ whenever $\|u\|<1$: the series converges in [norm](../../../functional-analysis.md#norm) by [submultiplicativity](../../../banach-algebra.md#submultiplicativity) and [completeness](../../../topological-analysis.md#completeness), and multiplication of its partial sums on either side gives $1-u^{N+1}\to1$. Consequently, if $g$ is invertible and $\|g^{-1}\|\|h-g\|<1$, write

$$
h=g(1+v),\qquad v=g^{-1}(h-g).
$$

The second factor has a [Neumann series](../../../banach-algebra.md#neumann-series) inverse, so $h$ is invertible. This exhibits a ball around each $g$ in the [group of invertible elements of a Banach algebra](../../../banach-algebra.md#group-of-invertible-elements-of-a-banach-algebra), proving that group is an [open set](../../../topology.md#open-set).

The same series proves [continuity of inversion in a Banach algebra](../../../banach-algebra.md#continuity-of-inversion-in-a-banach-algebra), with the useful quantitative estimate

$$
\|h^{-1}-g^{-1}\|
=\|[(1+v)^{-1}-1]g^{-1}\|
\le\frac{\|g^{-1}\|^2\|h-g\|}{1-\|g^{-1}\|\|h-g\|}.
$$

The right side tends to zero as $h\to g$. Since applying inversion twice gives the original element, it is a [bijection](../../../function.md#bijection) whose inverse is the same [continuous](../../../calculus.md#continuous-function) map. Thus **inversion is a homeomorphism of the open group of invertibles onto itself**.

For the final unheaded request, define

$$
E=\{\lambda\in\mathbb C:1-\lambda a\text{ is invertible}\}.
$$

It is open by the preceding argument and contains $0$. If $\lambda_0$ were a [boundary](../../../topology.md#boundary-of-a-set) point, a sequence $\lambda_n\in E$ would converge to $\lambda_0$, while openness gives $\lambda_0\notin E$. Then $1-\lambda_na\to1-\lambda_0a$ is a noninvertible limit of invertibles. The one-sided-inverse argument in part (ii) shows that this limit has neither a [left inverse of an algebra element](../../../banach-algebra.md#left-inverse-of-an-algebra-element) nor a [right inverse of an algebra element](../../../banach-algebra.md#right-inverse-of-an-algebra-element), contradicting the hypothesis. Therefore $E$ has empty [boundary](../../../topology.md#boundary-of-a-set); it is both open and [closed](../../../topology.md#closed-set) in the [connected](../../../geometry-and-topology.md#connected-space) [complex plane](../../../complex-analysis.md#complex-plane), and $E=\mathbb C$.

For every nonzero $\mu$, put $\lambda=\mu^{-1}$. The identity $\mu1-a=\mu(1-\lambda a)$ proves invertibility, so the [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) $a$ is contained in $\{0\}$. It is nonempty: if the [resolvent of an element](../../../banach-algebra.md#resolvent-of-an-element) existed for all $\mu\in\mathbb C$, it would be an entire algebra-valued function tending to zero at infinity by the [Neumann series](../../../banach-algebra.md#neumann-series). Applying any [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) and then the [Liouville theorem](../../../complex-analysis.md#liouville-theorem) would make it zero; the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) separates points and would force the resolvent itself to be zero, contradicting its inverse equation. Hence

$$
\boxed{\sigma_A(a)=\{0\}.}
$$

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

If $\|x_n^{-1}\|\|x-x_n\|<1$, then

$$
x=x_n\bigl(1+x_n^{-1}(x-x_n)\bigr)
$$

is invertible by the [Neumann series](../../../banach-algebra.md#neumann-series), a contradiction. Thus every $n$ satisfies

$$
\|x_n^{-1}\|\ge\frac1{\|x-x_n\|}.
$$

Here $x\ne x_n$ because $x_n$ is invertible and $x$ is not. Since $x_n\to x$, this proves the [inverse norm divergence at noninvertible boundary points](../../../banach-algebra.md#inverse-norm-divergence-at-noninvertible-boundary-points):

$$
\boxed{\|x_n^{-1}\|\longrightarrow\infty.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Suppose $b$ were a [left inverse of an algebra element](../../../banach-algebra.md#left-inverse-of-an-algebra-element) $x$, so $bx=1$. Then $bx_n\to1$, and $bx_n$ is invertible for all sufficiently large $n$ by the [Neumann series](../../../banach-algebra.md#neumann-series). For such $n$, $b=(bx_n)x_n^{-1}$ is a product of invertibles, hence invertible. The equation $bx=1$ then gives $x=b^{-1}$, a contradiction.

If instead $xb=1$, then $x_nb\to1$, so $x_nb$ is eventually invertible. Now $b=x_n^{-1}(x_nb)$ is invertible, and again $x=b^{-1}$, a contradiction. This proves that **a noninvertible limit of invertibles has neither type of one-sided inverse**. No finite-dimensional assumption is used.

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $K=\sigma_A(x)$ and equip $\mathcal O(U)$ with the [compact-open topology](../../../real-analysis.md#compact-open-topology). All [algebra homomorphisms](../../../algebra.md#algebra-homomorphism-over-a-field) here are complex linear. Choose a finite positively oriented [boundary](../../../topology.md#boundary-of-a-set) cycle $\Gamma$ in $U\setminus K$ with [winding number](../../../complex-analysis.md#winding-number) one on a neighborhood of $K$ and zero outside $U$. Such a cycle can be obtained as the [boundary](../../../topology.md#boundary-of-a-set) of a finite union of sufficiently small squares whose [interior](../../../topology.md#interior-topology) contains $K$ and whose closure is contained in $U$; holes are included with negative [boundary](../../../topology.md#boundary-of-a-set) orientation. Define the [holomorphic functional calculus](../../../banach-algebra.md#holomorphic-functional-calculus) by the norm-convergent [contour integral](../../../complex-analysis.md#contour-integral)

$$
\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(z)R(z)\,dz,
\qquad R(z)=(z1-x)^{-1}.
$$

The [resolvent identity](../../../banach-algebra.md#resolvent-identity) proves that $R$ is a [Banach-space-valued holomorphic function](../../../complex-analysis.md#banach-space-valued-holomorphic-function) off $K$. The [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem), applied after each [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional), makes the integral independent of the chosen [boundary](../../../topology.md#boundary-of-a-set) cycle. The [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) then gives equality of the algebra-valued integrals. Moreover,

$$
\|\Theta_x(f)\|\le\frac{\operatorname{length}(\Gamma)}{2\pi}\sup_\Gamma\|R(z)\|\sup_\Gamma|f(z)|,
$$

which proves complex [linearity](../../../vector-space.md#linearity) and [continuity](../../../calculus.md#continuous-function) for the [compact-open topology](../../../real-analysis.md#compact-open-topology).

For the constant function $1$ and the coordinate function $Z$, the contour can be deformed to a large circle because their integrands are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) everywhere outside $K$. There the [Neumann series](../../../banach-algebra.md#neumann-series) gives $R(z)=\sum_{n\ge0}x^nz^{-n-1}$. Integrating term by term shows

$$
\Theta_x(1)=1,\qquad\Theta_x(Z)=x.
$$

To prove multiplicativity, take nested cycles $\Gamma_o,\Gamma_i$ around $K$, with the outer cycle winding once on the inner cycle and the inner winding zero on the outer cycle. Use the outer cycle for $f$ and the inner for $g$. The [resolvent identity](../../../banach-algebra.md#resolvent-identity) reads

$$
R(z)R(w)=\frac{R(w)-R(z)}{z-w}.
$$

In the resulting double integral, the term containing $R(w)$ gives $f(w)g(w)R(w)$ after the $z$ integral, by the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula). The term containing $R(z)$ vanishes after the $w$ integral, because $w\mapsto g(w)/(z-w)$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on and inside the inner cycle's region. Therefore

$$
\Theta_x(f)\Theta_x(g)=\Theta_x(fg).
$$

The integrals are over finite [compact](../../../topology.md#compact-space) curves and have [continuous](../../../calculus.md#continuous-function) integrands, so exchanging their order is legitimate. This proves the existence of the required [continuous](../../../calculus.md#continuous-function) unital [algebra homomorphism](../../../algebra.md#algebra-homomorphism-over-a-field).

For uniqueness, the [Runge approximation theorem](../../../complex-analysis.md#runge-s-theorem) gives density in $\mathcal O(U)$, for the [compact-open topology](../../../real-analysis.md#compact-open-topology), of [rational functions](../../../isolated-singularity.md#rational-function) with poles outside $U$. More explicitly, exhaust $U$ by [compact](../../../topology.md#compact-space) sets that are holomorphically convex relative to $U$, and approximate on those sets by [rational functions](../../../isolated-singularity.md#rational-function) whose poles lie in the complement of $U$; this gives convergence on every [compact](../../../topology.md#compact-space) subset. Any unital [algebra homomorphism](../../../algebra.md#algebra-homomorphism-over-a-field) taking $Z$ to $x$ must take $(Z-\alpha)^{-1}$, for $\alpha\notin U$, to $(x-\alpha1)^{-1}$, since it preserves inverse equations. Partial fractions and [polynomial](../../../polynomial.md) algebra therefore fix its value on every such [rational function](../../../isolated-singularity.md#rational-function). [Continuity](../../../calculus.md#continuous-function) fixes its value on their limits. Thus **the [continuous](../../../calculus.md#continuous-function) unital homomorphism with the prescribed coordinate value is unique**. Restricting a function to a smaller neighborhood of $K$ gives the same value, either by the contour definition or this uniqueness argument.

To prove the [holomorphic spectral mapping theorem](../../../mathematics.md#holomorphic-spectral-mapping-theorem), first let $\mu\notin f(K)$. There is an open neighborhood $V\subseteq U$ of $K$ on which $f-\mu$ has no zeros. The [holomorphic function](../../../complex-analysis.md#holomorphic-function) $h=1/(f-\mu)$ on $V$ supplies a two-sided inverse through

$$
\Theta_x(f)-\mu1=\Theta_x(f-\mu),\qquad
\Theta_x(f-\mu)\Theta_x(h)=\Theta_x(h)\Theta_x(f-\mu)=1.
$$

Thus $\sigma_A(\Theta_x(f))\subseteq f(K)$. Conversely, if $\lambda\in K$ and $\mu=f(\lambda)$, the divided difference

$$
g(z)=\frac{f(z)-f(\lambda)}{z-\lambda},\qquad g(\lambda)=f'(\lambda),
$$

is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on $U$, and multiplicativity gives

$$
\Theta_x(f)-\mu1=(x-\lambda1)\Theta_x(g).
$$

The two factors commute. A commuting product $uv$ can be invertible only if both factors are invertible: its inverse commutes with each factor, and $v(uv)^{-1}$ is a two-sided inverse for $u$. Invertibility of the displayed product would therefore contradict $\lambda\in K$. This proves

$$
\boxed{\sigma_A(\Theta_x(f))=f(\sigma_A(x)).}
$$

For the root, let $D=\mathbb C\setminus(-\infty,0]$ and $q(z)=\exp(\operatorname{Log}z/3)$, using the [principal complex logarithm](../../../analysis.md#principal-complex-logarithm). Define $y=\Theta_x(q)$. Since $q(z)^3=z$, multiplicativity and the [holomorphic spectral mapping theorem](../../../mathematics.md#holomorphic-spectral-mapping-theorem) give

$$
\boxed{y^3=x,\qquad\sigma_A(y)=q(K)\subseteq S,\qquad S=\{z\ne0:|\arg z|<\pi/3\}.}
$$

This is the [principal cube root of a Banach-algebra element](../../../banach-algebra.md#principal-cube-root-of-a-banach-algebra-element).

For uniqueness, suppose $v^3=x$ and $\sigma_A(v)\subset S$. Cubing maps the whole open sector $S$ into $D$, so

$$
F:\mathcal O(D)\longrightarrow A,\qquad F(h)=\Theta_v\bigl(z\mapsto h(z^3)\bigr)
$$

is a [continuous](../../../calculus.md#continuous-function) unital [algebra homomorphism](../../../algebra.md#algebra-homomorphism-over-a-field): pullback by cubing is [continuous](../../../calculus.md#continuous-function) for the [compact-open topology](../../../real-analysis.md#compact-open-topology), since images of [compact](../../../topology.md#compact-space) sets are [compact](../../../topology.md#compact-space). It takes the coordinate function to $v^3=x$, and uniqueness already proved gives $F=\Theta_x$. For $z\in S$, the scalar [principal cube root](../../../analysis.md#principal-cube-root) satisfies $q(z^3)=z$, because $3\arg z\in(-\pi,\pi)$. Hence

$$
v=\Theta_v(q\circ(z\mapsto z^3))=F(q)=\Theta_x(q)=y.
$$

This proves **uniqueness with the stated spectral sector**, without assuming the ambient [Banach algebra](../../../banach-algebra.md) is [commutative](../../../algebra.md#commutativity) or that [algebra characters](../../../banach-algebra.md#character-of-an-algebra) separate its elements.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

First, a [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal) $L$ is [closed](../../../topology.md#closed-set). Its [norm](../../../functional-analysis.md#norm) closure is again a [left ideal](../../../associative-algebra.md#left-ideal), since multiplication is [continuous](../../../calculus.md#continuous-function). If that closure were all of $A$, some $\ell\in L$ would satisfy $\|1-\ell\|<1$ and would be invertible by the [Neumann series](../../../banach-algebra.md#neumann-series). But a proper [left ideal](../../../associative-algebra.md#left-ideal) cannot contain an invertible element: $\ell^{-1}\ell=1$ would put $1$ in $L$. Maximality therefore forces $\overline L=L$.

Consequently $X=A/L$ is a nonzero [quotient Banach space](../../../banach-space.md#quotient-banach-space). It is a [simple module](../../../module-theory.md#irreducible-module) for left multiplication by $A$, because the inverse image of any [submodule](../../../module-theory.md#submodule) under $A\to A/L$ is a [left ideal](../../../associative-algebra.md#left-ideal) containing $L$, and hence is either $L$ or $A$. Since $La\subseteq L$, right multiplication defines a well-defined bounded [module endomorphism](../../../module-theory.md#module-endomorphism)

$$
T:X\longrightarrow X,\qquad T(u+L)=ua+L,\qquad\|T\|\le\|a\|.
$$

Indeed, changing $u$ by an element of $L$ changes $ua$ by an element of $L$, and taking the infimum over representatives proves the [quotient norm](../../../banach-space.md#quotient-norm) bound. Right multiplication commutes with the left action by [associativity](../../../group.md#associative-property).

Choose $\lambda$ in the nonempty [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) of $T$ in the [Banach algebra](../../../banach-algebra.md) $\mathcal B(X)$. Both the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and range of $T-\lambda I$ are [submodules](../../../module-theory.md#submodule). If this [module endomorphism](../../../module-theory.md#module-endomorphism) were nonzero, simplicity would force its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) to be zero and its range to be all of $X$. It would be a bounded bijection of [Banach spaces](../../../banach-space.md), with bounded inverse by the [bounded inverse theorem](../../../functional-analysis.md#bounded-inverse-theorem), contradicting the choice of $\lambda$. Thus $T=\lambda I$. Applying this identity to $1+L$ yields $a-\lambda1\in L$. If also $a-\mu1\in L$, then $(\lambda-\mu)1\in L$; since $1\notin L$, $\lambda=\mu$. Therefore

$$
\boxed{\text{There is exactly one }\lambda\in\mathbb C\text{ with }a-\lambda1\in L.}
$$

This is the [scalar right action on a maximal-left-ideal quotient](../../../associative-algebra.md#scalar-right-action-on-a-maximal-left-ideal-quotient); it does not assume that $L$ is a two-sided ideal or that $A/L$ is an algebra.

Now consider the [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra) $Z$. For each $u\in A$, the map $z\mapsto zu-uz$ is a [continuous](../../../calculus.md#continuous-function) [linear map](../../../vector-space.md#linear-map), so its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is [closed](../../../topology.md#closed-set). Their intersection $Z$ is therefore [closed](../../../topology.md#closed-set). The identity belongs to $Z$, as do sums and scalar multiples of its elements. If $z,w\in Z$, then for every $u\in A$,

$$
(zw)u=z(wu)=z(uw)=(zu)w=(uz)w=u(zw).
$$

Thus $zw\in Z$. Also $zw=wz$, since $z$ commutes with every element of $A$, including $w$. Hence **the center is a [closed](../../../topology.md#closed-set) [commutative](../../../algebra.md#commutativity) unital [subalgebra](../../../algebra.md#subalgebra)**, and is a [Banach algebra](../../../banach-algebra.md) in the inherited [norm](../../../functional-analysis.md#norm).

For every $z\in Z$, the inclusion $Lz=zL\subseteq L$ allows the first argument to apply. Let $\chi(z)$ be the unique scalar for which $z-\chi(z)1\in L$. Equivalently, the induced right multiplication on $A/L$ is $T_z=\chi(z)I$. Since

$$
T_{z+w}=T_z+T_w,\qquad T_{\alpha z}=\alpha T_z,\qquad T_{zw}=T_wT_z,\qquad T_1=I,
$$

the map $\chi:Z\to\mathbb C$ is a complex-linear unital [character of an algebra](../../../banach-algebra.md#character-of-an-algebra). It is surjective because $\chi(\alpha1)=\alpha$, and its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is precisely $L\cap Z$. Consequently

$$
\boxed{Z/(L\cap Z)\cong\mathbb C,\qquad L\cap Z\text{ is a maximal ideal of }Z.}
$$

Indeed any ideal properly containing the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) would have a nonzero image in the [field](../../../algebra.md#field) $\mathbb C$ and thus would be all of $Z$. The [algebra character](../../../banach-algebra.md#character-of-an-algebra) is also [continuous](../../../calculus.md#continuous-function): $|\chi(z)|=\|\chi(z)I\|=\|T_z\|\le\|z\|$, although [continuity](../../../calculus.md#continuous-function) is not needed for maximality.

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Fix $z\in K$. If $z\in\partial K$, the conclusion is immediate. Otherwise $z$ is in the [interior](../../../topology.md#interior-topology) of $K$. If $f(z)=0$, nonnegativity of the [boundary](../../../topology.md#boundary-of-a-set) [supremum](../../../real-analysis.md#supremum) suffices. For $f(z)\ne0$, the complex [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) gives a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $\ell:A\to\mathbb C$ with $\|\ell\|=1$ and $\ell(f(z))=\|f(z)\|$. The scalar function $g=\ell\circ f$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point).

Let $V$ be the [connected component](../../../geometry-and-topology.md#connected-component) of the [interior](../../../topology.md#interior-topology) of $K$ containing $z$. It is bounded, its closure is contained in $K$, and $\partial V\subseteq\partial K$. To see the last inclusion, a [boundary](../../../topology.md#boundary-of-a-set) point of $V$ lying in the [interior](../../../topology.md#interior-topology) of $K$ would have a small [connected](../../../geometry-and-topology.md#connected-space) open ball in that [interior](../../../topology.md#interior-topology) meeting $V$; the ball would belong to the same component, contradicting that it is a [boundary](../../../topology.md#boundary-of-a-set) point. The scalar [maximum modulus principle on a bounded domain](../../../complex-analysis.md#maximum-modulus-principle-on-a-bounded-domain) therefore gives

$$
\|f(z)\|=|g(z)|\le\sup_{w\in\partial V}|g(w)|\le\sup_{w\in\partial K}\|f(w)\|.
$$

For [completeness](../../../topological-analysis.md#completeness), this [boundary](../../../topology.md#boundary-of-a-set) form of the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) follows by taking the maximum on the [compact](../../../topology.md#compact-space) closure of $V$. An [interior](../../../topology.md#interior-topology) maximum makes $g$ constant on $V$, in which case [continuity](../../../calculus.md#continuous-function) gives the same value on its nonempty [boundary](../../../topology.md#boundary-of-a-set). Thus the [norm maximum principle for a Banach-space-valued holomorphic function](../../../complex-analysis.md#norm-maximum-principle-for-a-banach-space-valued-holomorphic-function) applies to arbitrary [compact](../../../topology.md#compact-space) $K$, even when it is disconnected or has nonsmooth [boundary](../../../topology.md#boundary-of-a-set):

$$
\boxed{\|f(z)\|\le\sup_{w\in\partial K}\|f(w)\|.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For $n\ge0$, put

$$
p_n(w)=\|f(w)^{2^n}\|^{1/2^n},\qquad M=\sup_{w\in\partial K}r(f(w)).
$$

The bound $r(u)\le\|u\|$ makes $M$ finite. Each $p_n$ is [continuous](../../../calculus.md#continuous-function); [submultiplicativity](../../../banach-algebra.md#submultiplicativity) gives $p_{n+1}\le p_n$, and the [spectral radius formula](../../../analysis.md#spectral-radius-formula) gives $p_n(w)\to r(f(w))$. [Spectral radius](../../../analysis.md#spectral-radius) need not be [continuous](../../../calculus.md#continuous-function), so applying the [Dini theorem](../../../real-analysis.md#dini-s-theorem) directly to $p_n$ would not be justified. Instead define, on the [compact](../../../topology.md#compact-space) [boundary](../../../topology.md#boundary-of-a-set),

$$
q_n(w)=\max\{p_n(w),M\}.
$$

These are [continuous](../../../calculus.md#continuous-function), decrease pointwise to the [continuous](../../../calculus.md#continuous-function) constant $M$, and therefore converge uniformly by the [Dini theorem](../../../real-analysis.md#dini-s-theorem). In particular,

$$
\limsup_{n\to\infty}\sup_{w\in\partial K}p_n(w)\le M.
$$

Multiplication is a [continuous](../../../calculus.md#continuous-function) bilinear operation in a [Banach algebra](../../../banach-algebra.md), so the [product rule](../../../calculus.md#product-rule) shows that $w\mapsto f(w)^{2^n}$ is a [Banach-space-valued holomorphic function](../../../complex-analysis.md#banach-space-valued-holomorphic-function). Part (i), applied to this power, gives

$$
\|f(z)^{2^n}\|^{1/2^n}\le\sup_{w\in\partial K}\|f(w)^{2^n}\|^{1/2^n}.
$$

Taking the limit on the left and the limit superior on the right proves the [spectral-radius maximum principle](../../../complex-analysis.md#spectral-radius-maximum-principle):

$$
\boxed{r(f(z))\le\sup_{w\in\partial K}r(f(w)).}
$$

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Apply the [spectral-radius maximum principle](../../../complex-analysis.md#spectral-radius-maximum-principle) to the entire [Banach-space-valued holomorphic function](../../../complex-analysis.md#banach-space-valued-holomorphic-function) $f(z)=a+zb$ on the [closed](../../../topology.md#closed-set) disk $|z|\le\varepsilon$. On its [boundary](../../../topology.md#boundary-of-a-set) the assumed estimate gives $r(f(z))\le C\varepsilon$. Therefore

$$
0\le r(a)=r(f(0))\le C\varepsilon
$$

for every $\varepsilon>0$. Letting $\varepsilon\downarrow0$ proves

$$
\boxed{r(a)=0.}
$$

The puncture at $z=0$ in the hypothesis causes no difficulty: the bound is used only on the nonzero [boundary](../../../topology.md#boundary-of-a-set) circle.

## 5

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

An [algebra involution](../../../associative-algebra.md#algebra-involution) is a map $x\mapsto x^*$ satisfying

$$
(\alpha x+\beta y)^*=\overline\alpha x^*+\overline\beta y^*,\qquad
(xy)^*=y^*x^*,\qquad (x^*)^*=x.
$$

Thus it is a [conjugate-linear map](../../../vector-space.md#antilinear-map), reverses multiplication, and has square equal to the identity map. These are algebraic axioms; [norm](../../../functional-analysis.md#norm) [continuity](../../../calculus.md#continuous-function), when included in a convention for a Banach star algebra, is an additional requirement and is not used here. A [Hermitian element of a star algebra](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) satisfies $h^*=h$.

Conjugate [linearity](../../../vector-space.md#linearity) gives $0^*=0$. The map $*$ is surjective, so every $u$ is $v^*$ for some $v$. The identities $(v1)^*=1^*v^*=v^*$ and $(1v)^*=v^*1^*=v^*$ show that $1^*$ is a two-sided identity; uniqueness of the identity gives $1^*=1$. Therefore **both zero and the identity are [Hermitian algebra elements](../../../associative-algebra.md#hermitian-element-of-a-star-algebra)**.

For the final unheaded request, first prove equality of the two spectra for a [Hermitian element of a star algebra](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) $h\in B$. Write $D=\mathbb C\setminus\sigma_A(h)$. The spectrum is a [compact](../../../topology.md#compact-space) subset of the real axis by the assumption that $A$ is a [Hermitian Banach algebra](../../../banach-algebra.md#hermitian-banach-algebra), so $D$ is [connected](../../../geometry-and-topology.md#connected-space): points above and below the real axis can be joined by paths passing beyond the endpoints of an interval containing the spectrum; points of the real axis outside the spectrum can first move a short distance vertically. Define

$$
E=\{\lambda\in D:(\lambda1-h)^{-1}\in B\}.
$$

For large $|\lambda|$, the [Neumann series](../../../banach-algebra.md#neumann-series) $\lambda^{-1}\sum_{n\ge0}(h/\lambda)^n$ converges in the [closed](../../../topology.md#closed-set) unital [star-subalgebra](../../../associative-algebra.md#star-subalgebra) $B$, so $E$ is nonempty. It is relatively open in $D$ by the same series applied to a perturbation of an already invertible element of $B$. It is relatively [closed](../../../topology.md#closed-set) in $D$, since the [resolvent of an element](../../../banach-algebra.md#resolvent-of-an-element) is [continuous](../../../calculus.md#continuous-function) in $A$ and $B$ is [closed](../../../topology.md#closed-set). Connectedness gives $E=D$. Conversely an inverse in $B$ is an inverse in $A$, so

$$
\sigma_B(h)=\sigma_A(h).
$$

This proves the needed [spectrum in a closed unital subalgebra](../../../banach-algebra.md#spectrum-in-a-closed-unital-subalgebra) equality for [Hermitian algebra elements](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) without presupposing that their spectra in $B$ are real.

Now suppose $b\in B$ is invertible in $A$. Both $bb^*$ and $b^*b$ are [Hermitian algebra elements](../../../associative-algebra.md#hermitian-element-of-a-star-algebra), since reversing products and applying $*$ twice fixes them. They are invertible in $A$, by part (ii), so the preceding equality of spectra of [Hermitian algebra elements](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) makes them invertible in $B$. Part (ii), applied within $B$, then makes $b$ invertible in $B$. Applying this to $b-\lambda1$ for every scalar $\lambda$, and using the automatic converse for an inverse already in $B$, proves [spectral permanence for Hermitian Banach algebras](../../../banach-algebra.md#spectral-permanence-for-hermitian-banach-algebras):

$$
\boxed{\sigma_B(b)=\sigma_A(b)\quad(b\in B).}
$$

Only closedness, a common identity, closure under the [algebra involution](../../../associative-algebra.md#algebra-involution), and real ambient spectra of [Hermitian algebra elements](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) were used; the [C-star identity](../../../banach-algebra.md#c-star-identity) was not assumed.

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

If $u$ is invertible, applying the [algebra involution](../../../associative-algebra.md#algebra-involution) to $u^{-1}u=uu^{-1}=1$ gives

$$
u^*(u^{-1})^*=(u^{-1})^*u^*=1,
$$

so $u^*$ is invertible and $(u^*)^{-1}=(u^{-1})^*$. The converse follows by applying $*$ again. Since

$$
(x-\lambda1)^*=x^*-\overline\lambda1,
$$

we have $\lambda\notin\sigma_A(x)$ if and only if $\overline\lambda\notin\sigma_A(x^*)$. Taking complements and using that [complex conjugation](../../../complex-analysis.md#complex-conjugation) is a bijection gives

$$
\boxed{\sigma_A(x^*)=\{\overline\lambda:\lambda\in\sigma_A(x)\}.}
$$

The conjugation bar in the printed PDF is essential; this is not an assertion that the two spectra always coincide.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

If $x$ is invertible, part (i)'s inverse calculation gives an inverse for $x^*$, and therefore both $xx^*$ and $x^*x$ are invertible. Conversely, if both products are invertible, set

$$
r=x^*(xx^*)^{-1},\qquad \ell=(x^*x)^{-1}x^*.
$$

Then $xr=1$ and $\ell x=1$: $r$ is a [right inverse of an algebra element](../../../banach-algebra.md#right-inverse-of-an-algebra-element) $x$ and $\ell$ is a [left inverse of an algebra element](../../../banach-algebra.md#left-inverse-of-an-algebra-element) $x$. They coincide because $\ell=\ell(xr)=(\ell x)r=r$, providing a two-sided inverse. Thus

$$
\boxed{x\text{ invertible}\iff xx^*\text{ and }x^*x\text{ both invertible},\qquad x^{-1}=x^*(xx^*)^{-1}=(x^*x)^{-1}x^*.}
$$

Both products are required in a general [Banach algebra](../../../banach-algebra.md); a single one-sided inverse need not suffice.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
