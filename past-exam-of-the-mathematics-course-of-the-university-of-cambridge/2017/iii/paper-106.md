# Paper 106

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_106.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_106.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 106](paper-106.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) for [bounded linear functionals](../../../topological-vector-space.md#continuous-linear-functional) says that a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) on any [linear subspace](../../../vector-space.md#vector-subspace) of a [normed vector space](../../../functional-analysis.md#normed-vector-space) extends to the whole space with its [norm](../../../functional-analysis.md#norm) unchanged. No closedness or completeness of the subspace is required. Question 1 uses real-valued $\ell_\infty(\Gamma)$, so its operator assertions are read over the real scalar field. The analogous complex statements use complex-valued indexed functions.

For $x\ne0$, define $g(tx)=t\|x\|$ on its one-dimensional span. This is a norm-one functional, so [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) supplies an extension $f\in X^*$ with

$$
\boxed{\|f\|=1,\qquad f(x)=\|x\|.}
$$

The [canonical embedding into the bidual](../../../functional-analysis.md#canonical-embedding-into-the-bidual) is $Jx(f)=f(x)$. It is linear and $\|Jx\|\le\|x\|$. The [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) just constructed gives the reverse inequality for nonzero $x$, and the zero case is immediate. Thus $\boxed{\|Jx\|=\|x\|}$ and $J$ is injective.

For the [coordinate functional representation of an operator into bounded indexed functions](../../../banach-space.md#coordinate-functional-representation-of-an-operator-into-bounded-indexed-functions), let $e_\gamma$ evaluate a coordinate and put $f_\gamma=e_\gamma T$. If $T$ is bounded and linear, then $f_\gamma\in X^*$ and $\|f_\gamma\|\le\|T\|$. Conversely, if $M=\sup_\gamma\|f_\gamma\|<\infty$, the formula $(Tx)(\gamma)=f_\gamma(x)$ defines a bounded scalar function for each $x$, is linear, and satisfies $\|Tx\|_\infty\le M\|x\|$. Combining the two estimates gives

$$
\boxed{T\in\mathcal B(X,\ell_\infty(\Gamma))\iff\sup_\gamma\|f_\gamma\|<\infty,
\qquad\|T\|=\sup_\gamma\|f_\gamma\|.}
$$

For an empty index set both spaces/families have [norm](../../../functional-analysis.md#norm) bound zero; the [supremum](../../../real-analysis.md#supremum) of the empty nonnegative family is taken as zero.

Choose $\Gamma=B_{X^*}$ and $Tx=(f(x))_{f\in B_{X^*}}$. The [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) makes $\|Tx\|_\infty=\|x\|$, so this is a linear [isometric embedding](../../../riemannian-geometry.md#isometric-embedding) into [bounded scalar functions on an index set](../../../banach-space.md#bounded-scalar-functions-on-an-index-set).

If $X$ is nonzero and separable, choose a dense sequence $u_n$ in its unit sphere and supporting functionals $f_n$ with $\|f_n\|=f_n(u_n)=1$. For a unit vector $u$ and $\epsilon>0$, some $u_n$ satisfies $\|u-u_n\|<\epsilon$, whence $|f_n(u)|\ge1-\epsilon$. Thus $(f_n)$ is a [countable norming family](../../../functional-analysis.md#countable-norming-family) and $x\mapsto(f_n(x))$ is an [isometry](../../../riemannian-geometry.md#isometry) into the [l-infinity sequence space](../../../banach-space.md#l-infinity-sequence-space). Completeness of $X$ is not needed.

If instead $X=E^*$ for a separable [normed vector space](../../../functional-analysis.md#normed-vector-space) $E$, choose a dense sequence $v_n$ in $B_E$. The evaluations $f_n(x)=x(v_n)$ lie in $B_{X^*}$ and continuity of $x\in E^*$ gives $\sup_n|x(v_n)|=\|x\|$. This again gives $\Gamma=\mathbb N$, even when $E^*$ is not separable. If $X=\{0\}$, use zero coordinates throughout.

To prove 1-injectivity, take $T:Y\to\ell_\infty(\Gamma)$ on a subspace of $Z$. Extend every coordinate $f_\gamma\in Y^*$ to $\widetilde f_\gamma\in Z^*$ by [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem), keeping its [norm](../../../functional-analysis.md#norm). Their uniform bound defines $\widetilde Tz=(\widetilde f_\gamma(z))$, and the coordinate [norm](../../../functional-analysis.md#norm) identity yields

$$
\boxed{\widetilde T|_Y=T,\qquad\|\widetilde T\|=\|T\|.}
$$

Selection of these extensions uses the usual choice convention for arbitrary index sets. This verifies the [lambda-injective normed space](../../../functional-analysis.md#lambda-injective-normed-space) definition with $\lambda=1$.

For the final [retraction characterization of lambda-injectivity](../../../functional-analysis.md#retraction-characterization-of-lambda-injectivity), suppose first that $X$ is lambda-injective and $i:X\to Z$ is a linear [isometry](../../../riemannian-geometry.md#isometry). The inverse $i(X)\to X$ has [norm](../../../functional-analysis.md#norm) one when $X\ne0$; extend it to $P:Z\to X$ with $\|P\|\le\lambda$. Then $Pi=I_X$, and $iP$ is a bounded projection onto $i(X)$. For the zero space take $P=0$.

Conversely, suppose every linear [isometry](../../../riemannian-geometry.md#isometry) out of $X$ has such a left inverse. Fix an [isometry](../../../riemannian-geometry.md#isometry) $j:X\to\ell_\infty(\Gamma)$ as above and a left inverse $P$ with $\|P\|\le\lambda$. For any $T:Y\to X$, extend $jT$ to $S:Z\to\ell_\infty(\Gamma)$ by 1-injectivity. Then $\widetilde T=PS$ extends $T$, and $\|\widetilde T\|\le\lambda\|S\|=\lambda\|T\|$. Therefore $X$ is lambda-injective exactly when every isometric embedding $i:X\to Z$ admits a bounded map $P:Z\to X$ satisfying

$$
\boxed{Pi=I_X,\qquad\|P\|\le\lambda.}
$$

## 2

↑ **Parent:** [Paper 106](paper-106.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [weak topology](../../../weak-topology.md) $\sigma(X,X^*)$ is the coarsest topology making every [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) continuous. A neighbourhood basis at $x$ consists of sets $\{y:|f_j(y-x)|<\epsilon,\ 1\le j\le m\}$ for finite families in $X^*$.

[Mazur theorem](../../../hilbert-space.md#mazur-theorem) says that for any [convex](../../../real-analysis.md#convex-function) subset $C$ of a real or complex [normed vector space](../../../functional-analysis.md#normed-vector-space),

$$
\boxed{\overline C^{\,w}=\overline C^{\,\|\cdot\|}.}
$$

The [norm](../../../functional-analysis.md#norm) closure is [convex](../../../real-analysis.md#convex-function). If $x$ is outside it, the [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) gives a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $f$ and a real $a$ with $\operatorname{Re}f(x)>a\ge\sup_{y\in C}\operatorname{Re}f(y)$. In the real case omit the real part. Thus $x$ has a weak neighbourhood missing $C$, proving that the weak closure lies in the [norm](../../../functional-analysis.md#norm) closure. The other inclusion follows because the weak topology is weaker than the [norm](../../../functional-analysis.md#norm) topology. In the complex case real separation is converted to a complex functional by $f(z)=h(z)-ih(iz)$.

The sequential formulation, [Mazur lemma](../../../hilbert-space.md#mazur-s-lemma), follows as well. If $x_n\rightharpoonup x$, then $x$ lies in the weak closure of each tail and hence in the [norm](../../../functional-analysis.md#norm) closure of its [convex hull](../../../mathematical-optimization.md#convex-hull). Select a finite [convex](../../../real-analysis.md#convex-function) combination of the $n$th tail at [norm](../../../functional-analysis.md#norm) distance less than $1/n$ from $x$.

A [weakly bounded set](../../../weak-topology.md#weakly-bounded-set) $D$ satisfies $\sup_{x\in D}|f(x)|<\infty$ for every $f\in X^*$. Regard $J(D)$ as a pointwise bounded family of functionals on $X^*$. The [completeness of the dual space](../../../continuous-dual-space.md#completeness-of-the-dual-space) holds even if $X$ is incomplete: a norm-Cauchy sequence of functionals has a pointwise bounded linear limit and then converges uniformly on the [unit ball](../../../functional-analysis.md#unit-ball). The [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) therefore gives $\sup_{x\in D}\|Jx\|<\infty$, and $\|Jx\|=\|x\|$ proves [norm](../../../functional-analysis.md#norm) boundedness.

One can see the precise Baire argument here. The closed sets $F_n=\{f\in X^*:\sup_{x\in D}|f(x)|\le n\}$ cover the [Banach space](../../../banach-space.md) $X^*$. The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) makes some $F_n$ contain a ball $f_0+rB_{X^*}$, after shrinking the radius. For $\|g\|\le r$, both $f_0$ and $f_0+g$ lie in $F_n$, so $\sup_D|g(x)|\le2n$. Scaling and the dual [norm](../../../functional-analysis.md#norm) formula yield $\sup_D\|x\|\le2n/r$. A [weakly compact set](../../../weak-topology.md#weakly-compact-set) is weakly bounded because each functional has compact, hence bounded, image. Consequently it is [norm](../../../functional-analysis.md#norm) bounded.

For a [Banach space](../../../banach-space.md), let $J:X\to X^{**}$ be its canonical [isometry](../../../riemannian-geometry.md#isometry). We use two explicitly stated weak-star facts: [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) makes a dual [unit ball](../../../functional-analysis.md#unit-ball) weak-star compact, and [Goldstine theorem](../../../functional-analysis.md#goldstine-theorem) makes $J(B_X)$ weak-star dense in $B_{X^{**}}$. The weak topology on $X$ is carried by $J$ to $\sigma(X^{**},X^*)$ on its image, since their coordinates are the same evaluations $f(x)$.

If $X$ is a [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space), $J(B_X)=B_{X^{**}}$ and Banach-Alaoglu proves weak compactness. Conversely, if $B_X$ is weakly compact, its image is weak-star compact and hence closed in the [Hausdorff space](../../../topology.md#hausdorff-space) $X^{**}$. Goldstine density then forces $J(B_X)=B_{X^{**}}$, which implies $JX=X^{**}$. This proves the [weak compactness characterization of reflexivity](../../../functional-analysis.md#weak-compactness-characterization-of-reflexivity):

$$
\boxed{X\text{ is reflexive}\iff B_X\text{ is weakly compact}.}
$$

Finally let $K\subset X$ be weakly compact and let $(f_n)\subset B_{X^*}$ separate points. If $K$ is empty there is nothing to prove; otherwise define

$$
\boxed{d(x,y)=\sum_{n=1}^\infty 2^{-n}\frac{|f_n(x-y)|}{1+|f_n(x-y)|}.}
$$

The summands are bounded by $2^{-n}$ and separation makes $d(x,y)=0$ only for $x=y$. The coordinate maps are weakly continuous, so the series, being uniformly convergent, makes the identity from weak $K$ to metric $K$ continuous. A continuous bijection from a compact space to a [Hausdorff space](../../../topology.md#hausdorff-space) is a [homeomorphism](../../../topology.md#homeomorphism). Thus $d$ induces precisely the weak topology on $K$, the [countable separating family metrizes a weakly compact set](../../../weak-topology.md#countable-separating-family-metrizes-a-weakly-compact-set) result. No norm-density of the separating family in $X^*$ is claimed or required.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

For each $t\in[0,1]$, evaluation $\delta_t:f\mapsto f(t)$ is a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) of [norm](../../../functional-analysis.md#norm) one. Thus [weak convergence](../../../weak-topology.md#weak-convergence) to zero gives $f_n(t)\to0$ at every $t$. The set $\{f_n:n\ge1\}$ is a [weakly bounded set](../../../weak-topology.md#weakly-bounded-set), since every scalar sequence $\ell(f_n)$ converges, and part (a) supplies a uniform bound $\|f_n\|_\infty\le M$.

The constant $M$ is integrable for [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) on $[0,1]$. Applying the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) to $|f_n|$ gives the [weakly null continuous functions converge in L1](../../../functional-analysis.md#weakly-null-continuous-functions-converge-in-l1) conclusion

$$
\boxed{\|f_n\|_{L^1[0,1]}=\int_0^1|f_n(t)|\,dt\longrightarrow0.}
$$

Pointwise convergence alone would not provide the needed uniform dominating function; it is the weak boundedness argument that supplies it.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Put $d=\inf\{\|x\|:x\in C\}$. The nonemptiness of $C$ gives $0\le d<\infty$. By [Mazur theorem](../../../hilbert-space.md#mazur-theorem), a norm-closed [convex](../../../real-analysis.md#convex-function) set is weakly closed. This applies to both $C$ and every closed [norm](../../../functional-analysis.md#norm) ball.

For $n\ge1$, the sets $C_n=C\cap(d+1/n)B_X$ are nonempty by the definition of the [infimum](../../../real-analysis.md#infimum), weakly closed and nested. They all lie in the [weakly compact set](../../../weak-topology.md#weakly-compact-set) $(d+1)B_X$, by the [weak compactness characterization of reflexivity](../../../functional-analysis.md#weak-compactness-characterization-of-reflexivity). Hence they have the [finite intersection property](../../../topology.md#finite-intersection-property), and compactness gives $x_0\in\bigcap_n C_n$. Then $x_0\in C$ and $\|x_0\|\le d+1/n$ for every $n$, so

$$
\boxed{x_0\in C,\qquad\|x_0\|=\min_{x\in C}\|x\|=d.}
$$

This proves the [norm minimizer in a closed convex subset of a reflexive Banach space](../../../functional-analysis.md#norm-minimizer-in-a-closed-convex-subset-of-a-reflexive-banach-space) assertion without assuming sequential weak compactness. It includes $d=0$; uniqueness is not asserted without an additional condition such as strict convexity of the [norm](../../../functional-analysis.md#norm).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The coordinate evaluations $e_n:x\mapsto x_n$ belong to the dual [unit ball](../../../functional-analysis.md#unit-ball) of the [l-infinity sequence space](../../../banach-space.md#l-infinity-sequence-space) and separate its points. Therefore the [countable separating family metrizes a weakly compact set](../../../weak-topology.md#countable-separating-family-metrizes-a-weakly-compact-set) result makes any nonempty weakly compact $K\subset\ell_\infty$ a compact [metric space](../../../topological-analysis.md#metric-space) in its weak topology. Choose finite $1/n$-nets and take their countable union $D$; it is weakly dense in $K$.

It follows that $K\subset\overline D^{\,w}\subset\overline{\operatorname{conv}D}^{\,w}$. By [Mazur theorem](../../../hilbert-space.md#mazur-theorem), the last set is $\overline{\operatorname{conv}D}^{\,\|\cdot\|}$. Finite [convex](../../../real-analysis.md#convex-function) combinations of members of $D$ with nonnegative rational coefficients summing to one form a countable norm-dense subset of $\operatorname{conv}D$: for each fixed finite list, approximate its coefficients in the simplex by rational coefficients, and use the [norm](../../../functional-analysis.md#norm) triangle inequality. Thus its [norm](../../../functional-analysis.md#norm) closure is a separable [metric space](../../../topological-analysis.md#metric-space) containing $K$.

Every subset of a separable [metric space](../../../topological-analysis.md#metric-space) is separable: balls centred on a countable dense set with positive rational radii form a countable base; intersect this base with the subset and choose one point from each nonempty intersection. Consequently the [weakly compact subsets of l-infinity are norm separable](../../../weak-topology.md#weakly-compact-subsets-of-l-infinity-are-norm-separable) conclusion is

$$
\boxed{K\text{ is separable for the supremum norm}.}
$$

The empty case is immediate. The convexification matters: the chosen weakly dense set $D$ itself need not be [norm](../../../functional-analysis.md#norm) dense in a nonconvex $K$.

## 3

↑ **Parent:** [Paper 106](paper-106.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [weak-star topology](../../../weak-topology.md#weak-star-topology) $\sigma(X^*,X)$ is the coarsest topology making $f\mapsto f(x)$ continuous for every $x\in X$. Its basic neighbourhoods of zero impose finitely many inequalities $|f(x_j)|<\epsilon$.

Suppose first that zero had a countable neighbourhood base $(U_n)$ in the entire dual. Choose a basic neighbourhood $V_n\subset U_n$ controlled by a finite set $F_n\subset X$, and let $E_n=\operatorname{span}(F_1\cup\cdots\cup F_n)$. Given $x\in X$, the neighbourhood $W_x=\{f:|f(x)|<1\}$ contains some $U_n$, hence $V_n$. If $x\notin\operatorname{span}F_n$, the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) supplies a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $h$ which vanishes on $F_n$ but has $h(x)\ne0$. Indeed, the finite-dimensional span is closed, and the functional taking $e+tx$ to $t$ on its sum with $\mathbb F x$ is bounded because $\operatorname{dist}(x,\operatorname{span}F_n)>0$. Every scalar multiple of $h$ lies in $V_n$, contradicting $V_n\subset W_x$. Thus $x\in E_n$, and $X=\bigcup_n E_n$ has countable Hamel dimension.

If $X$ is infinite-dimensional, every finite-dimensional $E_n$ is closed and has empty interior. Completeness rules out their union. For clarity, the [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) needed here has a direct nested-ball proof: inside a starting open ball choose a closed ball missing $E_1$, then inside its interior choose a closed ball missing $E_2$, and continue with positive radii tending to zero. The centres are Cauchy; their limit belongs to every ball and to none of the $E_n$, a contradiction. A metric topology would have a countable ball base at zero. Hence

$$
\boxed{\sigma(X^*,X)\text{ is not metrizable on }X^*.}
$$

This is the [weak-star topology on an entire infinite-dimensional Banach dual is not metrizable](../../../weak-topology.md#weak-star-topology-on-an-entire-infinite-dimensional-banach-dual-is-not-metrizable) result. It does not contradict [weak-star metrizability of the dual ball](../../../weak-topology.md#weak-star-metrizability-of-the-dual-ball) for a separable predual: that assertion concerns a bounded subset.

The [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) states that $B_{X^*}$ is compact for $\sigma(X^*,X)$ for every [normed vector space](../../../functional-analysis.md#normed-vector-space) $X$, whether complete or not. Embed it in the product $\prod_{x\in X}\{a\in\mathbb F:|a|\le\|x\|\}$ by its evaluations. Each factor is compact, so [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem) makes the product compact Hausdorff. The equations expressing additivity and scalar homogeneity define a closed subset of the product. Its elements are exactly the bounded linear functionals of [norm](../../../functional-analysis.md#norm) at most one, since the coordinate bounds give $|f(x)|\le\|x\|$. The induced product topology is precisely weak-star, proving the theorem.

The theorem printed as “Goldstein” is the standard [Goldstine theorem](../../../functional-analysis.md#goldstine-theorem): $J(B_X)$ is weak-star dense in $B_{X^{**}}$ for the [canonical embedding into the bidual](../../../functional-analysis.md#canonical-embedding-into-the-bidual). To prove it, fix $\Phi\in B_{X^{**}}$ and $f_1,\ldots,f_m\in X^*$. The set $S=\{(f_1(x),\ldots,f_m(x)):x\in B_X\}$ is [convex](../../../real-analysis.md#convex-function). If $b=(\Phi(f_1),\ldots,\Phi(f_m))$ were outside its closure, finite-dimensional [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) would supply coefficients $a_j$ such that, for $f=\sum_j a_jf_j$,

$$
\operatorname{Re}\Phi(f)>\sup_{x\in B_X}\operatorname{Re}f(x)=\|f\|.
$$

The real case omits real parts; in the complex case every real-linear separating functional on $\mathbb C^m$ has the displayed form. The [supremum](../../../real-analysis.md#supremum) equals the dual [norm](../../../functional-analysis.md#norm) by multiplying vectors by signs or unimodular scalars. The strict inequality contradicts $\|\Phi\|\le1$. Thus $b\in\overline S$, which is exactly approximation on every prescribed finite family of weak-star coordinates.

Now take $K=B_{X^*}$ with its compact Hausdorff weak-star topology. For each $x\in X$, the evaluation $\widehat x:f\mapsto f(x)$ is continuous on $K$, and [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) gives $\|\widehat x\|_\infty=\|x\|$. Therefore

$$
\boxed{X\longrightarrow C(K),\qquad x\longmapsto\widehat x}
$$

is the [isometric evaluation embedding into continuous functions on a compact dual ball](../../../functional-analysis.md#isometric-evaluation-embedding-into-continuous-functions-on-a-compact-dual-ball), over the same scalar field as $X$.

For the final sequential assertions, choose a norm-dense sequence $(f_j)$ in the separable dual $X^*$ and suppose $\|x_n\|\le M$. Each bounded scalar sequence $f_j(x_n)$ has a convergent subsequence: divide a bounding interval or square into finitely many smaller closed pieces, repeatedly retain one containing infinitely many terms, and let the diameters tend to zero. Successive extraction for $j=1,2,\ldots$, followed by a diagonal subsequence $(y_n)$, makes every $f_j(y_n)$ converge.

If $M=0$ the conclusion is immediate. Otherwise, for any $f\in X^*$ and $\epsilon>0$, choose $j$ with $\|f-f_j\|<\epsilon/(4M)$. For sufficiently large $n,m$,

$$
|f(y_n)-f(y_m)|\le2M\|f-f_j\|+|f_j(y_n)-f_j(y_m)|<\epsilon.
$$

Thus $\varphi(f)=\lim_n f(y_n)$ exists for every $f$. Taking limits proves linearity, and $|\varphi(f)|\le M\|f\|$ proves

$$
\boxed{\varphi\in X^{**},\qquad\|\varphi\|\le M.}
$$

This diagonal argument includes the continuity estimate rather than appealing to a sequential compactness theorem.

If $X$ is not reflexive, choose $\Phi\in B_{X^{**}}\setminus JX$, scaling a bidual element outside $JX$ if necessary. The Goldstine theorem proved above supplies $x_n\in B_X$ with $|f_j(x_n)-\Phi(f_j)|<1/n$ for $j\le n$. [Norm](../../../functional-analysis.md#norm) density and the bound $\|Jx_n-\Phi\|\le2$ extend this convergence to every $f\in X^*$. Hence $Jx_n\to\Phi$ weak-star. Every subsequence has the same coordinate limits, so a weakly convergent subsequence with limit $x\in X$ would give $Jx=\Phi$, a contradiction. This [sequential Goldstine approximation for a separable dual](../../../functional-analysis.md#sequential-goldstine-approximation-for-a-separable-dual) proves

$$
\boxed{\|x_n\|\le1,\quad(x_n)\text{ has no weakly convergent subsequence in }X.}
$$

The construction uses the Goldstine proof already given, not an unproved weak sequential compactness result.

## 4

↑ **Parent:** [Paper 106](paper-106.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is a nonzero complex-linear multiplicative map $\varphi:A\to\mathbb C$. The [character space of an algebra](../../../banach-algebra.md#character-space-of-an-algebra) $\Phi_A$ carries the [Gelfand topology](../../../banach-algebra.md#gelfand-topology), namely pointwise convergence on $A$, equivalently the subspace weak-star topology in $A^*$.

For a unital complex [Banach algebra](../../../banach-algebra.md), $\varphi(1)=1$: multiplicativity and nonzeroness force this. If $a-\varphi(a)1$ were invertible, applying $\varphi$ to its product with its inverse would give $0=1$. Thus $\varphi(a)\in\sigma_A(a)$. The [Neumann series](../../../banach-algebra.md#neumann-series) shows $\sigma_A(a)\subset\{|z|\le\|a\|\}$, so $|\varphi(a)|\le\|a\|$ and the [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is automatically bounded. The same conclusion for a nonunital algebra follows by extending $\varphi$ to its [unitization of an algebra](../../../banach-algebra.md#unitization-of-an-algebra) via $\widetilde\varphi(a,t)=\varphi(a)+t$ and using the standard [norm](../../../functional-analysis.md#norm) $\|(a,t)\|=\|a\|+|t|$.

In the algebra $R(K)$ let $u(z)=z$ and fix $\varphi\in\Phi_{R(K)}$. Write $\lambda=\varphi(u)$. If $\lambda\notin K$, the [rational function](../../../isolated-singularity.md#rational-function) $(u-\lambda)^{-1}$ belongs to $R(K)$, which is impossible because a [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) cannot vanish on an invertible element. Thus $\lambda\in K$. For a [rational function](../../../isolated-singularity.md#rational-function) $r=p/q$ without poles in $K$, choose a reduced denominator having no zeros in $K$. Multiplicativity gives $\varphi(r)=p(\lambda)/q(\lambda)=r(\lambda)$. Density of these [rational functions](../../../isolated-singularity.md#rational-function) and boundedness of $\varphi$ then yield $\varphi(h)=h(\lambda)$ for every $h\in R(K)$.

Conversely, evaluation at each $\lambda\in K$ is a [character of an algebra](../../../banach-algebra.md#character-of-an-algebra). The map $\lambda\mapsto\delta_\lambda$ is continuous in the Gelfand topology because every $h\in R(K)$ is continuous; its inverse is $\varphi\mapsto\varphi(u)$, also continuous. Hence the [character space of R(K)](../../../banach-algebra.md#character-space-of-r-k) is

$$
\boxed{\Phi_{R(K)}\cong K,\qquad\varphi=\delta_\lambda.}
$$

The identification includes the topology, not merely a bijection of sets.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Work over the complex scalar field. If $\lambda\in\sigma_A(x)$, the [ideal](../../../commutative-algebra.md#ideal) generated by $x-\lambda1$ is proper: otherwise commutativity would make $x-\lambda1$ invertible. By [Zorn lemma](../../../set-theory.md#zorn-s-lemma) extend it to a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $M$. This [ideal](../../../commutative-algebra.md#ideal) is closed. Indeed, if its closure were all of $A$, it would contain an element of $M$ sufficiently close to $1$ to be invertible, since the invertible group is open; a proper [ideal](../../../commutative-algebra.md#ideal) cannot contain such an element. Its closure is therefore proper, and maximality gives $\overline M=M$.

The quotient $A/M$ is a complex unital [Banach algebra](../../../banach-algebra.md) and a division algebra. The [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem) identifies it with $\mathbb C$, giving a [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) $\varphi$ with $\varphi(x)=\lambda$. Conversely, the argument in (a) shows that every $\varphi(x)$ is in the spectrum. Thus

$$
\boxed{\sigma_A(x)=\{\varphi(x):\varphi\in\Phi_A\}.}
$$

Here, as usual, a unital [Banach algebra](../../../banach-algebra.md) has a nonzero identity; the zero algebra is excluded.

The [holomorphic functional calculus](../../../banach-algebra.md#holomorphic-functional-calculus) assigns to every function holomorphic on an open neighbourhood $U$ of $\sigma_A(x)$ an element $f(x)\in A$. It is a unital algebra homomorphism, sends the coordinate function to $x$, agrees with evaluation of [rational functions](../../../isolated-singularity.md#rational-function) having no poles on the spectrum, depends only on the germ near the spectrum, and is continuous for uniform convergence on a fixed surrounding contour. Its formula is

$$
\boxed{f(x)=\frac1{2\pi i}\int_\Gamma f(z)(z1-x)^{-1}\,dz.}
$$

Here $\Gamma$ is a finite oriented contour cycle in $U\setminus\sigma_A(x)$, with [winding number](../../../complex-analysis.md#winding-number) one on the spectrum and zero off $U$. A finite union of suitable polygonal boundary cycles suffices; no connectedness of $U$ is required. Such cycles exist by compactness of the spectrum, and the calculus is independent of the choice. The inverse is the [resolvent of an element](../../../banach-algebra.md#resolvent-of-an-element).

For the exponential, use a circle $|z|=R>\|x\|$. The uniformly convergent Neumann expansion $(z1-x)^{-1}=\sum_{n\ge0}x^n z^{-n-1}$ may be integrated term by term. The scalar [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) gives $\frac1{2\pi i}\int e^z z^{-n-1}\,dz=1/n!$, proving

$$
\boxed{\exp(x)=\sum_{n=0}^\infty\frac{x^n}{n!}.}
$$

This series converges absolutely in the [Banach algebra](../../../banach-algebra.md) [norm](../../../functional-analysis.md#norm).

A [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is bounded and takes the resolvent to $(z-\varphi(x))^{-1}$. Applying it inside the contour integral and using the scalar Cauchy formula gives $\varphi(f(x))=f(\varphi(x))$. The [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) description of the spectrum, now applied to $f(x)$, proves the [spectral mapping theorem](../../../mathematics.md#spectral-mapping-theorem):

$$
\boxed{\sigma_A(f(x))=f(\sigma_A(x)).}
$$

In particular this spectrum is contained in $V$ when $V\supset f(U)$.

For the [composition rule for holomorphic functional calculus](../../../banach-algebra.md#composition-rule-for-holomorphic-functional-calculus), choose a relatively compact open neighbourhood $D$ of $f(\sigma_A(x))$ whose closure is contained in $V$, and a surrounding contour cycle $\Delta$ in $V$ with [winding number](../../../complex-analysis.md#winding-number) one on $D$. Choose a sufficiently small neighbourhood $\Omega$ of $\sigma_A(x)$ with $\overline\Omega\subset U$ and $f(\overline\Omega)\subset D$, and a contour $\Gamma$ in $\Omega$ surrounding the spectrum. The neighbourhoods and cycles may be finite unions, obtained from finite covers of the relevant compact sets. For $\zeta\in\Delta$ the function $h_\zeta(z)=(\zeta-f(z))^{-1}$ is holomorphic near $\overline\Omega$. Locality and multiplicativity of the calculus give

$$
(\zeta1-f(x))^{-1}=h_\zeta(x)
=\frac1{2\pi i}\int_\Gamma\frac{(z1-x)^{-1}}{\zeta-f(z)}\,dz.
$$

Insert this in the formula for $g(f(x))$ and interchange the two vector-valued integrals. The scalar inner integral is $g(f(z))$, so

$$
\begin{aligned}
g(f(x))&=\frac1{(2\pi i)^2}\int_\Gamma (z1-x)^{-1}
\left(\int_\Delta\frac{g(\zeta)}{\zeta-f(z)}\,d\zeta\right)dz\\
&=\frac1{2\pi i}\int_\Gamma g(f(z))(z1-x)^{-1}\,dz
=\boxed{(g\circ f)(x)}.
\end{aligned}
$$

This proves equality as algebra elements. Equality of their [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) values alone would be insufficient in a [Banach algebra](../../../banach-algebra.md) with nonzero radical.

Finally, $\|x\|<1$ places the spectrum in the open unit disk. On that disk $f(z)=\log(1-z)=-\sum_{n\ge1}z^n/n$ is a holomorphic branch. Its calculus value is the norm-convergent series $y=-\sum_{n\ge1}x^n/n$: one may integrate the uniformly convergent scalar series on a circle with $\|x\|<R<1$. Since $\exp(f(z))=1-z$, the composition rule gives the [logarithm of an element near the identity](../../../banach-algebra.md#logarithm-of-an-element-near-the-identity) formula

$$
\boxed{1-x=\exp(y),\qquad y=-\sum_{n=1}^\infty\frac{x^n}{n}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The prescribed-pole form of [Runge theorem](../../../complex-analysis.md#runge-s-theorem) is this: let $K\subset\mathbb C$ be compact, and let $E\subset\widehat{\mathbb C}\setminus K$ meet every [connected component](../../../geometry-and-topology.md#connected-component) of the complement in the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). If $f$ is holomorphic on a neighbourhood of $K$, then for every $\epsilon>0$ there is a [rational function](../../../isolated-singularity.md#rational-function) with all its poles in $E$ whose uniform distance from $f$ on $K$ is less than $\epsilon$. A polynomial is regarded as having its only possible pole at infinity. The empty compact set is trivial, so assume $K\ne\varnothing$.

First suppose $\infty\in E$. Let $A\subset C(K)$ be the [uniform rational approximation algebra with prescribed poles](../../../complex-analysis.md#uniform-rational-approximation-algebra-with-prescribed-poles), the uniform closure of [rational functions](../../../isolated-singularity.md#rational-function) whose finite poles lie in $E$. It is a commutative unital [Banach algebra](../../../banach-algebra.md), and contains $u(z)=z$. Set

$$
S=\{\lambda\in\mathbb C\setminus K:(u-\lambda1)^{-1}\in A\},
$$

where the inverse in this definition is the pointwise [continuous function](../../../calculus.md#continuous-function) on $K$. The set $S$ is relatively open: if the inverse at $\lambda$ belongs to $A$, the [Neumann series](../../../banach-algebra.md#neumann-series) gives inverses at nearby points. It is relatively closed: when $\lambda_n\to\lambda\notin K$, the corresponding scalar functions converge uniformly on $K$, and $A$ is closed.

Each bounded complementary component meets $E$ in a finite point $a$, and $(u-a1)^{-1}$ is an allowed [rational function](../../../isolated-singularity.md#rational-function). The unbounded component meets $S$ because for $|\lambda|>\|u\|$ the geometric series for $(u-\lambda1)^{-1}$ belongs to $A$. Being both open and closed in the complement, $S$ therefore contains every component, so it is the entire complement. Conversely, evaluation at any $z\in K$ prevents $u-z1$ from being invertible. Hence

$$
\boxed{\sigma_A(u)=K.}
$$

Apply the [holomorphic functional calculus](../../../banach-algebra.md#holomorphic-functional-calculus) in $A$ to $f$ near $K$. For every $z\in K$, the evaluation [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) and the contour formula from (b) give $f(u)(z)=f(z)$. Thus $f|_K\in A$. By the definition of this uniform closure, the required rational approximations exist.

If $\infty\notin E$, choose a finite point $a\in E$ in the component containing infinity. The [Möbius transformation](../../../group-theory.md#mobius-transformation) $w=(z-a)^{-1}$ sends $K$ to a compact subset $K'$ of the plane and sends $E$ to a set $E'$ containing infinity. It preserves complementary components, so $E'$ meets every component of the complement of $K'$. The transformed function $F(w)=f(a+1/w)$ is holomorphic near $K'$, since $0\notin K'$. The case already proved approximates $F$ by [rational functions](../../../isolated-singularity.md#rational-function) with poles in $E'$. Pulling them back gives rational approximations to $f$ on $K$ with poles only in $E$: a pole at infinity in the $w$-plane becomes a pole at $a$, and every other pole has its prescribed preimage. In particular the pullbacks do not acquire a pole at the original infinity, since $0\notin E'$.

This proves the full prescribed-pole theorem, including the case where a pole at infinity is forbidden. If $\mathbb C\setminus K$ is connected, take $E=\{\infty\}$ to obtain the [polynomial Runge theorem](../../../complex-analysis.md#polynomial-runge-theorem) as a corollary.

## 5

↑ **Parent:** [Paper 106](paper-106.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [Riesz-Markov-Kakutani representation theorem](../../../functional-analysis.md#riesz-markov-kakutani-representation-theorem) identifies the dual of the complex [space of continuous functions on a compact space](../../../functional-analysis.md#space-of-continuous-functions-on-a-compact-space) $C(K)$ with finite regular complex [Borel measures](../../../measure-theory.md#borel-measure) on $K$: each [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) has a unique representation

$$
\boxed{L(f)=\int_K f\,d\mu,\qquad\|L\|=|\mu|(K).}
$$

Here $|\mu|$ is the [variation measure](../../../measure-theory.md#variation-measure); positive functionals correspond exactly to positive regular measures. This is the measure representation theorem, rather than the Hilbert-space representation of a functional by a vector.

For the spectral construction use the convention that the Hilbert [inner product](../../../linear-algebra.md#inner-product) is linear in its first argument. A unital subalgebra of $\mathcal B(H)$ is understood to contain $I_H$: an algebra whose abstract identity is a smaller projection could not give a resolution normalized by $P(K)=I_H$. On a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space), a resolution of the identity is understood to be a normalized regular [projection-valued measure](../../../hilbert-space.md#projection-valued-measure): its scalar measures are regular, its values are [orthogonal projections](../../../hilbert-space.md#orthogonal-projection), and it is countably additive in the strong operator topology. Regularity is part of the usual convention needed for the uniqueness assertion; the statement is interpreted in this sense.

The [Commutative Gelfand--Naimark theorem](../../../banach-algebra.md#commutative-gelfand-naimark-theorem) makes the Gelfand transform an isometric unital star-isomorphism $A\to C(K)$, where $K=\Phi_A$ is compact Hausdorff. Denote its inverse by $\pi:C(K)\to A\subset\mathcal B(H)$. For $x,y\in H$, the [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $f\mapsto\langle\pi(f)x,y\rangle$ has [norm](../../../functional-analysis.md#norm) at most $\|x\|\|y\|$. Riesz-Markov-Kakutani gives a regular complex measure $\mu_{x,y}$ such that

$$
\langle\pi(f)x,y\rangle=\int_K f\,d\mu_{x,y},\qquad
|\mu_{x,y}|(K)\le\|x\|\|y\|.
$$

Uniqueness makes these measures sesquilinear in $x,y$. For $f\ge0$, the identity $\pi(f)=\pi(\sqrt f)\pi(\sqrt f)^*$ shows positivity, so $\mu_{x,x}$ is positive with total mass $\|x\|^2$.

For every Borel set $B$, the bounded sesquilinear form $(x,y)\mapsto\mu_{x,y}(B)$ determines an operator $P(B)$ by Hilbert-space [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem), with

$$
\langle P(B)x,y\rangle=\mu_{x,y}(B).
$$

In particular $0\le P(B)\le I$ and $P(B)$ is self-adjoint. We now verify the projection identity rather than assume it.

For continuous $f$, uniqueness of the representing measure applied to continuous test functions gives

$$
\mu_{\pi(f)x,y}=f\mu_{x,y},\qquad
\mu_{x,\pi(\overline f)y}=f\mu_{x,y}.
$$

These identities imply $P(B)\pi(f)=\pi(f)P(B)$. Testing once more against a continuous $g$ gives

$$
\langle\pi(g)P(B)x,y\rangle=\int_B g\,d\mu_{x,y}.
$$

The restriction $1_B\mu_{x,y}$ of a finite regular Borel measure is still regular, so uniqueness in Riesz-Markov-Kakutani yields $\mu_{P(B)x,y}=1_B\mu_{x,y}$. Consequently, for any Borel $C$,

$$
\langle P(C)P(B)x,y\rangle=\mu_{P(B)x,y}(C)
=\mu_{x,y}(B\cap C),\qquad
\boxed{P(C)P(B)=P(B\cap C).}
$$

Taking $C=B$ proves that $P(B)$ is an [orthogonal projection](../../../hilbert-space.md#orthogonal-projection). Also $P(K)=I$ and $P(\varnothing)=0$. For disjoint $B_j$, these projections are orthogonal, and scalar countable additivity gives weak countable additivity. If $B=\bigcup_j B_j$, then $R_N=P(B)-\sum_{j\le N}P(B_j)$ is the projection of the remaining union and

$$
\|R_Nx\|^2=\mu_{x,x}\left(\bigcup_{j>N}B_j\right)\longrightarrow0.
$$

Thus countable additivity holds in the [strong operator topology](../../../functional-analysis.md#strong-operator-topology). The scalar measures are the regular measures already constructed. This completes the [scalar-measure construction of a projection-valued measure](../../../hilbert-space.md#scalar-measure-construction-of-a-projection-valued-measure).

By the integral theorem permitted in the question, continuous $f$ satisfies $\langle(\int f\,dP)x,y\rangle=\int f\,d\mu_{x,y}=\langle\pi(f)x,y\rangle$, and hence $\int f\,dP=\pi(f)$. For $T\in A$, this proves the [spectral theorem for a commutative operator algebra](../../../hilbert-space.md#spectral-theorem-for-a-commutative-operator-algebra):

$$
\boxed{T=\int_K\widehat T\,dP.}
$$

Any other regular resolution giving these integrals has the same scalar integrals on all of $C(K)$; Riesz-Markov-Kakutani uniqueness forces the same scalar measures and therefore the same projections on every Borel set.

For nonempty open $U\subset K$, compact Hausdorff normality supplies a nonzero [continuous function](../../../calculus.md#continuous-function) $f$ supported in $U$. If $P(U)=0$, the stated squared-norm identity for spectral integrals gives $\pi(f)=\int f\,dP=0$, contradicting the [isometry](../../../riemannian-geometry.md#isometry) of $\pi$. This proves the [full support of a faithful spectral measure](../../../hilbert-space.md#full-support-of-a-faithful-spectral-measure) property

$$
\boxed{P(U)\ne0\quad\text{for every nonempty open }U\subset K.}
$$

Faithfulness of the representation is essential here.

The [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators) says that a bounded [normal operator](../../../hilbert-space.md#normal-operator) $T$ on a nonzero complex [Hilbert space](../../../hilbert-space.md) has a unique regular projection-valued measure $E$ on $\sigma(T)$ such that $T=\int z\,dE(z)$. Its support is all of $\sigma(T)$, and bounded Borel functions have the associated [Borel functional calculus for a normal operator](../../../banach-algebra.md#borel-functional-calculus-for-a-normal-operator).

For the proof sketch, $A=C^*(I,T)$ is commutative because $T$ commutes with $T^*$; polynomials in these two operators commute, as do their [norm](../../../functional-analysis.md#norm) limits. The map $\Phi_A\to\sigma(T)$, $\varphi\mapsto\varphi(T)$, is onto by the [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) formula and [spectral permanence for C-star algebras](../../../banach-algebra.md#spectral-permanence-for-c-star-algebras). It is one-to-one because a [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) preserves the star operation and its values on $T,T^*$ determine it on their dense polynomial algebra. It is therefore a [homeomorphism](../../../topology.md#homeomorphism) from compact $\Phi_A$ to the Hausdorff spectrum. Transport the resolution just constructed through this [homeomorphism](../../../topology.md#homeomorphism). It gives the formula for $T$ and full support; conversely a regular resolution for $T$ gives the same integrals for polynomials in $T,T^*$, hence by density the same continuous functional calculus and the same resolution. This argument works without separability of $H$.

Finally choose disjoint nonempty relatively open sets $U,V\subset\sigma(T)$ around two distinct spectral points, and put $Q=E(U)$. Full support gives $Q\ne0$ and $E(V)\ne0$, while $QE(V)=0$, so $Q\ne I$. The spectral integral, or multiplicativity of its Borel calculus with $1_U$, gives $QT=TQ$ and also $QT^*=T^*Q$. Thus $Y=QH$ is closed, nonzero and proper, and $T(Qx)=Q(Tx)\in Y$. The [spectral projection gives a reducing subspace](../../../hilbert-space.md#spectral-projection-gives-a-reducing-subspace) conclusion is

$$
\boxed{Y=E(U)H\text{ is a nontrivial closed invariant subspace of }T.}
$$

In fact it is a reducing subspace, since it is also invariant under $T^*$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
