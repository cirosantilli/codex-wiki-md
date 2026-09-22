# Paper 9

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper9.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper9.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [topological group](../../../topological-group.md) is a [group](../../../group.md) with a topology for which multiplication $G\times G\to G$ and inversion $G\to G$ are continuous. A Hausdorff axiom is not built into this definition. For [neighbourhood bases](../../../topology.md#neighbourhood-basis) $\mathcal B_x$ at each point, the precise [neighbourhood criterion for a topological group](../../../topological-group.md#neighbourhood-criterion-for-a-topological-group) is

$$
\begin{aligned}&U\in\mathcal B_{xy}\ \Longrightarrow\ \exists V\in\mathcal B_x,\ W\in\mathcal B_y:\ VW\subseteq U,\\&U\in\mathcal B_{x^{-1}}\ \Longrightarrow\ \exists V\in\mathcal B_x:\ V^{-1}\subseteq U.\end{aligned}
$$

Necessity follows from continuity: the inverse image of a neighbourhood of $xy$ contains a product neighbourhood of $(x,y)$, and the inverse image of a neighbourhood of $x^{-1}$ contains a neighbourhood of $x$. Conversely, these inclusions give exactly those neighbourhood conditions for continuity of multiplication and inversion, since the rectangles $V\times W$ form a basis for the [product topology](../../../geometry-and-topology.md#product-topology).

An equivalent identity-level formulation is useful. Bases must be obtainable by translation, $\mathcal B_x=x\mathcal B_e$, and for every $U\in\mathcal B_e$ one must have

$$
\boxed{\exists V\in\mathcal B_e:\ V^2\subseteq U;\qquad\exists V\in\mathcal B_e:\ V^{-1}\subseteq U;\qquad\forall g\in G\ \exists V\in\mathcal B_e:\ gVg^{-1}\subseteq U.}
$$

These conditions are necessary because translations are [homeomorphisms](../../../topology.md#homeomorphism), multiplication is continuous at $(e,e)$, inversion is continuous at $e$, and each conjugation is a [homeomorphism](../../../topology.md#homeomorphism). For sufficiency at $(x,y)$, first choose $D$ with $D^2\subseteq U$, then $V$ with $y^{-1}Vy\subseteq D$ and take $W=D$. This gives $(xV)(yW)\subseteq xyU$. For inversion near $x$, first choose $H$ with $xHx^{-1}\subseteq U$, then $V$ with $V^{-1}\subseteq H$; thus $(xV)^{-1}=x^{-1}(xV^{-1}x^{-1})\subseteq x^{-1}U$. The pointwise criterion is therefore satisfied everywhere. If Hausdorffness is also required, the additional identity-neighbourhood condition is $\bigcap_{U\in\mathcal B_e}U=\{e\}$: it gives separation of distinct points by translating sufficiently small neighbourhoods.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

**False.** In the additive [topological group](../../../topological-group.md) $\mathbb R$, the [subgroup](../../../group.md#subgroup) $\mathbb Z$ is closed: every noninteger has a sufficiently small interval disjoint from it. It is not open, because no neighbourhood of an integer consists only of integers. Thus a [closed subgroup](../../../topological-group.md#closed-subgroup) need not be an [open subgroup](../../../topological-group.md#open-subgroup).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

**True.** If $H$ is an [open subgroup](../../../topological-group.md#open-subgroup), every left [coset](../../../group-theory.md#coset) $gH$ is open because left translation is a [homeomorphism](../../../topology.md#homeomorphism). The other cosets partition the complement:

$$
G\setminus H=\bigcup_{g\notin H}gH.
$$

That complement is open, so $H$ is a [closed subgroup](../../../topological-group.md#closed-subgroup).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**False as a whole: the [identity component](../../../geometry-and-topology.md#identity-component) is normal, but need not be open.** Write $G^\circ$ for the [identity component](../../../geometry-and-topology.md#identity-component). The [continuous function](../../../calculus.md#continuous-function) $(x,y)\mapsto xy^{-1}$ maps the connected space $G^\circ\times G^\circ$ to a connected set containing $e$, hence into $G^\circ$. Thus $G^\circ$ is a [subgroup](../../../group.md#subgroup). Conjugation by any $g$ is a [homeomorphism](../../../topology.md#homeomorphism) fixing $e$, so it maps $G^\circ$ onto itself; therefore it is a [normal subgroup](../../../group-theory.md#normal-subgroup). It is also closed, since the closure of a connected set is connected and a [connected component](../../../geometry-and-topology.md#connected-component) is maximal.

For failure of openness, take the additive group $\mathbb Q$ with its usual topology. Any two distinct rational numbers can be separated inside $\mathbb Q$ by an irrational cut between them, so every connected subset is a singleton. Its [identity component](../../../geometry-and-topology.md#identity-component) is consequently $\{0\}$, which is not open because every neighbourhood of zero contains nonzero rational numbers.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**False.** The additive group $\mathbb Q$ with its usual metric is a [Hausdorff space](../../../topology.md#hausdorff-space) but not a [locally compact space](../../../topology.md#locally-compact-space). If a compact set were a neighbourhood of zero, it would contain all rationals in some interval $(-\epsilon,\epsilon)$. Choose an irrational $a$ in that interval and rational numbers $q_n\to a$ in the real line. All sufficiently late $q_n$ would lie in the compact neighbourhood, so a subsequence would converge in $\mathbb Q$. Its real limit would have to be $a$, a contradiction.

The other suggested example is the additive [Hilbert space](../../../hilbert-space.md) $\ell^2$. A compact neighbourhood of zero would contain a closed ball of some positive radius $r$. The vectors $re_n$ in that ball have pairwise distance $r\sqrt2$, and thus no convergent subsequence. This again contradicts metric compactness. Both examples are [topological groups](../../../topological-group.md) whose operations are continuous, so Hausdorffness cannot supply local compactness.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

**True.** Choose a compact neighbourhood $K$ of the identity in the [locally compact group](../../../topological-group.md#locally-compact-group) and put $S=K\cup K^{-1}\cup\{e\}$. Inversion is a [homeomorphism](../../../topology.md#homeomorphism), so $S$ is compact; it is symmetric and still a neighbourhood of $e$. Define

$$
\boxed{H=\bigcup_{n=1}^{\infty}S^n.}
$$

The identity belongs to $S$, so these powers are increasing. Symmetry gives $H^{-1}=H$, and $S^mS^n=S^{m+n}$ gives closure under multiplication; hence $H$ is a [subgroup](../../../group.md#subgroup). Each $S^n$ is compact, being the continuous image of the finite product of compact spaces. Thus $H$ is a [sigma-compact space](../../../topology.md#sigma-compact-space). Finally $S$ contains some open identity neighbourhood $U$, and $H=\bigcup_{h\in H}hU$ is open. This constructs the required [sigma-compact open subgroup of a locally compact group](../../../topological-group.md#sigma-compact-open-subgroup-of-a-locally-compact-group). The argument also works without Hausdorffness if local compactness means possession of compact neighbourhoods.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

**False.** Give the two-element group $C_2$ the [indiscrete topology](../../../topology.md#indiscrete-topology) and take $G=\mathbb R\times C_2$ with the [product topology](../../../geometry-and-topology.md#product-topology). The indiscrete factor is a [topological group](../../../topological-group.md), since every map into an indiscrete space is continuous, and the product group operations are continuous. Points $(0,e)$ and $(0,a)$, $a\neq e$, have identical neighbourhoods, so $G$ is not a [Hausdorff space](../../../topology.md#hausdorff-space). However, its continuous projection onto $\mathbb R$ is surjective. If $G$ were compact, its image $\mathbb R$ would be compact, which it is not.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

**True.** Given a compatible [left-invariant group metric](../../../topological-group.md#left-invariant-group-metric) $d$, define

$$
\boxed{d_R(x,y)=d(x^{-1},y^{-1}).}
$$

Pullback by the bijection $x\mapsto x^{-1}$ preserves all metric axioms, and because inversion is a [homeomorphism](../../../topology.md#homeomorphism), $d_R$ induces the same topology. For right translation by $a$, left invariance gives

$$
d_R(xa,ya)=d(a^{-1}x^{-1},a^{-1}y^{-1})=d(x^{-1},y^{-1})=d_R(x,y).
$$

Thus $d_R$ is the required compatible [right-invariant group metric](../../../topological-group.md#right-invariant-group-metric). No metrizability theorem is needed.

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

**False.** On the additive [topological group](../../../topological-group.md) $\mathbb R$, put $d(x,y)=|x-y|$ and $d'(x,y)=\sqrt{|x-y|}$. Both are invariant under left and right translations and induce the usual topology. The triangle inequality for $d'$ follows from $\sqrt{a+b}\leq\sqrt a+\sqrt b$ for $a,b\geq0$. But

$$
\frac{d(x,y)}{d'(x,y)}=\sqrt{|x-y|}
$$

can be arbitrarily close to zero and arbitrarily large. Consequently no $K>0$ can satisfy both proposed inequalities. Compatibility of the two invariant metrics is topological equivalence, which need not be [bilipschitz equivalence](../../../geometric-group-theory.md#bilipschitz-equivalence).

## 2

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

There is a definitional qualification. If a [compactly generated group](../../../topological-group.md#compactly-generated-group) means a group algebraically generated by a compact subset, the assertion as printed is false. In the usual topology on the additive group $\mathbb Q$, the set

$$
K=\{0\}\cup\{1/n!:n\geq1\}
$$

is compact and generates $\mathbb Q$: every positive integer denominator divides some factorial. The group is metrizable, but it has no nonzero [Haar measure](../../../measure-theory.md#haar-measure) finite on compact sets. Indeed, translation invariance gives a common singleton mass $a\geq0$. If $a>0$, the infinite compact set $K$ has infinite mass; if $a=0$, countable additivity gives zero mass to the whole countable group. This proves that [compact generation does not imply local compactness](../../../topological-group.md#compact-generation-does-not-imply-local-compactness) or existence of [Haar measure](../../../measure-theory.md#haar-measure).

If the convention includes a compact generating neighbourhood, local compactness is already part of the hypothesis. More explicitly, the standard corrected result is **every locally compact, compactly generated metrizable group has [Haar measure](../../../measure-theory.md#haar-measure)**. Here is a construction, rather than an invocation of that existence theorem.

Fix a nonzero $h\geq0$ in the [space of continuous compactly supported functions](../../../functional-analysis.md#space-of-continuous-compactly-supported-functions) $C_c(G)$. For nonzero $u\geq0$ in $C_c(G)$ and $f\geq0$ in $C_c(G)$, define the covering number and its normalized functional by

$$
(f:u)=\inf\left\{\sum_{j=1}^r a_j:f(t)\leq\sum_{j=1}^r a_j u(x_j^{-1}t)\ \text{for all }t,\ a_j>0\right\},\qquad I_u(f)=\frac{(f:u)}{(h:u)}.
$$

These numbers are finite: translates of the region where $u>0$ cover the [compact support](../../../function.md#compact-support) of $f$, and a finite subcover, multiplied by a sufficiently large coefficient, dominates $f$. They are positive when $f\neq0$, since every cover has total coefficient at least $\|f\|_\infty/\|u\|_\infty$. Composition of covers gives $(f:u)\leq(f:h)(h:u)$. Thus, with $M_f=(f:h)$,

$$
0\leq I_u(f)\leq M_f,\qquad I_u(h)=1.
$$

The functionals are homogeneous, monotone, subadditive and exactly invariant under left translation; the last property follows by relabelling the covering translates.

The key step in [Haar measure from normalized covering functionals](../../../measure-theory.md#haar-measure-from-normalized-covering-functionals) is asymptotic additivity as $\operatorname{supp}u$ shrinks to $e$. Given $f_1,f_2\geq0$, put $f=f_1+f_2$ and choose $p\in C_c(G)$ with $p\geq1$ on both supports. For $\delta>0$, set $\alpha_i=f_i/(f+\delta p)$, extended by zero where the denominator vanishes. These are continuous [compactly supported](../../../function.md#compact-support) functions and $\alpha_1+\alpha_2\leq1$. For any $\eta>0$, a sufficiently small identity neighbourhood $V$ ensures

$$
|\alpha_i(xv)-\alpha_i(x)|<\eta\quad\text{for every }x\in G,\ v\in V.
$$

Take $\operatorname{supp}u\subseteq V$ and any cover $f\leq\sum_j a_jT_{x_j}u$, where $T_xu(t)=u(x^{-1}t)$. Since $f_i\leq\alpha_i f+\delta p$, it follows that

$$
(f_i:u)\leq\sum_j a_j(\alpha_i(x_j)+\eta)+\delta(p:u).
$$

Adding and then taking the infimum over the cover of $f$ gives

$$
0\leq I_u(f_1)+I_u(f_2)-I_u(f)\leq2\eta M_f+2\delta M_p.
$$

First make $\delta$ small, then $\eta$ small, and finally the support of $u$ small enough for the oscillation bound. The additivity defect therefore tends to zero.

Compact generation gives a countable compact cover by finite products of a compact symmetric generating set. Local compactness upgrades this to a compact exhaustion with interiors covering $G$. Metrizability supplies a countable identity-neighbourhood base and a countable family of nonnegative $C_c$ functions dense in the uniform norm on each fixed [compact support](../../../function.md#compact-support); this is the countable family whose existence may be assumed. Choose nonzero $u_n\geq0$ with supports shrinking to $e$. The uniform bounds $I_{u_n}(f)\leq M_f$ and a diagonal subsequence give convergence on that countable family. To extend convergence to every nonnegative $f$ supported in a fixed compact $L$, choose a cutoff $p_L\geq1$ on $L$. Monotonicity and subadditivity give

$$
|I_u(f)-I_u(g)|\leq I_u(|f-g|)\leq\|f-g\|_\infty M_{p_L}
$$

for $f,g$ supported in $L$. Uniform approximation therefore makes the chosen subsequence Cauchy on every such $f$.

Let $I(f)$ be its limit. Asymptotic additivity, homogeneity and invariance give an additive positive invariant functional on the nonnegative cone, with $I(h)=1$. Extend it by differences to real $C_c(G)$ and then complex linearly. It is bounded on each fixed [compact support](../../../function.md#compact-support) by the cutoff bound. The [Riesz representation on compactly supported continuous functions](../../../functional-analysis.md#riesz-representation-on-compactly-supported-continuous-functions) consequently produces a positive [Radon measure](../../../measure-theory.md#radon-measure) $m$ with $I(f)=\int f\,dm$. Invariance of $I$ and uniqueness of that representation imply $m(xE)=m(E)$. The measure is nonzero because $I(h)=1$, and finite on compact sets by the cutoff estimate. Moreover, for any nonzero $f\geq0$, composition of covers gives $I_u(f)\geq1/(h:f)>0$, so every nonempty open set has positive measure. Hence

$$
\boxed{m\text{ is a nonzero left Haar measure on the locally compact group}.}
$$

This completes the intended construction under the convention supplying local compactness, while the rational example settles the weaker literal interpretation.

## 3

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use additive notation and fix [Haar measure](../../../measure-theory.md#haar-measure) $m$ on $G$. A [continuous unitary character](../../../topological-group.md#continuous-unitary-character) is a continuous homomorphism $\chi:G\to\mathbb T$. With the convention

$$
\widehat f(\chi)=\int_G f(t)\overline{\chi(t)}\,dm(t),\qquad (f*g)(t)=\int_G f(y)g(t-y)\,dm(y),
$$

the [Fubini theorem](../../../measure-theory.md#fubini-s-theorem) and the character identity imply $\widehat{f*g}(\chi)=\widehat f(\chi)\widehat g(\chi)$. Also $|\widehat f(\chi)|\leq\|f\|_1$, and choosing $f=\chi a$ for a nonzero nonnegative $a\in C_c(G)$ shows that evaluation at $\chi$ is a nonzero functional. Thus each character gives a [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) on the [L1 convolution algebra](../../../banach-algebra.md#l1-convolution-algebra). Here a multiplicative linear functional means a [nonzero multiplicative linear functional](../../../banach-algebra.md#character-of-an-algebra); the zero functional must be excluded for the claimed bijection.

Conversely, let $\varphi$ be such a functional. It is automatically bounded with $|\varphi(f)|\leq\|f\|_1$: extend it to the [unitization of an algebra](../../../banach-algebra.md#unitization-of-an-algebra) by $\widetilde\varphi(f+z1)=\varphi(f)+z$. If $|z|>\|f\|_1$, the [Neumann series](../../../banach-algebra.md#neumann-series) makes $z1-f$ invertible, so its image under the unital homomorphism cannot be zero. Hence $\varphi(f)$ cannot lie outside the norm disc.

Choose $a\in L^1(G)$ with $\varphi(a)\neq0$, and let $T_xa(t)=a(t-x)$. The Abelian translation identities $(T_xa)*b=a*(T_xb)$ give

$$
\varphi(T_xa)\varphi(b)=\varphi(a)\varphi(T_xb).
$$

Therefore, defining $c(x)=\varphi(T_xa)/\varphi(a)$, one has $\varphi(T_xb)=c(x)\varphi(b)$ for every $b$. Applying this to two successive translations gives $c(x+y)=c(x)c(y)$ and $c(0)=1$. By [translation continuity in Lp on a locally compact group](../../../measure-theory.md#translation-continuity-in-lp-on-a-locally-compact-group), $c$ is continuous. It is uniformly bounded by $\|a\|_1/|\varphi(a)|$; applying this bound to $c(nx)=c(x)^n$ for positive and negative integers forces $|c(x)|=1$. Thus $\chi(x)=\overline{c(x)}$ is a [continuous unitary character](../../../topological-group.md#continuous-unitary-character).

The [Bochner integral](../../../measure-theory.md#bochner-integral) identity $a*b=\int_G b(y)T_ya\,dm(y)$ holds in $L^1$, since $\|T_ya\|_1=\|a\|_1$. Applying the bounded functional yields

$$
\varphi(a)\varphi(b)=\varphi(a*b)=\varphi(a)\int_G b(y)c(y)\,dm(y).
$$

Cancel $\varphi(a)\neq0$ to obtain the required correspondence

$$
\boxed{\varphi(b)=\int_Gb(y)\overline{\chi(y)}\,dm(y)=\widehat b(\chi).}
$$

The recovery formula $\overline{\chi(x)}=\varphi(T_xa)/\varphi(a)$ proves uniqueness. These functionals have norm exactly one, since $b=\chi a$ with $a\geq0$ and $\int a=1$ has $\|b\|_1=\varphi(b)=1$.

For the topology, identify the [Pontryagin dual group](../../../group.md#pontryagin-dual-group) with these functionals and give it the [Gelfand topology](../../../banach-algebra.md#gelfand-topology), namely pointwise convergence of $\widehat f(\chi)$ for every $f\in L^1$. If a net $\chi_\lambda$ converges to $\gamma$ uniformly on every compact subset of $G$, then for $f\in C_c(G)$,

$$
|\widehat f(\chi_\lambda)-\widehat f(\gamma)|\leq\|f\|_1\sup_{x\in\operatorname{supp}f}|\chi_\lambda(x)-\gamma(x)|\longrightarrow0.
$$

Density of $C_c$ in $L^1$ and the uniform functional norm bound one extend this convergence to every $f\in L^1$.

Conversely, suppose convergence in the [Gelfand topology](../../../banach-algebra.md#gelfand-topology) and choose $a$ with $\widehat a(\gamma)\neq0$. For compact $K\subseteq G$, the set $\{T_xa:x\in K\}$ is compact in $L^1$ by [translation continuity in Lp on a locally compact group](../../../measure-theory.md#translation-continuity-in-lp-on-a-locally-compact-group). Evaluation convergence is uniform on this compact set: a finite $\delta$-net reduces its supremum to finitely many convergent evaluations plus $2\delta$, using the common functional norm one. Thus

$$
\sup_{x\in K}|\widehat{T_xa}(\chi_\lambda)-\widehat{T_xa}(\gamma)|\longrightarrow0.
$$

Now $\widehat{T_xa}(\chi)=\overline{\chi(x)}\widehat a(\chi)$, and $\widehat a(\chi_\lambda)\to\widehat a(\gamma)\neq0$. Dividing this identity proves $\sup_{x\in K}|\chi_\lambda(x)-\gamma(x)|\to0$. Hence the [Gelfand topology](../../../banach-algebra.md#gelfand-topology) is exactly the [compact-open topology](../../../real-analysis.md#compact-open-topology), with the requested [neighbourhood basis](../../../topology.md#neighbourhood-basis)

$$
\boxed{U(\gamma;K,\epsilon)=\{\chi\in\widehat G:|\chi(x)-\gamma(x)|<\epsilon\text{ for every }x\in K\}.}
$$

For compact $K$, the continuous difference attains its maximum, so this strict pointwise inequality on $K$ is equivalent to a strict uniform bound. Finite intersections contain another such set by taking the union of the compact sets and the minimum of the tolerances.

## 4

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Fix [Haar measure](../../../measure-theory.md#haar-measure) $m_G$ and use $\widehat f(\chi)=\int_G f(x)\overline{\chi(x)}\,dm_G(x)$. A [positive-definite function](../../../analysis.md#positive-definite-function) $p$ satisfies $\sum_{i,j}z_i\overline{z_j}p(x_i-x_j)\geq0$ for every finite choice of points and coefficients. The [Bochner theorem](../../../analysis.md#bochner-s-theorem) states that a continuous positive-definite function on a locally compact Hausdorff Abelian group has a unique representation

$$
\boxed{p(x)=\int_{\widehat G}\chi(x)\,d\mu_p(\chi),\qquad \mu_p\geq0,\qquad\mu_p(\widehat G)=p(0)<\infty,}
$$

where $\mu_p$ is a [Radon measure](../../../measure-theory.md#radon-measure). Conversely, any finite positive [Radon measure](../../../measure-theory.md#radon-measure) on the [Pontryagin dual group](../../../group.md#pontryagin-dual-group) has a continuous positive-definite inverse transform. The sign convention here is the one compatible with the displayed Fourier transform.

First note that the dual is a locally compact Hausdorff [topological group](../../../topological-group.md). Its group operations are continuous in the [compact-open topology](../../../real-analysis.md#compact-open-topology) proved in question 3. For local compactness, adjoin the zero functional to the [character space of an algebra](../../../banach-algebra.md#character-space-of-an-algebra) of $L^1(G)$. All its elements lie in the closed unit ball of $L^1(G)^*$, and the equations $\varphi(a*b)=\varphi(a)\varphi(b)$ define a closed subset in the [weak-star topology](../../../weak-topology.md#weak-star-topology). The [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) makes that subset compact Hausdorff. Removing the zero functional gives an open, hence locally compact, subspace. This provides the setting for constructing the measure on the dual, without assuming a [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem).

Let $u^*(x)=\overline{u(-x)}$ and let $\mathcal P$ be the finite sums of convolution squares $u*u^*$, $u\in C_c(G)$. Each such square is continuous with [compact support](../../../function.md#compact-support), and is positive-definite because

$$
\sum_{i,j}z_i\overline{z_j}(u*u^*)(x_i-x_j)=\int_G\left|\sum_i z_i u(t+x_i)\right|^2dm_G(t)\geq0.
$$

Its transform is $|\widehat u|^2$, so every $p\in\mathcal P$ has $\widehat p\geq0$. Also $p*q\in\mathcal P$: convolution of two squares is $(u*v)*(u*v)^*$, and finite sums distribute. Insert the Bochner representation of $q$ into $p*q$ and use the [Fubini theorem](../../../measure-theory.md#fubini-s-theorem) to obtain

$$
(p*q)(x)=\int_{\widehat G}\chi(x)\widehat p(\chi)\,d\mu_q(\chi).
$$

The representing measure on the right is finite and positive. Uniqueness in the [Bochner theorem](../../../analysis.md#bochner-s-theorem) and commutativity now give the [Bochner consistency identity for convolution squares](../../../analysis.md#bochner-consistency-identity-for-convolution-squares)

$$
\widehat p\,\mu_q=\widehat q\,\mu_p=\mu_{p*q}.
$$

For every compact $K\subseteq\widehat G$ there is $p\in\mathcal P$ with $\widehat p>0$ throughout $K$. Indeed, at any $\chi_0$ choose $u=\chi_0 a$, where $a\geq0$ is a nonzero member of $C_c(G)$. Then $\widehat u(\chi_0)=\int a>0$, and continuity supplies a neighbourhood where it stays nonzero. A finite subcover of $K$ and the sum of the corresponding squares give such a $p$.

For $\psi\in C_c(\widehat G)$, choose $p$ positive in transform on its support and define

$$
J(\psi)=\int_{\widehat G}\frac{\psi(\chi)}{\widehat p(\chi)}\,d\mu_p(\chi).
$$

The quotient is set to zero away from the support; its denominator is bounded away from zero there. If $q$ is another choice, the consistency identity, multiplied by $\psi/(\widehat p\widehat q)$ on that [compact support](../../../function.md#compact-support), shows that the integral is unchanged. Choosing one $p$ for a union of supports proves linearity; positivity follows from positivity of $\mu_p$. On each fixed [compact support](../../../function.md#compact-support) it is bounded by $\mu_p(K)/\min_K\widehat p$ times the uniform norm. Moreover, for every $p\in\mathcal P$ and $\psi\in C_c(\widehat G)$, choosing $q$ positive on the support of $\psi$ gives

$$
J(\psi\widehat p)=\int\frac{\psi\widehat p}{\widehat q}\,d\mu_q=\int\psi\,d\mu_p.
$$

A nonzero square has $\mu_p(\widehat G)=p(0)=\|u\|_2^2>0$; a suitable nonnegative [compactly supported](../../../function.md#compact-support) $\psi$ consequently makes this last expression positive. Thus $J$ is nonzero.

To prove translation invariance, fix $\eta\in\widehat G$ and modulate $p$ by $p_\eta(x)=\eta(x)p(x)$. This again belongs to $\mathcal P$, since modulation takes $u*u^*$ to $(\eta u)*(\eta u)^*$. Direct calculation and Bochner uniqueness give

$$
\widehat{p_\eta}(\chi)=\widehat p(\eta^{-1}\chi),\qquad\mu_{p_\eta}=(T_\eta)_*\mu_p,\qquad T_\eta(\chi)=\eta\chi.
$$

Hence, for $\psi_\eta(\chi)=\psi(\eta^{-1}\chi)$, using $p_\eta$ as the denominator function and changing variables gives $J(\psi_\eta)=J(\psi)$. The [Riesz representation on compactly supported continuous functions](../../../functional-analysis.md#riesz-representation-on-compactly-supported-continuous-functions) now produces a nonzero translation-invariant positive [Radon measure](../../../measure-theory.md#radon-measure) $\nu$ on the dual. It is finite on compact sets, so it is [Haar measure](../../../measure-theory.md#haar-measure). This is the compatible [dual Haar measure](../../../group.md#dual-haar-measure), denoted $m_{\widehat G}=\nu$.

The identity for $J(\psi\widehat p)$ says, by uniqueness of [Radon measures](../../../measure-theory.md#radon-measure),

$$
d\mu_p=\widehat p\,d\nu.
$$

Thus $\widehat p\in L^1(\widehat G,\nu)$ and the Bochner representation immediately proves

$$
p(x)=\int_{\widehat G}\widehat p(\chi)\chi(x)\,d\nu(\chi)\qquad(p\in\mathcal P).
$$

It also proves the formula for all finite complex linear combinations of these functions. The measure scale is fixed by this identity: at $x=0$, a nonzero square gives $\int|\widehat u|^2d\nu=\|u\|_2^2$.

A wider inversion class is $f\in L^1(G)$ with $\widehat f\in L^1(\widehat G,\nu)$. To prove this extension, choose nonnegative $a_U\in C_c(G)$ with integral one and support in a small identity neighbourhood $U$, and put $p_U=a_U*a_U^*$. These functions form an [approximate identity](../../../fourier-analysis.md#approximate-identity): they are nonnegative, have integral one and support in $U-U$. Also $0\leq\widehat p_U=|\widehat a_U|^2\leq1$, and $\widehat p_U\to1$ uniformly on compact subsets of the dual. For this [uniform convergence](../../../real-analysis.md#uniform-convergence) use [equicontinuity of compact families of characters](../../../group.md#equicontinuity-of-compact-families-of-characters): evaluation is jointly continuous, as follows from the translation quotient in question 3, and a finite cover of a compact family gives uniform control near the identity.

Convolving the already established inversion formula for $p_U$ with $f$, the [Fubini theorem](../../../measure-theory.md#fubini-s-theorem) gives

$$
(f*p_U)(x)=\int_{\widehat G}\widehat f(\chi)\widehat p_U(\chi)\chi(x)\,d\nu(\chi).
$$

This is justified by $\|f\|_1\mu_{p_U}(\widehat G)<\infty$. Compact-set [uniform convergence](../../../real-analysis.md#uniform-convergence) and an integrable-tail split imply

$$
\int_{\widehat G}|\widehat f|\,|\widehat p_U-1|\,d\nu\longrightarrow0.
$$

Explicitly, first choose a compact set outside which $\int|\widehat f|$ is small, use the bound $|\widehat p_U-1|\leq2$ on that tail, and use [uniform convergence](../../../real-analysis.md#uniform-convergence) on the compact remainder. This argument works for neighbourhood-indexed nets, without assuming metrizability. Consequently $f*p_U$ converges uniformly to the continuous inverse integral. On the other hand, [translation continuity in Lp on a locally compact group](../../../measure-theory.md#translation-continuity-in-lp-on-a-locally-compact-group) gives $f*p_U\to f$ in $L^1$; testing these two limits against $C_c(G)$ shows they agree almost everywhere. At every continuity point of the chosen representative of $f$, the shrinking-support [approximate identity](../../../fourier-analysis.md#approximate-identity) also converges pointwise to $f(x)$. We obtain [Fourier inversion on a locally compact abelian group](../../../analysis.md#fourier-inversion-on-a-locally-compact-abelian-group):

$$
\boxed{f(x)=\int_{\widehat G}\widehat f(\chi)\langle x,\chi\rangle\,dm_{\widehat G}(\chi),\qquad \langle x,\chi\rangle=\chi(x),}
$$

valid everywhere for continuous $f\in L^1(G)$ with integrable transform, and in general as equality with a continuous representative almost everywhere. This class includes all convolution squares above, and their linear span.

Finally, for arbitrary $h\in C_c(G)$, apply the inversion formula at zero to $h*h^*$:

$$
\int_{\widehat G}|\widehat h(\chi)|^2\,d\nu(\chi)=(h*h^*)(0)=\int_G|h(x)|^2\,dm_G(x).
$$

Thus the integral Fourier transform is linear and norm-preserving on $C_c(G)$. That space is dense in $L^2(G)$, so for $f\in L^2(G)$ choose $h_n\in C_c(G)$ with $h_n\to f$ in $L^2$ and define $\mathcal Ff$ as the $L^2(\widehat G,\nu)$ limit of $\widehat h_n$. The norm identity makes this limit exist and independent of the approximating sequence, and preserves linearity. This proves the [Plancherel theorem for locally compact abelian groups](../../../fourier-analysis.md#plancherel-theorem-for-locally-compact-abelian-groups) in the requested form:

$$
\boxed{\mathcal F:L^2(G,m_G)\longrightarrow L^2(\widehat G,m_{\widehat G})\text{ is linear},\qquad\|\mathcal Ff\|_2=\|f\|_2.}
$$

On $L^1\cap L^2$, choose the approximating sequence to converge in both norms; [uniform convergence](../../../real-analysis.md#uniform-convergence) of the integral transforms and their $L^2$ convergence show that this extension agrees almost everywhere with the original transform. For general $L^2$ functions the extension is defined by norm limits, not by presuming that the pointwise integral exists.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
