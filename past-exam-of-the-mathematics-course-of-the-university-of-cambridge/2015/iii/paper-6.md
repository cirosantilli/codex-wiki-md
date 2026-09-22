# Paper 6

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_6.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_6.pdf)

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
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For $1\leq p<\infty$, the real [Lp space](../../../measure-theory.md#lp-space) is the [vector space](../../../vector-space.md) of real [measurable functions](../../../measure-theory.md#measurable-function) with $\int_\Omega|f|^p\,d\mu<\infty$, identifying functions equal [almost everywhere](../../../measure-theory.md#almost-everywhere). Its [Lp norm](../../../real-analysis.md#lp-norm) is $\|f\|_p=(\int|f|^p\,d\mu)^{1/p}$. For $p=\infty$, take the essentially bounded real [measurable functions](../../../measure-theory.md#measurable-function), with the same identification and [norm](../../../functional-analysis.md#norm) $\|f\|_\infty=\operatorname{ess\,sup}|f|$. The identification makes each [norm](../../../functional-analysis.md#norm) definite; absolute homogeneity follows from the [Lebesgue integral](../../../measure-theory.md#lebesgue-integral), and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) follows from [Minkowski inequality](../../../real-analysis.md#minkowski-inequality) for finite $p$, or directly from the [essential supremum](../../../measure-theory.md#essential-supremum) for $p=\infty$.

Here is a [completeness](../../../topological-analysis.md#completeness) proof valid on any [measure space](../../../measure-theory.md#measure-space). For $p<\infty$, a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) $(f_n)$ has a [subsequence](../../../real-analysis.md#subsequence) $(f_{n_k})$ with $\|f_{n_{k+1}}-f_{n_k}\|_p\leq2^{-k}$. Choose [measurable function](../../../measure-theory.md#measurable-function) representatives and put $h_k=f_{n_{k+1}}-f_{n_k}$. By [Minkowski inequality](../../../real-analysis.md#minkowski-inequality) and the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem),

$$
\left\|\sum_{k=1}^N|h_k|\right\|_p\leq\sum_{k=1}^N2^{-k}\leq1,
\qquad
\int\left(\sum_{k=1}^\infty|h_k|\right)^p\,d\mu\leq1.
$$

Consequently the [series](../../../real-analysis.md#series-mathematics) $\sum h_k$ converges absolutely [almost everywhere](../../../measure-theory.md#almost-everywhere). Define $f=f_{n_1}+\sum h_k$ there, and define it to be zero on the measurable exceptional null set. Then $f\in L^p$, and [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) applied to each tail gives $\|f-f_{n_k}\|_p\leq\sum_{j=k}^\infty2^{-j}\to0$. The original [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) also converges in [Lp norm](../../../real-analysis.md#lp-norm), by the [triangle inequality](../../../topological-analysis.md#triangle-inequality). For $p=\infty$, choose the same [subsequence](../../../real-analysis.md#subsequence) using the [essential supremum](../../../measure-theory.md#essential-supremum) [norm](../../../functional-analysis.md#norm). Outside one measurable null set, all the bounds $|h_k|\leq2^{-k}$ hold and $f_{n_1}$ is bounded. The [series](../../../real-analysis.md#series-mathematics) then converges uniformly there, with an essentially bounded [measurable function](../../../measure-theory.md#measurable-function) limit and the same tail estimate in [essential supremum](../../../measure-theory.md#essential-supremum) [norm](../../../functional-analysis.md#norm). Thus **all these spaces are [Banach spaces](../../../banach-space.md)**.

The [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces) says that, for $1<p<\infty$ and $q=p/(p-1)$, the map

$$
I_p:L^q\longrightarrow(L^p)^*,\qquad (I_pg)(f)=\int fg\,d\mu
$$

is an [isometric isomorphism of normed spaces](../../../functional-analysis.md#isometric-isomorphism-of-normed-spaces). This form of [Lp duality on an arbitrary measure space](../../../continuous-dual-space.md#lp-duality-on-an-arbitrary-measure-space) requires no finiteness hypothesis on $\mu$. At $p=1$, a standard version assumes a [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) and identifies $(L^1)^*$ with $L^\infty$ through the same [dual pairing](../../../continuous-dual-space.md#dual-pairing). That endpoint assertion must not be made without a suitable measure-space hypothesis.

We first prove the required [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces) for a [finite measure](../../../measure-theory.md#finite-measure). Let $F\in(L^p)^*$ and set $\nu(E)=F(\mathbf1_E)$. For disjoint measurable $E_j$, the [indicator functions](../../../measure-theory.md#indicator-function) of their partial unions converge in [Lp norm](../../../real-analysis.md#lp-norm) to that of their union, so $\nu$ is countably additive. It has finite [variation measure](../../../measure-theory.md#variation-measure): for every finite measurable partition $(E_j)$, choosing real signs gives

$$
\sum_j|\nu(E_j)|=F\left(\sum_j\operatorname{sgn}(\nu(E_j))\mathbf1_{E_j}\right)
\leq\|F\|\mu(\Omega)^{1/p}.
$$

Also $\mu(E)=0$ implies $\nu(E)=0$. The [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem) supplies a [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) $g\in L^1$ with $\nu(E)=\int_Eg\,d\mu$. Linearity gives $F(f)=\int fg\,d\mu$ for [simple functions](../../../measure-theory.md#simple-function). Uniform approximation by [simple functions](../../../measure-theory.md#simple-function) extends this identity to bounded [measurable functions](../../../measure-theory.md#measurable-function): both their [Lp norm](../../../real-analysis.md#lp-norm) errors and the errors in integration against $g$ tend to zero.

To establish the correct [integrability](../../../measure-theory.md#integrability), test with the bounded [measurable function](../../../measure-theory.md#measurable-function) $f_N=\operatorname{sgn}(g)|g|^{q-1}\mathbf1_{\{|g|\leq N\}}$. Since $(q-1)p=q$, writing $A_N=\int_{\{|g|\leq N\}}|g|^q\,d\mu$ gives

$$
A_N=F(f_N)\leq\|F\|A_N^{1/p},\qquad A_N^{1/q}\leq\|F\|.
$$

The second inequality is also valid when $A_N=0$. The [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) gives $g\in L^q$ and $\|g\|_q\leq\|F\|$. Density of [simple functions](../../../measure-theory.md#simple-function) in the [Lp space](../../../measure-theory.md#lp-space), together with [Hölder's inequality](../../../real-analysis.md#holder-s-inequality), now gives $F=I_pg$ on all of $L^p$. Conversely [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) gives $\|I_pg\|\leq\|g\|_q$. If $g\ne0$, testing against

$$
f=\frac{\operatorname{sgn}(g)|g|^{q-1}}{\|g\|_q^{q-1}}
$$

gives $\|f\|_p=1$ and $(I_pg)(f)=\|g\|_q$, so **$\boxed{\|I_pg\|=\|g\|_q}$**. This also proves uniqueness of the representing [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative).

For completeness, the passage to an arbitrary [measure space](../../../measure-theory.md#measure-space) can be made without losing a hypothesis in the [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space) argument below. On a [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) space, exhaust by nested finite-measure sets $E_n$. The representing [Radon-Nikodym derivatives](../../../measure-theory.md#radon-nikodym-derivative) on $E_n$ agree on overlaps by uniqueness. Their glued density has [Lp norm](../../../real-analysis.md#lp-norm) $\|g\|_q\leq\|F\|$ by the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem), and represents $F$ because $f\mathbf1_{E_n}\to f$ in [Lp norm](../../../real-analysis.md#lp-norm). Every $f\in L^p$ on an arbitrary [measure space](../../../measure-theory.md#measure-space) is supported on a sigma-finite measurable set: the sets $\{|f|>1/n\}$ have finite measure and their union is $\{f\ne0\}$.

Use [support localization of an Lp functional](../../../continuous-dual-space.md#support-localization-of-an-lp-functional) as follows. For a sigma-finite measurable $A$, let $m_A$ be the [operator norm](../../../continuous-dual-space.md#operator-norm) of $F$ restricted to functions supported in $A$. The support observation gives $\sup_A m_A=\|F\|$. Choose $A_n$ approaching this supremum and set $A=\bigcup_nA_n$; then $m_A=\|F\|$. If a sigma-finite $B\subseteq\Omega\setminus A$ had $m_B=\beta>0$, functions supported on the disjoint sets $A,B$ have the direct-sum [Lp norm](../../../real-analysis.md#lp-norm). Optimizing their two scalar coefficients by [Hölder's inequality](../../../real-analysis.md#holder-s-inequality), and using functions approaching the two restriction [operator norms](../../../continuous-dual-space.md#operator-norm), would give

$$
\|F\|\geq(m_A^q+\beta^q)^{1/q}>m_A,
$$

a contradiction. Thus $F$ vanishes on functions supported outside $A$. The density on $A$, extended by zero, represents $F$ globally. The case $F=0$ simply uses $g=0$. This proves the stated [Lp duality on an arbitrary measure space](../../../continuous-dual-space.md#lp-duality-on-an-arbitrary-measure-space).

Finally let $X=L^p$ and let $\Phi\in X^{**}$, where stars denote [continuous dual spaces](../../../continuous-dual-space.md). Compose with $I_p$ to obtain the [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $g\mapsto\Phi(I_pg)$ on $L^q$. Applying [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces) with the exponents reversed gives $f\in L^p$ with $\Phi(I_pg)=\int fg\,d\mu$. For the [canonical embedding into the bidual](../../../functional-analysis.md#canonical-embedding-into-the-bidual) $J_Xf$, its value on $I_pg$ is also $\int fg\,d\mu$. Since $I_p$ is onto, $\Phi=J_Xf$. Its [norm](../../../functional-analysis.md#norm) is $\|f\|_p$ by the same [dual pairing](../../../continuous-dual-space.md#dual-pairing) [norm](../../../functional-analysis.md#norm) identity. Therefore **$\boxed{J_X(L^p)=(L^p)^{**}}$**, which proves that $L^p$ is a [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space) through its actual [canonical embedding into the bidual](../../../functional-analysis.md#canonical-embedding-into-the-bidual).

## 2

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [weak topology](../../../weak-topology.md) on a [normed vector space](../../../functional-analysis.md#normed-vector-space) $X$ is $\sigma(X,X^*)$, the coarsest [topology](../../../topology.md) making every [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) continuous. A neighbourhood base at $x$ is given by finitely many inequalities $|f_j(y-x)|<\varepsilon$, with $f_j\in X^*$. In the complex case, separation uses [real parts](../../../complex-analysis.md#real-part) of [bounded linear functionals](../../../topological-vector-space.md#continuous-linear-functional).

[Mazur theorem](../../../hilbert-space.md#mazur-theorem) states that the [weak closure](../../../weak-topology.md#weak-closure) of a [convex set](../../../mathematical-optimization.md#convex-set) equals its closure in the [norm topology](../../../functional-analysis.md#norm-topology). The [weak topology](../../../weak-topology.md) is coarser than the [norm topology](../../../functional-analysis.md#norm-topology), so the norm closure is contained in the [weak closure](../../../weak-topology.md#weak-closure). Conversely, if $x$ is outside the norm closure of a [convex set](../../../mathematical-optimization.md#convex-set) $C$, the [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) gives $f\in X^*$ and $a\in\mathbb R$ with $\operatorname{Re}f(x)>a\geq\sup_{c\in C}\operatorname{Re}f(c)$. The corresponding [weak topology](../../../weak-topology.md) neighbourhood of $x$ misses $C$, so $x$ is outside its [weak closure](../../../weak-topology.md#weak-closure). This proves [Mazur theorem](../../../hilbert-space.md#mazur-theorem), including the empty-set case. In particular, if $x_n$ converges weakly to $x$, then $x$ is in the [weak closure](../../../weak-topology.md#weak-closure) of every tail and therefore in the norm closure of its [convex hull](../../../mathematical-optimization.md#convex-hull). Choosing a finite [convex combination](../../../mathematical-optimization.md#convex-combination) of the $n$th tail within $1/n$ of $x$ proves the usual [Mazur lemma](../../../hilbert-space.md#mazur-s-lemma) formulation as well.

The [weak-star topology](../../../weak-topology.md#weak-star-topology) on the [continuous dual space](../../../continuous-dual-space.md) $X^*$ is $\sigma(X^*,X)$: convergence means pointwise convergence on $X$, and a neighbourhood base prescribes finitely many evaluation inequalities. The [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) states that the [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of $X^*$ is compact in this [weak-star topology](../../../weak-topology.md#weak-star-topology), even if $X$ is incomplete. Embed this [closed unit ball](../../../functional-analysis.md#closed-unit-ball) into

$$
P=\prod_{x\in X}\{z\in\mathbb K:|z|\leq\|x\|\},\qquad f\longmapsto(f(x))_{x\in X},
$$

where $\mathbb K=\mathbb R$ or $\mathbb C$. Each factor is compact, so $P$ is compact by the [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem). Inside $P$, the equations $a_{x+y}=a_x+a_y$ and $a_{\lambda x}=\lambda a_x$ define a [closed set](../../../topology.md#closed-set). Every such point defines a [linear functional](../../../linear-algebra.md#linear-functional) satisfying $|a_x|\leq\|x\|$, hence belongs to the [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of $X^*$. Thus this image is closed in $P$. The [product topology](../../../geometry-and-topology.md#product-topology) on it is exactly the [weak-star topology](../../../weak-topology.md#weak-star-topology), proving [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem). Evaluations also separate its points, so the [weak-star topology](../../../weak-topology.md#weak-star-topology) is Hausdorff.

For the [canonical embedding into the bidual](../../../functional-analysis.md#canonical-embedding-into-the-bidual) $J_X:X\to X^{**}$, we have $(J_Xx)(f)=f(x)$. Restricting all evaluations at $f\in X^*$ therefore gives exactly $\sigma(X,X^*)$. Thus **the induced [subspace topology](../../../topology.md#subspace-topology) is the [weak topology](../../../weak-topology.md) on $X$**.

Now identify $X$ with $J_XX$. Let $C$ be a bounded [convex set](../../../mathematical-optimization.md#convex-set), write $D$ for its norm closure in $X$, and let $K$ be its [weak-star topology](../../../weak-topology.md#weak-star-topology) closure in $X^{**}$. Boundedness places $K$ in a multiple of the [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of $X^{**}$, so $K$ is compact by [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem). The preceding [subspace topology](../../../topology.md#subspace-topology) identification and [Mazur theorem](../../../hilbert-space.md#mazur-theorem) give

$$
K\cap X=\overline C^{\,w}=D.
$$

If $D$ is a [weakly compact set](../../../weak-topology.md#weakly-compact-set), its image in the Hausdorff [weak-star topology](../../../weak-topology.md#weak-star-topology) is compact and therefore closed. It contains $C$, so $K\subseteq D\subseteq X$. Conversely, if $K\subseteq X$, the displayed identity gives $K=D$, and its compactness is precisely weak compactness in $X$. Hence **$\boxed{D\text{ is weakly compact}\iff K\subseteq X}$**. This argument also covers $C=\varnothing$.

For a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) $T:X\to Y$, its [Banach-space adjoint](../../../continuous-dual-space.md#transpose-of-a-bounded-linear-operator) is $T^*:Y^*\to X^*$, defined by $(T^*y^*)(x)=y^*(Tx)$. Evaluation at any fixed $x$ is thus evaluation at $Tx$ after applying $T^*$. Each is continuous in the relevant [weak-star topology](../../../weak-topology.md#weak-star-topology), proving that **$T^*$ is weak-star continuous**. Applying the same result to $T^*$ shows that $T^{**}:X^{**}\to Y^{**}$ is weak-star continuous. Direct evaluation gives

$$
T^{**}J_X=J_YT.
$$

Use $B_X$ for the [closed unit ball](../../../functional-analysis.md#closed-unit-ball); using the open ball gives the same norm closure of $T(B_X)$. [Goldstine theorem](../../../functional-analysis.md#goldstine-theorem) says that $J_XB_X$ is weak-star dense in $B_{X^{**}}$. Put $K=T^{**}(B_{X^{**}})$. It is compact and closed in the [weak-star topology](../../../weak-topology.md#weak-star-topology) by [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) and the established continuity. It contains $J_YT(B_X)$. Conversely, [Goldstine theorem](../../../functional-analysis.md#goldstine-theorem) gives, for every $x^{**}\in B_{X^{**}}$, a [net](../../../topology.md#net-mathematics) $(J_Xx_\alpha)$ from $J_XB_X$ converging weak-star to $x^{**}$; its image converges weak-star to $T^{**}x^{**}$. Consequently

$$
\overline{J_YT(B_X)}^{\,w^*}=T^{**}(B_{X^{**}}).
$$

Apply the preceding bounded [convex set](../../../mathematical-optimization.md#convex-set) criterion in $Y$, and then scale the [closed unit ball](../../../functional-analysis.md#closed-unit-ball). We obtain the [bidual characterization of weakly compact operators](../../../functional-analysis.md#bidual-characterization-of-weakly-compact-operators):

$$
\boxed{\overline{T(B_X)}^{\,\|\cdot\|}\text{ is weakly compact}
\iff T^{**}(X^{**})\subseteq J_YY.}
$$

The [canonical embedding into the bidual](../../../functional-analysis.md#canonical-embedding-into-the-bidual) on the right specifies exactly which copy of $Y$ is intended.

## 3

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

All [vector spaces](../../../vector-space.md) in this solution are complex, while [convex combinations](../../../mathematical-optimization.md#convex-combination) use real coefficients. An [extreme point](../../../mathematical-optimization.md#extreme-point) $x$ of a [convex set](../../../mathematical-optimization.md#convex-set) $C$ is one for which $x=ty+(1-t)z$, $y,z\in C$ and $0<t<1$, forces $y=z=x$. Equivalently, $x$ is not the midpoint of two distinct points of $C$.

The [Krein-Milman theorem](../../../functional-analysis.md#krein-milman-theorem) says that every nonempty compact [convex set](../../../mathematical-optimization.md#convex-set) $K$ in a Hausdorff [locally convex space](../../../topological-vector-space.md#locally-convex-space) is the [closed convex hull](../../../mathematical-optimization.md#closed-convex-hull) of its [extreme points](../../../mathematical-optimization.md#extreme-point). Here is a proof. A [face of a convex set](../../../mathematical-optimization.md#face-of-a-convex-set) $F\subseteq K$ is a [convex set](../../../mathematical-optimization.md#convex-set) such that whenever an interior point of a segment in $K$ belongs to $F$, both endpoints belong to $F$. Consider nonempty compact faces, ordered by reverse inclusion. A chain has nonempty intersection by compactness and the [finite intersection property](../../../topology.md#finite-intersection-property); that intersection is again a compact face. The [Zorn lemma](../../../set-theory.md#zorn-s-lemma) therefore gives a minimal nonempty compact face $F$.

If $F$ contains distinct $x,y$, a continuous real [linear functional](../../../linear-algebra.md#linear-functional) $\ell$ on the underlying real [locally convex space](../../../topological-vector-space.md#locally-convex-space) distinguishes them. Such a [linear functional](../../../linear-algebra.md#linear-functional) exists because the space is Hausdorff and locally convex, by the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem). The maximizers of $\ell$ on $F$ form a nonempty proper compact face of $F$. A face of a face is a face of $K$, contradicting minimality. Therefore $F$ is a singleton, yielding an [extreme point](../../../mathematical-optimization.md#extreme-point). The same argument inside any nonempty compact face of $K$ supplies an [extreme point](../../../mathematical-optimization.md#extreme-point) of $K$ lying in that face.

Let $D$ be the [closed convex hull](../../../mathematical-optimization.md#closed-convex-hull) of the [extreme points](../../../mathematical-optimization.md#extreme-point) of $K$. It is a nonempty closed subset of compact $K$, hence compact. If $x_0\in K\setminus D$, the [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem) provides a continuous real [linear functional](../../../linear-algebra.md#linear-functional) $\ell$ with $\ell(x_0)>\sup_D\ell$. Its maximizer set on $K$ is a nonempty compact face, which contains an [extreme point](../../../mathematical-optimization.md#extreme-point) $e$ of $K$. But $e\in D$ and $\ell(e)\geq\ell(x_0)>\sup_D\ell$, a contradiction. Thus **$\boxed{K=\overline{\operatorname{co}}(\operatorname{ext}K)}$**, proving [Krein-Milman theorem](../../../functional-analysis.md#krein-milman-theorem).

For a nonempty compact [Hausdorff space](../../../topology.md#hausdorff-space) $K$, the [extreme points of the dual unit ball of C(K)](../../../functional-analysis.md#extreme-points-of-the-dual-unit-ball-of-c-k) are

$$
\boxed{\operatorname{ext}B_{C(K)^*}=\{\alpha\delta_x:x\in K,\ |\alpha|=1\},}
\qquad \delta_x(f)=f(x).
$$

This is the permitted description without proof, with $C(K)$ denoting the complex [space of continuous functions on a compact space](../../../functional-analysis.md#space-of-continuous-functions-on-a-compact-space) equipped with the [supremum norm](../../../functional-analysis.md#supremum-norm). If $K$ is empty, $C(K)=\{0\}$ and the [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of its [continuous dual space](../../../continuous-dual-space.md) has the single [extreme point](../../../mathematical-optimization.md#extreme-point) $0$ instead.

The complex [Banach–Stone theorem](../../../functional-analysis.md#banach-stone-theorem) states that a surjective complex-linear [isometric isomorphism of normed spaces](../../../functional-analysis.md#isometric-isomorphism-of-normed-spaces) $T:C(K)\to C(L)$ has the form

$$
\boxed{(Tf)(y)=u(y)f(\varphi(y)),\qquad |u(y)|=1,}
$$

where $u\in C(L)$ and $\varphi:L\to K$ is a [homeomorphism](../../../topology.md#homeomorphism). Conversely, every such map is a surjective complex-linear [isometric isomorphism of normed spaces](../../../functional-analysis.md#isometric-isomorphism-of-normed-spaces) for the [supremum norm](../../../functional-analysis.md#supremum-norm).

To prove this, suppose first that $K,L$ are nonempty. The [Banach-space adjoint](../../../continuous-dual-space.md#transpose-of-a-bounded-linear-operator) $T^*$ is a bijective [isometric isomorphism of normed spaces](../../../functional-analysis.md#isometric-isomorphism-of-normed-spaces) on the [continuous dual spaces](../../../continuous-dual-space.md), so it bijects their [closed unit balls](../../../functional-analysis.md#closed-unit-ball) and preserves [extreme points](../../../mathematical-optimization.md#extreme-point). The displayed [extreme point](../../../mathematical-optimization.md#extreme-point) description gives uniquely

$$
T^*\delta_y=u(y)\delta_{\varphi(y)},\qquad |u(y)|=1.
$$

Uniqueness follows by evaluating at the constant function $1$, and then using that [continuous functions](../../../calculus.md#continuous-function) separate points of a compact [Hausdorff space](../../../topology.md#hausdorff-space). Evaluation gives the required formula for $Tf$, and $u=T1$ is continuous. Surjectivity of $T^*$ on [extreme points](../../../mathematical-optimization.md#extreme-point) proves surjectivity of $\varphi$: the preimage of any $\delta_x$ is $\alpha\delta_y$ for some $y$. If $\varphi(y_1)=\varphi(y_2)$, every function in the range of $T$ has equal values at these two points after division by $u$; surjectivity of $T$ and separation of points force $y_1=y_2$. Thus $\varphi$ is bijective.

For every $f\in C(K)$, $f\circ\varphi=(Tf)/u$ is continuous. The evaluation map $K\to\mathbb C^{C(K)}$, $x\mapsto(f(x))_f$, is a continuous injection of a compact [Hausdorff space](../../../topology.md#hausdorff-space) into a Hausdorff [product topology](../../../geometry-and-topology.md#product-topology), hence a [homeomorphism](../../../topology.md#homeomorphism) onto its image. Continuity of every coordinate $f\circ\varphi$ proves continuity of $\varphi$. A continuous bijection between compact [Hausdorff spaces](../../../topology.md#hausdorff-space) is a [homeomorphism](../../../topology.md#homeomorphism). Conversely the weighted-composition formula plainly preserves the [supremum norm](../../../functional-analysis.md#supremum-norm), and its inverse is

$$
(T^{-1}g)(x)=\frac{g(\varphi^{-1}(x))}{u(\varphi^{-1}(x))}.
$$

If one compact space is empty, a surjective [isometric isomorphism of normed spaces](../../../functional-analysis.md#isometric-isomorphism-of-normed-spaces) forces the other to be empty, and the empty [homeomorphism](../../../topology.md#homeomorphism) gives the corresponding trivial case. This completes [Banach–Stone theorem](../../../functional-analysis.md#banach-stone-theorem).

Neither the [space of sequences converging to zero](../../../functional-analysis.md#space-of-sequences-converging-to-zero) $c_0$ nor $L^1[0,1]$ can be isometrically a [continuous dual space](../../../continuous-dual-space.md) of a [Banach space](../../../banach-space.md). Indeed, every nonzero [continuous dual space](../../../continuous-dual-space.md) has a nonempty weak-star compact [closed unit ball](../../../functional-analysis.md#closed-unit-ball) by [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem), and [Krein-Milman theorem](../../../functional-analysis.md#krein-milman-theorem) then guarantees an [extreme point](../../../mathematical-optimization.md#extreme-point). A bijective linear [isometry](../../../riemannian-geometry.md#isometry) preserves [extreme points](../../../mathematical-optimization.md#extreme-point) of [closed unit balls](../../../functional-analysis.md#closed-unit-ball).

The [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of $c_0$ has no [extreme points](../../../mathematical-optimization.md#extreme-point). Given $x\in c_0$ with $\|x\|_\infty\leq1$, choose $n$ with $|x_n|<1$ and $0<\varepsilon<1-|x_n|$. The two distinct elements $x\pm\varepsilon e_n$ remain in that [closed unit ball](../../../functional-analysis.md#closed-unit-ball) and have midpoint $x$.

The [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of the complex [Lp space](../../../measure-theory.md#lp-space) $L^1[0,1]$ also has no [extreme points](../../../mathematical-optimization.md#extreme-point). An element of [norm](../../../functional-analysis.md#norm) less than one can be perturbed by a sufficiently small nonzero [Lp space](../../../measure-theory.md#lp-space) element in both directions. If $\|f\|_1=1$, the [non-atomic measure](../../../measure-theory.md#non-atomic-measure) $|f(t)|\,dt$ admits a measurable set $A$ of mass $1/2$; for example the continuous function $s\mapsto\int_0^s|f(t)|\,dt$ attains $1/2$. Put $h=f(\mathbf1_A-\mathbf1_{A^c})$. For $0<\varepsilon<1$, the distinct functions $f\pm\varepsilon h$ both have [Lp norm](../../../real-analysis.md#lp-norm)

$$
(1+\varepsilon)\int_A|f|+(1-\varepsilon)\int_{A^c}|f|=1,
$$

with the two coefficients interchanged for the minus sign. Their midpoint is $f$. Thus **neither proposed space is isometrically a Banach dual**.

Finally, $[0,1]$ is a [connected space](../../../geometry-and-topology.md#connected-space), whereas $[0,1]\cup[2,3]$ is disconnected. They cannot be homeomorphic. By [Banach–Stone theorem](../../../functional-analysis.md#banach-stone-theorem), **$C[0,1]$ and $C([0,1]\cup[2,3])$ are not isometrically isomorphic** as complex [Banach spaces](../../../banach-space.md).

## 4

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work over $\mathbb C$ and take a nonzero commutative unital [Banach algebra](../../../banach-algebra.md) $A$, with $\|1\|=1$. A [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is a nonzero multiplicative complex [linear functional](../../../linear-algebra.md#linear-functional) $\chi:A\to\mathbb C$. It satisfies $\chi(1)=1$. Moreover $\chi(a)\in\sigma_A(a)$: otherwise $a-\chi(a)1$ would be invertible, although its image under $\chi$ is zero. The bound on the [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) therefore gives $|\chi(a)|\leq\|a\|$, proving [automatic continuity of characters](../../../banach-algebra.md#automatic-continuity-of-characters) and $\|\chi\|=1$.

Every proper [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $M$ of $A$ is closed. Indeed its closure is an [ideal](../../../commutative-algebra.md#ideal); if this closure were all of $A$, $M$ would contain an element within distance less than one of $1$. Such an element is invertible by the Neumann [series](../../../real-analysis.md#series-mathematics), forcing $1\in M$. Thus the closure is proper and maximality makes it equal to $M$. The [quotient Banach space](../../../banach-space.md#quotient-banach-space) $A/M$, with its quotient [Banach algebra](../../../banach-algebra.md) structure, is a complex [normed division algebra](../../../algebra.md#normed-division-algebra). By the [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem), it is $\mathbb C$, so the quotient map gives a [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) with kernel $M$. Conversely, the kernel of every [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is a [maximal ideal](../../../commutative-algebra.md#maximal-ideal), since the character is onto $\mathbb C$. The [Zorn lemma](../../../set-theory.md#zorn-s-lemma) supplies a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) containing every proper [ideal](../../../commutative-algebra.md#ideal), so the [character space of an algebra](../../../banach-algebra.md#character-space-of-an-algebra) $\Delta(A)$ is nonempty.

These facts give the exact relation between the [character space](../../../banach-algebra.md#character-space-of-an-algebra) and the [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element):

$$
\boxed{\sigma_A(a)=\{\chi(a):\chi\in\Delta(A)\}.}
$$

One inclusion was proved above. For the other, if $a-\lambda1$ is noninvertible, the principal [ideal](../../../commutative-algebra.md#ideal) it generates is proper because $A$ is commutative. Contain it in a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) and use its corresponding [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) to obtain $\chi(a)=\lambda$.

Give $\Delta(A)$ the [Gelfand topology](../../../banach-algebra.md#gelfand-topology), namely its [subspace topology](../../../topology.md#subspace-topology) from the [weak-star topology](../../../weak-topology.md#weak-star-topology) on $A^*$. In the [closed unit ball](../../../functional-analysis.md#closed-unit-ball) of $A^*$, it is the intersection of the closed conditions

$$
\chi(1)=1,\qquad \chi(ab)=\chi(a)\chi(b)\quad(a,b\in A).
$$

Consequently [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) makes $\Delta(A)$ a compact [Hausdorff space](../../../topology.md#hausdorff-space). For every $a\in A$, define the [Gelfand transform](../../../banach-algebra.md#gelfand-representation) $\widehat a(\chi)=\chi(a)$. This is a [continuous function](../../../calculus.md#continuous-function) on $\Delta(A)$ by definition of the [Gelfand topology](../../../banach-algebra.md#gelfand-topology). The [Gelfand representation theorem](../../../banach-algebra.md#gelfand-representation-theorem) gives a contractive unital [algebra homomorphism over a field](../../../algebra.md#algebra-homomorphism-over-a-field)

$$
\Gamma:A\longrightarrow C(\Delta(A)),\qquad a\longmapsto\widehat a,
\qquad
\boxed{\|\widehat a\|_\infty=r(a)\leq\|a\|.}
$$

Multiplicativity and linearity follow by evaluating at each [character of an algebra](../../../banach-algebra.md#character-of-an-algebra); the [supremum norm](../../../functional-analysis.md#supremum-norm) equality follows from the preceding [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) identity. Its kernel is

$$
\ker\Gamma=\bigcap_{\chi\in\Delta(A)}\ker\chi
=\bigcap_{M\text{ maximal}}M=\operatorname{rad}A,
$$

the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical). Equivalently, its elements have [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) $\{0\}$. Thus $\Gamma$ is injective precisely when $A$ is a [semisimple commutative Banach algebra](../../../banach-algebra.md#semisimple-commutative-banach-algebra), and it gives a faithful continuous representation of $A/\operatorname{rad}A$ as a function algebra. Its range contains the constants and separates points of $\Delta(A)$, because distinct [characters of an algebra](../../../banach-algebra.md#character-of-an-algebra) differ on some $a$. An arbitrary [Banach algebra](../../../banach-algebra.md) need not have an isometric or surjective [Gelfand transform](../../../banach-algebra.md#gelfand-representation), nor a uniformly dense range: those conclusions require further hypotheses.

For the [Banach algebra](../../../banach-algebra.md) $C(K)$ on a nonempty compact [Hausdorff space](../../../topology.md#hausdorff-space) $K$, all [characters of an algebra](../../../banach-algebra.md#character-of-an-algebra) are [evaluation characters](../../../banach-algebra.md#evaluation-character). To see this, let $M$ be a [maximal ideal](../../../commutative-algebra.md#maximal-ideal). If its elements had no common zero, compactness would supply $f_1,\ldots,f_n\in M$ with no common zero. The [continuous function](../../../calculus.md#continuous-function) $h=\sum_i\overline{f_i}f_i$ belongs to $M$, is strictly positive on $K$, and has a continuous reciprocal. It is therefore invertible, a contradiction. Hence all elements of $M$ vanish at some $x\in K$, so $M\subseteq\ker\delta_x$ and maximality gives equality. The associated [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) must be $\delta_x$: since $f-f(x)1\in M$, its value on $f$ is $f(x)$.

The map $x\mapsto\delta_x$ is a continuous bijection $K\to\Delta(C(K))$, using separation of points by [continuous functions](../../../calculus.md#continuous-function). Compactness and the Hausdorff property make it a [homeomorphism](../../../topology.md#homeomorphism). Under this identification the [Gelfand transform](../../../banach-algebra.md#gelfand-representation) is **$\boxed{\widehat f(\delta_x)=f(x)}$**, so it is the identity representation of $C(K)$, in particular an isometric onto map. The empty $K$ gives the zero algebra, whose empty [character space](../../../banach-algebra.md#character-space-of-an-algebra) represents the zero function space; it was excluded by the nonzero unital convention above.

Now let $A$ be a commutative unital [C-star algebra](../../../banach-algebra.md#c-star-algebra). The stronger conclusion is the [Commutative Gelfand--Naimark theorem](../../../banach-algebra.md#commutative-gelfand-naimark-theorem): **the [Gelfand transform](../../../banach-algebra.md#gelfand-representation) is an isometric onto [C-star homomorphism](../../../banach-algebra.md#c-star-homomorphism) $A\cong C(\Delta(A))$**. We prove the additional assertions without assuming this conclusion.

First every [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) respects the [C-star algebra](../../../banach-algebra.md#c-star-algebra) involution. If $h=h^*$, the elements $e^{ith}$, $t\in\mathbb R$, are [unitary elements of a C-star algebra](../../../banach-algebra.md#unitary-element-of-a-c-star-algebra), and their [norm](../../../functional-analysis.md#norm) is one by the [C-star identity](../../../banach-algebra.md#c-star-identity). Continuity and multiplicativity give $\chi(e^{ith})=e^{it\chi(h)}$. Thus $|e^{it\chi(h)}|\leq1$ for every real $t$, forcing $\chi(h)$ to be real. Writing $a=h+ik$ with $h=(a+a^*)/2$ and $k=(a-a^*)/(2i)$ self-adjoint gives $\chi(a^*)=\overline{\chi(a)}$. Therefore the range of $\Gamma$ is closed under [complex conjugation](../../../complex-analysis.md#complex-conjugation).

Every element of commutative $A$ is a [Normal element of a C-star algebra](../../../banach-algebra.md#normal-element-of-a-c-star-algebra). For a normal $b$, use the [C-star identity](../../../banach-algebra.md#c-star-identity), and then the same identity for the self-adjoint element $b^*b$, to obtain

$$
\|b^2\|^2=\|(b^2)^*b^2\|=\|(b^*b)^2\|
=\|b^*b\|^2=\|b\|^4.
$$

Its powers are also normal, so $\|a^{2^n}\|=\|a\|^{2^n}$. The [spectral radius formula](../../../analysis.md#spectral-radius-formula) gives $r(a)=\|a\|$, hence $\|\widehat a\|_\infty=\|a\|$. The [Gelfand transform](../../../banach-algebra.md#gelfand-representation) is therefore an [isometry](../../../riemannian-geometry.md#isometry), and its range is complete and closed in the [supremum norm](../../../functional-analysis.md#supremum-norm). It contains constants, separates points and is closed under [complex conjugation](../../../complex-analysis.md#complex-conjugation). The complex [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) makes that range dense, hence all of $C(\Delta(A))$.

The approximation step in [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) can also be seen directly here. For a unital conjugation-closed point-separating subalgebra $B\subseteq C(K)$, the real-valued part of its uniform closure is closed under absolute values, by polynomial approximation to $|t|$ on bounded intervals, hence under pointwise maxima and minima. Its real-valued functions separate points. Given real $f\in C(K)$ and $\varepsilon>0$, for each $x,y$ an affine rescaling of a separating function produces $b_{x,y}$ agreeing with $f$ at $x,y$; take a constant when $x=y$. For fixed $x$, finitely many neighbourhoods of $y$ where $b_{x,y}>f-\varepsilon$ cover $K$. Their maximum $b_x$ exceeds $f-\varepsilon$ everywhere and agrees with $f$ at $x$, hence is less than $f+\varepsilon$ near $x$. Finitely many of these latter neighbourhoods cover $K$; the minimum of their $b_x$ lies between $f-\varepsilon$ and $f+\varepsilon$ everywhere. Approximate real and imaginary parts separately. This proves the density used above and completes the [C-star algebra](../../../banach-algebra.md#c-star-algebra) conclusion.

## 5

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

We prove the required [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) for a [seminorm](../../../topological-vector-space.md#seminorm) directly. First suppose the [vector space](../../../vector-space.md) is real. At an intermediate extension stage, let $g:E\to\mathbb R$ be a [linear functional](../../../linear-algebra.md#linear-functional) with $|g(y)|\leq p(y)$, and let $z\notin E$. Extending to $E+\mathbb Rz$ amounts to choosing $c=f(z)$. The upper domination $f\leq p$ requires

$$
\sup_{y\in E}\{g(y)-p(y-z)\}\ \leq c\leq\ \inf_{w\in E}\{p(w+z)-g(w)\}.
$$

The interval is nonempty: for all $y,w\in E$,

$$
g(y)+g(w)=g(y+w)\leq p(y+w)\leq p(y-z)+p(w+z).
$$

Its endpoints are finite since inserting zero gives bounds $-p(z)$ and $p(z)$, while every lower candidate is below every upper candidate. Choose $c$ in the interval and put $f(y+tz)=g(y)+tc$. For $t>0$, the upper bound with $w=y/t$ proves $f(y+tz)\leq p(y+tz)$. For $t<0$, writing $s=-t>0$ and applying the lower bound with $y/s$ proves the same inequality. The case $t=0$ is already known. Applying this domination to $-x$ and using $p(-x)=p(x)$ gives $|f(x)|\leq p(x)$.

Partially order all dominated [linear functional](../../../linear-algebra.md#linear-functional) extensions of the original $g$ by extension of their domains and values. They form a nonempty set. The union along any chain is a well-defined dominated [linear functional](../../../linear-algebra.md#linear-functional) on a [vector subspace](../../../vector-space.md#vector-subspace), so every chain has an upper bound. The [Zorn lemma](../../../set-theory.md#zorn-s-lemma) gives a maximal extension. If its domain were not $X$, the preceding one-dimensional construction would enlarge it, a contradiction. Thus the required extension exists on $X$.

For a complex [vector space](../../../vector-space.md), apply the proved real result to $\operatorname{Re}g$ on the underlying real [vector subspace](../../../vector-space.md#vector-subspace). Let $U:X\to\mathbb R$ be the resulting real [linear functional](../../../linear-algebra.md#linear-functional), with $|U(x)|\leq p(x)$, and set

$$
f(x)=U(x)-iU(ix).
$$

It is additive and real-linear, and $f(ix)=if(x)$, so it is complex-linear. On $Y$, the identity $\operatorname{Re}g(iy)=-\operatorname{Im}g(y)$ proves $f(y)=g(y)$. Choose $\alpha$ with $|\alpha|=1$ and $\alpha f(x)=|f(x)|$ when $f(x)\ne0$. Then

$$
|f(x)|=\operatorname{Re}f(\alpha x)=U(\alpha x)\leq p(\alpha x)=p(x).
$$

The bound is immediate if $f(x)=0$. This proves the real and complex [seminorm](../../../topological-vector-space.md#seminorm) forms of [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) without invoking any version of that theorem.

For the [distance to a set](../../../topological-analysis.md#distance-to-a-set) assertion, let $d=d(z,Y)>0$. Define on $Y+\mathbb Kz$ the [linear functional](../../../linear-algebra.md#linear-functional) $g(y+\alpha z)=\alpha d$. The decomposition is unique because $z\notin Y$, and for $\alpha\ne0$,

$$
|g(y+\alpha z)|=|\alpha|d
\leq|\alpha|\|z+y/\alpha\|=\|y+\alpha z\|.
$$

For $\alpha=0$ the bound is immediate. Apply the just-proved [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) with $p(x)=\|x\|$ to get $f\in X^*$, $f|_Y=0$, $f(z)=d$, and $\|f\|\leq1$. Choose $y_n\in Y$ with $\|z-y_n\|\to d$. Since

$$
d=|f(z-y_n)|\leq\|f\|\|z-y_n\|,
$$

and $d>0$, passage to the limit gives $\|f\|\geq1$. Thus **$\boxed{f|_Y=0,\quad f(z)=d(z,Y),\quad\|f\|=1}$**. This version of the [Hahn-Banach distance formula](../../../functional-analysis.md#hahn-banach-distance-formula) needs neither a closed $Y$ nor an attained [distance to a set](../../../topological-analysis.md#distance-to-a-set).

For the [Banach limit](../../../banach-space.md#banach-limit) construction below, take the real [l-infinity sequence space](../../../banach-space.md#l-infinity-sequence-space), let $S(x_1,x_2,\ldots)=(x_2,x_3,\ldots)$ be its [left shift on bounded sequences](../../../banach-space.md#left-shift-on-bounded-sequences), put $Y=(I-S)\ell^\infty$, and let $\mathbf1=(1,1,\ldots)$. This is a [vector subspace](../../../vector-space.md#vector-subspace) and its [distance to a set](../../../topological-analysis.md#distance-to-a-set) from $\mathbf1$ determines the construction.

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For $y=x-Sx\in Y$, the telescoping arithmetic means satisfy

$$
\frac1N\sum_{n=1}^Ny_n=\frac{x_1-x_{N+1}}N\longrightarrow0,
$$

because $x$ is a [bounded sequence](../../../real-analysis.md#bounded-sequence). Hence $\|\mathbf1-y\|_\infty\geq|1-N^{-1}\sum_{n=1}^Ny_n|$ for every $N$, and passage to the limit gives $\|\mathbf1-y\|_\infty\geq1$. Taking $y=0$ shows $d(\mathbf1,Y)=1$. The proved [Hahn-Banach distance formula](../../../functional-analysis.md#hahn-banach-distance-formula) therefore yields a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $L$ on the real [l-infinity sequence space](../../../banach-space.md#l-infinity-sequence-space) with

$$
\boxed{\|L\|=1,\qquad L(\mathbf1)=1,\qquad L|_Y=0.}
$$

We verify that this single [linear functional](../../../linear-algebra.md#linear-functional) also has the two remaining properties.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Every [finitely supported sequence](../../../banach-space.md#finitely-supported-sequence) $v$ lies in $Y$: if $v_n=0$ for $n>N$, set $x_n=\sum_{k=n}^Nv_k$ for $n\leq N$ and $x_n=0$ afterwards. Then $x$ is a [bounded sequence](../../../real-analysis.md#bounded-sequence) and $x-Sx=v$. Consequently $L(v)=0$. The [finitely supported sequences](../../../banach-space.md#finitely-supported-sequence) are dense in the [space of sequences converging to zero](../../../functional-analysis.md#space-of-sequences-converging-to-zero) $c_0$ for the [supremum norm](../../../functional-analysis.md#supremum-norm), by truncation, so continuity of the [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $L$ gives $L|_{c_0}=0$. For $x$ in the real [convergent sequence space](../../../functional-analysis.md#convergent-sequence-space), with ordinary limit $\ell$, we have $x-\ell\mathbf1\in c_0$. Therefore **$\boxed{L(x)=\ell L(\mathbf1)=\lim_{n\to\infty}x_n}$**.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For every [bounded sequence](../../../real-analysis.md#bounded-sequence) $x$, $x-Sx\in Y$ and $L|_Y=0$. Linearity gives **$\boxed{L(x)=L(Sx)}$**, as required. Thus the same $L$ satisfies all three conditions and is a [Banach limit](../../../banach-space.md#banach-limit).

The usual positivity condition for a [Banach limit](../../../banach-space.md#banach-limit) follows automatically here. If $x_n\geq0$ and $a=\|x\|_\infty>0$, then $\|\mathbf1-x/a\|_\infty\leq1$. Since $\|L\|=L(\mathbf1)=1$, we have $|1-L(x)/a|\leq1$, whence $L(x)\geq0$. The case $x=0$ is immediate. This explains why the constructed [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) is also a [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional) extending the ordinary limit while remaining invariant under the [left shift on bounded sequences](../../../banach-space.md#left-shift-on-bounded-sequences).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
