# Paper 9

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper9.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper9.pdf)

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
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)

## 1

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Assume $X$ is nonempty, as is necessary for a [probability measure](../../../probability-theory.md#probability-measure) to exist. Give its [isometry group](../../../riemannian-geometry.md#isometry-group) $I_X$ the uniform [metric](../../../topological-analysis.md#metric)

$$
D(g,h)=\sup_{x\in X}d(gx,hx).
$$

Every distance-preserving self-map of a [compact metric space](../../../topological-analysis.md#compact-metric-space) is onto. Indeed, if $x_0\notin gX$, then $\delta=d(x_0,gX)>0$, and for $n>m$ the iterates satisfy $d(g^mx_0,g^nx_0)=d(x_0,g^{n-m}x_0)\geq\delta$. This infinite separated set contradicts [compactness](../../../topology.md#compact-space). Consequently $I_X$ is a [group](../../../group.md) under composition, with the identity and inverses again [isometries](../../../riemannian-geometry.md#isometry).

The [metric](../../../topological-analysis.md#metric) $D$ is invariant under both left and right multiplication: left invariance uses preservation of distances, and right invariance uses surjectivity. Inversion is an [isometry](../../../riemannian-geometry.md#isometry) for $D$, and $D(gh,g'h')\leq D(g,g')+D(h,h')$ proves continuity of multiplication. Moreover, $I_X$ is compact. A sequence of [isometries](../../../riemannian-geometry.md#isometry) has a subsequence converging at every point of a countable dense subset of $X$, by a diagonal argument. Their common [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) $1$ and finite [epsilon-nets](../../../topological-analysis.md#metric-epsilon-net) of $X$ make this subsequence uniformly Cauchy. Its [uniform limit](../../../real-analysis.md#uniform-limit) preserves distances and is onto by the preceding argument. Thus **$I_X$ is a compact metrizable [topological group](../../../topological-group.md)**. A [transitive group action](../../../group-theory.md#transitive-group-action) means that for every $x,y\in X$ some $g\in I_X$ has $gx=y$.

We construct the invariant [Borel probability measure](../../../measure-theory.md#borel-probability-measure) directly. The [Hall marriage theorem](../../../graph-theory.md#hall-s-marriage-theorem) says that a finite [bipartite graph](../../../graph-theory.md#bipartite-graph) with equal-sized vertex classes $A,B$ has a [perfect matching](../../../graph-theory.md#perfect-matching) precisely when every subset $S\subseteq A$ has at least $|S|$ neighbours in $B$. Its following consequence is useful. If $A,B$ are $\varepsilon$-separated subsets of maximum [cardinality](../../../set-theory.md#cardinality) in a [compact metric space](../../../topological-analysis.md#compact-metric-space), join points whose distance is less than $\varepsilon$. If some $S\subseteq A$ had fewer than $|S|$ neighbours, replacing those neighbours in $B$ by $S$ would produce a larger $\varepsilon$-separated set. This contradicts maximal [cardinality](../../../set-theory.md#cardinality). Hence there is a bijection between $A$ and $B$ moving each point by less than $\varepsilon$.

Choose $\varepsilon_n\downarrow0$ and maximum-[cardinality](../../../set-theory.md#cardinality) $\varepsilon_n$-separated sets $A_n\subset I_X$. Such sets exist: a finite covering by balls of radius less than $\varepsilon_n/2$ bounds every separated set's [cardinality](../../../set-theory.md#cardinality). Fix $x_0\in X$ and define the empirical [probability measures](../../../probability-theory.md#probability-measure)

$$
\mu_n=\frac1{|A_n|}\sum_{a\in A_n}\delta_{ax_0}.
$$

For $f\in C(X)$ let $\omega_f(r)=\sup_{d(x,y)\leq r}|f(x)-f(y)|$, which tends to zero with $r$ by [uniform continuity](../../../topological-analysis.md#uniform-continuity). For every $h\in I_X$, left invariance of $D$ makes $hA_n$ another maximum-[cardinality](../../../set-theory.md#cardinality) separated set. Match it to $A_n$ as above. Then

$$
\left|\int f\,d\mu_n-\int f(hx)\,d\mu_n(x)\right|\leq\omega_f(\varepsilon_n).
$$

The allowed [compactness of probability measures on a compact metric space](../../../convergence-of-random-variables.md#compactness-of-probability-measures-on-a-compact-metric-space) supplies a subsequence converging to $\mu$ in the [weak-star topology](../../../weak-topology.md#weak-star-topology). Passing to that limit for each fixed $h,f$ gives $\int f\,d\mu=\int f\circ h\,d\mu$. The same subsequence works for every $h,f$, since the displayed estimate held for all of them before taking the limit.

For uniqueness, put $F_n(x)=|A_n|^{-1}\sum_{a\in A_n}f(ax)$. For $x=hx_0$, right invariance of $D$ lets us match $A_nh$ with $A_n$. Transitivity therefore gives the uniform estimate $|F_n(x)-F_n(x_0)|\leq\omega_f(\varepsilon_n)$ for every $x\in X$. If $\nu$ is any invariant [Borel probability measure](../../../measure-theory.md#borel-probability-measure), then

$$
\int f\,d\nu=\int F_n\,d\nu,\qquad
\left|\int f\,d\nu-F_n(x_0)\right|\leq\omega_f(\varepsilon_n).
$$

Two invariant [probability measures](../../../probability-theory.md#probability-measure) consequently differ on the integral of $f$ by at most $2\omega_f(\varepsilon_n)$, hence agree on every [continuous function](../../../calculus.md#continuous-function). [Continuous functions](../../../calculus.md#continuous-function) determine [Borel probability measures](../../../measure-theory.md#borel-probability-measure) on a [compact metric space](../../../topological-analysis.md#compact-metric-space), so **the invariant [probability measure](../../../probability-theory.md#probability-measure) exists and is unique**.

## 2

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A real [random variable](../../../random-variable.md) is a [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution) with exponent $b\geq0$ when its [moment-generating function](../../../probability-theory.md#moment-generating-function) satisfies

$$
\mathbb E e^{tX}\leq e^{b^2t^2/2}\qquad(t\in\mathbb R).
$$

Differentiating at $t=0$ from both sides gives $\mathbb EX=0$. Exponential integrability near zero justifies this differentiation. Conversely, if $|X|\leq M$ and $\mathbb EX=0$, [convexity](../../../real-analysis.md#convex-function) gives

$$
e^{tX}\leq\frac{M+X}{2M}e^{tM}+\frac{M-X}{2M}e^{-tM},\qquad
\mathbb Ee^{tX}\leq\cosh(tM)\leq e^{t^2M^2/2}.
$$

The last inequality follows by comparing power series using $(2j)!\geq2^j j!$. The case $M=0$ is immediate. Thus **a bounded [random variable](../../../random-variable.md) is sub-Gaussian exactly when it is centered**; the bound $M$ is one possible exponent.

For $b>0$, the [Markov inequality](../../../probability-inequality.md#markov-inequality) applied to $e^{tX}$ gives $\mathbb P(X>R)\leq\exp(b^2t^2/2-tR)$. Choose $t=R/b^2$ and repeat with $-X$. The [union bound](../../../probability-inequality.md#boole-s-inequality) yields

$$
\boxed{\mathbb P(|X|>R)\leq2e^{-R^2/(2b^2)}}\qquad(R>0).
$$

If $b=0$, the same exponential estimate with arbitrarily large $t$ shows $X=0$ almost surely, so all subsequent inequalities are trivial.

Integrating this [tail probability](../../../probability-theory.md#tail-probability) estimate gives, for every real $k\geq2$,

$$
\mathbb E|X|^{2k}=2k\int_0^\infty r^{2k-1}\mathbb P(|X|>r)\,dr
\leq2(2b^2)^k\Gamma(k+1).
$$

We need $2\Gamma(k+1)\leq k^k$. For integer $k$ this follows inductively from $2\cdot2!=2^2$ and $(k+1)k^k\leq(k+1)^{k+1}$. To cover real $k$ as well, set $H(k)=k\log k-\log\Gamma(k+1)-\log2$. Differentiating the [Gamma function](../../../complex-analysis.md#gamma-function) integral gives $(\log\Gamma)'(k+1)=\mathbb E\log Y$ for a [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $k+1$ and rate $1$. The [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) bounds this by $\log(k+1)$. Hence $H'(k)\geq1-\log(1+1/k)>0$ and $H(2)=0$. Taking the $2k$th root now proves

$$
\boxed{\|X\|_{2k}\leq b\sqrt{2k}\quad(k\geq2)}.
$$

Here $\|X\|_p=(\mathbb E|X|^p)^{1/p}$ is the [Lp norm](../../../real-analysis.md#lp-norm).

For the final assertion we prove the required [Littlewood interpolation inequality](../../../functional-analysis.md#littlewood-interpolation-inequality), rather than assuming it. Apply [Holder inequality](../../../functional-analysis.md#holder-inequality) with conjugate exponents $3/2$ and $3$:

$$
\mathbb E|X|^2=\mathbb E\bigl(|X|^{2/3}|X|^{4/3}\bigr)
\leq(\mathbb E|X|)^{2/3}(\mathbb E|X|^4)^{1/3}.
$$

Raising to the power $3/2$ gives $\|X\|_2^3\leq\|X\|_1\|X\|_4^2$. The preceding [Lp norm](../../../real-analysis.md#lp-norm) estimate with $k=2$ says $\|X\|_4\leq2b$. Therefore

$$
\boxed{\|X\|_2^3\leq4b^2\|X\|_1}.
$$

## 3

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $K=B_E$ and change coordinates so that its [John ellipsoid](../../../geometry-and-topology.md#john-ellipsoid) is $B_2^d$, the [Euclidean unit ball](../../../functional-analysis.md#euclidean-unit-ball). Then the standard symmetric-body inequalities are

$$
B_2^d\subseteq K\subseteq\sqrt d\,B_2^d,\qquad
\boxed{\|x\|_E\leq |x|\leq\sqrt d\,\|x\|_E}.
$$

We give the contact argument underlying the construction. The [John contact decomposition](../../../geometry-and-topology.md#john-contact-decomposition) provides unit contact vectors $u_j\in\partial K\cap S^{d-1}$ and positive numbers $c_j$ such that

$$
\sum_j c_j u_j\otimes u_j=I,\qquad \sum_jc_j=d,\qquad
|\langle u_j,x\rangle|\leq\|x\|_E.
$$

The last inequality follows because the supporting hyperplane of $K$ at $u_j$ must also support the contained [Euclidean unit ball](../../../functional-analysis.md#euclidean-unit-ball), hence has normal $u_j$. For completeness, the decomposition follows from maximal volume as follows. If $I$ were not in the [convex cone](../../../mathematical-optimization.md#convex-cone) generated by $u\otimes u$ at contact points, finite-dimensional separation would give a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A$ with $\operatorname{tr}A>0$ and $\langle Au,u\rangle\leq0$ at every contact. Subtract $\delta I$ for small $\delta>0$, retaining positive [trace](../../../linear-algebra.md#matrix-trace) and obtaining strict negative values. For small $t>0$, the [support function](../../../mathematical-optimization.md#support-function) $|(I+t(A-\delta I))v|$ is less than $1$ near all contact directions. On the compact complement of those neighbourhoods, $h_K(v)-1$ has a positive minimum, so the perturbed [ellipsoid](../../../geometry-and-topology.md#ellipsoid) remains inside $K$ there too. But its [determinant](../../../linear-algebra.md#determinant) is $1+t\operatorname{tr}(A-\delta I)+O(t^2)>1$, contradicting maximum volume. The cone is closed: its generating contact matrices form a [compact set](../../../topology.md#compact-space) of [trace](../../../linear-algebra.md#matrix-trace) $1$, so bounded traces bound their nonnegative coefficient sums. Finite-dimensional [convexity](../../../real-analysis.md#convex-function) then supplies finitely many contacts in the decomposition. Finally, for $x\in K$ the identity gives $|x|^2=\sum_jc_j\langle u_j,x\rangle^2\leq d$, proving the second containment above.

Construct an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) recursively. After $e_1,\ldots,e_{i-1}$ have been chosen, let $H_i$ be their orthogonal complement. The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $P_{H_i}$ satisfies

$$
\sum_jc_j|P_{H_i}u_j|^2=\operatorname{tr}P_{H_i}=d-i+1.
$$

As $\sum_jc_j=d$, some contact $v_i$ satisfies $|P_{H_i}v_i|\geq\sqrt{(d-i+1)/d}$. Choose $e_i=P_{H_i}v_i/|P_{H_i}v_i|$. This works through $i=d$ and gives

$$
\|e_i\|_E\geq\langle v_i,e_i\rangle=|P_{H_i}v_i|
\geq\sqrt{\frac{d-i+1}{d}}.
$$

In particular, **$\|e_i\|_E\geq1/\sqrt2>1/4$ for $i\leq d/2$**.

Keep the contact vectors $v_i$ used for this basis. They lie in $\operatorname{span}(e_1,\ldots,e_i)$. Therefore, if $j<i\leq m=\lfloor d/2\rfloor$, then $\langle v_j,e_i\rangle=0$ and

$$
|v_i-v_j|\geq|\langle v_i,e_i\rangle|\geq1/\sqrt2.
$$

For a [standard Gaussian random vector](../../../probability-and-statistics.md#standard-gaussian-random-vector) $G$ in these coordinates, put $Z_i=\langle v_i,G\rangle$. These centered [Gaussian random variables](../../../probability-theory.md#gaussian-random-variable) have $\mathbb E(Z_i-Z_j)^2=|v_i-v_j|^2\geq1/2$, and $\|G\|_E\geq\max_{i\leq m}Z_i$.

Here is a proof of the [Sudakov-Fernique inequality](../../../stochastic-process.md#sudakov-fernique-inequality) needed for this finite family. Let $Y_i=g_i/2$ with independent standard [Gaussian random variables](../../../probability-theory.md#gaussian-random-variable) $g_i$, so that $\mathbb E(Y_i-Y_j)^2=1/2$ for $i\ne j$. Take $Z,Y$ independently and use

$$
F_\beta(z)=\beta^{-1}\log\sum_i e^{\beta z_i},\qquad
p_i(z)=\frac{e^{\beta z_i}}{\sum_j e^{\beta z_j}}.
$$

The Hessian is $\partial_{ij}F_\beta=\beta(p_i\delta_{ij}-p_ip_j)$. Along $Z_s=\sqrt s Z+\sqrt{1-s}Y$, [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) gives

$$
\frac{d}{ds}\mathbb E F_\beta(Z_s)
=\frac\beta4\sum_{i,j}\mathbb E[p_i(Z_s)p_j(Z_s)]
\left(\mathbb E(Z_i-Z_j)^2-\mathbb E(Y_i-Y_j)^2\right)\geq0.
$$

Indeed, the one-dimensional identity $\mathbb E[g\phi(g)]=\mathbb E\phi'(g)$ follows by integrating the standard [Gaussian density](../../../probability-and-statistics.md#multivariate-normal-density) by parts, and applying it to a linear representation of these [Gaussian vectors](../../../probability-and-statistics.md#gaussian-random-vector) gives the covariance formula used here. Since $0\leq F_\beta(z)-\max_i z_i\leq\log(m)/\beta$, letting $\beta\to\infty$ yields $\mathbb E\max Z_i\geq\tfrac12\mathbb E\max g_i$.

To estimate that last maximum, integrating the [Gaussian density](../../../probability-and-statistics.md#multivariate-normal-density) on $[t,t+(t+1)^{-1}]$ gives $\mathbb P(g_1>t)\geq a e^{-t^2/2}/(t+1)$ for an absolute $a>0$. With $t=\tfrac12\sqrt{\log m}$, [independence](../../../random-variable.md#independent-random-variables) shows

$$
\mathbb P(\max_i g_i>t)=1-(1-\mathbb P(g_1>t))^m\longrightarrow1.
$$

Its negative part has expectation at most $\mathbb E[|g_1|\mathbf1_{g_1<0}]\,2^{-(m-1)}$. Hence $\mathbb E\max_i g_i\geq a'\sqrt{\log m}$ for all sufficiently large $m$, and adjusting $a'>0$ covers every $m\geq2$; for these finitely many cases the expectation is strictly positive. For $d\geq4$, $\log\lfloor d/2\rfloor\geq\tfrac13\log d$. For $d=2,3$ use one contact vector and $\mathbb E\|G\|_E\geq\mathbb E|\langle u,G\rangle|=\sqrt{2/\pi}$; for $d=1$ the requested right side is zero. Thus

$$
\boxed{\int\|x\|_E\,d\gamma_d(x)\geq c\sqrt{\log d}}
$$

for an absolute $c>0$, independent of both dimension and the [norm](../../../functional-analysis.md#norm).

## 4

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a $d$-dimensional [normed vector space](../../../functional-analysis.md#normed-vector-space), with [unit ball](../../../functional-analysis.md#unit-ball) $K$ and [John ellipsoid](../../../geometry-and-topology.md#john-ellipsoid) $\mathcal E$, its [volume ratio](../../../functional-analysis.md#volume-ratio) is

$$
\operatorname{vr}(E)=\left(\frac{\operatorname{vol}K}{\operatorname{vol}\mathcal E}\right)^{1/d}.
$$

It is at least $1$ and invariant under invertible linear coordinate changes.

For $\ell_1^n$, the [unit ball](../../../functional-analysis.md#unit-ball) has volume $2^n/n!$: its intersection with each orthant is the standard simplex of volume $1/n!$. Its [John ellipsoid](../../../geometry-and-topology.md#john-ellipsoid) is $n^{-1/2}B_2^n$. To verify maximum volume, let $AB_2^n$ be any centered inscribed [ellipsoid](../../../geometry-and-topology.md#ellipsoid). For each sign vector $\varepsilon\in\{-1,1\}^n$, containment gives $|A^T\varepsilon|\leq1$. Averaging over independent [Rademacher random variables](../../../probability-theory.md#rademacher-distribution) yields $\operatorname{tr}(AA^T)\leq1$. The [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) for its squared [singular values](../../../linear-algebra.md#singular-value) gives $|\det A|\leq n^{-n/2}$. The scalar [matrix](../../../vector-space.md#matrix) $n^{-1/2}I$ attains this bound because $\|x\|_1\leq\sqrt n|x|$. Centered [ellipsoids](../../../geometry-and-topology.md#ellipsoid) suffice: if $a+AB_2^n$ is contained in the symmetric convex [unit ball](../../../functional-analysis.md#unit-ball), averaging it with $-a+AB_2^n$ gives the centered copy with the same volume.

Using the stated [Euclidean ball](../../../functional-analysis.md#euclidean-ball) volume and $n=2k$,

$$
\operatorname{vr}(\ell_1^{2k})^{2k}
=\frac{2^{2k}(2k)^k k!}{(2k)!\pi^k}
\leq\left(\frac8\pi\right)^k,
$$

since $(2k)!/k!=\prod_{j=k+1}^{2k}j\geq k^k$. Therefore **$\operatorname{vr}(\ell_1^{2k})\leq\sqrt{8/\pi}$ uniformly in $k$**.

**The subsequent assertion for an arbitrary $2k$-dimensional space is false as printed.** Here is a counterexample independent of any asymptotic section theorem. Take $E=\ell_\infty^{2k}$. Its [John ellipsoid](../../../geometry-and-topology.md#john-ellipsoid) is $B_2^{2k}$: an inscribed $AB_2^{2k}$ has every row of $A$ of Euclidean length at most $1$, so the [Hadamard inequality](../../../linear-algebra.md#hadamard-determinant-inequality) gives $|\det A|\leq1$, attained by $A=I$. Let $F$ be any $k$-dimensional subspace and $f_1,\ldots,f_k$ an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of it. The random unit vector

$$
x=\frac1{\sqrt k}\sum_{j=1}^k\varepsilon_j f_j
$$

has $|x|=1$. Since $\sum_j f_j(i)^2\leq1$ for each coordinate $i$, the [moment-generating function](../../../probability-theory.md#moment-generating-function) bound for independent [Rademacher random variables](../../../probability-theory.md#rademacher-distribution) gives

$$
\mathbb E e^{t x_i}\leq e^{t^2/(2k)},\qquad
\mathbb P(\|x\|_\infty>r)\leq4k\,e^{-kr^2/2}.
$$

Choose $r=\sqrt{2\log(8k)/k}$; the latter [probability](../../../probability-theory.md#probability) is at most $1/2$, so some unit vector in $F$ has $\|x\|_\infty\leq r$. The proposed section inequality would therefore force

$$
\boxed{L\geq\sqrt{\frac{k}{2\log(8k)}}\longrightarrow\infty}.
$$

Thus even one half-dimensional section cannot have the printed universal constant.

The valid [orthogonal splitting with bounded volume ratio](../../../functional-analysis.md#orthogonal-splitting-with-bounded-volume-ratio) is that $L$ may depend on $V=\operatorname{vr}(E)$, and **$L=32V^2$ suffices**. This supplies a dimension-independent constant for the preceding $\ell_1^{2k}$ case, or whenever $V$ is bounded uniformly. We prove the complete qualified assertion, including its [epsilon-net](../../../topological-analysis.md#metric-epsilon-net) ingredient.

In [John position](../../../geometry-and-topology.md#john-position), $\|x\|_E\leq|x|$. Polar integration of the radial function $\rho(u)=1/\|u\|_E$ gives

$$
V^{2k}=\frac{\operatorname{vol}K}{\operatorname{vol}B_2^{2k}}
=\int_{S^{2k-1}}\|u\|_E^{-2k}\,d\sigma(u),\qquad
\sigma\{\|u\|_E\leq r\}\leq(Vr)^{2k},
$$

where $\sigma$ is normalized spherical measure.

A maximal $\varepsilon$-separated subset of $S^{k-1}$ is an [epsilon-net](../../../topological-analysis.md#metric-epsilon-net). Balls of radius $\varepsilon/2$ about its points have disjoint interiors and lie in the ball of radius $1+\varepsilon/2$. Comparing volumes bounds its [cardinality](../../../set-theory.md#cardinality) by $(1+2/\varepsilon)^k$. Finite existence follows from this packing bound, and maximality proves the net property without assuming a separate covering theorem.

Choose two orthogonal $k$-dimensional subspaces $F_0,F_0^\perp$ and one such net on each [unit sphere](../../../topology.md#unit-sphere). Rotate both by a common uniformly distributed orthogonal [matrix](../../../vector-space.md#matrix) $U$. This distribution can be obtained from Question 1 applied to the compact [orthogonal group](../../../linear-algebra.md#orthogonal-group) with its Frobenius [metric](../../../topological-analysis.md#metric); left and right multiplication are transitive [isometries](../../../riemannian-geometry.md#isometry). Consequently $Uv$ is uniformly distributed on $S^{2k-1}$ for every fixed unit vector $v$. The [union bound](../../../probability-inequality.md#boole-s-inequality) shows that the [probability](../../../probability-theory.md#probability) that some rotated net point has [norm](../../../functional-analysis.md#norm) less than $2\varepsilon$ is at most

$$
2(1+2/\varepsilon)^k(2V\varepsilon)^{2k}
=2\left[4V^2(\varepsilon^2+2\varepsilon)\right]^k.
$$

Set $\varepsilon=(32V^2)^{-1}$. Because $V\geq1$, the bracket is at most $1/4+1/256$, and twice its $k$th power is less than $1$ for every $k\geq1$. Some rotation therefore makes every point of both nets have [norm](../../../functional-analysis.md#norm) at least $2\varepsilon$.

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) and $\|x\|_E\leq|x|$ imply that $\|\cdot\|_E$ is $1$-[Lipschitz](../../../real-analysis.md#lipschitz-continuity) for the [Euclidean metric](../../../differential-geometry.md#euclidean-metric). Every unit vector of $UF_0$ or $UF_0^\perp$ is within $\varepsilon$ of a good net point and thus has [norm](../../../functional-analysis.md#norm) at least $\varepsilon$. By homogeneity, on both orthogonal subspaces,

$$
\boxed{\|x\|_E\leq |x|\leq32\operatorname{vr}(E)^2\|x\|_E}.
$$

For $\ell_1^{2k}$ the first computation gives the absolute choice $L=256/\pi$. The missing bounded-[volume ratio](../../../functional-analysis.md#volume-ratio) restriction is essential; the literal unrestricted assertion cannot be proved.

## 5

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Use the [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) convention $\|f\|_L=\sup_{x\ne y}|f(x)-f(y)|/d(x,y)$ in the final quantity; it is a seminorm, with constants having value zero. Also interpret the [coupling](../../../probability-and-statistics.md#coupling) space as $\mathcal P(X\times X)$. The printed $\mathcal P(X,Y)$ has an undefined $Y$. The third quantity has a duplicated printed label; it is placed in part iii here, with the fourth in part iv.

First prove weak [optimal transport](../../../mathematical-optimization.md#optimal-transport) duality. For any feasible continuous pair $f,g$ and any [coupling of probability distributions](../../../probability-and-statistics.md#coupling) $\pi$ with marginals $P,Q$,

$$
\int f\,dP+\int g\,dQ
=\int_{X\times X}(f(x)+g(y))\,d\pi(x,y)
\leq\int_{X\times X}d(x,y)\,d\pi(x,y).
$$

Taking the supremum over pairs and infimum over [couplings](../../../probability-and-statistics.md#coupling) gives **$m_d(P,Q)\leq W(P,Q)$**. These quantities are finite: $P\otimes Q$ is a [coupling](../../../probability-and-statistics.md#coupling) and the continuous cost $d$ is bounded on the [compact metric space](../../../topological-analysis.md#compact-metric-space) $X\times X$. The zero pair is feasible, so $0\leq m_d\leq W\leq\operatorname{diam}X$.

The reverse inequality is established in part ii by finite approximation and a proof of the required finite [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality). Parts iii and iv then show that all the dual formulations agree.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Fix $\varepsilon>0$ and a finite [epsilon-net](../../../topological-analysis.md#metric-epsilon-net) $x_1,\ldots,x_N$ in $X$. Choose a Borel map $r:X\to\{x_1,\ldots,x_N\}$ with $d(x,r(x))\leq\varepsilon$, for example the nearest point with ties broken by index. Its cells $A_i$ give discrete [probability measures](../../../probability-theory.md#probability-measure) with masses $p_i=P(A_i)$ and $q_i=Q(A_i)$. Let

$$
W_\varepsilon=\min\left\{\sum_{i,j}d(x_i,x_j)\pi_{ij}:\pi_{ij}\geq0,\ \sum_j\pi_{ij}=p_i,\ \sum_i\pi_{ij}=q_j\right\}.
$$

The feasible set is nonempty and compact, so the minimum exists. Pushing any [coupling](../../../probability-and-statistics.md#coupling) forward by $(r,r)$ changes its cost by at most $2\varepsilon$, hence $W_\varepsilon\leq W+2\varepsilon$. Conversely, lift a discrete [coupling](../../../probability-and-statistics.md#coupling) by the measure

$$
\sum_{i,j:\,p_iq_j>0}\pi_{ij}\,
\frac{P|_{A_i}}{p_i}\otimes\frac{Q|_{A_j}}{q_j}.
$$

Terms with zero row or column masses vanish. This lift has marginals $P,Q$, and its cost differs by at most $2\varepsilon$. Therefore

$$
|W-W_\varepsilon|\leq2\varepsilon.
$$

Here is the finite [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) proof. Write $d_{ij}=d(x_i,x_j)$ and consider the [convex cone](../../../mathematical-optimization.md#convex-cone)

$$
C=\left\{\left((\sum_j\pi_{ij})_i,(\sum_i\pi_{ij})_j,\sum_{i,j}d_{ij}\pi_{ij}+s\right):\pi_{ij}\geq0,\ s\geq0\right\}.
$$

It is closed and finitely generated. One elementary justification of closedness is to reduce each nonnegative representation to linearly independent generators, eliminating a coefficient along any linear dependence; after choosing a subsequence using the same subset of generators, their independent coordinates have bounded, convergent coefficients whenever the represented vectors converge. For $\eta>0$, the point $(p,q,W_\varepsilon-\eta)$ lies outside $C$. Separation from this closed [convex cone](../../../mathematical-optimization.md#convex-cone) gives coefficients $(a,b,\tau)$ with

$$
\tau\geq0,\qquad a_i+b_j+\tau d_{ij}\geq0,\qquad
\sum_i a_ip_i+\sum_j b_jq_j+\tau(W_\varepsilon-\eta)<0.
$$

If $\tau=0$, summing the middle inequalities against any feasible $\pi$ contradicts the last one. Thus $\tau>0$, and $f_i=-a_i/\tau$, $g_j=-b_j/\tau$ obey $f_i+g_j\leq d_{ij}$ with dual objective greater than $W_\varepsilon-\eta$. The weak inequality already proved gives the reverse bound. Letting $\eta\downarrow0$ proves finite strong duality.

Reduce this discrete dual to a single [Lipschitz function](../../../real-analysis.md#lipschitz-continuity). For a feasible pair put $\phi_i=\min_j(d_{ij}-g_j)$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $|\phi_i-\phi_l|\leq d_{il}$, while $f_i\leq\phi_i$ and $g_i\leq-\phi_i$. Consequently

$$
\sum_i p_if_i+\sum_iq_ig_i\leq\sum_i(p_i-q_i)\phi_i.
$$

Conversely, any $1$-[Lipschitz](../../../real-analysis.md#lipschitz-continuity) vector $\phi$ gives a feasible pair $(\phi,-\phi)$. Adding a constant leaves its objective unchanged, so impose $\phi_1=0$. The resulting feasible set is compact, and its maximum is $W_\varepsilon$.

For a maximizing vector, the [McShane extension theorem](../../../real-analysis.md#mcshane-extension-theorem) has the following explicit proof in this situation. Define

$$
\phi(x)=\min_i\{\phi_i+d(x,x_i)\}.
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) proves that this extension is $1$-[Lipschitz](../../../real-analysis.md#lipschitz-continuity), and the discrete [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity) makes $\phi(x_i)=\phi_i$. Thus $(\phi,-\phi)$ is a continuous feasible pair. Because $|\phi(x)-\phi(r(x))|\leq\varepsilon$,

$$
m_d\geq\int\phi\,dP-\int\phi\,dQ\geq W_\varepsilon-2\varepsilon
\geq W-4\varepsilon.
$$

Letting $\varepsilon\downarrow0$, together with part i, proves **$m_d(P,Q)=W(P,Q)$**. The infimum defining $W$ is also attained: the set of [couplings](../../../probability-and-statistics.md#coupling) is a closed subset of the compact space of [probability measures](../../../probability-theory.md#probability-measure) on $X\times X$, and integrating the continuous cost is continuous for the [weak-star topology](../../../weak-topology.md#weak-star-topology).

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Since [Lipschitz functions](../../../real-analysis.md#lipschitz-continuity) are continuous, the feasible class here is smaller, giving $m_L\leq m_d$. To prove the reverse inequality, take any continuous feasible pair $f,g$ and perform [Lipschitz regularization of transport potentials](../../../probability-and-statistics.md#lipschitz-regularization-of-transport-potentials):

$$
h(x)=\min_{y\in X}\{d(x,y)-g(y)\}.
$$

The minimum exists by [compactness](../../../topology.md#compact-space). For every $x,x'$ the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $h(x)\leq d(x,x')+h(x')$; interchanging $x,x'$ proves $|h(x)-h(x')|\leq d(x,x')$. Thus $h$ has [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) at most $1$.

The original constraint yields $f(x)\leq h(x)$, and evaluating the minimum at $y=x$ gives $h(x)\leq-g(x)$. Moreover, $h(x)-h(y)\leq d(x,y)$, so $(h,-h)$ is a feasible [Lipschitz](../../../real-analysis.md#lipschitz-continuity) pair with

$$
\int f\,dP+\int g\,dQ\leq\int h\,dP-\int h\,dQ\leq m_L.
$$

Taking the supremum over the original continuous pairs proves **$m_L(P,Q)=m_d(P,Q)=W(P,Q)$**. Notice that this is an exact regularization, with no density or approximation assumption about the initial pair.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

Every function $h$ with [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) at most $1$ yields a feasible pair $(h,-h)$, and replacing $h$ by $-h$ reverses the objective. Hence

$$
\gamma(P,Q)=\sup_{\|h\|_L\leq1}\left(\int h\,dP-\int h\,dQ\right)\leq m_L(P,Q).
$$

Conversely, the [Lipschitz regularization of transport potentials](../../../probability-and-statistics.md#lipschitz-regularization-of-transport-potentials) in part iii dominates every feasible pair by $(h,-h)$ with $\|h\|_L\leq1$, so $m_L\leq\gamma$. Together with the preceding parts this proves the [Kantorovich–Rubinstein theorem](../../../probability-and-statistics.md#kantorovich-rubinstein-theorem) here in all four requested forms:

$$
\boxed{m_d(P,Q)=W(P,Q)=m_L(P,Q)=\gamma(P,Q)}.
$$

The seminorm convention is essential. If instead $\|h\|_L$ meant $\|h\|_\infty+\operatorname{Lip}(h)$, the equality would fail: on a two-point space at distance $2$, with point masses at the two different points, $W=2$ whereas the latter unit-ball supremum is $1$. Indeed, an oscillation $a$ needs supremum [norm](../../../functional-analysis.md#norm) at least $a/2$ and [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) $a/2$, so the sum [norm](../../../functional-analysis.md#norm) bounds $a$ by $1$, attained by values $-1/2,1/2$. This distinguishes the [Lipschitz](../../../real-analysis.md#lipschitz-continuity) seminorm used above from a full bounded-[Lipschitz](../../../real-analysis.md#lipschitz-continuity) [norm](../../../functional-analysis.md#norm).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
