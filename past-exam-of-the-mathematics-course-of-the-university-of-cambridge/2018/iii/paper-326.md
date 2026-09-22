# Paper 326

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_326.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_326.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [a](#1/1/a)
      - [Solution](#1/1/a/solution)
    - [b](#1/1/b)
      - [Solution](#1/1/b/solution)
    - [c](#1/1/c)
      - [Solution](#1/1/c/solution)
    - [d](#1/1/d)
      - [Solution](#1/1/d/solution)
    - [2](#1/1/2)
      - [a](#1/1/2/a)
        - [Solution](#1/1/2/a/solution)
      - [b](#1/1/2/b)
        - [Solution](#1/1/2/b/solution)
      - [c](#1/1/2/c)
        - [Solution](#1/1/2/c/solution)
      - [d](#1/1/2/d)
        - [Solution](#1/1/2/d/solution)
      - [e](#1/1/2/e)
        - [Solution](#1/1/2/e/solution)
- [2](#2)
  - [1](#2/1)
    - [a](#2/1/a)
      - [Solution](#2/1/a/solution)
    - [b](#2/1/b)
      - [Solution](#2/1/b/solution)
    - [c](#2/1/c)
      - [Solution](#2/1/c/solution)
  - [2](#2/2)
    - [a](#2/2/a)
      - [Solution](#2/2/a/solution)
    - [b](#2/2/b)
      - [Solution](#2/2/b/solution)
    - [c](#2/2/c)
      - [Solution](#2/2/c/solution)
    - [d](#2/2/d)
      - [Solution](#2/2/d/solution)
    - [e](#2/2/e)
      - [Solution](#2/2/e/solution)
    - [f](#2/2/f)
      - [Solution](#2/2/f/solution)
- [3](#3)
  - [1](#3/1)
    - [a](#3/1/a)
      - [Solution](#3/1/a/solution)
    - [b](#3/1/b)
      - [Solution](#3/1/b/solution)
    - [c](#3/1/c)
      - [Solution](#3/1/c/solution)
    - [d](#3/1/d)
      - [Solution](#3/1/d/solution)
    - [e](#3/1/e)
      - [Solution](#3/1/e/solution)
  - [2](#3/2)
    - [a](#3/2/a)
      - [Solution](#3/2/a/solution)
    - [b](#3/2/b)
      - [Solution](#3/2/b/solution)
    - [c](#3/2/c)
      - [Solution](#3/2/c/solution)
    - [d](#3/2/d)
      - [Solution](#3/2/d/solution)

## 1

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/a">a</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/a/solution">Solution</h5>

↑ **Parent:** [A](#1/1/a)

Use the [Hilbert space](../../../hilbert-space.md) interpretation of a linear [inverse problem](../../../inverse-problem.md), with a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) $K:\mathcal U\to\mathcal V$. A [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) minimizes $\|Ku-f\|_{\mathcal V}$ over $u\in\mathcal U$. A [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) additionally has the smallest $\mathcal U$-[norm](../../../functional-analysis.md#norm) among all [least-squares solutions](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem). When the equation is consistent this is the smallest-[norm](../../../functional-analysis.md#norm) exact solution.

The [least-squares solutions](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) form a nonempty closed [affine subspace](../../../vector-space.md#affine-subspace) precisely when

$$
\boxed{f\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

The [closest point theorem in a Hilbert space](../../../hilbert-space.md#hilbert-projection-theorem) then gives a unique nearest point to zero, hence a unique [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution). Equivalently, it is the unique [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) in $\mathcal N(K)^\perp$. If $\mathcal R(K)$ is closed, this exists for every datum; a nonclosed [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator) can leave some data without any [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem).

For example, on the [l2 sequence space](../../../banach-space.md#l2-sequence-space), take $(Ku)_n=u_n/n$ and $f_n=1/n$. The equation would require $u_n=1$ for every $n$, which is not square summable. However, setting the first $N$ coordinates of $u$ to one and the rest to zero gives

$$
\|Ku-f\|^2=\sum_{n>N}\frac1{n^2}\longrightarrow0.
$$

Thus the least-squares [infimum](../../../real-analysis.md#infimum) is zero but is not attained, and **no [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) exists for these data**.

<h4 id="1/1/b">b</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/b/solution">Solution</h5>

↑ **Parent:** [B](#1/1/b)

The map $K^*K$ is a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator), so the inverse image of the closed singleton $\{K^*f\}$ is closed. That inverse image is also a [convex set](../../../mathematical-optimization.md#convex-set): if $K^*Ku=K^*Kv=K^*f$, every convex combination has the same image.

The identity $\mathcal N(K^*)=\mathcal R(K)^\perp$ gives

$$
K^*Ku=K^*f\quad\Longleftrightarrow\quad f-Ku\in\mathcal R(K)^\perp.
$$

Consequently such a $u$ exists exactly when $f$ is the sum of an element of $\mathcal R(K)$ and one of its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). Thus

$$
\boxed{\mathbb L\neq\varnothing\ \Longleftrightarrow\
f\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

These are precisely the [least-squares solutions](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem). Indeed, if $r=Ku-f$ and $K^*r=0$, then for every $h$ the [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
\|K(u+h)-f\|^2=\|r\|^2+\|Kh\|^2\geq\|r\|^2.
$$

Conversely, differentiating the squared residual along any real direction $h$ forces $\operatorname{Re}\langle K^*r,h\rangle=0$, hence the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem). For any $u_*\in\mathbb L$, the difference of two solutions of the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) lies in $\mathcal N(K)$, since $\langle K^*Kh,h\rangle=\|Kh\|^2$. Therefore

$$
\boxed{\mathbb L=u_*+\mathcal N(K),}
$$

a closed [affine subspace](../../../vector-space.md#affine-subspace); the empty case is closed and [convex](../../../real-analysis.md#convex-function) as well.

<h4 id="1/1/c">c</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/c/solution">Solution</h5>

↑ **Parent:** [C](#1/1/c)

The [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) is the linear map

$$
K^\dagger:\mathcal D(K^\dagger)=\mathcal R(K)\oplus\mathcal R(K)^\perp
\longrightarrow\mathcal N(K)^\perp
$$

that assigns each admissible datum its [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution). If $f=y+z$ with $y\in\mathcal R(K)$ and $z\in\mathcal R(K)^\perp$, then $K^\dagger f$ is the unique $u\in\mathcal N(K)^\perp$ satisfying $Ku=y$. In particular it vanishes on $\mathcal R(K)^\perp$, and

$$
KK^\dagger f=P_{\overline{\mathcal R(K)}}f,\qquad
K^\dagger Ku=P_{\mathcal N(K)^\perp}u.
$$

The continuity criterion, with the inherited data [norm](../../../functional-analysis.md#norm) on its domain, is

$$
\boxed{K^\dagger\text{ is continuous}\ \Longleftrightarrow\ \mathcal R(K)\text{ is closed}.}
$$

For a closed [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator), the restriction of $K$ from $\mathcal N(K)^\perp$ to $\mathcal R(K)$ is a bounded bijection between [Banach spaces](../../../banach-space.md), so its inverse is bounded by the [bounded inverse theorem](../../../functional-analysis.md#bounded-inverse-theorem). Conversely, if $K^\dagger$ is bounded and $Ku_n\to y$, replace each $u_n$ by $P_{\mathcal N(K)^\perp}u_n=K^\dagger Ku_n$. This is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), hence converges to $u$, and $Ku=y$. Thus every limit of range elements remains in the [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator).

<h4 id="1/1/d">d</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/d/solution">Solution</h5>

↑ **Parent:** [D](#1/1/d)

Write $u^\dagger=K^\dagger f$. Every [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) is $u^\dagger+w$ for some $w\in\mathcal N(K)$, while $u^\dagger\in\mathcal N(K)^\perp$. Decompose $u_0=P_{\mathcal N(K)}u_0+P_{\mathcal N(K)^\perp}u_0$ using [orthogonal projections](../../../hilbert-space.md#orthogonal-projection). Then the [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
\|u^\dagger+w-u_0\|^2
=\|u^\dagger-P_{\mathcal N(K)^\perp}u_0\|^2
+\|w-P_{\mathcal N(K)}u_0\|^2.
$$

The first term is independent of $w$, and the second vanishes at exactly one point. Hence the unique [nearest least-squares solution](../../../inverse-problem.md#nearest-least-squares-solution) is

$$
\boxed{u_0^\dagger=K^\dagger f+P_{\mathcal N(K)}u_0.}
$$

Geometrically this is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) of $u_0$ onto the closed [affine subspace](../../../vector-space.md#affine-subspace) of [least-squares solutions](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem).

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/a">a</h5>

↑ **Parent:** [2](#1/1/2)

<h6 id="1/1/2/a/solution">Solution</h6>

↑ **Parent:** [A](#1/1/2/a)

A finite-valued [global minimizer](../../../analysis.md#global-minimizer) of the [functional](../../../calculus-of-variations.md#functional) $E$ is an element $\bar u\in\operatorname{dom}E$ satisfying

$$
\boxed{E(\bar u)=\inf_{u\in\mathcal U}E(u)<+\infty,\qquad
\operatorname{dom}E=\{u:E(u)<+\infty\}.}
$$

Here $\operatorname{dom}E$ is its [effective domain](../../../real-analysis.md#effective-domain). The finite-value convention avoids treating an infeasible problem as solved.

The [functional](../../../calculus-of-variations.md#functional) is a [proper extended-real function](../../../real-analysis.md#proper-extended-real-function) if its [effective domain](../../../real-analysis.md#effective-domain) is nonempty; the specified codomain already excludes $-\infty$. It has [coercivity](../../../real-analysis.md#coercive-function) if $\|u_n\|\to\infty$ always implies $E(u_n)\to+\infty$, equivalently every finite [sublevel set](../../../calculus.md#sublevel-set) is bounded. It is $\tau$-[sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity) if

$$
\boxed{u_n\xrightarrow{\tau}u\ \Longrightarrow\
E(u)\leq\liminf_{n\to\infty}E(u_n).}
$$

The topology in this definition matters: norm [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity) and weak [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity) need not coincide for a nonconvex [functional](../../../calculus-of-variations.md#functional).

<h5 id="1/1/2/b">b</h5>

↑ **Parent:** [2](#1/1/2)

<h6 id="1/1/2/b/solution">Solution</h6>

↑ **Parent:** [B](#1/1/2/b)

On $\mathcal U=\mathbb R$ with its usual [topology](../../../topology.md), the following examples isolate the three failures.

A nonproper [functional](../../../calculus-of-variations.md#functional) is $E(x)=+\infty$ for every $x$. Its [effective domain](../../../real-analysis.md#effective-domain) is empty, so **it has no finite-valued [global minimizer](../../../analysis.md#global-minimizer)**. It nevertheless has [coercivity](../../../real-analysis.md#coercive-function) and is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity). If a minimizer is instead defined only by $E(x)=\inf E$ without requiring finiteness, every point formally minimizes this function; under that convention the requested nonproper counterexample is impossible with the given codomain.

A noncoercive [functional](../../../calculus-of-variations.md#functional) is $E(x)=e^x$. It is a [proper extended-real function](../../../real-analysis.md#proper-extended-real-function) and is [continuous](../../../calculus.md#continuous-function), but its [infimum](../../../real-analysis.md#infimum) zero is approached as $x\to-\infty$ and is never attained. Hence **it has no [global minimizer](../../../analysis.md#global-minimizer)**.

A failure of [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity) is

$$
E(x)=\begin{cases}x^2,&x\neq0,\\1,&x=0.\end{cases}
$$

It is a [proper extended-real function](../../../real-analysis.md#proper-extended-real-function) with [coercivity](../../../real-analysis.md#coercive-function), but $E(1/n)\to0<E(0)$. Its [infimum](../../../real-analysis.md#infimum) is zero, while every function value is positive. Thus **it has no [global minimizer](../../../analysis.md#global-minimizer)**.

<h5 id="1/1/2/c">c</h5>

↑ **Parent:** [2](#1/1/2)

<h6 id="1/1/2/c/solution">Solution</h6>

↑ **Parent:** [C](#1/1/2/c)

The [epigraph](../../../calculus-of-variations.md#epigraph) is

$$
\boxed{\operatorname{epi}E=\{(u,t)\in\mathcal U\times\mathbb R:E(u)\leq t\}.}
$$

Assume $E$ is $\tau$-[sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity). If $(u_n,t_n)$ lies in the [epigraph](../../../calculus-of-variations.md#epigraph) and converges to $(u,t)$ in the [product topology](../../../geometry-and-topology.md#product-topology), then

$$
E(u)\leq\liminf E(u_n)\leq\lim t_n=t.
$$

The limit remains in the [epigraph](../../../calculus-of-variations.md#epigraph), so it is a [sequentially closed set](../../../topology.md#sequentially-closed-set).

Conversely, suppose the [epigraph](../../../calculus-of-variations.md#epigraph) is a [sequentially closed set](../../../topology.md#sequentially-closed-set) and [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity) fails along $u_n\xrightarrow{\tau}u$. Choose a finite real number $a$ with $\liminf E(u_n)<a<E(u)$. There is a [subsequence](../../../real-analysis.md#subsequence) along which $E(u_{n_j})\leq a$. Thus $(u_{n_j},a)$ lies in the [epigraph](../../../calculus-of-variations.md#epigraph) and converges to $(u,a)$, which does not lie there. This contradiction proves

$$
\boxed{E\text{ is }\tau\text{-sequentially lsc}
\ \Longleftrightarrow\ \operatorname{epi}E\text{ is sequentially closed}.}
$$

This is a sequential statement; identifying it with ordinary closedness requires an appropriate assumption on the [topology](../../../topology.md).

<h5 id="1/1/2/d">d</h5>

↑ **Parent:** [2](#1/1/2)

<h6 id="1/1/2/d/solution">Solution</h6>

↑ **Parent:** [D](#1/1/2/d)

The [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) gives the following existence theorem. Suppose bounded sequences in the [Banach space](../../../banach-space.md) $\mathcal U$ have $\tau$-[convergent subsequences](../../../real-analysis.md#convergent-subsequence), and $E$ is a [proper extended-real function](../../../real-analysis.md#proper-extended-real-function) with [coercivity](../../../real-analysis.md#coercive-function) and is $\tau$-[sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity). Then **$E$ has a finite-valued [global minimizer](../../../analysis.md#global-minimizer)**.

To prove this, properness makes $m=\inf E<+\infty$. First rule out $m=-\infty$: a sequence with $E(u_n)\to-\infty$ eventually lies in a fixed [sublevel set](../../../calculus.md#sublevel-set), which is bounded by [coercivity](../../../real-analysis.md#coercive-function). A $\tau$-[convergent subsequence](../../../real-analysis.md#convergent-subsequence) would then have a limit $u$ with $E(u)\leq-\infty$, contradicting the codomain. Hence $m$ is finite.

Choose a [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) with $E(u_n)\to m$. It eventually belongs to the bounded [sublevel set](../../../calculus.md#sublevel-set) $\{E\leq m+1\}$. Extract $u_{n_j}\xrightarrow{\tau}\bar u$. By [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity),

$$
m\leq E(\bar u)\leq\liminf_jE(u_{n_j})=m.
$$

Thus $E(\bar u)=m$. In particular, a [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space) with the [weak topology](../../../weak-topology.md) supplies the required subsequence property by [weak sequential compactness of bounded sequences in a reflexive Banach space](../../../functional-analysis.md#weak-sequential-compactness-of-bounded-sequences-in-a-reflexive-banach-space). A [strictly convex function](../../../real-analysis.md#strictly-convex-function) has at most one minimizer; this is an additional property, not part of the existence theorem.

<h5 id="1/1/2/e">e</h5>

↑ **Parent:** [2](#1/1/2)

<h6 id="1/1/2/e/solution">Solution</h6>

↑ **Parent:** [E](#1/1/2/e)

Take the [weak topology](../../../weak-topology.md) on the [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space) $\mathcal U$. A [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) is weak-to-weak continuous: $u_n\rightharpoonup u$ implies $\langle Ku_n,v\rangle\to\langle Ku,v\rangle$ for every $v\in\mathcal V$, by its [adjoint operator](../../../hilbert-space.md#adjoint-operator). The [weak lower semicontinuity of the Hilbert norm](../../../hilbert-space.md#weak-lower-semicontinuity-of-the-hilbert-norm) therefore makes $D(u)=\|Ku-f\|$ weakly [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity).

This [functional](../../../calculus-of-variations.md#functional) is finite everywhere and nonnegative. If it has [coercivity](../../../real-analysis.md#coercive-function), the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) supplies a [global minimizer](../../../analysis.md#global-minimizer) $\bar u$. Squaring the residual does not change its [global minimizers](../../../analysis.md#global-minimizer). Here the [adjoint operator](../../../hilbert-space.md#adjoint-operator) has codomain $\mathcal U^*$, since the source is a [Banach space](../../../banach-space.md). Differentiating the squared residual along every real direction $h\in\mathcal U$ gives $\operatorname{Re}\langle K^*(K\bar u-f),h\rangle=0$ in the [dual pairing](../../../continuous-dual-space.md#dual-pairing), hence the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) $K^*(K\bar u-f)=0$. Hence

$$
\boxed{f=K\bar u+(f-K\bar u)\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

The converse fails. For $K:\mathbb R^2\to\mathbb R$, $K(x,y)=x$, and $f=1$, the datum is in the [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator), but $D(1,n)=0$ while $\|(1,n)\|\to\infty$. Thus **admissible data do not imply [coercivity](../../../real-analysis.md#coercive-function) of the residual**; an unpenalized [null space](../../../linear-algebra.md#kernel-of-a-linear-map) already prevents it.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/a">a</h4>

↑ **Parent:** [1](#2/1)

<h5 id="2/1/a/solution">Solution</h5>

↑ **Parent:** [A](#2/1/a)

Fix a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator), with $Kv_j=\sigma_jw_j$ and $K^*w_j=\sigma_jv_j$, $\sigma_j>0$. A [spectral regularization method](../../../inverse-problem.md#spectral-regularization-method) has the form

$$
\boxed{R_\alpha f=\sum_j\sigma_jg_\alpha(\sigma_j^2)
\langle f,w_j\rangle v_j.}
$$

It annihilates $\mathcal R(K)^\perp$. Standard sufficient [spectral filter](../../../inverse-problem.md#spectral-filter) conditions are boundedness of $\sup_{0<\sigma\leq\|K\|}|\sigma g_\alpha(\sigma^2)|$ for each $\alpha$, pointwise $\lambda g_\alpha(\lambda)\to1$ as $\alpha\downarrow0$ for $\lambda>0$, and a uniform bound on $|\lambda g_\alpha(\lambda)|$. These give bounded linear operators and convergence on the domain of the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) by the [Picard criterion](../../../inverse-problem.md#picard-criterion) and [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem).

For [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization),

$$
g_\alpha(\lambda)=\frac1{\lambda+\alpha},\qquad
\boxed{R_\alpha=(K^*K+\alpha I)^{-1}K^*.}
$$

This can be computed by solving the [Tikhonov normal equation](../../../inverse-problem.md#tikhonov-normal-equation), without knowing the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition).

For [spectral cutoff regularization](../../../inverse-problem.md#truncated-singular-value-decomposition), take

$$
\boxed{g_\alpha(\lambda)=\frac{\mathbf1_{[\alpha,\infty)}(\lambda)}{\lambda},}
$$

with value zero at $\lambda=0$. Only [singular values](../../../linear-algebra.md#singular-value) $\sigma_j\geq\sqrt\alpha$ are inverted. Here $g_\alpha$ multiplies $\sigma$; conventions calling the full coefficient $\sigma g_\alpha(\sigma^2)$ the [spectral filter](../../../inverse-problem.md#spectral-filter) are equivalent.

<h4 id="2/1/b">b</h4>

↑ **Parent:** [1](#2/1)

<h5 id="2/1/b/solution">Solution</h5>

↑ **Parent:** [B](#2/1/b)

Suppose each $R_\alpha:\mathcal V\to\mathcal U$ is a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) and $R_\alpha f\to K^\dagger f$ for every $f\in\mathcal D(K^\dagger)$ as $\alpha\downarrow0$. A standard sufficient [a priori regularization parameter choice](../../../inverse-problem.md#a-priori-regularization-parameter-choice) satisfies

$$
\boxed{\alpha(\delta)\longrightarrow0,\qquad
\delta\|R_{\alpha(\delta)}\|\longrightarrow0\quad(\delta\downarrow0).}
$$

For every datum with $\|f^\delta-f\|\leq\delta$, the [noise-bias decomposition for linear regularization](../../../inverse-problem.md#noise-bias-decomposition-for-linear-regularization) gives

$$
\|R_{\alpha(\delta)}f^\delta-K^\dagger f\|
\leq\delta\|R_{\alpha(\delta)}\|
+\|R_{\alpha(\delta)}f-K^\dagger f\|\longrightarrow0.
$$

Thus **the parameter rule gives a [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem)**, uniformly over data in the prescribed noise ball for each fixed admissible exact datum. For [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization), $\|R_\alpha\|\leq1/(2\sqrt\alpha)$, so $\alpha\to0$ and $\delta/\sqrt\alpha\to0$ suffice. The same sufficient noise scaling holds for [spectral cutoff regularization](../../../inverse-problem.md#truncated-singular-value-decomposition).

<h4 id="2/1/c">c</h4>

↑ **Parent:** [1](#2/1)

<h5 id="2/1/c/solution">Solution</h5>

↑ **Parent:** [C](#2/1/c)

Starting from zero, the [Landweber iteration](../../../inverse-problem.md#landweber-iteration) is

$$
\boxed{u_\delta^{(0)}=0,\qquad
u_\delta^{(k+1)}=u_\delta^{(k)}+\tau K^*(f^\delta-Ku_\delta^{(k)}).}
$$

For $K\neq0$, take the [step size](../../../convex-optimization.md#step-size) $0<\tau<2/\|K\|^2$. Iterating the linear update gives

$$
R_{1/k}=\tau\sum_{m=0}^{k-1}(I-\tau K^*K)^mK^*,
$$

and its [Landweber spectral filter](../../../inverse-problem.md#landweber-spectral-filter) in a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) is

$$
\boxed{R_{1/k}f^\delta=
\sum_j\frac{1-(1-\tau\sigma_j^2)^k}{\sigma_j}
\langle f^\delta,w_j\rangle v_j.}
$$

The strict upper [step size](../../../convex-optimization.md#step-size) bound makes $|1-\tau\sigma_j^2|<1$ for every positive [singular value](../../../linear-algebra.md#singular-value). A common more restrictive choice is $0<\tau\leq\|K\|^{-2}$, giving nonnegative damping factors. Each finite iterate is bounded and linear; [early stopping of Landweber iteration](../../../inverse-problem.md#early-stopping-of-landweber-iteration) controls the amplification of noise as smaller [singular values](../../../linear-algebra.md#singular-value) are progressively inverted. If $K=0$, every iterate is zero for any positive [step size](../../../convex-optimization.md#step-size).

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/a">a</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/a/solution">Solution</h5>

↑ **Parent:** [A](#2/2/a)

For [Iterated Tikhonov regularization](../../../inverse-problem.md#iterated-tikhonov-regularization), set $A=K^*K$ and $B=(I+\tau A)^{-1}$. In a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator), each coefficient obeys

$$
c_j^{(k+1)}=\frac{c_j^{(k)}+\tau\sigma_j\langle f^\delta,w_j\rangle}
{1+\tau\sigma_j^2},\qquad c_j^{(0)}=0.
$$

Summing this geometric recurrence gives

$$
\boxed{R_{1/k}f^\delta=u_\delta^{(k)}
=\sum_j\frac{1-(1+\tau\sigma_j^2)^{-k}}{\sigma_j}
\langle f^\delta,w_j\rangle v_j.}
$$

Equivalently, its [iterated Tikhonov spectral filter](../../../inverse-problem.md#iterated-tikhonov-spectral-filter) is $g_k(\lambda)=[1-(1+\tau\lambda)^{-k}]/\lambda$. For $x\geq0$, the finite geometric sum gives

$$
0\leq1-(1+x)^{-k}\leq\min(kx,1).
$$

Consequently the inverse coefficient is at most $\min(k\tau\sigma,1/\sigma)\leq\sqrt{k\tau}$. Thus every $R_{1/k}$ is a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) with

$$
\boxed{\|R_{1/k}\|\leq\sqrt{k\tau}.}
$$

For exact admissible data, write $f_j=\langle f,w_j\rangle$. The [Picard criterion](../../../inverse-problem.md#picard-criterion) gives $\sum_j|f_j|^2/\sigma_j^2<\infty$, and

$$
\|R_{1/k}f-K^\dagger f\|^2
=\sum_j(1+\tau\sigma_j^2)^{-2k}\frac{|f_j|^2}{\sigma_j^2}\longrightarrow0
$$

by [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). Therefore this is a linear [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem) with discrete parameter $\alpha=1/k$; a family for all positive $\alpha$ can be obtained by setting $k=\max(1,\lceil1/\alpha\rceil)$. No upper restriction on the positive [step size](../../../convex-optimization.md#step-size) $\tau$ is needed for this implicit iteration.

<h4 id="2/2/b">b</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/b/solution">Solution</h5>

↑ **Parent:** [B](#2/2/b)

Let $\eta=f^\delta-f$, so $\|\eta\|\leq\delta$. By linearity, $u_\delta^{(k)}-u^{(k)}=R_{1/k}\eta$. The preceding [operator norm](../../../continuous-dual-space.md#operator-norm) estimate gives

$$
\boxed{\|u_\delta^{(k)}-u^{(k)}\|\leq\sqrt{k\tau}\,\delta.}
$$

Moreover, $KR_{1/k}$ has factors $1-(1+\tau\sigma_j^2)^{-k}$ on the data [singular vectors](../../../semisimple-lie-algebra.md#singular-vector), and is zero on $\mathcal R(K)^\perp$. Every factor is in $[0,1]$, hence

$$
\boxed{\|Ku_\delta^{(k)}-Ku^{(k)}\|\leq\delta.}
$$

Thus, for any fixed $k$, one can take $C=\sqrt{k\tau}$ and $\gamma=1$.

**The first constant cannot generally be chosen independently of the iteration count.** On the [l2 sequence space](../../../banach-space.md#l2-sequence-space), take $(Ku)_n=u_n/n$, $\tau=1$, and noise $\eta=\delta e_n$. At $k=n^2$ the solution perturbation has [norm](../../../functional-analysis.md#norm)

$$
\delta n\left[1-\left(1+\frac1{n^2}\right)^{-n^2}\right]
\sim(1-e^{-1})\delta n.
$$

This disproves a uniform-in-$k$ interpretation of the stated first estimate. For a closed [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator), boundedness of the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) instead supplies the uniform constant $\|K^\dagger\|$.

<h4 id="2/2/c">c</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/c/solution">Solution</h5>

↑ **Parent:** [C](#2/2/c)

With exact data $f=Ku^\dagger$, the iteration error obeys

$$
u^{(k)}-u^\dagger=-(I+\tau K^*K)^{-k}u^\dagger.
$$

The [source condition for quadratic regularization](../../../inverse-problem.md#source-condition-for-quadratic-regularization) $u^\dagger=K^*v$ excludes any [null space](../../../linear-algebra.md#kernel-of-a-linear-map) component. Using its [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) coefficients,

$$
\|u^{(k)}-u^\dagger\|^2
=\sum_j\frac{\sigma_j^2}{(1+\tau\sigma_j^2)^{2k}}
|\langle v,w_j\rangle|^2.
$$

By [Bernoulli's inequality](../../../algebra.md#bernoulli-s-inequality), $(1+\tau\sigma^2)^k\geq1+k\tau\sigma^2$. Also $1+k\tau\sigma^2\geq2\sqrt{k\tau}\,\sigma$. Therefore

$$
\frac{\sigma}{(1+\tau\sigma^2)^k}\leq\frac1{2\sqrt{k\tau}}.
$$

Summing the squared coefficients and using [Bessel inequality](../../../hilbert-space.md#bessel-s-inequality) yields

$$
\boxed{\|u^{(k)}-u^\dagger\|
\leq\frac{\|v\|}{2\sqrt{k\tau}}=O(k^{-1/2}).}
$$

This is an a priori error rate from the [source condition for quadratic regularization](../../../inverse-problem.md#source-condition-for-quadratic-regularization), with constant independent of $k$.

<h4 id="2/2/d">d</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/d/solution">Solution</h5>

↑ **Parent:** [D](#2/2/d)

Write the [residual of an inverse problem](../../../inverse-problem.md#residual-of-an-inverse-problem) as $r_k=Ku_\delta^{(k)}-f^\delta$. The iteration can be rearranged as

$$
u_\delta^{(k+1)}-u_\delta^{(k)}=-\tau K^*r_{k+1}.
$$

Applying $K$ gives $(I+\tau KK^*)r_{k+1}=r_k$. Since $KK^*$ is a [positive operator](../../../hilbert-space.md#positive-operator), its [resolvent operator](../../../functional-analysis.md#resolvent-of-an-operator) $(I+\tau KK^*)^{-1}$ has [operator norm](../../../continuous-dual-space.md#operator-norm) at most one. Hence

$$
\boxed{\|r_{k+1}\|\leq\|r_k\|.}
$$

More explicitly, taking the [inner product](../../../linear-algebra.md#inner-product) of the residual equation with $r_{k+1}$ gives

$$
\|r_{k+1}\|^2+\tau\|K^*r_{k+1}\|^2
=\operatorname{Re}\langle r_k,r_{k+1}\rangle
\leq\|r_k\|\,\|r_{k+1}\|.
$$

This directly proves the same monotonicity by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), including the case $r_{k+1}=0$. An unresolvable data component in $\mathcal R(K)^\perp$ remains unchanged.

<h4 id="2/2/e">e</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/e/solution">Solution</h5>

↑ **Parent:** [E](#2/2/e)

Assume $Ku^\dagger=f$, as in the exact-solution setting used for the preceding [source condition for quadratic regularization](../../../inverse-problem.md#source-condition-for-quadratic-regularization). Let $r=r_{k+1}$, $\eta=f^\delta-f$, and $s=u_\delta^{(k+1)}-u_\delta^{(k)}=-\tau K^*r$. Then $K(u_\delta^{(k+1)}-u^\dagger)=r+\eta$, and expanding the two squared errors gives

$$
\begin{aligned}
\|u_\delta^{(k+1)}-u^\dagger\|^2-\|u_\delta^{(k)}-u^\dagger\|^2
&=2\operatorname{Re}\langle s,u_\delta^{(k+1)}-u^\dagger\rangle-\|s\|^2\\
&=-2\tau\operatorname{Re}\langle r,r+\eta\rangle-\|s\|^2\\
&\leq-2\tau\|r\|(\|r\|-\delta)-\|s\|^2.
\end{aligned}
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) supplies the last line. Thus while the residual remains at least the noise bound,

$$
\boxed{\|r_{k+1}\|\geq\delta\ \Longrightarrow\
\|u_\delta^{(k+1)}-u^\dagger\|\leq\|u_\delta^{(k)}-u^\dagger\|.}
$$

**Compatibility of the exact data is essential.** If only $f\in\mathcal D(K^\dagger)$ is retained, let $Kx=(x,0)$, $f=(0,1)$, $f^\delta=(1/2,1)$, $\delta=1/2$ and $\tau=1$. The [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) is zero, but the first iterate is $1/4$ and its residual [norm](../../../functional-analysis.md#norm) is $\sqrt{17}/4>\delta$. Its error has increased from zero. Thus the original assertion uses the implicit exact-data assumption from part (c), and is false without it.

<h4 id="2/2/f">f</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/f/solution">Solution</h5>

↑ **Parent:** [F](#2/2/f)

The [Iterated Tikhonov regularization](../../../inverse-problem.md#iterated-tikhonov-regularization) update is the [proximal operator](../../../convex-optimization.md#proximal-operator) step

$$
\boxed{u_\delta^{(k+1)}=\underset{u\in\mathcal U}{\operatorname{argmin}}
\left\{\frac12\|Ku-f^\delta\|^2
+\frac1{2\tau}\|u-u_\delta^{(k)}\|^2\right\}.}
$$

The objective has [coercivity](../../../real-analysis.md#coercive-function) and is weakly [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity) and [strongly convex](../../../real-analysis.md#strongly-convex-function), so the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) and [uniqueness of a minimizer of a strictly convex function](../../../real-analysis.md#uniqueness-of-a-minimizer-of-a-strictly-convex-function) give existence and uniqueness. Its [gradient](../../../calculus.md#gradient) equation is

$$
K^*(Ku-f^\delta)+\tau^{-1}(u-u_\delta^{(k)})=0,
$$

which is exactly $(I+\tau K^*K)u=u_\delta^{(k)}+\tau K^*f^\delta$. The second term penalizes the change from the previous iterate, rather than the [norm](../../../functional-analysis.md#norm) of $u$ relative to zero.

## 3

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/a">a</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/a/solution">Solution</h5>

↑ **Parent:** [A](#3/1/a)

First interpret the stated well-definedness as including uniqueness of the [global minimizer](../../../analysis.md#global-minimizer) for each positive parameter. Under that assumption, the [parameter continuity of variational regularization](../../../inverse-problem.md#parameter-continuity-of-variational-regularization) follows from the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) argument below.

Let $M=D(0)=\|f\|^2/2$. For large $n$, $\alpha_n\geq\beta:=\alpha/2$. Comparison with zero, using $J(0)=0$, gives

$$
\Phi_{\beta,f}(u_{\alpha_n})\leq\Phi_{\alpha_n,f}(u_{\alpha_n})\leq M,
\qquad J(u_{\alpha_n})\leq M/\beta.
$$

[Coercivity](../../../real-analysis.md#coercive-function) of $\Phi_{\beta,f}$ therefore bounds the sequence. Take a $\tau$-[convergent subsequence](../../../real-analysis.md#convergent-subsequence) with limit $\bar u$. For any $v\in\operatorname{dom}J$, optimality gives

$$
\Phi_{\alpha,f}(u_{\alpha_n})
\leq\Phi_{\alpha,f}(v)
+(\alpha_n-\alpha)J(v)+(\alpha-\alpha_n)J(u_{\alpha_n}).
$$

The last two terms vanish. [Sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity) at the fixed parameter $\alpha$ implies $\Phi_{\alpha,f}(\bar u)\leq\Phi_{\alpha,f}(v)$. Thus every cluster point is a [global minimizer](../../../analysis.md#global-minimizer) at $\alpha$. Uniqueness makes it $u_\alpha$, and the subsequence property proves

$$
\boxed{u_{\alpha_n}\xrightarrow{\tau}u_\alpha.}
$$

Indeed, a subsequence staying outside a neighborhood of $u_\alpha$ would have a further convergent subsequence, whose limit must be $u_\alpha$, a contradiction.

**The listed existence hypotheses alone do not imply uniqueness or convergence of an arbitrary selection.** For example, on $\mathbb R^2$, set $K(x,y)=x$, $f=1$, and

$$
J(x,y)=x^2+\bigl(\max\{|y|-1,0\}\bigr)^2.
$$

This is nonnegative, [convex](../../../real-analysis.md#convex-function), [continuous](../../../calculus.md#continuous-function) and has $J(0)=0$; every $\Phi_{\alpha,f}$ has [coercivity](../../../real-analysis.md#coercive-function). Its minimizers are $(1/(1+2\alpha),y)$ for all $|y|\leq1$. Along $\alpha_n=\alpha+1/n$, selecting $y_n=(-1)^n$ prevents convergence. Without uniqueness, the valid conclusion is that every cluster point minimizes the limiting objective.

<h4 id="3/1/b">b</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/b/solution">Solution</h5>

↑ **Parent:** [B](#3/1/b)

Use the [value function of variational regularization](../../../inverse-problem.md#value-function-of-variational-regularization) in its selection-independent form

$$
\Psi(\alpha)=\inf_u\{D(u)+\alpha J(u)\},\qquad 0\leq\Psi(\alpha)\leq M:=D(0).
$$

Because $J\geq0$, each objective is non-decreasing with $\alpha$, hence so is its [infimum](../../../real-analysis.md#infimum). For $0\leq t\leq1$, the [affine function](../../../vector-space.md#affine-function) of the parameter at each fixed $u$ gives

$$
\begin{aligned}
\Psi(t\alpha+(1-t)\beta)
&=\inf_u\{t\Phi_{\alpha,f}(u)+(1-t)\Phi_{\beta,f}(u)\}\\
&\geq t\Psi(\alpha)+(1-t)\Psi(\beta).
\end{aligned}
$$

Thus $\Psi$ is [concave](../../../real-analysis.md#concave-function).

For continuity, on any interval $0<a\leq\alpha<\beta\leq b$, comparison using $u_\alpha$ gives

$$
0\leq\Psi(\beta)-\Psi(\alpha)
\leq(\beta-\alpha)J(u_\alpha)
\leq\frac{M}{a}(\beta-\alpha).
$$

It follows that $\Psi$ is a [locally Lipschitz function](../../../real-analysis.md#locally-lipschitz-function), hence [continuous](../../../calculus.md#continuous-function), on $(0,\infty)$. Therefore **the [value function of variational regularization](../../../inverse-problem.md#value-function-of-variational-regularization) is non-decreasing, [concave](../../../real-analysis.md#concave-function) and [continuous](../../../calculus.md#continuous-function)**. No uniqueness of minimizers is needed for these conclusions.

<h4 id="3/1/c">c</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/c/solution">Solution</h5>

↑ **Parent:** [C](#3/1/c)

For $0<\alpha<\beta$, abbreviate $D_\alpha=D(u_\alpha)$ and $J_\alpha=J(u_\alpha)$. Optimality of the two [variational regularization](../../../inverse-problem.md#variational-regularization) solutions gives

$$
D_\alpha+\alpha J_\alpha\leq D_\beta+\alpha J_\beta,\qquad
D_\beta+\beta J_\beta\leq D_\alpha+\beta J_\alpha.
$$

Adding shows $(\beta-\alpha)(J_\beta-J_\alpha)\leq0$, so $J_\beta\leq J_\alpha$. Rearranging each comparison then gives the [monotonicity of data fidelity and regularization penalty](../../../inverse-problem.md#monotonicity-of-data-fidelity-and-regularization-penalty)

$$
\boxed{0\leq\alpha(J_\alpha-J_\beta)
\leq D_\beta-D_\alpha
\leq\beta(J_\alpha-J_\beta).}
$$

Hence **the regulariser value is non-increasing and the data misfit is non-decreasing with the parameter**. These inequalities hold for any choices of minimizers at the two distinct parameters, including when uniqueness fails.

<h4 id="3/1/d">d</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/d/solution">Solution</h5>

↑ **Parent:** [D](#3/1/d)

Comparison with zero and nonnegativity of the two terms gives

$$
0\leq D(u_\alpha)+\alpha J(u_\alpha)
\leq D(0)+\alpha J(0)=\frac12\|f\|^2.
$$

Therefore

$$
\boxed{0\leq J(u_\alpha)\leq\frac{\|f\|^2}{2\alpha},\qquad
J(u_\alpha)\longrightarrow0\quad(\alpha\to\infty).}
$$

For a concrete [variational regularization](../../../inverse-problem.md#variational-regularization) example, take a [Hilbert space](../../../hilbert-space.md) and $J(u)=\|u\|^2$. The bound forces $u_\alpha\to0$ in [norm](../../../functional-analysis.md#norm). Since $K$ is a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator), $Ku_\alpha\to0$, and continuity of the squared [norm](../../../functional-analysis.md#norm) gives

$$
\boxed{D(u_\alpha)\longrightarrow\tfrac12\|f\|^2.}
$$

The same conclusion is not forced by $J(u_\alpha)\to0$ for a regulariser with a nontrivial zero set.

<h4 id="3/1/e">e</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/e/solution">Solution</h5>

↑ **Parent:** [E](#3/1/e)

The small-parameter limit depends on [data compatibility with the regularizer domain](../../../inverse-problem.md#data-compatibility-with-the-regularizer-domain). Set

$$
m=\inf_{v\in\operatorname{dom}J}D(v),\qquad 0\leq m\leq D(0).
$$

For every such $v$, optimality gives

$$
m\leq D(u_\alpha)\leq\Phi_{\alpha,f}(u_\alpha)
\leq D(v)+\alpha J(v).
$$

Taking the upper limit as $\alpha\downarrow0$ and then the [infimum](../../../real-analysis.md#infimum) over $v$ proves $\Phi_{\alpha,f}(u_\alpha)\to m$. Its two nonnegative contributions above $m$ must vanish, yielding the general result

$$
\boxed{D(u_\alpha)\longrightarrow m,\qquad
\alpha J(u_\alpha)\longrightarrow0.}
$$

In particular, the requested zero-misfit limit holds when $f\in\overline{K(\operatorname{dom}J)}$. A sufficient condition is an exact solution $v$ with $Kv=f$ and $J(v)<\infty$; then

$$
0\leq D(u_\alpha)\leq\alpha J(v),\qquad
0\leq\alpha J(u_\alpha)\leq\alpha J(v)\longrightarrow0.
$$

**Membership of $f$ in $\mathcal R(K)$ alone is insufficient.** Take $\mathcal U=\mathcal V=\mathbb R$, $K=I$, $f=1$, and $J$ the [indicator functional of a constraint set](../../../inverse-problem.md#indicator-functional-of-a-constraint-set) $\{0\}$. All positive-parameter objectives are [proper extended-real functions](../../../real-analysis.md#proper-extended-real-function) with [coercivity](../../../real-analysis.md#coercive-function) and [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity), with the unique minimizer $u_\alpha=0$, yet $D(u_\alpha)=1/2$ for every $\alpha$. Thus the first printed limit needs compatibility with the regulariser's [effective domain](../../../real-analysis.md#effective-domain); the second limit remains true under the given assumptions.

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/a">a</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/a/solution">Solution</h5>

↑ **Parent:** [A](#3/2/a)

For a [functional](../../../calculus-of-variations.md#functional) $E$ on a real [Banach space](../../../banach-space.md), its [convex conjugate](../../../convex-optimization.md#convex-conjugate) is defined on the [dual space](../../../linear-algebra.md#dual-space) by

$$
\boxed{E^*(p)=\sup_{u\in\mathcal U}\{\langle p,u\rangle-E(u)\},\qquad p\in\mathcal U^*.}
$$

Here $\langle p,u\rangle$ is the [dual pairing](../../../continuous-dual-space.md#dual-pairing). For complex spaces, use its real part, equivalently regard the space as real for [convex analysis](../../../convex-optimization.md#convex-analysis). The [convex conjugate](../../../convex-optimization.md#convex-conjugate) is a [convex function](../../../real-analysis.md#convex-function), being the supremum of [affine functions](../../../vector-space.md#affine-function) of $p$, even when $E$ itself is not [convex](../../../real-analysis.md#convex-function).

<h4 id="3/2/b">b</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/b/solution">Solution</h5>

↑ **Parent:** [B](#3/2/b)

Let $G=E\mathbin\square F$. To prove [convexity](../../../real-analysis.md#convex-function), take $u_1,u_2$ with finite $G$ values, $0<t<1$, and $\varepsilon>0$. By the definition of [infimum](../../../real-analysis.md#infimum), choose $v_i$ with

$$
E(v_i)+F(u_i-v_i)\leq G(u_i)+\varepsilon.
$$

Put $u_t=tu_1+(1-t)u_2$ and $v_t=tv_1+(1-t)v_2$. [Convexity](../../../real-analysis.md#convex-function) of $E$ and $F$ gives

$$
\begin{aligned}
G(u_t)&\leq E(v_t)+F(u_t-v_t)\\
&\leq t[E(v_1)+F(u_1-v_1)]
+(1-t)[E(v_2)+F(u_2-v_2)]\\
&\leq tG(u_1)+(1-t)G(u_2)+\varepsilon.
\end{aligned}
$$

Let $\varepsilon\downarrow0$. If either endpoint value is infinite, the convexity inequality is automatic, and $t=0,1$ gives equality. Thus **the [infimal convolution](../../../convex-optimization.md#infimal-convolution) of two [convex functions](../../../real-analysis.md#convex-function) is [convex](../../../real-analysis.md#convex-function)** under the stated properness assumption. The proof uses approximate minimizing splits, so no attainment of the inner [infimum](../../../real-analysis.md#infimum) is assumed.

<h4 id="3/2/c">c</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/c/solution">Solution</h5>

↑ **Parent:** [C](#3/2/c)

For $p\in\mathcal U^*$, the definition of the [convex conjugate](../../../convex-optimization.md#convex-conjugate) gives

$$
\begin{aligned}
(E\mathbin\square F)^*(p)
&=\sup_u\sup_v\{\langle p,u\rangle-E(v)-F(u-v)\}\\
&=\sup_{v,w}\{\langle p,v\rangle-E(v)+\langle p,w\rangle-F(w)\}\\
&=E^*(p)+F^*(p),
\end{aligned}
$$

where the substitution $w=u-v$ is a bijection of the independent pairs. Therefore

$$
\boxed{(E\mathbin\square F)^*=E^*+F^*.}
$$

This [infimal convolution](../../../convex-optimization.md#infimal-convolution) identity does not need [convexity](../../../real-analysis.md#convex-function) of $E,F$ or attainment of the inner [infimum](../../../real-analysis.md#infimum). The assumptions ensure that both functions have nonempty [effective domains](../../../real-analysis.md#effective-domain); their conjugates never take $-\infty$, so the separated sum is well defined, allowing $+\infty$.

<h4 id="3/2/d">d</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/d/solution">Solution</h5>

↑ **Parent:** [D](#3/2/d)

Write $\iota_C$ for the [indicator functional of a constraint set](../../../inverse-problem.md#indicator-functional-of-a-constraint-set) $C$ and $q(u)=\|u\|^2/2$. Then

$$
d_C=\iota_C\mathbin\square q.
$$

Both terms are [convex](../../../real-analysis.md#convex-function), hence their [infimal convolution](../../../convex-optimization.md#infimal-convolution) is the [convex](../../../real-analysis.md#convex-function) [squared distance to a convex set](../../../convex-optimization.md#squared-distance-to-a-convex-set). The [closest point theorem in a Hilbert space](../../../hilbert-space.md#hilbert-projection-theorem) supplies the unique [metric projection onto a closed convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) $P_Cu$ and gives $d_C(u)=\|u-P_Cu\|^2/2$.

Identify the [Hilbert space](../../../hilbert-space.md) with its [dual space](../../../linear-algebra.md#dual-space) using the [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem). Completing the square yields $q^*(p)=\|p\|^2/2$, while $\iota_C^*(p)=\sup_{v\in C}\langle p,v\rangle=\sigma_C(p)$ is the [support function](../../../mathematical-optimization.md#support-function). The [conjugate of the squared distance to a convex set](../../../convex-optimization.md#conjugate-of-the-squared-distance-to-a-convex-set) is therefore

$$
\boxed{d_C^*(p)=\frac12\|p\|^2+\sigma_C(p).}
$$

For the closed unit ball, the [metric projection onto a closed convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) is $P_Cu=u$ if $\|u\|\leq1$, and $P_Cu=u/\|u\|$ otherwise. Therefore

$$
\boxed{d_C(u)=\frac12\bigl(\max\{\|u\|-1,0\}\bigr)^2,\qquad
d_C^*(p)=\frac12\|p\|^2+\|p\|.}
$$

The last equality uses the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) to compute the unit ball's [support function](../../../mathematical-optimization.md#support-function), attained in the direction of $p$ when $p\neq0$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
