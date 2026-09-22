# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2013/PaperIB_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2013/PaperIB_2.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4G](#4g)
  - [i](#4g/i)
    - [Solution](#4g/i/solution)
  - [ii](#4g/ii)
    - [Solution](#4g/ii/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
- [7A](#7a)
  - [Solution](#7a/solution)
- [8H](#8h)
  - [Solution](#8h/solution)
- [9H](#9h)
  - [Solution](#9h/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11G](#11g)
  - [i](#11g/i)
    - [Solution](#11g/i/solution)
  - [ii](#11g/ii)
    - [Solution](#11g/ii/solution)
  - [iii](#11g/iii)
    - [Solution](#11g/iii/solution)
- [12F](#12f)
  - [Solution](#12f/solution)
- [13D](#13d)
  - [i](#13d/i)
    - [Solution](#13d/i/solution)
  - [ii](#13d/ii)
    - [Solution](#13d/ii/solution)
  - [iii](#13d/iii)
    - [Solution](#13d/iii/solution)
- [14F](#14f)
  - [Solution](#14f/solution)
- [15A](#15a)
  - [Solution](#15a/solution)
- [16B](#16b)
  - [Solution](#16b/solution)
- [17B](#17b)
  - [i](#17b/i)
    - [Solution](#17b/i/solution)
  - [ii](#17b/ii)
    - [Solution](#17b/ii/solution)
- [18D](#18d)
  - [Solution](#18d/solution)
- [19C](#19c)
  - [Solution](#19c/solution)
- [20H](#20h)
  - [i](#20h/i)
    - [Solution](#20h/i/solution)
  - [ii](#20h/ii)
    - [Solution](#20h/ii/solution)
  - [iii](#20h/iii)
    - [Solution](#20h/iii/solution)

## 1E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

Write $U^*=\overline U^T$ for the [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose). Taking [determinants](../../../linear-algebra.md#determinant) in $U^*AU=A$ gives $|\det U|^2\det A=\det A$. Since the [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) $A$ is invertible, **every such $U$ is invertible and $|\det U|=1$.** The identity belongs to $U_A$; if $U,V\in U_A$, then $(UV)^*A(UV)=V^*AV=A$; and multiplying $U^*AU=A$ by $(U^*)^{-1}$ and $U^{-1}$ gives $(U^{-1})^*AU^{-1}=A$. Associativity comes from [matrix multiplication](../../../vector-space.md#matrix-multiplication), so this is a [group](../../../group.md).

The [Hermitian form](../../../linear-algebra.md#hermitian-form) $h_A(v,w)=v^*Aw$ obeys $h_A(Uv,Uw)=h_A(v,w)$ precisely when $U\in U_A$. Thus **$U_A$ is the group of linear isometries of this nondegenerate [Hermitian form](../../../linear-algebra.md#hermitian-form)**; positivity of $A$ is unnecessary.

For $A=I$, $U$ is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix). Here is a direct [diagonalization of a matrix](../../../linear-operator-theory.md#diagonalization-of-a-matrix) proof. Over $\mathbb C$, its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) has a root, giving a unit [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$ with $Uv=\lambda v$. Preservation of the [inner product](../../../linear-algebra.md#inner-product) gives $|\lambda|=1$. If $w\perp v$, then $\langle Uw,Uv\rangle=\langle w,v\rangle=0$, so $v^\perp$ is invariant. The restriction is again a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix). Induction on the [dimension](../../../vector-space.md#dimension-vector-space) supplies an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector). In that [basis](../../../vector-space.md#basis), **$U$ is diagonal, with diagonal entries on the unit [circle](../../../topology.md#circle)**.

## 2G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

Let $R$ be a [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) and $I$ a nonzero [ideal](../../../commutative-algebra.md#ideal). Choose $d\in I\setminus\{0\}$ minimizing the Euclidean size. For any $a\in I$, [Euclidean division](../../../number-theory.md#euclidean-division) gives $a=qd+r$, where either $r=0$ or $r$ has smaller size than $d$. But $r=a-qd\in I$, so minimality forces $r=0$. Consequently $I=(d)$. The zero [ideal](../../../commutative-algebra.md#ideal) is $(0)$, proving that **every [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain)**.

A commutative ring is [Noetherian](../../../algebra.md#noetherian-ring) if every [ideal](../../../commutative-algebra.md#ideal) is finitely generated; equivalently, every ascending chain of [ideals](../../../commutative-algebra.md#ideal) stabilizes. To see the equivalence, the union of an ascending chain is an [ideal](../../../commutative-algebra.md#ideal). Finitely many generators for that union already belong to one member of the chain, after which the chain is constant. Conversely, an [ideal](../../../commutative-algebra.md#ideal) which is not finitely generated permits successive choices outside the [ideals](../../../commutative-algebra.md#ideal) generated by previous choices, producing a strictly ascending chain.

Every [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) is therefore [Noetherian](../../../algebra.md#noetherian-ring). The given [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) property of the [Gaussian integers](../../../commutative-algebra.md#gaussian-integer) yields

$$
\boxed{\mathbb Z[i]\text{ is Noetherian}.}
$$

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

Both maxima exist by continuity on the [compact set](../../../topology.md#compact-space) $[a,b]$. Their sum is nonnegative and vanishes only for $f=0$. The identities $\|cf\|_1=|c|\|f\|_1$ and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) follow by applying the corresponding [supremum norm](../../../functional-analysis.md#supremum-norm) facts to $f$ and $f'$. This proves that $\|\cdot\|_1$ is a [norm](../../../functional-analysis.md#norm).

For $m=(a+b)/2$, $|\Phi(f)|=|f'(m)|\leq\max|f'|\leq\|f\|_1$. Hence **the first unit ball has image contained in $[-1,1]$**: [derivative](../../../calculus.md#derivative) evaluation is a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) for this [norm](../../../functional-analysis.md#norm).

For the [supremum norm](../../../functional-analysis.md#supremum-norm) alone, take $f_N(x)=\sin(N(x-m))$. These smooth functions satisfy $\|f_N\|_0\leq1$, but $\Phi(f_N)=N$. Thus **the second image is unbounded**. The distinction is the [unboundedness of derivative evaluation in the supremum norm](../../../functional-analysis.md#unboundedness-of-derivative-evaluation-in-the-supremum-norm), not a failure of differentiability of the individual functions.

## 4G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4g/i">i</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/i/solution">Solution</h4>

↑ **Parent:** [I](#4g/i)

**True.** In a [discrete topology](../../../topology.md#discrete-space), the singletons form an [open cover](../../../topology.md#open-cover). If $X$ is [compact](../../../topology.md#compact-space), a finite subcover exists, so $X$ is finite. Conversely, any [open cover](../../../topology.md#open-cover) of a finite set has a finite subcover: choose one member containing each point. This converse does not require the [discrete topology](../../../topology.md#discrete-space).

<h3 id="4g/ii">ii</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4g/ii)

**False without a separation assumption.** Give $X=\{0,1\}$ the [indiscrete topology](../../../topology.md#indiscrete-topology) $\{\varnothing,X\}$, and take $Y=\{0\}$. Both spaces are finite and hence [compact](../../../topology.md#compact-space), but $Y$ is not a [closed set](../../../topology.md#closed-set) because $X\setminus Y=\{1\}$ is not open. In a [Hausdorff space](../../../topology.md#hausdorff-space), a [compact subset](../../../topology.md#compact-space) would be closed; that hypothesis is absent here.

## 5B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

Parametrize the [characteristics](../../../algebra.md#characteristic-of-a-field) by $s$, starting from $(x,y,u)=(1,r,r)$. Their [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) are

$$
\frac{dx}{ds}=x,\qquad \frac{dy}{ds}=x+y,\qquad \frac{du}{ds}=1.
$$

They give $x=e^s$, $y=e^s(r+s)$ and $u=r+s$. Thus $s=\log x$ and $r=y/x-\log x$, so

$$
\boxed{u(x,y)=\frac yx\quad(x>0).}
$$

Indeed, $u_x=-y/x^2$, $u_y=1/x$ give $xu_x+(x+y)u_y=1$, and $u(1,y)=y$. The initial line is noncharacteristic, and its [characteristics](../../../algebra.md#characteristic-of-a-field) cover the half-plane $x>0$. The data do not determine a solution on $x<0$; a smooth solution through the origin is impossible because the differential equation there would read $0=1$.

## 6D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

Take the [divergence](../../../calculus.md#divergence) of the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law), $\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E$. Since the [divergence of a curl is zero](../../../calculus.md#divergence-of-a-curl-is-zero) vanishes, and [Gauss's law](../../../electromagnetism.md#gauss-s-law) gives $\nabla\cdot\mathbf E=\rho/\epsilon_0$, the result is

$$
\boxed{\partial_t\rho+\nabla\cdot\mathbf J=0.}
$$

This is the [charge continuity equation](../../../electromagnetism.md#charge-continuity-equation).

At an internal point of a homogeneous [Ohmic conductor](../../../electromagnetism.md#ohmic-conductor), [Ohm's law](../../../electromagnetism.md#ohm-s-law) gives $\mathbf J=\sigma\mathbf E$. Since $\sigma$ is constant, the [charge continuity equation](../../../electromagnetism.md#charge-continuity-equation) becomes $\partial_t\rho=-(\sigma/\epsilon_0)\rho$. Therefore

$$
\boxed{\rho(\mathbf x,t)=\rho(\mathbf x,0)e^{-t/\tau},\qquad \tau=\epsilon_0/\sigma.}
$$

This is [charge relaxation](../../../electromagnetism.md#charge-relaxation). Here $\rho$ is the total charge appearing in the vacuum form of [Gauss's law](../../../electromagnetism.md#gauss-s-law); in a homogeneous dielectric description of free charge the corresponding constant permittivity replaces $\epsilon_0$.

For a finite isolated body, charge travels to the surface. The bulk formula applies at internal points, not across the interface where [electrical conductivity](../../../electromagnetism.md#electrical-conductivity) jumps and [surface charge density](../../../electromagnetism.md#surface-charge-density) accumulates. Integrating the [charge continuity equation](../../../electromagnetism.md#charge-continuity-equation) over the body, including its surface charge, gives constant total [electric charge](../../../electromagnetism.md#electric-charge) because no [electric current](../../../electromagnetism.md#electric-current) crosses the external boundary. Bulk decay and [conservation of electric charge](../../../electromagnetism.md#charge-conservation) are therefore compatible.

## 7A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7a/solution">Solution</h3>

↑ **Parent:** [7A](#7a)

The [free surface](../../../fluid-mechanics.md#free-surface) is a material surface, so its [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) is

$$
\eta_t+\phi_x\eta_x=\phi_y\quad\text{at }y=\eta.
$$

With constant atmospheric pressure $p_a$ and no [surface tension](../../../fluid-mechanics.md#surface-tension), the [dynamic boundary condition for an inviscid interface](../../../fluid-mechanics.md#dynamic-boundary-condition-for-an-inviscid-interface) follows from [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation):

$$
\phi_t+\tfrac12|\nabla\phi|^2+g\eta=F(t)-p_a/\rho\quad\text{at }y=\eta.
$$

Write $\phi=Ux+\varphi$, where $\varphi$ and $\eta$ are small. Choose the time-dependent potential gauge so the undisturbed right-hand side is $U^2/2$. Retaining first-order terms, evaluated at $y=0$, gives

$$
\boxed{\eta_t+U\eta_x=\varphi_y,\qquad \varphi_t+U\varphi_x+g\eta=0.}
$$

The [incompressibility](../../../fluid-mechanics.md#incompressible-flow) condition also gives [Laplace's equation](../../../partial-differential-equation.md#laplace-equation) for $\varphi$.

Set $\Omega=\omega-kU$. Substitution of the specified [normal mode](../../../wave-equation.md#normal-mode) into the two linearized [boundary conditions](../../../differential-equation.md#boundary-condition) yields $-i\Omega a=ikb$ and $\Omega b+ga=0$. Eliminating $b$ gives the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{(\omega-kU)^2=gk.}
$$

The decay factor $e^{ky}$ in a fluid extending to $y=-\infty$ uses $k>0$. With signed [wavenumber](../../../wave-equation.md#wavenumber) the decaying factor is $e^{|k|y}$ and the right-hand side is $g|k|$. The frequency shift is the [advection](../../../fluid-mechanics.md#advection) of a [deep-water gravity wave](../../../fluid-mechanics.md#deep-water-gravity-wave) by the uniform current.

## 8H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8h/solution">Solution</h3>

↑ **Parent:** [8H](#8h)

The [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem) says that if $S$ is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic) and $\delta$ a finite-variance [estimator](../../../statistical-modelling.md#estimator), then $\delta^*=\mathbb E(\delta\mid S)$ is an [estimator](../../../statistical-modelling.md#estimator) with the same expectation and no larger [variance](../../../variance.md). Sufficiency ensures the conditional distribution, and hence this formula as a function of the data, does not involve the unknown parameter. The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives $\mathbb E\delta^*=\mathbb E\delta$, while the [law of total variance](../../../probability-theory.md#law-of-total-variance) gives

$$
\operatorname{Var}(\delta)=\operatorname{Var}(\delta^*)+\mathbb E\operatorname{Var}(\delta\mid S).
$$

This proves the theorem and shows that equality holds exactly when $\delta$ is already determined by $S$, almost surely. In particular, unbiasedness is preserved.

Assume $n\geq3$. Independence gives $\mathbb E\hat\theta=p_0p_1p_2=\theta$, so the proposed indicator is unbiased and has [variance](../../../variance.md) $\theta(1-\theta)$. The type counts $S=(n_0,n_1,n_2)$ are a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic): conditional on them, every ordering of the labels is equally likely. Consequently,

$$
\boxed{\theta^*=\mathbb E(\hat\theta\mid S)=\frac{n_0n_1n_2}{n(n-1)(n-2)}.}
$$

For example, the conditional probability of the ordered first three labels is $(n_0/n)(n_1/(n-1))(n_2/(n-2))$. This is [Rao-Blackwellization of a multinomial probability product](../../../probability-and-statistics.md#rao-blackwellization-of-a-multinomial-probability-product).

If all three $p_i$ are positive, there is positive probability that all three counts are positive. On such an event the conditional indicator has probability strictly between zero and one, so its [conditional variance](../../../variance.md#conditional-variance) is positive. Thus **$\operatorname{Var}(\theta^*)<\theta(1-\theta)$ for interior parameter values**. If any $p_i=0$, then $\theta=0$ and both [estimators](../../../statistical-modelling.md#estimator) have zero [variance](../../../variance.md); the printed strict inequality is impossible at those boundary parameters. The valid unrestricted statement is the non-strict inequality.

## 9H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9h/solution">Solution</h3>

↑ **Parent:** [9H](#9h)

An [cut of a flow network](../../../graph-theory.md#cut-of-a-flow-network) partitions a [flow network](../../../graph-theory.md#flow-network) into $S,S^c$, with source $A\in S$ and sink $B\notin S$. Its [cut capacity](../../../graph-theory.md#cut-capacity) is the sum of capacities of arcs directed from $S$ to $S^c$; a [minimum cut](../../../graph-theory.md#minimum-cut) minimizes this sum.

Use the suggested nodes. Give $A\to a_e$ capacity $1$, each $a_e\to b_v$ capacity $M=m+kn+1$, and each $b_v\to B$ capacity $k$. By the [max-flow min-cut theorem](../../../graph-theory.md#max-flow-min-cut-theorem), a flow of value $kn$ exists once every [cut capacity](../../../graph-theory.md#cut-capacity) is at least $kn$.

Consider a [cut of a flow network](../../../graph-theory.md#cut-of-a-flow-network) containing no crossing arc of capacity $M$, and let $U$ be the intersections on the sink side. Every street incident to $U$ must also be on that side, or its arc to an endpoint in $U$ would cross the [cut of a flow network](../../../graph-theory.md#cut-of-a-flow-network). Hence at least $d(U)$ source-to-street arcs cross, as do the $n-|U|$ intersection-to-sink arcs from the other intersections. Therefore its [cut capacity](../../../graph-theory.md#cut-capacity) is at least

$$
d(U)+k(n-|U|)\geq kn.
$$

A [cut of a flow network](../../../graph-theory.md#cut-of-a-flow-network) crossing a capacity-$M$ arc has still larger capacity. The [cut of a flow network](../../../graph-theory.md#cut-of-a-flow-network) just before the sink has capacity $kn$, proving the maximum flow value is exactly $kn$.

The [integral max-flow theorem](../../../graph-theory.md#integral-max-flow-theorem) supplies an integral maximum flow. Every intersection sends $k$ units to the sink; each street can supply at most one unit, assigned to one endpoint. Orient each assigned street **away from its assigned endpoint**. Orient unassigned streets arbitrarily. Then each vertex has at least $k$ outgoing streets. An [Ford-Fulkerson algorithm](../../../graph-theory.md#ford-fulkerson-algorithm) with integer capacities constructs this [flow](../../../graph-theory.md#flow) and therefore the street directions. Notice that the condition also is necessary: outgoing streets from vertices in $U$ are distinct edges incident to $U$, so $d(U)\geq k|U|$. This is an [outdegree orientation criterion](../../../graph-theory.md#outdegree-orientation-criterion).

## 10E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

A set is [linearly dependent](../../../vector-space.md#linear-dependence) if some finite selection of distinct vectors admits a relation $\sum_jc_jv_j=0$ with coefficients not all zero. For a finite set this is just such a nontrivial relation using its vectors.

Prove dependence of $n+1$ vectors in $\mathbb R^n$ by induction, starting with the zero-dimensional case. If all first coordinates vanish, select $n$ of the vectors and apply induction in $\mathbb R^{n-1}$. Otherwise relabel so the last vector has first coordinate $a\ne0$. For $1\leq j\leq n$, put $w_j=v_j-(v_{j,1}/a)v_{n+1}$. These $n$ vectors have zero first coordinate, so induction supplies $\sum_{j=1}^nc_jw_j=0$, with some $c_j\ne0$. Expanding gives a nontrivial [linear dependence](../../../vector-space.md#linear-dependence) among the original vectors. The same proof works over any [field](../../../algebra.md#field).

Now express vectors of $V$ in coordinates relative to its given $n$-element [basis](../../../vector-space.md#basis). Any other [basis](../../../vector-space.md#basis) has at most $n$ elements: more would contain $n+1$ [linearly dependent](../../../vector-space.md#linear-dependence) vectors. If it has $m<n$ elements, expressing the original [basis](../../../vector-space.md#basis) in its coordinates makes the original $n$ vectors [linearly dependent](../../../vector-space.md#linear-dependence), a contradiction. Thus **every [basis](../../../vector-space.md#basis) has exactly $n$ elements**.

Finally, the functions $\sin(jx)$, $j=1,2,\ldots$, are bounded and continuous. Any finite relation among them can be multiplied by $\sin(rx)$ and integrated over $[0,2\pi]$. The [orthogonality](../../../linear-algebra.md#orthogonal-vectors) identity

$$
\int_0^{2\pi}\sin(jx)\sin(rx)\,dx=\pi\,\delta_{jr}
$$

forces every coefficient to vanish. Arbitrarily large [linearly independent](../../../vector-space.md#linear-independence) finite sets exist, so **the [vector space](../../../vector-space.md) of bounded continuous functions is infinite-dimensional**.

## 11G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11g/i">i</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/i/solution">Solution</h4>

↑ **Parent:** [I](#11g/i)

The [structure theorem for finitely generated modules over a principal ideal domain](../../../module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain) applies because a [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain). For a finitely generated $R$-[module](../../../module-theory.md#module-mathematics),

$$
\boxed{M\cong R^r\oplus R/(d_1)\oplus\cdots\oplus R/(d_s),\qquad d_1\mid d_2\mid\cdots\mid d_s,}
$$

where the $d_i$ are nonzero nonunits. The free rank $r$ and the [invariant factors of a finitely generated module](../../../module-theory.md#invariant-factor-of-a-finitely-generated-module) $d_i$ are unique, with each $d_i$ determined up to multiplication by a unit. Equivalently, the [torsion submodule](../../../module-theory.md#torsion-submodule) decomposes into cyclic [modules](../../../module-theory.md#module-mathematics) $R/(P^a)$ for irreducible $P$, with uniquely determined prime-power elementary factors.

<h3 id="11g/ii">ii</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11g/ii)

The annihilating polynomial excludes any free $\mathbb C[X]$-summand. In a cyclic [primary decomposition](../../../module-theory.md#primary-decomposition) summand $\mathbb C[X]/(P^a)$, the same condition requires $P^a$ to divide $(X-2)^4$. Thus $P=X-2$, up to a scalar unit, and $1\leq a\leq4$. The complex [dimension](../../../vector-space.md#dimension-vector-space) of this summand is $a$.

Write $A_j=\mathbb C[X]/((X-2)^j)$. The exponents must form a [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) $4$, giving exactly

$$
\boxed{A_4,\quad A_3\oplus A_1,\quad A_2\oplus A_2,\quad A_2\oplus A_1\oplus A_1,\quad A_1^{\oplus4}.}
$$

They are distinct [module isomorphism](../../../module-theory.md#module-isomorphism) types by uniqueness in the [structure theorem for finitely generated modules over a principal ideal domain](../../../module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain); equivalently they are the five possible [Jordan block](../../../linear-operator-theory.md#jordan-block) patterns for eigenvalue $2$ in dimension four.

<h3 id="11g/iii">iii</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11g/iii)

Factor $X^3+X=X(X-i)(X+i)$. These factors generate pairwise comaximal [ideals](../../../commutative-algebra.md#ideal), so the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) gives

$$
\Phi([p])=(p(0),p(i),p(-i)).
$$

The three copies of $\mathbb C$ have different [module](../../../module-theory.md#module-mathematics) structures: $X$ acts by $0,i,-i$, respectively. Thus $q(X)$ acts on $(a,b,c)$ as $(q(0)a,q(i)b,q(-i)c)$, making $\Phi$ a [module homomorphism](../../../module-theory.md#module-homomorphism).

The inverse, obtained by [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial), is

$$
\boxed{\Phi^{-1}(a,b,c)=\left[a(1+X^2)-\frac b2(X^2+iX)-\frac c2(X^2-iX)\right].}
$$

Evaluating at $0,i,-i$ recovers $(a,b,c)$. Conversely, a polynomial whose three evaluations vanish is divisible by $X(X-i)(X+i)$, so these maps are mutual inverses on the [quotient module](../../../module-theory.md#quotient-module). Three copies with identical trivial $X$-action would not give the required isomorphism.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

Fix $(x,y)\in U$ and a sufficiently small rectangle inside $U$. Its rectangular increment

$$
\Delta=f(x+h,y+k)-f(x+h,y)-f(x,y+k)+f(x,y)
$$

can be evaluated twice using the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus), giving

$$
\Delta=\int_x^{x+h}\int_y^{y+k}D_2D_1f(s,t)\,dt\,ds
=\int_y^{y+k}\int_x^{x+h}D_1D_2f(s,t)\,ds\,dt.
$$

Divide by $hk$ and let $h,k\to0$. Continuity of the [mixed partial derivatives](../../../calculus.md#mixed-partial-derivative) makes the two limits $D_2D_1f(x,y)$ and $D_1D_2f(x,y)$. **They are equal everywhere on $U$.**

Repeated interchange of adjacent [partial derivatives](../../../calculus.md#partial-derivative) reduces every order-$m$ [derivative](../../../calculus.md#derivative) of a smooth function to $D_1^jD_2^{m-j}f$, $0\leq j\leq m$. Hence there are at most $m+1$ distinct functions. This maximum is attained by $f(x,y)=e^{x+2y}$, whose listed [partial derivatives](../../../calculus.md#partial-derivative) are the distinct functions $2^{m-j}e^{x+2y}$. The answer is **$m+1$**, rather than the $2^m$ possible written orders.

For the supplied $f$, $f(t,t)=1/2$ for $t\ne0$, whereas $f(0,0)=0$. It is not even continuous at the origin, so **$f$ is neither differentiable nor infinitely differentiable there**.

For $g$, $|g(x,y)|\leq|xy|\leq(x^2+y^2)/2$. Thus $g(x,y)=o(\sqrt{x^2+y^2})$, proving [Fréchet differentiability](../../../calculus.md#frechet-differentiability) at the origin with [derivative](../../../calculus.md#derivative) zero. However,

$$
D_1g(0,y)=-y,\qquad D_2g(x,0)=x,
$$

including zero at the origin. Therefore $D_2D_1g(0,0)=-1$ and $D_1D_2g(0,0)=1$. **$g$ is differentiable but not infinitely differentiable at the origin**: it cannot have continuous second [partial derivatives](../../../calculus.md#partial-derivative) near that point.

## 13D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13d/i">i</h3>

↑ **Parent:** [13D](#13d)

<h4 id="13d/i/solution">Solution</h4>

↑ **Parent:** [I](#13d/i)

The denominator vanishes when $z=(2j+1)i\pi/2$. For $R>0$, only $z_0=i\pi/2$ lies inside the rectangle. This is a [simple pole](../../../isolated-singularity.md#simple-pole), since the denominator [derivative](../../../calculus.md#derivative) there is $2$. Its [residue](../../../analysis.md#residue) is

$$
\operatorname{Res}_{z_0}\frac{e^{iz^2/\pi}}{1+e^{-2z}}=\frac12e^{-i\pi/4}.
$$

The positive orientation and the [residue theorem](../../../analysis.md#residue-theorem) consequently give

$$
\boxed{I=2\pi i\left(\tfrac12e^{-i\pi/4}\right)=\frac{\pi(1+i)}{\sqrt2}.}
$$

<h3 id="13d/ii">ii</h3>

↑ **Parent:** [13D](#13d)

<h4 id="13d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#13d/ii)

On the top side put $z=x+i\pi$, with $x$ running from $R$ to $-R$. Since $e^{i(x+i\pi)^2/\pi}=-e^{ix^2/\pi}e^{-2x}$ and $e^{-2(x+i\pi)}=e^{-2x}$, the reversed orientation cancels the minus sign. The two horizontal integrals therefore sum to

$$
\int_{-R}^R e^{ix^2/\pi}\left(\frac1{1+e^{-2x}}+\frac{e^{-2x}}{1+e^{-2x}}\right)dx
=\int_{-R}^R e^{ix^2/\pi}\,dx.
$$

If the vertical contributions vanish, the previous [residue theorem](../../../analysis.md#residue-theorem) evaluation yields the [Fresnel integral](../../../analysis.md#fresnel-integral)

$$
\boxed{\int_{-\infty}^{\infty}e^{ix^2/\pi}\,dx=\frac{\pi(1+i)}{\sqrt2}.}
$$

This also is an ordinary oscillatory [improper integral](../../../real-analysis.md#improper-integral), not merely a symmetric principal value: [integration by parts](../../../calculus.md#integration-by-parts), using $(e^{ix^2/\pi})'=(2ix/\pi)e^{ix^2/\pi}$, bounds either tail beginning at $R$ by a constant times $1/R$.

<h3 id="13d/iii">iii</h3>

↑ **Parent:** [13D](#13d)

<h4 id="13d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#13d/iii)

For $z=R+iy$, $0\leq y\leq\pi$, the numerator modulus is $e^{-2Ry/\pi}$ and the denominator modulus is at least $1-e^{-2R}$. Hence the magnitude of the right-side [contour integral](../../../complex-analysis.md#contour-integral) is at most

$$
\frac1{1-e^{-2R}}\int_0^\pi e^{-2Ry/\pi}\,dy=\frac\pi{2R}.
$$

On $z=-R+iy$ the corresponding bounds are $e^{2Ry/\pi}$ and $e^{2R}-1$, giving exactly the same bound $\pi/(2R)$. Thus **the total vertical contribution is $O(R^{-1})$ and vanishes**. This integral estimate handles the endpoints where a pointwise uniform-decay argument would fail.

## 14F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14f/solution">Solution</h3>

↑ **Parent:** [14F](#14f)

First normalize the two [circles](../../../topology.md#circle) by translation and rotation so their centres are $0,d$ and radii $a,b$. If $d=0$ nothing further is needed. Otherwise choose real $s,t$ satisfying

$$
st=a^2,\qquad s+t=\frac{d^2+a^2-b^2}{d}.
$$

The discriminant of this quadratic is

$$
\frac{(d^2-(a+b)^2)(d^2-(a-b)^2)}{d^2}>0,
$$

since two disjoint [circle](../../../topology.md#circle) boundaries are either externally separated or strictly nested. Thus $s\ne t$, and $M(z)=(z-s)/(z-t)$ is a [Möbius transformation](../../../group-theory.md#mobius-transformation). Direct expansion shows that on the first [circle](../../../topology.md#circle) $|M(z)|^2=s/t$, and on the second $|M(z)|^2=(s-d)/(t-d)$. Both constants are positive; the pole is on neither [circle](../../../topology.md#circle). Their images are distinct concentric [circles](../../../topology.md#circle). This proves the [concentric normalization of disjoint circles](../../../group-theory.md#concentric-normalization-of-disjoint-circles).

For a construction with $n\geq3$, use inner radius $\rho=1$, outer radius

$$
R=\frac{1+\sin(\pi/n)}{1-\sin(\pi/n)},\qquad r=\frac{R-1}{2},\qquad d=\frac{R+1}{2},
$$

and small [circles](../../../topology.md#circle) of radius $r$ centred at $d e^{2\pi ij/n}$. Each touches the two boundaries, and adjacent centre distances are $2d\sin(\pi/n)=2r$. All other distances are at least $2r$, so there are no unwanted intersections. These are [Steiner chains](../../../topology.md#steiner-chain). For the literal $n=2$ requirement, take $\rho=1$, $R=3$, and two radius-one [circles](../../../topology.md#circle) centred at $2e^{\pm i\pi/6}$. Their centre distance is $2$, so this gives two distinct mutually tangent [circles](../../../topology.md#circle) touching both boundaries. **Existence holds for every $n\geq2$**, but the two-[circle](../../../topology.md#circle) case has only one tangency between neighbours, repeated by the cyclic indexing.

<a id="14f/image-two-mutually-tangent-circles-and-a-five-circle-steiner-chain-between-concentric-boundaries"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2-circle-chains.png)

**[Figure 1](#14f/image-two-mutually-tangent-circles-and-a-five-circle-steiner-chain-between-concentric-boundaries). Two mutually tangent circles and a five-circle Steiner chain between concentric boundaries**.

For an annular [circle](../../../topology.md#circle) touching radii $\rho,R$, its radius and centre distance are $r=(R-\rho)/2$ and $d=(R+\rho)/2$. Two neighbouring such [circles](../../../topology.md#circle) have angular separation $\delta=2\arcsin(r/d)$; their tangency point is the midpoint of their centres. Its distance from the common centre is

$$
d\cos(\delta/2)=\sqrt{d^2-r^2}=\sqrt{R\rho}.
$$

Thus **the tangency locus in concentric coordinates is a [circle](../../../topology.md#circle) of radius $\sqrt{R\rho}$**. For $n\geq3$, disjointness forces the constellation to use these annular [circles](../../../topology.md#circle). Indeed, the other family of [circles](../../../topology.md#circle) touching both boundaries has radius $d$ and centre distance $r$, enclosing the inner boundary. Two members of that larger family intersect. One such [circle](../../../topology.md#circle) can be disjoint from an annular [circle](../../../topology.md#circle) only at the two opposite centre directions where their boundaries are tangent; those two annular [circles](../../../topology.md#circle) cannot be tangent to each other. Hence this family cannot occur in a constellation of three or more [circles](../../../topology.md#circle).

Under the inverse [Möbius transformation](../../../group-theory.md#mobius-transformation), the tangency locus is a [generalized circle](../../../group-theory.md#generalized-circle-under-a-mobius-transformation), which can be an ordinary [circle](../../../topology.md#circle) or a straight line. **The printed claim that it is always an ordinary [circle](../../../topology.md#circle) is false without this qualification.** For an explicit counterexample, use the above $n=3$ construction, put $L=\sqrt R$, and apply $w=1/(z-L)$. Its pole lies on the tangency locus but on none of the original boundary or chain [circles](../../../topology.md#circle). Consequently all the transformed individual [circles](../../../topology.md#circle) remain ordinary [circles](../../../topology.md#circle). The three distinct tangency points transform to three points on the line $\operatorname{Re}w=-1/(2L)$, so they cannot lie on an ordinary [circle](../../../topology.md#circle).

The usual closure assertion is [Steiner's porism](../../../topology.md#steiner-porism), with two essential conventions: stay in the annular family and always choose the next tangent [circle](../../../topology.md#circle) in the same angular direction. For a disjoint closed chain with $n\geq3$, distinctness prevents reversing direction: a reversed step would return immediately to the preceding [circle](../../../topology.md#circle). Thus every step has the same sign and closure gives $n\delta=2\pi m$ for an integer $m\geq1$. If $m>1$, the $n$ distinct centres have some angular gap $2\pi/n<\delta$, making two [circles](../../../topology.md#circle) intersect. Hence $m=1$ and $\delta=2\pi/n$. Starting at any new angle $\theta_0$ produces centres $de^{i(\theta_0+j\delta)}$, a rotation of the original chain, so

$$
\boxed{Y_n=Y_0\quad\text{for the consistently directed annular chain}.}
$$

Mapping back proves the same porism on the corresponding branch of [circles](../../../topology.md#circle) for the original pair.

The literal final request, with arbitrary tangent choices and $n=2$ included, is stronger and false. In the two-[circle](../../../topology.md#circle) example above, the forward angular step is $\pi/3$. Starting at angle $0$, a next [circle](../../../topology.md#circle) at $\pi/3$ and then one at $2\pi/3$ satisfy every inductive tangency requirement, but $Y_2\ne Y_0$. Even for $n\geq3$, allowing backtracking lets the construction reverse instead of completing the chain. Thus the genuine geometric conclusion is the qualified porism, not unrestricted closure under the printed induction.

## 15A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15a/solution">Solution</h3>

↑ **Parent:** [15A](#15a)

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is $f_y-d(f_{y'})/dx=0$. Since $f$ has no explicit $x$ dependence,

$$
\frac d{dx}(f-y'f_{y'})=y'\left(f_y-\frac d{dx}f_{y'}\right)=0.
$$

Thus a stationary curve satisfies the [Beltrami identity](../../../analysis.md#beltrami-identity), $f-y'f_{y'}=C$.

By [Fermat principle](../../../physics.md#fermat-principle), the [light ray](../../../optics.md#light-ray) makes the travel time $\int\sqrt{1+y'^2}/(y+c_0)\,dx$ stationary. Its [Beltrami identity](../../../analysis.md#beltrami-identity) becomes

$$
\frac1{(y+c_0)\sqrt{1+y'^2}}=C>0.
$$

Writing $R=1/C$ and integrating the resulting first-order equation gives $(x-x_0)^2+(y+c_0)^2=R^2$. Both endpoints have height zero, so subtracting their equations gives $x_0=0$, and then $R^2=a^2+c_0^2$. The arc lying in $y>0$ is

$$
\boxed{y(x)=\sqrt{a^2+c_0^2-x^2}-c_0,\qquad -a\leq x\leq a.}
$$

Its maximum height is $\sqrt{a^2+c_0^2}-c_0$. The ray rises into the faster region before returning to the boundary; its [circle](../../../topology.md#circle) centre is $(0,-c_0)$. The prescribed boundary endpoints are understood by continuity from the open half-plane. This is the [circular light ray in a linear speed profile](../../../optics.md#circular-light-ray-in-a-linear-speed-profile).

<a id="15a/image-circular-light-ray-arching-into-a-region-where-propagation-speed-increases-with-height"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2-light-ray.png)

**[Figure 2](#15a/image-circular-light-ray-arching-into-a-region-where-propagation-speed-increases-with-height). Circular light ray arching into a region where propagation speed increases with height**.

## 16B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16b/solution">Solution</h3>

↑ **Parent:** [16B](#16b)

For the [Dirichlet Green's function](../../../analysis.md#dirichlet-green-function), solve $-DG_{xx}=\delta(x-\xi)$ with zero endpoint values. Away from $\xi$, $G$ is linear. Continuity at $\xi$ and the [derivative](../../../calculus.md#derivative) jump $G_x(\xi+,\xi)-G_x(\xi-,\xi)=-1/D$ give

$$
\boxed{G(x,\xi)=\begin{cases}\dfrac{x(l-\xi)}{Dl},&x\leq\xi,\\[4pt]\dfrac{\xi(l-x)}{Dl},&x\geq\xi.\end{cases}}
$$

For nonzero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), subtract their linear interpolant. The resulting [boundary value problem](../../../differential-equation.md#boundary-value-problem) has solution

$$
\boxed{u(x)=\alpha+\frac{\beta-\alpha}{l}x+\int_0^lG(x,\xi)f(\xi)\,d\xi.}
$$

In the final [heat equation](../../../diffusion-equation.md#heat-equation), a [steady state](../../../dynamical-systems.md#steady-state) has zero time [derivative](../../../calculus.md#derivative). Here $l=1$, $f(x)=x$, $\alpha=1/D$, $\beta=2/D$. Integrating $u''=-x/D$ twice and imposing the endpoint values gives

$$
\boxed{u_{\mathrm{steady}}(x)=\frac1D\left(1+\frac76x-\frac16x^3\right).}
$$

Its second [derivative](../../../calculus.md#derivative) and both [boundary conditions](../../../differential-equation.md#boundary-condition) verify the answer directly.

## 17B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17b/i">i</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/i/solution">Solution</h4>

↑ **Parent:** [I](#17b/i)

The time-independent [Schrödinger equation](../../../physics.md#schrodinger-equation) gives the even interior [wavefunction](../../../quantum-mechanics.md#wave-function) $\psi=A\cos(\alpha x)$, with $\alpha^2=2m(U+E)/\hbar^2$. Outside, normalizability of a [bound state](../../../quantum-mechanics.md#bound-state) requires $\psi=C e^{-\beta(|x|-l)}$, with $\beta^2=-2mE/\hbar^2$.

Continuity of the [wavefunction](../../../quantum-mechanics.md#wave-function) and its [derivative](../../../calculus.md#derivative) at $x=l$ gives $C=A\cos(\alpha l)$ and $-\beta C=-\alpha A\sin(\alpha l)$. A nonzero solution cannot have $\cos(\alpha l)=0$, so division gives

$$
\boxed{\alpha\tan(\alpha l)=\beta.}
$$

At the formally allowed endpoint $E=-U$, the even interior solution is constant; [derivative](../../../calculus.md#derivative) matching would force the exterior amplitude to vanish, leaving the zero solution. Nontrivial [bound states](../../../quantum-mechanics.md#bound-state) therefore have $-U<E<0$. The matching formula is the even-state condition for a [finite square well](../../../quantum-mechanics.md#finite-square-well).

<h3 id="17b/ii">ii</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#17b/ii)

Put $p=\sqrt{2mE}/\hbar$ and $\gamma=mk/\hbar^2$. Integrating the [Schrödinger equation](../../../physics.md#schrodinger-equation) across the [delta potential](../../../quantum-mechanics.md#delta-potential) gives continuity of $\psi$ and

$$
\psi'(0+)-\psi'(0-)=2\gamma\psi(0).
$$

For incidence from the left, write $\psi=e^{ipx}+r e^{-ipx}$ on $x<0$ and $\psi=t e^{ipx}$ on $x>0$. Matching gives $t=1+r$ and $ip(t-1+r)=2\gamma t$, hence

$$
r=-\frac{i\gamma}{p+i\gamma},\qquad t=\frac p{p+i\gamma}.
$$

The incident and transmitted [probability currents](../../../quantum-mechanics.md#probability-current) have the same velocity factor, so the [reflection coefficient](../../../partial-differential-equation.md#reflection-coefficient) and [transmission coefficient](../../../partial-differential-equation.md#transmission-coefficient) are

$$
\boxed{R=\frac{\gamma^2}{p^2+\gamma^2},\qquad T=\frac{p^2}{p^2+\gamma^2},\qquad R+T=1.}
$$

For $k<0$, an even [bound state](../../../quantum-mechanics.md#bound-state) has $\psi=Ae^{-\kappa|x|}$, $\kappa=\sqrt{-2mE}/\hbar$. The [derivative](../../../calculus.md#derivative) jump now gives $-2\kappa A=2\gamma A$, so $\kappa=-\gamma>0$ and

$$
\boxed{E=-\frac{mk^2}{2\hbar^2}.}
$$

There is exactly one positive value of $\kappa$, hence exactly one even [bound state](../../../quantum-mechanics.md#bound-state). Its normalized amplitude is $A=\sqrt\kappa$. An odd decaying solution would have to vanish at zero and is therefore trivial.

In the shrinking [finite square well](../../../quantum-mechanics.md#finite-square-well), its integrated potential is $k=-2Ul$, not $-Ul$: the full width is $2l$. With $Ul$ fixed and $l\to0$, $0\leq(\alpha l)^2\leq2mUl^2/\hbar^2\to0$. The matching condition then bounds $\beta$ by $(2mUl/\hbar^2)(1+o(1))$, so $E$ remains bounded. Consequently $El\to0$, and the previous matching condition gives

$$
\beta=\alpha\tan(\alpha l)\sim\alpha^2l=\frac{2m(U+E)l}{\hbar^2}\longrightarrow-\frac{mk}{\hbar^2}.
$$

Using $E=-\hbar^2\beta^2/(2m)$ recovers the same bound-state energy. All other even levels disappear as the width shrinks.

## 18D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18d/solution">Solution</h3>

↑ **Parent:** [18D](#18d)

For a thin wire carrying current $I$, the given [magnetic vector potential](../../../electromagnetism.md#magnetic-vector-potential) reduces to $\mathbf A=(\mu_0I/4\pi)\oint_Cd\mathbf r'/|\mathbf r-\mathbf r'|$. Taking its [curl](../../../calculus.md#curl) and using $\nabla_{\mathbf r}(1/|\mathbf r-\mathbf r'|)=-(\mathbf r-\mathbf r')/|\mathbf r-\mathbf r'|^3$ gives the [Biot-Savart law](../../../electromagnetism.md#biot-savart-law)

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0I}{4\pi}\oint_C\frac{d\mathbf r'\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}.}
$$

This is exactly the sign convention in the printed form using $\mathbf r'-\mathbf r$.

Let $\mathbf v=(\mathbf r-\mathbf r')/|\mathbf r-\mathbf r'|^3$. Away from the wire, $\nabla\cdot\mathbf v=0$. The supplied [divergence and curl of a cross product](../../../calculus.md#divergence-and-curl-of-a-cross-product) therefore gives $\nabla\times(d\mathbf r'\times\mathbf v)=-(d\mathbf r'\cdot\nabla_{\mathbf r})\mathbf v$. But $\nabla_{\mathbf r}\mathbf v=-\nabla_{\mathbf r'}\mathbf v$, so the integrand is the total differential of $\mathbf v$ along the source loop. Its closed-loop integral is zero. Thus **$\nabla\times\mathbf B=0$ at every point outside $C$**, as demanded by the current-free magnetostatic [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law).

For $r'=f(\theta)>0$, $z'=0$, and counterclockwise current, $d\mathbf r'=(f'\mathbf e_r+f\mathbf e_\theta)d\theta$. At the origin, $\mathbf v=-\mathbf e_r/f^2$, so

$$
\boxed{\mathbf B(0)=\widehat{\mathbf z}\,\frac{\mu_0I}{4\pi}\int_0^{2\pi}\frac{d\theta}{f(\theta)}.}
$$

For the [ellipse](../../../geometry-and-topology.md#ellipse) expressed relative to a focus, $1/f=(1-e\cos\theta)/\ell$. The cosine integrates to zero, giving

$$
\boxed{\mathbf B_{\mathrm{focus}}=\widehat{\mathbf z}\,\frac{\mu_0I}{2\ell}.}
$$

Here $\ell$ is the [semilatus rectum](../../../geometry-and-topology.md#semilatus-rectum). Reversing the current reverses the field direction.

## 19C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19c/solution">Solution</h3>

↑ **Parent:** [19C](#19c)

[Convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) on $[0,T]$ means that its grid error obeys $\max_{0\leq nh\leq T}|y_n-y(nh)|\to0$ as $h\to0$, with consistent initial values.

First, the implicit step of [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) is well-defined for $hL<1$: the map $z\mapsto y_n+hf(t_{n+1},z)$ is a [contraction mapping](../../../analysis.md#contraction-mapping) on $\mathbb R$, so the [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) gives a unique solution. Let $M=\max_{[0,T]}|y''|$, finite under the stated smoothness. The exact solution's step defect is

$$
d_n=y(t_{n+1})-y(t_n)-hy'(t_{n+1})=\int_{t_n}^{t_{n+1}}[y'(s)-y'(t_{n+1})]ds,
$$

so $|d_n|\leq Mh^2/2$. Subtract the exact and numerical step equations. The [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity) gives

$$
|e_{n+1}|\leq\frac{|e_n|+Mh^2/2}{1-hL},\qquad e_n=y_n-y(t_n).
$$

With exact initial data, sum this [geometric progression](../../../real-analysis.md#geometric-progression) to obtain

$$
|e_n|\leq\frac{Mh}{2L}\big[(1-hL)^{-n}-1\big].
$$

For $hL\leq1/2$ and $nh\leq T$, $-\log(1-hL)\leq2hL$, so the bracket is at most $e^{2LT}-1$. Thus **the global error is $O(h)$, uniformly on $[0,T]$, and [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) converges with order one**. A vanishing initial error adds only $(1-hL)^{-n}|e_0|$.

Order one is sharp: for $y'=y$, $y(0)=1$ and $nh=T$, $y_n=(1-h)^{-n}=e^T(1+Th/2+O(h^2))$.

For the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$, the [stability function](../../../numerical-analysis.md#stability-function) is $R(z)=1/(1-z)$, $z=h\lambda$. Therefore its [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) is

$$
\boxed{\{z\in\mathbb C:|1-z|\geq1\}.}
$$

The strict inequality gives decay; equality gives bounded amplification. The whole closed left half-plane lies in this region, so [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) is [A-stable](../../../numerical-analysis.md#a-stability).

## 20H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="20h/i">i</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/i/solution">Solution</h4>

↑ **Parent:** [I](#20h/i)

Let $T_j=\inf\{n\geq1:X_n=j\}$. By the [Strong Markov property](../../../markov-process.md#strong-markov-property), the probability of hitting $j$ and subsequently returning to $i$ is $f_{ij}f_{ji}$. This event implies a return to $i$, so **$f_{ii}\geq f_{ij}f_{ji}$**. For $i=j$, interpret the event as two successive returns.

Set $T_i^{(0)}=0$ and let $T_i^{(r)}$ be the $r$th successive return. Repeated use of the [Strong Markov property](../../../markov-process.md#strong-markov-property) gives $\mathbb P_i(T_i^{(r)}<\infty)=f_{ii}^r$. The total number $N_i$ of visits, including time zero, is both $\sum_{n\geq0}\mathbf1_{\{X_n=i\}}$ and $\sum_{r\geq0}\mathbf1_{\{T_i^{(r)}<\infty\}}$. By [Tonelli theorem](../../../measure-theory.md#tonelli-theorem),

$$
\boxed{\sum_{n=0}^\infty\mathbb P_i(X_n=i)=\mathbb E_iN_i=\sum_{r=0}^\infty f_{ii}^r.}
$$

The identity is valid with value $+\infty$. In particular, divergence of the return-probability sum is equivalent to [Markov-chain recurrence](../../../markov-process.md#recurrent-markov-chain).

<h3 id="20h/ii">ii</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#20h/ii)

For a planar [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) write its coordinates as $(S_n,T_n)$ and rotate to $(S_n+T_n,S_n-T_n)$. Each step now has four equally likely values $(1,1),(1,-1),(-1,1),(-1,-1)$. Thus the two rotated coordinates are independent one-dimensional [simple symmetric random walks](../../../probability-theory.md#simple-symmetric-random-walk).

A return is impossible at odd times, and at time $2n$ its probability is

$$
p_{2n}(0,0)=\left(2^{-2n}\binom{2n}{n}\right)^2.
$$

For $n\geq2$, the supplied estimate gives $1/(4n)<p_{2n}(0,0)<1/n$. At $n=1$ the lower bound is actually equality, $p_2(0,0)=1/4$; this harmless strict-endpoint typo does not affect the argument. The [harmonic series](../../../real-analysis.md#harmonic-series) diverges, so the criterion proved above shows that the origin is recurrent, in the terminology of a [recurrent Markov chain](../../../markov-process.md#recurrent-markov-chain). Translation invariance gives the same conclusion for every state. The [Markov chain](../../../markov-process.md#markov-chain) is [irreducible](../../../representation-theory.md#irreducible-representation), so from any starting point it hits any fixed state almost surely and revisits it infinitely often. One can see the hitting assertion directly: repeated returns to the starting point give repeated positive-probability opportunities to follow a finite path to the target.

<h3 id="20h/iii">iii</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#20h/iii)

For an active monster, independence gives

$$
\mathbb P(\text{capture})\leq\sum_{n\geq0}\mathbb P_{(100,0)}(X_n=0)\mathbb P_{(0,100)}(Y_n=0).
$$

Both probabilities vanish before time $100$ and at odd times. By convolution and [Cauchy-Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $p_{2m}(a,0)\leq p_{2m}(0,0)<1/m$: indeed, write the $2m$-step probability as the inner product of two translates of the $m$-step probability mass function. Therefore

$$
\boxed{0<\mathbb P(\text{active capture})\leq\sum_{m\geq50}\frac1{m^2}<\frac1{49}<1.}
$$

Positivity follows by prescribing $100$ simultaneous steps taking both walkers straight to the origin; that event has probability $4^{-200}$. An active monster thus leaves a positive escape probability.

For a sleepy monster, the [origin capture by a sufficiently sleepy planar random walk](../../../probability-theory.md#origin-capture-by-a-sufficiently-sleepy-planar-random-walk) can be proved using the printed schedule: during $I_j=\{n_j+1,\ldots,n_{j+1}\}$ it occupies $Y_{j+1}$. For any $M$, let $J_M$ be the first $j\geq M$ with $Y_{j+1}=0$. [Markov-chain recurrence](../../../markov-process.md#recurrent-markov-chain) of $Y$ makes $J_M$ finite almost surely, and it is independent of $X$. By conditioning on $J_M$ and using the stated block bound,

$$
\mathbb P(\text{some capture in a block }j\geq M)\geq\mathbb P(X\text{ visits }0\text{ in }I_{J_M})>\tfrac12.
$$

As $M\to\infty$, continuity of probability for decreasing events shows that the event $C_\infty$ of infinitely many simultaneous origin visits has probability at least $1/2$. Regard the independent trajectories as continuing even after a possible first capture.

To turn this into probability one, use the [eventual coupling of planar symmetric random walks](../../../probability-and-statistics.md#eventual-coupling-of-planar-symmetric-random-walks); the block events need not be independent. Two planar [simple symmetric random walks](../../../probability-theory.md#simple-symmetric-random-walk) begun at sites of the same parity can be coupled to agree eventually. Run them independently until they meet. Their difference walk is [irreducible](../../../representation-theory.md#irreducible-representation) on the even-parity sublattice, and its $m$-step return probability is $p_{2m}(0,0)$, by convolution and symmetry. The preceding divergent-series criterion makes this difference walk a [recurrent Markov chain](../../../markov-process.md#recurrent-markov-chain), so it hits zero almost surely. After that [stopping time](../../../martingale.md#stopping-time), use identical increments for both copies, preserving their marginal laws by the [Strong Markov property](../../../markov-process.md#strong-markov-property).

Fix any finite calendar time $N$ and any two possible histories up to that time. Corresponding princess positions have the same parity, as do the corresponding monster positions at its internal walk time. Apply the eventual [probabilistic coupling](../../../probability-and-statistics.md#coupling) separately to the two princess futures and the two monster futures, keeping the princess and monster walks independent in each pair. Both the calendar clock and the monster's internal clock tend to infinity. Hence after a finite calendar time the two pairs of trajectories agree, so either both realize $C_\infty$ or neither does. The conditional probability of $C_\infty$ is therefore the same for every possible finite history.

Consequently $\mathbb E(\mathbf1_{C_\infty}\mid\mathcal F_N)=\mathbb P(C_\infty)$ for every $N$. By the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem), these conditional expectations converge to $\mathbf1_{C_\infty}$ as the histories exhaust the trajectories. Thus $\mathbb P(C_\infty)$ is zero or one. Since it is at least $1/2$, it is one. In particular,

$$
\boxed{\mathbb P(\text{sleepy capture})=1.}
$$

This argument uses the supplied unconditional block probabilities; it does not silently strengthen them to conditional probabilities given past failures.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
