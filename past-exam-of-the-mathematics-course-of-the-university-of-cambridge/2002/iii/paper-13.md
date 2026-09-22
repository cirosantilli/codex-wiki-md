# Paper 13

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper13.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper13.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $X$ be a connected [compact Riemann surface](../../../complex-analysis.md#compact-riemann-surface) of [genus](../../../topology.md#genus-of-a-surface) $g$. Choose an oriented [symplectic basis](../../../linear-algebra.md#symplectic-basis) $a_1,\ldots,a_g,b_1,\ldots,b_g$ of $H_1(X,\mathbb Z)$, with $a_i\cdot b_j=\delta_{ij}$. For a closed complex [differential form](../../../differential-form.md) $\alpha$, write $A_i(\alpha)=\int_{a_i}\alpha$ and $B_i(\alpha)=\int_{b_i}\alpha$. The [Riemann bilinear relations](../../../complex-analysis.md#riemann-bilinear-relations-for-a-compact-surface) begin with the identity

$$
\int_X\alpha\wedge\beta=\sum_{i=1}^g\bigl(A_i(\alpha)B_i(\beta)-B_i(\alpha)A_i(\beta)\bigr).
$$

To prove it, cut $X$ along the chosen cycles to obtain a fundamental polygon $P$. On this simply connected polygon, a closed [differential form](../../../differential-form.md) has a primitive $F$, with $dF=\alpha$. [Stokes theorem](../../../calculus.md#stokes-theorem) gives $\int_P\alpha\wedge\beta=\int_{\partial P}F\beta$. The two copies of each edge have opposite orientations, and their values of $F$ differ by the period acquired in passing between them. Pairing the copies of the $a_i$ and $b_i$ edges gives, respectively, $-B_i(\alpha)A_i(\beta)$ and $A_i(\alpha)B_i(\beta)$. Summing proves the identity; the convention $a_i\cdot b_i=1$ fixes its sign.

For [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) $\omega,\eta$, their [wedge product](../../../linear-algebra.md#exterior-product) is zero because locally both are multiples of $dz$. Thus the first [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) [Riemann bilinear relations](../../../complex-analysis.md#riemann-bilinear-relations-for-a-compact-surface) is

$$
\sum_i\bigl(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\bigr)=0.
$$

For a nonzero [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) $\omega=f(z)\,dz$, the second relation follows by applying the bilinear identity to $\omega,\overline\omega$:

$$
i\sum_i\bigl(A_i(\omega)\overline{B_i(\omega)}-B_i(\omega)\overline{A_i(\omega)}\bigr)
=i\int_X\omega\wedge\overline\omega
=2\int_X|f|^2\,dx\,dy>0.
$$

In particular, a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) with all $a$-periods zero must vanish. Since $\dim H^0(X,K_X)=g$, the map taking a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) to its $a$-periods is an [isomorphism](../../../algebra.md#isomorphism). We can therefore choose normalized [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) $\omega_1,\ldots,\omega_g$ with $\int_{a_i}\omega_j=\delta_{ij}$. Put $B_{ij}=\int_{b_i}\omega_j$. The first relation applied to $\omega_j,\omega_k$ gives $B_{jk}=B_{kj}$, and the second applied to $\sum_jc_j\omega_j$ gives $2\overline c^{,t}(\operatorname{Im}B)c>0$ for $c\ne0$. Consequently

$$
\boxed{B=B^t,\qquad Y=\operatorname{Im}B>0.}
$$

These conclusions make the construction of the [Jacobian variety](../../../abelian-variety.md#jacobian-variety) work. Integration identifies the image of $H_1(X,\mathbb Z)$ in $H^0(X,K_X)^*$ with the [period lattice](../../../complex-analysis.md#period-lattice) $\Lambda=\mathbb Z^g+B\mathbb Z^g$. The real-linear map $(m,n)\mapsto m+Bn$ is invertible: its imaginary part is $Yn$, and $Y$ is invertible. Hence $\Lambda$ is a discrete lattice of full real [rank](../../../linear-algebra.md#rank-one-quadratic-form) $2g$, and

$$
\boxed{\operatorname{Jac}(X)=H^0(X,K_X)^*/H_1(X,\mathbb Z)\simeq\mathbb C^g/(\mathbb Z^g+B\mathbb Z^g)}
$$

is a [compact](../../../topology.md#compact-space) [complex torus](../../../complex-geometry.md#complex-torus), rather than a non-Hausdorff quotient. Changing the [symplectic basis](../../../linear-algebra.md#symplectic-basis) changes the displayed coordinates but not this intrinsic quotient.

The [Riemann bilinear relations](../../../complex-analysis.md#riemann-bilinear-relations-for-a-compact-surface) also supply its [polarization of a complex torus](../../../complex-geometry.md#polarization-of-a-complex-torus). Use the [Hermitian form](../../../linear-algebra.md#hermitian-form) $H(z,w)=z^tY^{-1}\overline w$, linear in the first argument, and set $E=-\operatorname{Im}H$. Symmetry of $B$ gives

$$
E(m+Bn,m'+Bn')=m^tn'-n^tm',\qquad E(v,iv)=H(v,v)>0.
$$

Thus $E$ is an integral positive [Riemann form on a complex torus](../../../complex-geometry.md#riemann-form-on-a-complex-torus). Its matrix on the displayed lattice basis is the unimodular [symplectic matrix](../../../symplectic-geometry.md#symplectic-matrix). The corresponding positive [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle), equivalently the one constructed from theta automorphy in Solution 4, gives a principal [polarization of a complex torus](../../../complex-geometry.md#polarization-of-a-complex-torus). By the [Kodaira embedding theorem](../../../complex-geometry.md#kodaira-embedding-theorem) this makes the [complex torus](../../../complex-geometry.md#complex-torus) projective, hence an [abelian variety](../../../abelian-variety.md). The normalization $E=-\operatorname{Im}H$ here is important because $H$ was chosen linear in its first argument. If $g=0$, the spaces of [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) and periods are zero and the [Jacobian variety](../../../abelian-variety.md#jacobian-variety) is a point.

## 2

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Fix $p_0\in X$ and use the normalized [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) and [period lattice](../../../complex-analysis.md#period-lattice) of Solution 1. The [Abel-Jacobi map of a compact Riemann surface](../../../complex-analysis.md#abel-jacobi-map-of-a-compact-riemann-surface) is

$$
u(p)=\left(\int_{p_0}^p\omega_1,\ldots,\int_{p_0}^p\omega_g\right)\pmod\Lambda.
$$

Changing paths changes the vector by a period, so this is well defined and [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). Adding these vectors gives a symmetric map on $X^d$ and therefore the [Abelian sum map](../../../abelian-variety.md#abel-map-of-an-algebraic-curve) $u_d:X^{(d)}\to\operatorname{Jac}(X)$. Locally, even where points coincide, symmetric [holomorphic functions](../../../complex-analysis.md#holomorphic-function) descend to the elementary symmetric coordinates of the [symmetric product of a curve](../../../algebraic-geometry.md#symmetric-product-of-a-curve). For any [divisor](../../../number-theory.md#divisor) $D=\sum_pn_pp$ of degree zero, define $u(D)=\sum_pn_pu(p)$. **[Abel's theorem](../../../complex-analysis.md#abel-theorem-for-divisors) says that $D$ is a [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) if and only if $u(D)=0$.** Equivalently, two effective [divisors](../../../number-theory.md#divisor) of the same degree have the same Abel sum exactly when they are [linearly equivalent](../../../algebraic-geometry.md#linear-equivalence-of-weil-divisors).

We first establish the [residue](../../../analysis.md#residue) version of the bilinear identity. Let $\eta$ be a [meromorphic differential on a Riemann surface](../../../complex-analysis.md#meromorphic-differential-on-a-riemann-surface) with only simple poles and total [residue](../../../analysis.md#residue) zero, and let $F=\int_{p_0}^p\omega$ on the cut polygon, for a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) $\omega$. Excise small disks about the poles. Since $d(F\eta)=\omega\wedge\eta=0$ off the poles, the outer boundary integral is the sum of the positive small-circle integrals. The latter are $2\pi i\operatorname{res}_p(\eta)F(p)$. Pairing the outer edges as in Solution 1 therefore gives

$$
\sum_i\bigl(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\bigr)
=2\pi i\sum_p\operatorname{res}_p(\eta)\int_{p_0}^p\omega.
$$

The paths and the cut polygon are fixed together in this equality. Changing them changes the Abel vector by its [period lattice](../../../complex-analysis.md#period-lattice), which is precisely the ambiguity we need.

For the sufficiency direction, we need a [differential of the third kind](../../../complex-analysis.md#differential-of-the-third-kind) with prescribed [residues](../../../analysis.md#residue) $n_p$. Let $S$ be the reduced support of $D$, consisting of $s$ points. When $s>0$, the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives $h^0(K_X(S))=g-1+s$. The [residue](../../../analysis.md#residue) map from this space has [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $H^0(K_X)$, of dimension $g$: a differential with at most a simple pole and [residue](../../../analysis.md#residue) zero has no pole. Its image therefore has dimension $s-1$. The [residue theorem](../../../analysis.md#residue-theorem) puts the image inside the $s-1$ dimensional space of tuples with sum zero, so it is all that space. In particular there is a [meromorphic differential on a Riemann surface](../../../complex-analysis.md#meromorphic-differential-on-a-riemann-surface) $\eta$ with [residues](../../../analysis.md#residue) $n_p$. Subtracting a combination of the normalized [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) makes all its $a$-periods zero. The bilinear identity then says

$$
(B_1(\eta),\ldots,B_g(\eta))=2\pi i\,u(D),
$$

where on the right we temporarily choose the representative determined by the paths. If $D=0$, we simply take $\eta=0$.

Suppose now that $u(D)=0$ in the [Jacobian variety](../../../abelian-variety.md#jacobian-variety), so the chosen vector is $m+Bn$, with $m,n\in\mathbb Z^g$. Replace $\eta$ by

$$
\eta'=\eta-2\pi i\sum_jn_j\omega_j.
$$

Its $a$-periods are $-2\pi in_j$ and its $b$-periods are $2\pi im_i$. The periods around the punctures are $2\pi in_p$. These loops together generate the [homology](../../../homology.md) of the punctured [Riemann surface](../../../complex-analysis.md#riemann-surfaces), so every period of $\eta'$ lies in $2\pi i\mathbb Z$. Consequently $f(p)=\exp(\int^p\eta')$ is a single-valued nonzero [holomorphic function](../../../complex-analysis.md#holomorphic-function) off the support of $D$. At a support point, $\eta'=n_p\,dt/t+$ a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) differential, so $f=t^{n_p}$ times a nonvanishing [holomorphic function](../../../complex-analysis.md#holomorphic-function). It extends meromorphically and has [divisor](../../../number-theory.md#divisor) exactly $D$. This proves sufficiency, including negative coefficients.

Conversely, if $D=\operatorname{div}(f)$, take $\eta=df/f$. Its [residues](../../../analysis.md#residue) are the coefficients of $D$, while its $a$- and $b$-periods are integer multiples of $2\pi i$, by the winding numbers of $f$ along these loops. Writing them as $2\pi ia$ and $2\pi ib$, the [residue](../../../analysis.md#residue) bilinear identity gives $u(D)=b-Ba\in\Lambda$. Thus $u(D)=0$ in the [Jacobian variety](../../../abelian-variety.md#jacobian-variety), proving necessity and hence

$$
\boxed{\operatorname{div}(f)=D\text{ for some meromorphic }f\ne0\ \Longleftrightarrow\ \deg D=0\text{ and }u(D)=0.}
$$

Here the displayed necessity of degree zero is also the [residue theorem](../../../analysis.md#residue-theorem) applied to $df/f$.

There is a useful geometric version of the conclusion. For an effective [divisor](../../../number-theory.md#divisor) $D$, the fiber of $u_d$ through $D$ consists precisely of the effective [divisors](../../../number-theory.md#divisor) [linearly equivalent](../../../algebraic-geometry.md#linear-equivalence-of-weil-divisors) to $D$. A nonzero section of $\mathcal O_X(D)$ is a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) $f$ with $\operatorname{div}(f)+D\ge0$, and its zero [divisor](../../../number-theory.md#divisor) as a section is $\operatorname{div}(f)+D$. Two such sections give the same effective [divisor](../../../number-theory.md#divisor) exactly when their ratio is a nonzero constant. Thus the fiber is the [complete linear system of a divisor](../../../cartier-divisor.md#complete-linear-system-of-a-divisor) $|D|=\mathbb P H^0(X,\mathcal O_X(D))$.

## 3

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $D=\sum_pr_pp\in X^{(d)}$. The [derivative of the Abelian sum map](../../../abelian-variety.md#derivative-of-the-abelian-sum-map) is most naturally stated using [principal parts](../../../complex-geometry.md#principal-part-of-a-meromorphic-function). The [tangent space](../../../differential-geometry.md#tangent-space) of the [symmetric product of a curve](../../../algebraic-geometry.md#symmetric-product-of-a-curve) at $D$ is $H^0(\mathcal O_D(D))$, and the [tangent space](../../../differential-geometry.md#tangent-space) of the [Jacobian variety](../../../abelian-variety.md#jacobian-variety) is $H^0(K_X)^*$. With these identifications,

$$
\boxed{(d u_d)_D(v)(\omega)=\sum_p\operatorname{res}_p(v_p\omega),\qquad \omega\in H^0(K_X).}
$$

Its dual is restriction of [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) to the length-$d$ [divisor](../../../number-theory.md#divisor) scheme. In particular,

$$
\boxed{\ker(d u_d)_D^*=H^0(K_X(-D)),\qquad
\operatorname{rank}(d u_d)_D=g-h^0(K_X(-D))=d+1-h^0(\mathcal O_X(D)).}
$$

The last equality is the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem). These formulas apply to repeated points as well as distinct ones.

Here is a direct proof of the [repeated-point Abel differential formula](../../../abelian-variety.md#repeated-point-abel-differential-formula). At a multiplicity-$r$ point, choose a [local coordinate](../../../complex-analysis.md#local-coordinate) $t$ with $t(p)=0$. A nearby local [divisor](../../../number-theory.md#divisor) is described by the roots $t_1,\ldots,t_r$, or, without making an ordering choice, by their elementary symmetric functions $e_1,\ldots,e_r$:

$$
\prod_{i=1}^r(t-t_i)=t^r-e_1t^{r-1}+e_2t^{r-2}-\cdots+(-1)^re_r.
$$

These $e_k$ are smooth [local coordinates](../../../complex-analysis.md#local-coordinate) on the [symmetric product of a curve](../../../algebraic-geometry.md#symmetric-product-of-a-curve), including at the repeated [divisor](../../../number-theory.md#divisor). Under a first-order deformation, minus the logarithmic variation of this defining polynomial is the [principal part](../../../complex-geometry.md#principal-part-of-a-meromorphic-function)

$$
v_p=\sum_{k=1}^r(-1)^{k-1}\delta e_k\,t^{-k}\pmod{\mathcal O_{X,p}}.
$$

The sign can be checked at $r=1$: moving the point from $0$ to $\epsilon a$ gives $v=a/t$, and the Abel integral changes by $a\omega(p)$.

Write $\omega=(\sum_{j\ge0}c_jt^j)dt$ and its local primitive as $F(t)=\sum_{j\ge0}c_jt^{j+1}/(j+1)$. The local contribution to the [Abelian sum map](../../../abelian-variety.md#abel-map-of-an-algebraic-curve) is $\sum_i F(t_i)$. [Newton's identities](../../../polynomial.md#newton-s-identities), linearized at $e_1=\cdots=e_r=0$, give

$$
d\!\left(\sum_i t_i^k\right)=(-1)^{k-1}k\,de_k\quad(1\le k\le r),
\qquad d\!\left(\sum_i t_i^k\right)=0\quad(k>r).
$$

Substituting in the primitive therefore gives

$$
d\!\left(\sum_iF(t_i)\right)=\sum_{k=1}^r(-1)^{k-1}c_{k-1}\,de_k
=\operatorname{res}_p(v_p\omega).
$$

Summing over the support proves the theorem. In particular, a multiplicity-$r$ point tests the first $r$ coefficients of a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form), not just its value. The [residue](../../../analysis.md#residue) pairing between [principal parts](../../../complex-geometry.md#principal-part-of-a-meromorphic-function) of order at most $r$ and differential jets through order $r-1$ is perfect. Thus the annihilator of the derivative is precisely the [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form) vanishing to order at least $r_p$ at every $p$, namely $H^0(K_X(-D))$.

There is also a [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) description that explains its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) geometrically. The sequence

$$
0\longrightarrow\mathcal O_X\longrightarrow\mathcal O_X(D)\longrightarrow\mathcal O_D(D)\longrightarrow0
$$

gives a [connecting homomorphism](../../../homology.md#connecting-homomorphism) $\delta:H^0(\mathcal O_D(D))\to H^1(\mathcal O_X)$. Represent a [principal part](../../../complex-geometry.md#principal-part-of-a-meromorphic-function) by [meromorphic](../../../isolated-singularity.md#meromorphic-function) lifts on coordinate disks; their differences on overlaps give its [Čech cohomology](../../../ringed-space.md#cech-cohomology) class. Under [Serre duality](../../../ringed-space.md#serre-duality), pairing this class with $\omega$ is the sum of the [residues](../../../analysis.md#residue) of $v_p\omega$, so $\delta$ is the displayed derivative. Exactness shows that its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $H^0(\mathcal O_X(D))/\mathbb C$, of dimension $h^0(\mathcal O_X(D))-1$, in agreement with the tangent directions to the [complete linear system of a divisor](../../../cartier-divisor.md#complete-linear-system-of-a-divisor) in Solution 2.

Two consequences will be useful below. If $d\ge2g-1$, then $K_X(-D)$ has negative degree and no nonzero sections, so $u_d$ is a [submersion](../../../differential-geometry.md#submersion) everywhere. Its image is open, and it is also closed because $X^{(d)}$ is [compact](../../../topology.md#compact-space). Since the [Jacobian variety](../../../abelian-variety.md#jacobian-variety) is connected, $u_d$ is surjective. Thus the points $u(p)$ generate the [Jacobian variety](../../../abelian-variety.md#jacobian-variety) as a group. Together with [Abel's theorem](../../../complex-analysis.md#abel-theorem-for-divisors), this identifies the degree-zero [Picard group](../../../ringed-space.md#picard-group) with the [Jacobian variety](../../../abelian-variety.md#jacobian-variety): every [line bundle](../../../ringed-space.md#line-bundle) has a [meromorphic](../../../isolated-singularity.md#meromorphic-function) section and thus a [divisor](../../../number-theory.md#divisor) representation, injectivity is [Abel's theorem](../../../complex-analysis.md#abel-theorem-for-divisors), and surjectivity follows from $u_d(D)-d u(p_0)$.

For $g\ge1$, one can choose $g-1$ distinct points imposing independent conditions on $H^0(K_X)$: at each step a surviving nonzero [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) has only finitely many zeros, so choose a point where it does not vanish. Their sum $D$ has $h^0(K_X(-D))=1$ and hence $h^0(\mathcal O_X(D))=1$. The derivative has [rank](../../../linear-algebra.md#rank-one-quadratic-form) $g-1$ there. Consequently $W_{g-1}=u_{g-1}(X^{(g-1)})$ is an [irreducible](../../../representation-theory.md#irreducible-representation) subvariety of dimension $g-1$. This also covers $g=1$, when $X^{(0)}$ and $W_0$ are points.

## 4

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a symmetric matrix $B$ with $Y=\operatorname{Im}B$ positive definite, the [Riemann theta function](../../../modular-function.md#riemann-theta-function) is

$$
\boxed{\theta(z,B)=\sum_{n\in\mathbb Z^g}\exp\bigl(\pi i n^tBn+2\pi i n^tz\bigr).}
$$

On any [compact](../../../topology.md#compact-space) set of $z$, the absolute value of the summand is bounded by $\exp(-c|n|^2+C|n|)$ for some $c>0$, so the series and all its derivatives converge uniformly there. It is therefore entire. Its constant [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) in $\operatorname{Re}z$ is $1$, so it is not identically zero. Reindexing $n$ gives its parity and automorphy laws:

$$
\theta(-z,B)=\theta(z,B),\qquad
\theta(z+m+Bn,B)=e^{-\pi i n^tBn-2\pi i n^tz}\theta(z,B),\quad m,n\in\mathbb Z^g.
$$

Although the [theta function](../../../modular-function.md#theta-function) is not itself a function on $J=\mathbb C^g/\Lambda$, these factors define a [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle) on $J$, and its zeros define a [divisor](../../../number-theory.md#divisor) $\Theta$ there.

For the period matrix of $X$, the [Riemann vanishing theorem](../../../abelian-variety.md#riemann-vanishing-theorem) asserts that a fixed class $\kappa\in J$, the [vector of Riemann constants](../../../abelian-variety.md#vector-of-riemann-constants) in the convention used here, satisfies

$$
\boxed{\Theta=W_{g-1}-\kappa.}
$$

We prove both its support statement and its reduced [divisor](../../../number-theory.md#divisor) structure. This will make the multiplicity calculation in Solution 5 independent of any assumed multiplicity theorem.

The essential contour calculation is the [theta pullback zero-divisor identity](../../../abelian-variety.md#theta-pullback-zero-divisor-identity). Put $f_z(p)=\theta(u(p)-z,B)$, regarding this as a local expression for a section on $X$. If it is not identically zero, let $D_z$ be its zero [divisor](../../../number-theory.md#divisor). We claim

$$
\deg D_z=g,\qquad u_g(D_z)=z+\kappa.
$$

Use the cut polygon from Solution 1 and choose cuts avoiding the zeros. There $\alpha_z=d_p\log f_z$ is a [meromorphic](../../../isolated-singularity.md#meromorphic-function) differential whose [residues](../../../analysis.md#residue) are the zero multiplicities. Under continuation by an $a_j$ period, $u$ changes by the integer vector $e_j$, so $\alpha_z$ is unchanged. Under a $b_j$ period, $u$ changes by $Be_j$, so automorphy gives $\alpha_z\mapsto\alpha_z-2\pi i\omega_j$. Pairing opposite boundary sides therefore gives

$$
2\pi i\deg D_z=\int_{\partial P}\alpha_z
=2\pi i\sum_j\int_{a_j}\omega_j=2\pi ig.
$$

For example, the two $a_j$ sides, traversed with opposite orientations and separated by a $b_j$ translation, contribute $\int_{a_j}(\alpha_z-(\alpha_z-2\pi i\omega_j))$. This fixes the sign of the count.

For the first moment of the zeros, the [residue theorem](../../../analysis.md#residue-theorem) on the polygon gives, component by component,

$$
\sum_q\operatorname{ord}_q(f_z)\,u_k(q)=\frac{1}{2\pi i}\int_{\partial P}u_k\alpha_z.
$$

This is interpreted modulo the [period lattice](../../../complex-analysis.md#period-lattice), with the lifts to the polygon fixed. Vary $z$ without letting zeros cross the cuts, and put $h=\delta\log f_z$. The coordinate $u_k$ does not vary, so integration by parts gives

$$
\delta\!\left(\sum_q\operatorname{ord}_q(f_z)u_k(q)\right)
=-\frac{1}{2\pi i}\int_{\partial P}\omega_k h.
$$

There is no endpoint term: the closed polygon boundary returns both the Abel integral and $h$ to their starting values. Across an $a_j$ translation $h$ is unchanged, while across a $b_j$ translation it changes by $2\pi i\delta z_j$. Pairing the boundary edges consequently gives $\int_{\partial P}\omega_k h=-2\pi i\sum_j\delta z_j\int_{a_j}\omega_k=-2\pi i\delta z_k$. Thus $\delta u_g(D_z)=\delta z$, and $u_g(D_z)-z$ is constant. The calculation uses weighted zeros, so their collisions cause no problem. The parameters where $f_z$ is identically zero form a proper analytic subset: they are given by the vanishing of all its local Taylor coefficients, and parameters outside $\Theta$ are not in it. Its complement in the connected [complex manifold](../../../complex-geometry.md#complex-manifold) $J$ is connected, so the constant is one class $\kappa$. This proves the pullback identity globally, with continuation of the zero [divisors](../../../number-theory.md#divisor) where necessary.

We must account for the parameters with identically zero pullback, rather than discard them. No [irreducible](../../../representation-theory.md#irreducible-representation) component $C$ of $\Theta$ can consist entirely of such parameters. Otherwise parity would imply $C-u(p)\subset\Theta$ for every $p\in X$. The image of $C\times X$ under subtraction is [irreducible](../../../representation-theory.md#irreducible-representation), is contained in $\Theta$, and contains $C$ when $p=p_0$. Since $C$ is an [irreducible](../../../representation-theory.md#irreducible-representation) component of the [hypersurface](../../../differential-geometry.md#hypersurface), that image must be $C$. Hence $C-u(p)=C$ for all $p$. The surjectivity of the large-degree [Abelian sum map](../../../abelian-variety.md#abel-map-of-an-algebraic-curve), proved in Solution 3, says that these translations generate all of $J$. This would make the nonempty proper subset $C$ invariant under every translation, which is impossible.

A generic point $z$ of each component of $\Theta$ therefore has nonzero pullback. Since $\theta(-z)=\theta(z)=0$, its zero [divisor](../../../number-theory.md#divisor) contains $p_0$. Write $D_z=p_0+D'$, with $D'$ effective of degree $g-1$. The pullback identity gives $u_{g-1}(D')=z+\kappa$. Each component of $\Theta$ is consequently contained in $W_{g-1}-\kappa$. By Solution 3 the latter is [irreducible](../../../representation-theory.md#irreducible-representation) of dimension $g-1$, so any such component equals it. The zero locus is nonempty for $g>0$: any parameter with nonzero pullback has $g$ pullback zeros. We have proved equality of supports, in both directions.

Finally the automorphy factors make the [First Chern class](../../../complex-geometry.md#first-chern-class) of the theta [line bundle](../../../ringed-space.md#line-bundle) primitive. On the two-torus spanned by $a_i,b_j$, the logarithm of the $b_j$ factor changes by $-2\pi i\delta_{ij}$ after the $a_i$ translation; equivalently the transition for local frames has opposite winding. Thus $c_1(a_i,b_j)=\delta_{ij}$, while $c_1(a_i,a_j)=c_1(b_i,b_j)=0$. In particular some integral pairing equals $1$. As its support is the single [irreducible](../../../representation-theory.md#irreducible-representation) [hypersurface](../../../differential-geometry.md#hypersurface) $W_{g-1}-\kappa$, the zero [divisor](../../../number-theory.md#divisor) is $m(W_{g-1}-\kappa)$ for a positive integer $m$. Its integral [First Chern class](../../../complex-geometry.md#first-chern-class) would then be divisible by $m$. Primitivity forces $m=1$, proving the displayed equality as reduced [divisors](../../../number-theory.md#divisor).

The sign convention is $\kappa=u_g(D_z)-z$, so the translate is $W_{g-1}-\kappa$; a convention naming $-\kappa$ the Riemann constant reverses that displayed sign. For $g=1$, $\kappa=(1+B)/2$ modulo periods and the zero locus is the corresponding single point. For $g=0$, the empty-lattice theta series is $1$, its zero locus is empty, and the degree-$-1$ effective locus is empty; no negative symmetric product is required.

## 5

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Identify $\operatorname{Pic}^{g-1}(X)$ with the [Jacobian variety](../../../abelian-variety.md#jacobian-variety) using the base point and the translation of Solution 4. A [line bundle](../../../ringed-space.md#line-bundle) $L$ of degree $g-1$ corresponds to the point $z=u(D)-\kappa$ for any [divisor](../../../number-theory.md#divisor) representation $L\simeq\mathcal O_X(D)$. The [Riemann singularity theorem](../../../abelian-variety.md#riemann-singularity-theorem) is

$$
\boxed{\operatorname{mult}_{z}\Theta=h^0(X,L).}
$$

In particular, the [theta divisor](../../../abelian-variety.md#theta-divisor) is singular exactly at the degree-$g-1$ [line bundles](../../../ringed-space.md#line-bundle) with at least two independent sections. We prove the equality, including the upper bound on multiplicity.

Choose a fixed effective [divisor](../../../number-theory.md#divisor) $A$ of degree $N\ge g$, and a local [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) family $L_\eta$ representing nearby points of $\operatorname{Pic}^{g-1}(X)$. Such a family can be constructed locally from the [holomorphic exponential sequence](../../../complex-geometry.md#holomorphic-exponential-sequence), by varying line-bundle transition functions through exponentials of [Čech cohomology](../../../ringed-space.md#cech-cohomology) representatives. By [Serre duality](../../../ringed-space.md#serre-duality), $H^1(L_\eta(A))$ is dual to $H^0(K_X\otimes L_\eta^{-1}(-A))$, whose degree is $g-1-N<0$, so it vanishes. The [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives $h^0(L_\eta(A))=N$. By [cohomology and base change for line bundles on a curve](../../../ringed-space.md#cohomology-and-base-change-for-line-bundles-on-a-curve), these spaces form a [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) $E$ of [rank](../../../linear-algebra.md#rank-one-quadratic-form) $N$. The spaces $H^0(L_\eta(A)|_A)$ form another [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) $F$ of [rank](../../../linear-algebra.md#rank-one-quadratic-form) $N$. Evaluation gives a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) square matrix $T(\eta)$ locally, with exact sequence

$$
0\longrightarrow H^0(L_\eta)\longrightarrow E_\eta
\xrightarrow{T(\eta)}F_\eta\longrightarrow H^1(L_\eta)\longrightarrow0.
$$

Consequently $\det T(\eta)=0$ exactly when $L_\eta$ has a nonzero section, namely on the support of the [theta divisor](../../../abelian-variety.md#theta-divisor).

At the point $L$, put $r=h^0(L)=h^1(L)$, the equality being [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem). An invertible minor of size $N-r$ persists near this point. [Holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) row and column operations, or the [Schur complement](../../../linear-algebra.md#schur-complement), give

$$
\det T(\eta)=a(\eta)\det M(\eta),\qquad a(0)\ne0,
\qquad M(0)=0,
$$

where $M$ is an $r\times r$ [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) matrix. This is the [Schur complement presentation of a theta singularity](../../../abelian-variety.md#schur-complement-presentation-of-a-theta-singularity). Its linear term in a tangent direction $\xi\in H^1(\mathcal O_X)$ is the [cup product](../../../cohomology.md#cup-product) map

$$
dM_0(\xi):H^0(L)\longrightarrow H^1(L),\qquad s\longmapsto\xi\smile s.
$$

To see this concretely, vary transition functions $g_{ij}$ of $L$ to $g_{ij}(1+\epsilon\xi_{ij})$. A section $s_i$ lifts to $s_i+\epsilon s'_i$ precisely when its first-order compatibility equation can be solved; the obstruction is the cocycle $\xi_{ij}s_j$. This is $\xi\smile s$. Passing to the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and [cokernel](../../../linear-algebra.md#cokernel) of $T(0)$ gives exactly the derivative of the reduced matrix $M$, proving the assertion without assuming a multiplicity formula.

Before extracting the order of $\det M$, we verify that $\det T$ is a reduced equation of the [theta divisor](../../../abelian-variety.md#theta-divisor). Generic points of $W_{g-1}$ have $h^0(L)=1$ by Solution 3. At such a point, both $H^0(L)$ and $H^0(K_X\otimes L^{-1})$ are one-dimensional. Their nonzero sections $s,t$ have nonzero product $st\in H^0(K_X)$. Choose $\xi\in H^1(\mathcal O_X)$ with $\langle\xi,st\rangle\ne0$ under [Serre duality](../../../ringed-space.md#serre-duality). The scalar $dM_0(\xi)$ is nonzero, so $\det T$ has a simple zero generically on the [irreducible](../../../representation-theory.md#irreducible-representation) [theta divisor](../../../abelian-variety.md#theta-divisor). Since its support is exactly that [irreducible](../../../representation-theory.md#irreducible-representation) [hypersurface](../../../differential-geometry.md#hypersurface), it defines the reduced [divisor](../../../number-theory.md#divisor). Solution 4 independently proved the same reduced structure for the [Riemann theta function](../../../modular-function.md#riemann-theta-function). On the smooth ambient [Jacobian variety](../../../abelian-variety.md#jacobian-variety), local equations of the same reduced [divisor](../../../number-theory.md#divisor) differ by a nonvanishing [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) unit. Hence the orders of the local theta equation and $\det M$ agree everywhere.

Every entry of $M$ vanishes at the point, so each term in its [determinant](../../../linear-algebra.md#determinant) has order at least $r$. This proves $\operatorname{mult}_z\Theta\ge r$. To obtain equality, we exhibit an [invertible cup-product direction for a line bundle on a curve](../../../abelian-variety.md#invertible-cup-product-direction-for-a-line-bundle-on-a-curve). Set $V=H^0(L)$ and $W=H^0(K_X\otimes L^{-1})$, both of dimension $r$. There are $r$ distinct points $p_1,\ldots,p_r$ at which evaluation is an [isomorphism](../../../algebra.md#isomorphism) for $V$: choose them inductively, since a surviving nonzero section has only finitely many zeros. The same holds for $W$. The nonvanishing of each evaluation [determinant](../../../linear-algebra.md#determinant) defines a nonempty open subset of the [irreducible](../../../representation-theory.md#irreducible-representation) variety $X^r$. Their intersection, also avoiding the diagonals, is therefore nonempty. Choose points in it and [local coordinates](../../../complex-analysis.md#local-coordinate) and compatible trivializations of $L$ and $K_X\otimes L^{-1}$ at each point.

Let $\xi$ be the [connecting homomorphism](../../../homology.md#connecting-homomorphism) class of the [meromorphic](../../../isolated-singularity.md#meromorphic-function) [principal parts](../../../complex-geometry.md#principal-part-of-a-meromorphic-function) $\lambda_i/t_i$ at these points, with all $\lambda_i\ne0$. The [residue](../../../analysis.md#residue) form of [Serre duality](../../../ringed-space.md#serre-duality) gives

$$
\langle\xi\smile s,t\rangle=\langle\xi,st\rangle
=\sum_{i=1}^r\lambda_i s(p_i)t(p_i).
$$

If $S$ and $U$ are the two invertible evaluation matrices, the matrix of this pairing is $S^t\operatorname{diag}(\lambda_1,\ldots,\lambda_r)U$, and is invertible. Thus the [cup product](../../../cohomology.md#cup-product) map $\xi\smile-:H^0(L)\to H^1(L)$ is an [isomorphism](../../../algebra.md#isomorphism). Along the corresponding analytic parameter line,

$$
M(\epsilon\xi)=\epsilon\,dM_0(\xi)+O(\epsilon^2),\qquad
\det M(\epsilon\xi)=\epsilon^r\det(dM_0(\xi))+O(\epsilon^{r+1}),
$$

with nonzero leading coefficient. The order is at most $r$, completing the proof of the [Riemann singularity theorem](../../../abelian-variety.md#riemann-singularity-theorem).

This argument also identifies the [tangent cone to a theta divisor](../../../abelian-variety.md#tangent-cone-to-a-theta-divisor): its degree-$r$ equation is $\det(\xi\smile-)$, which is not the zero polynomial. For $r=1$, the tangent hyperplane is $\langle\xi,st\rangle=0$, in agreement with the annihilator description of the [derivative of the Abelian sum map](../../../abelian-variety.md#derivative-of-the-abelian-sum-map). For $r\ge2$ all first derivatives vanish, proving singularity. In [genus](../../../topology.md#genus-of-a-surface) $1$ the [theta divisor](../../../abelian-variety.md#theta-divisor) is a single smooth point of multiplicity $1$. In [genus](../../../topology.md#genus-of-a-surface) $0$ the effective degree-$-1$ locus is empty, so there is no singularity statement at a point of it.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
