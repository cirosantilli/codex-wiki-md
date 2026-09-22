# Paper 6

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper6.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper6.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)

## 1

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

We first prove the algebraic extension step needed for [Hahn-Banach separation theorem](../../../functional-analysis.md#hahn-banach-separation-theorem). Suppose $p$ is a finite [sublinear functional](../../../functional-analysis.md#sublinear-function) on a real [vector space](../../../vector-space.md) and $g$ is a [linear functional](../../../linear-algebra.md#linear-functional) on a [vector subspace](../../../vector-space.md#vector-subspace) $W$, with $g\leq p$ there. For $v\notin W$, choose a real number $c$ between

$$
\sup_{w\in W}\{g(w)-p(w-v)\}
\quad\hbox{and}\quad
\inf_{w\in W}\{p(w+v)-g(w)\}.
$$

This interval is nonempty: for any $w,z\in W$,

$$
g(w)+g(z)=g(w+z)\leq p(w+z)\leq p(w-v)+p(z+v).
$$

Taking $w=0$ or $z=0$ also bounds the endpoints by finite numbers. Define $\widetilde g(w+tv)=g(w)+tc$. For $t>0$, the upper bound for $c$, applied to $w/t$, proves $\widetilde g(w+tv)\leq p(w+tv)$. For $t<0$, writing $t=-s$ and using the lower bound at $w/s$ proves the same inequality. The case $t=0$ is the original domination. Thus a dominated [linear functional](../../../linear-algebra.md#linear-functional) extends over one further direction. Order all dominated extensions by extension of their domains. A chain has its union as an upper bound, so [Zorn's lemma](../../../set-theory.md#zorn-s-lemma) supplies a maximal extension. The one-direction argument shows its domain is the whole [vector space](../../../vector-space.md). This proves the required algebraic [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem), rather than assuming the separation result.

Choose $a\in A$, and put $C=A-a$. This is a [radially open convex set](../../../mathematical-optimization.md#radially-open-convex-set) containing zero. It is absorbing: along each line through zero, sufficiently small multiples of any vector lie in $C$. Its [Minkowski functional](../../../topological-vector-space.md#minkowski-functional)

$$
p(x)=\inf\{t>0:x\in tC\}
$$

is finite and nonnegative. Positive homogeneity follows by rescaling $t$. If $x\in sC$ and $y\in tC$, convexity gives $x+y\in(s+t)C$, proving [subadditivity](../../../real-analysis.md#subadditive-sequence) by taking infima. Moreover,

$$
C=\{x:p(x)<1\}.
$$

Indeed, $p(x)<1$ gives $x\in sC$ for some $s<1$, hence $x\in C$ by convexity and $0\in C$. Conversely, radial openness at $x\in C$ permits $(1+\epsilon)x\in C$ for some $\epsilon>0$, giving $p(x)<1$.

Since $A\cap U=\varnothing$, $a\notin U$ and $u-a\notin C$ for every $u\in U$. Define a [linear functional](../../../linear-algebra.md#linear-functional) on $U+\mathbb Ra$ by

$$
g(u+ta)=-t.
$$

It is well defined because $a\notin U$. For $t<0$, write $s=-t$; then $p(u+ta)=s\,p(u/s-a)\geq s=g(u+ta)$. For $t\geq0$, domination follows from $g(u+ta)\leq0\leq p(u+ta)$. The extension step therefore gives $L:V\to\mathbb R$ with $L\leq p$, $L|_U=0$ and $L(a)=-1$. If $x\in A$, then

$$
L(x)+1=L(x-a)\leq p(x-a)<1,
$$

so $L(x)<0$. Consequently

$$
\boxed{H=\ker L\supseteq U,\qquad H\cap A=\varnothing.}
$$

Because $L(a)\ne0$, this [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) has codimension one and is a [hyperplane](../../../vector-space.md#hyperplane). This establishes the [geometric Hahn-Banach theorem for radially open sets](../../../functional-analysis.md#geometric-hahn-banach-theorem-for-radially-open-sets) without assuming a norm or a topology on $V$.

For the [convex function](../../../real-analysis.md#convex-function), use its strict [epigraph](../../../calculus-of-variations.md#epigraph) in $V\times\mathbb R$. It is nonempty and convex, and does not contain $(0,0)$. It is also radially open: on every affine line, a finite [convex function](../../../real-analysis.md#convex-function) is continuous. To justify this last fact, convexity orders secant slopes; on a smaller interval the slopes are bounded above and below by slopes to two fixed exterior endpoints, giving a local Lipschitz bound. Thus $t\mapsto f(x+ty)-\beta-ts$ is continuous, and a strict negative value persists near $t=0$.

Apply the separation theorem with the zero subspace. A nonzero separating [linear functional](../../../linear-algebra.md#linear-functional) has form $L(x,\beta)=g(x)+c\beta$. Its values on the convex [epigraph](../../../calculus-of-variations.md#epigraph) cannot have both signs, since a line segment would then meet its kernel. Choose the sign so that $L>0$ on the [epigraph](../../../calculus-of-variations.md#epigraph). At $x=0$ and $\beta>0$ this gives $c>0$. Letting $\beta$ decrease to $f(x)$ yields $g(x)+cf(x)\geq0$. Therefore

$$
\boxed{l(x)=-g(x)/c\leq f(x)\quad\hbox{for every }x\in V.}
$$

The resulting [linear functional](../../../linear-algebra.md#linear-functional) need not be nonzero: for example, the zero functional is the only linear minorant of $f(x)=x^2$ on $\mathbb R$.

Now suppose the norm and continuity hypotheses hold. Domination at $x$ and $-x$ gives

$$
-f(-x)\leq l(x)\leq f(x).
$$

If $x_n\in\ker l$ and $x_n\to x$ in norm, apply this inequality to $x-x_n$. Since $l(x-x_n)=l(x)$ and both bounding values tend to $f(0)=0$, we obtain $l(x)=0$. The [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) is therefore closed.

Finally, a [linear functional with closed kernel](../../../topological-vector-space.md#linear-functional-with-closed-kernel) on a [normed vector space](../../../functional-analysis.md#normed-vector-space) is continuous. If $l=0$, this is immediate. Otherwise choose $v$ with $l(v)=1$ and put $M=\ker l$. Closedness gives $d=\operatorname{dist}(v,M)>0$. For $l(x)\ne0$, $x/l(x)-v\in M$, so $d\leq\|x\|/|l(x)|$. The same resulting bound holds when $l(x)=0$:

$$
\boxed{|l(x)|\leq d^{-1}\|x\|.}
$$

This proves continuity and explains exactly how closedness of the kernel is used.

## 2

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

**False.** We construct a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) with a countable dense discrete subspace but no compatible [metric](../../../topological-analysis.md#metric). Let

$$
P=\{0,1\}^{\mathcal P(\mathbb N)},\qquad
j(n)_S=\begin{cases}1&n\in S,\\0&n\notin S,\end{cases}
$$

for each subset $S\subseteq\mathbb N$. Give $P$ its [product topology](../../../geometry-and-topology.md#product-topology), and let $X=\overline{j(\mathbb N)}$ in $P$. The [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem) makes $P$ compact, and the product is Hausdorff; hence $X$ is a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space). By construction, $Y=j(\mathbb N)$ is countable and dense in $X$, so $X$ is a [separable topological space](../../../topology.md#separable-topological-space). The coordinate $S=\{n\}$ isolates $j(n)$ within $Y$. Thus the subspace topology on $Y$ is discrete and is induced by the [discrete metric](../../../topological-analysis.md#discrete-metric).

Suppose $X$ were metrizable. An infinite sequence of distinct points of $Y$ would have a convergent subsequence, by sequential compactness of a [compact metric space](../../../topological-analysis.md#compact-metric-space). Write this subsequence as $j(n_k)$ with distinct $n_k$. For $S=\{n_2,n_4,n_6,\ldots\}$, its $S$ coordinate alternates between zero and one and therefore does not converge. But coordinate projections are continuous in the [product topology](../../../geometry-and-topology.md#product-topology), so every coordinate of a convergent sequence must converge. This contradiction proves that $X$ is not metrizable. This is a [separable compactification need not be metrizable](../../../topology.md#separable-compactification-need-not-be-metrizable) counterexample.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

**True.** In the [norm topology](../../../functional-analysis.md#norm-topology) on the unit ball, the set $\{x\in B:\|x\|<1/2\}$ is a neighbourhood of zero. If the relative [weak topology](../../../weak-topology.md) agrees with it, there are finitely many [continuous linear functionals](../../../topological-vector-space.md#continuous-linear-functional) $f_1,\ldots,f_m$ and positive $\epsilon_j$ such that

$$
\{x\in B:|f_j(x)|<\epsilon_j\text{ for }1\leq j\leq m\}
\subseteq\{x\in B:\|x\|<1/2\}.
$$

If $\bigcap_j\ker f_j$ contained a nonzero vector, rescaling it to have norm $3/4$ would put it in the left-hand set but not the right-hand set. Therefore $\bigcap_j\ker f_j=\{0\}$. The [linear map](../../../vector-space.md#linear-map)

$$
x\longmapsto(f_1(x),\ldots,f_m(x))
$$

is injective into a finite-dimensional scalar space, so

$$
\boxed{\dim E\leq m<\infty.}
$$

This proof works for either the open or closed unit-ball convention and does not require completeness.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

**False.** Take the separable [Banach space](../../../banach-space.md) $E=\ell^1$, whose [continuous dual space](../../../continuous-dual-space.md) is $\ell^\infty$. We prove that first countability of the weak unit ball would force this dual to be norm separable, producing a contradiction.

Suppose that $B$ had a countable weak neighbourhood base $(U_n)$ at zero. Inside each $U_n$, choose a basic relative weak neighbourhood specified by finitely many [continuous linear functionals](../../../topological-vector-space.md#continuous-linear-functional) $F_n$. The union $F=\bigcup_nF_n$ is countable. For any $f\in E'$ and $\epsilon>0$, some $U_n$ lies in $\{x\in B:|f(x)|<\epsilon\}$. On the [vector subspace](../../../vector-space.md#vector-subspace)

$$
M_n=\bigcap_{g\in F_n}\ker g,
$$

this implies $\|f|_{M_n}\|\leq\epsilon$, by scaling vectors into $B$. The [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) extends $f|_{M_n}$ to $h\in E'$ with $\|h\|\leq\epsilon$. The functional $f-h$ vanishes on $M_n$ and is therefore a linear combination of $F_n$: it factors through the finite-dimensional coordinate map $x\mapsto(g(x))_{g\in F_n}$, and a [linear functional](../../../linear-algebra.md#linear-functional) on that map's image extends to the finite-dimensional coordinate space. Hence

$$
\operatorname{dist}(f,\operatorname{span}F_n)\leq\epsilon.
$$

Every $f\in E'$ thus belongs to the norm closure of $\operatorname{span}F$. Taking rational coefficients, or rational real and imaginary parts, gives a countable norm-dense subset of $E'$. This proves that [weak-ball metrizability requires a norm-separable dual](../../../weak-topology.md#weak-ball-metrizability-requires-a-norm-separable-dual).

For $\ell^1$, every bounded sequence $a=(a_j)$ defines $f_a(x)=\sum_ja_jx_j$ with $\|f_a\|=\|a\|_\infty$. Conversely, the values $f(e_j)$ of any bounded [linear functional](../../../linear-algebra.md#linear-functional) determine such a sequence and recover $f$ by density of finitely supported vectors. Thus $E'=\ell^\infty$. The uncountable family $\{0,1\}^{\mathbb N}$ in $\ell^\infty$ has distance one between distinct members, so this dual is not norm separable: disjoint balls of radius less than $1/2$ would require distinct members of any countable dense set. Since every metrizable space is first countable, the weak unit ball of $\ell^1$ is not metrizable.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

**True.** Choose a norm-dense sequence $(x_n)$ in the unit ball of the separable [normed vector space](../../../functional-analysis.md#normed-vector-space) $E$. On the dual unit ball $B'$, define

$$
\boxed{d(\phi,\psi)=\sum_{n=1}^{\infty}2^{-n}|\phi(x_n)-\psi(x_n)|.}
$$

Each summand is at most $2^{1-n}$, so the series converges uniformly. Symmetry and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) follow term by term. If $d(\phi,\psi)=0$, the two continuous functionals agree on the dense sequence, hence on the unit ball and then on all of $E$. Thus $d$ is a [metric](../../../topological-analysis.md#metric).

A relative weak-star neighbourhood controls finitely many evaluations. Conversely, to make $d$ small, first choose a tail whose sum is small and then control the finitely many evaluations at $x_1,\ldots,x_N$. This proves that each [metric](../../../topological-analysis.md#metric) ball is weak-star open. For the other direction, let $x\in E$ and $\epsilon>0$. Approximate $x/\|x\|$ by $x_n$ when $x\ne0$. Since $\|\phi-\psi\|\leq2$ on $B'$,

$$
|\phi(x)-\psi(x)|
\leq\|x\|\,|\phi(x_n)-\psi(x_n)|+2\|x\|\,\|x/\|x\|-x_n\|.
$$

The second term can be made smaller than $\epsilon/2$ by choosing $n$; the first is smaller than $\epsilon/2$ whenever $d(\phi,\psi)$ is sufficiently small, because $|\phi(x_n)-\psi(x_n)|\leq2^n d(\phi,\psi)$. Every evaluation is therefore metric-continuous. These two inclusions show that $d$ induces exactly the [weak-star topology](../../../weak-topology.md#weak-star-topology), proving [weak-star metrizability of the dual ball](../../../weak-topology.md#weak-star-metrizability-of-the-dual-ball) without a completeness assumption on $E$.

## 3

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We construct a normalized positive translation-invariant functional on $C(G)$ and then represent it by a measure. The main step is a finite [matching in a graph](../../../graph-theory.md#matching-graph-theory) argument, for which we establish all the covering-net properties.

Let $V$ be an open neighbourhood of the identity in the compact [topological group](../../../topological-group.md) $G$. The sets $xV$, $x\in G$, form an open cover. Compactness supplies a finite set $F$ with $G=FV$. Among all such finite sets choose one of smallest cardinality, denoted $m(V)$. This is a [minimal left covering net of a compact group](../../../measure-theory.md#minimal-left-covering-net-of-a-compact-group). If $g\in G$, then $G=gFV$, and $gF$ has the same cardinality. Hence $gF$ is also minimal for the same $V$.

Let $F,F'$ be any two [minimal left covering nets of a compact group](../../../measure-theory.md#minimal-left-covering-net-of-a-compact-group) for $V$. They both have cardinality $m(V)$. Form a [bipartite graph](../../../graph-theory.md#bipartite-graph) by joining $x\in F$ to $y\in F'$ whenever $xV\cap yV\ne\varnothing$. For a subset $S\subseteq F$, let $N(S)$ be its set of neighbours. Every point of $SV$ lies in some $yV$ with $y\in F'$; that $y$ is a neighbour of a member of $S$. Therefore

$$
SV\subseteq N(S)V,
$$

and $(F\setminus S)\cup N(S)$ is still a left covering set. By minimality,

$$
m(V)\leq |(F\setminus S)\cup N(S)|\leq m(V)-|S|+|N(S)|.
$$

Thus $|N(S)|\geq|S|$. [Hall's marriage theorem](../../../graph-theory.md#hall-s-marriage-theorem) gives a [bijection](../../../function.md#bijection) $\pi:F\to F'$ with $xV\cap\pi(x)V\ne\varnothing$ for every $x$. If $xv=\pi(x)v'$ at an intersection point, then

$$
\boxed{x^{-1}\pi(x)=vv'^{-1}\in VV^{-1}.}
$$

This proves the [matching minimal covering nets of a compact group](../../../measure-theory.md#matching-minimal-covering-nets-of-a-compact-group) property, including the estimate needed below.

For a continuous complex-valued function $f$ on $G$, define

$$
I_F(f)=\frac1{|F|}\sum_{x\in F}f(x),\qquad
\omega_f(W)=\sup\{|f(xw)-f(x)|:x\in G,\ w\in W\}.
$$

Continuity and compactness imply $\omega_f(W)\to0$ as identity neighbourhoods $W$ shrink. Here is the uniformity argument: continuity of $(x,w)\mapsto f(xw)-f(x)$ at each $(x,e)$ gives a product neighbourhood where its absolute value is small; finitely many of the first-coordinate neighbourhoods cover $G$, and intersecting the corresponding second-coordinate neighbourhoods gives one $W$ that works for every $x$.

Matched pairs therefore give

$$
|I_F(f)-I_{F'}(f)|\leq\omega_f(VV^{-1}).
$$

In particular, with $F'=gF$,

$$
\boxed{|I_F(f\circ L_g)-I_F(f)|\leq\omega_f(VV^{-1}),\qquad L_g(x)=gx.}
$$

The estimate holds for every $g\in G$; no commutativity of $G$ is being assumed.

Direct the open identity neighbourhoods by reverse inclusion and choose a [minimal left covering net of a compact group](../../../measure-theory.md#minimal-left-covering-net-of-a-compact-group) $F_V$ for each. The values $I_{F_V}(f)$ lie in the closed complex disk of radius $\|f\|_\infty$. The [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem) makes the product of these disks over all $f\in C(G)$ compact. Consequently the [net](../../../topology.md#net-mathematics) of vectors $(I_{F_V}(f))_{f\in C(G)}$ has a convergent [subnet](../../../topology.md#subnet-of-a-net). Call its coordinatewise limit $I(f)$. Since each finite average is linear, positive on nonnegative real functions, and equal to one at the constant function one, the limit satisfies

$$
I(\alpha f+\beta h)=\alpha I(f)+\beta I(h),\qquad I(f)\geq0\ (f\geq0),\qquad I(1)=1,
$$

and $|I(f)|\leq\|f\|_\infty$. Thus $I$ is a bounded [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional).

Given an identity neighbourhood $W$, continuity of multiplication and inversion supplies a sufficiently small $V$ with $VV^{-1}\subseteq W$. The translation estimate consequently tends to zero along the [subnet](../../../topology.md#subnet-of-a-net). For every $f\in C(G)$ and every $g\in G$,

$$
\boxed{I(f\circ L_g)=I(f).}
$$

The [Riesz-Markov-Kakutani representation theorem](../../../functional-analysis.md#riesz-markov-kakutani-representation-theorem) now represents $I$ by a regular positive [Borel measure](../../../measure-theory.md#borel-measure) $\mu$ with $\mu(G)=1$. The preceding equality and uniqueness in that representation imply that the pushforward under every left translation equals $\mu$. Hence

$$
\boxed{\mu(gE)=\mu(E)\quad\hbox{for every Borel set }E\subseteq G.}
$$

This is the required normalized [Haar measure](../../../measure-theory.md#haar-measure). It is nonzero because its total mass is one. In fact every nonempty open set has positive measure: its left translates cover $G$, a finite subcover exists, and a zero measure for that open set would force $\mu(G)=0$.

For completeness, the constructed probability measure is also right invariant. Apply [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) to $f(x^{-1}y)$ with both variables distributed according to $\mu$. Integrating first in $y$ gives $\int f\,d\mu$ by left invariance. Integrating first in $x$ and substituting $x=yz$ gives $\int f(z^{-1})\,d\mu(z)$. Thus $\mu$ is invariant under inversion. Inversion turns a right translation into a left translation, so right invariance follows. This last observation is not needed for the existence of a left [Haar measure](../../../measure-theory.md#haar-measure), but confirms the usual two-sided normalization for [compact groups](../../../topological-group.md#compact-group).

## 4

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [uniform algebra](../../../banach-algebra.md#uniform-algebra) on a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) $K$ is a closed complex subalgebra $A\subseteq C(K)$ containing the constants and separating points of $K$, with the [supremum norm](../../../functional-analysis.md#supremum-norm). It is therefore a commutative unital [Banach algebra](../../../banach-algebra.md). Its [character space of an algebra](../../../banach-algebra.md#character-space-of-an-algebra) $\Phi_A$, also called its carrier space, consists of nonzero multiplicative [linear functionals](../../../linear-algebra.md#linear-functional), equipped with the [Gelfand topology](../../../banach-algebra.md#gelfand-topology).

For $x\in K$, evaluation gives the [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) $\delta_x(f)=f(x)$. The map $\delta:K\to\Phi_A$ is continuous: composing it with the coordinate $\varphi\mapsto\varphi(f)$ gives the continuous function $f$ for every $f\in A$. It is injective because $A$ separates points. The [Gelfand topology](../../../banach-algebra.md#gelfand-topology) is Hausdorff because distinct [algebra characters](../../../banach-algebra.md#character-of-an-algebra) differ on some element of $A$. A continuous injection from compact $K$ into a Hausdorff space is a [homeomorphism](../../../topology.md#homeomorphism) onto its image: closed subsets of $K$ have compact, hence closed, images. Its image is also compact and closed. Thus

$$
\boxed{\delta:K\longrightarrow j(K)=\{\delta_x:x\in K\}\subseteq\Phi_A}
$$

is the asserted [homeomorphism](../../../topology.md#homeomorphism). A [natural uniform algebra](../../../banach-algebra.md#natural-uniform-algebra) is one for which this image is all of $\Phi_A$.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

We prove the forward direction of the [finite-generator criterion for a natural uniform algebra](../../../banach-algebra.md#finite-generator-criterion-for-a-natural-uniform-algebra). Suppose that $A$ is a [natural uniform algebra](../../../banach-algebra.md#natural-uniform-algebra), and let $f_1,\ldots,f_n$ have no common zero on $K$. The [ideal](../../../commutative-algebra.md#ideal)

$$
J=f_1A+\cdots+f_nA
$$

is all of $A$. Otherwise it is contained in a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $M$, whose associated [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) vanishes on all the $f_j$. Since every [algebra character](../../../banach-algebra.md#character-of-an-algebra) is an [evaluation character](../../../banach-algebra.md#evaluation-character) under naturality, this would give a common zero, a contradiction. Therefore $1\in J$, meaning that

$$
\boxed{\sum_{j=1}^nf_jg_j=1\quad\hbox{for suitable }g_j\in A.}
$$

Here are the Banach-algebra details behind the [algebra character](../../../banach-algebra.md#character-of-an-algebra) associated with $M$. A proper [ideal](../../../commutative-algebra.md#ideal) cannot have dense closure: if it contained an element within distance less than one of $1$, the [Neumann series](../../../banach-algebra.md#neumann-series) would make that element invertible, forcing the [ideal](../../../commutative-algebra.md#ideal) to contain $1$. Thus the closure of a proper [ideal](../../../commutative-algebra.md#ideal) is proper. A [maximal ideal](../../../commutative-algebra.md#maximal-ideal), obtained from [Zorn's lemma](../../../set-theory.md#zorn-s-lemma), is therefore closed. Its quotient is a complex unital [Banach algebra](../../../banach-algebra.md) in which every nonzero element is invertible. The [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem) identifies this quotient with $\mathbb C$, so the quotient map is the required [algebra character](../../../banach-algebra.md#character-of-an-algebra). No closedness of the originally generated [ideal](../../../commutative-algebra.md#ideal) $J$ is needed.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Assume the finite-generator identity holds whenever there is no common zero. Let $\varphi\in\Phi_A$. For every finite family $f_1,\ldots,f_n\in\ker\varphi$, their zero sets must have nonempty intersection: otherwise an identity $\sum f_jg_j=1$ would give $0=\varphi(1)=1$. These zero sets are closed in compact $K$. The [finite intersection property](../../../topology.md#finite-intersection-property) therefore supplies $x\in K$ at which every member of $\ker\varphi$ vanishes. For any $f\in A$, the element $f-\varphi(f)1$ is in that kernel, so $f(x)=\varphi(f)$. Thus $\varphi=\delta_x$, proving

$$
\boxed{\text{the finite-generator identity holds}\iff A\text{ is natural}.}
$$

For $C(K)$, the identity is explicit. If the $f_j$ have no common zero, the continuous function $q=\sum_j|f_j|^2$ is strictly positive on compact $K$. Set

$$
g_j=\frac{\overline{f_j}}{q}\in C(K).
$$

Then $\sum f_jg_j=1$. The equivalence just proved shows that **$C(K)$ is natural**.

Next consider the [disc algebra](../../../banach-algebra.md#disk-algebra) $A(\overline{\mathbb D})$, the continuous functions on the closed unit disk that are holomorphic in its interior. We show directly that each [algebra character](../../../banach-algebra.md#character-of-an-algebra) is evaluation. Polynomials are uniformly dense in this algebra: for $0<r<1$, $f_r(z)=f(rz)$ tends uniformly to $f$ as $r\uparrow1$, by [uniform continuity](../../../topological-analysis.md#uniform-continuity). The function $f_r$ is holomorphic on $|z|<1/r$, so its Taylor polynomials converge uniformly on $|z|\leq1$.

Every [algebra character](../../../banach-algebra.md#character-of-an-algebra) of a unital [Banach algebra](../../../banach-algebra.md) is bounded, with $|\varphi(f)|\leq\|f\|$: if $f-\varphi(f)1$ were invertible, applying $\varphi$ would contradict invertibility, so $\varphi(f)$ belongs to the [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element), which is contained in the disk of radius $\|f\|$ by the [Neumann series](../../../banach-algebra.md#neumann-series). For the coordinate function $z$, put $\lambda=\varphi(z)$; then $|\lambda|\leq1$. Multiplicativity gives $\varphi(p)=p(\lambda)$ for every polynomial. By polynomial density and continuity, $\varphi(f)=f(\lambda)$ for every member of the [disc algebra](../../../banach-algebra.md#disk-algebra). Hence

$$
\boxed{\Phi_{A(\overline{\mathbb D})}\cong\overline{\mathbb D},\qquad A(\overline{\mathbb D})\text{ is natural}.}
$$

Finally consider the algebra $C$ in the last request. For each $f\in C$, its holomorphic extension $g$ from the boundary is unique by the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle). Define $T(f)=g\in A(\overline{\mathbb D})$. This is a surjective unital algebra homomorphism, since it restricts to the identity on the [disc algebra](../../../banach-algebra.md#disk-algebra). Also

$$
\|T(f)\|_\infty=\sup_{|z|=1}|f(z)|\leq\|f\|_\infty.
$$

The algebra $C$ is closed: if $f_n\to f$ uniformly, the associated $T(f_n)$ are uniformly Cauchy by this bound, so their limit belongs to the closed [disc algebra](../../../banach-algebra.md#disk-algebra) and agrees with $f$ on the boundary. Constants and the coordinate function belong to $C$, so it is itself a [uniform algebra](../../../banach-algebra.md#uniform-algebra) on the disk. Its [ideal](../../../commutative-algebra.md#ideal)

$$
I=\ker T=\{f\in C(\overline{\mathbb D}):f|_{\partial\mathbb D}=0\}
$$

is contained in $C$, and $C/I$ is the [disc algebra](../../../banach-algebra.md#disk-algebra).

If a [algebra character](../../../banach-algebra.md#character-of-an-algebra) $\chi$ on $C$ vanishes on $I$, it factors through $T$ and the preceding result gives

$$
\chi(f)=T(f)(\lambda)\quad\hbox{for some }\lambda\in\overline{\mathbb D}.
$$

If $\chi$ does not vanish on $I$, choose $h\in I$ with $\chi(h)\ne0$. For $F\in C(\overline{\mathbb D})$, define

$$
\widetilde\chi(F)=\frac{\chi(hF)}{\chi(h)}.
$$

The product $hF$ is in $I$, so this is well defined. It is unital and linear, and

$$
\chi(hF)\chi(hG)=\chi(h^2FG)=\chi(h)\chi(hFG)
$$

shows multiplicativity. Since $C(\overline{\mathbb D})$ is natural, $\widetilde\chi$ is evaluation at a point $x$ of the closed disk. The equality $h(x)=\widetilde\chi(h)=\chi(h)\ne0$ places $x$ in the open disk. On $C$, $\widetilde\chi(f)=\chi(f)$, so $\chi$ itself is evaluation at that interior point.

We therefore obtain two families: actual evaluations $f\mapsto f(x)$ on one closed disk, and analytic-extension evaluations $f\mapsto T(f)(\lambda)$ on a second closed disk. They agree on the boundary. They are distinct at interior points: functions in $I$ distinguish actual interior evaluations from every analytic-extension evaluation, and the coordinate function distinguishes points within each family. Thus

$$
\boxed{\Phi_C\cong\overline{\mathbb D}\ \cup_{\partial\mathbb D}\ \overline{\mathbb D}\cong S^2.}
$$

This is also a topological identification. Each disk family is continuous in the [Gelfand topology](../../../banach-algebra.md#gelfand-topology), and they agree along their boundary, giving a continuous [bijection](../../../function.md#bijection) from the glued disks to $\Phi_C$. The glued disks form a compact space, explicitly homeomorphic to the sphere by sending $(x,y)$ in the two copies to $(x,y,\pm\sqrt{1-x^2-y^2})$. Since the [character space](../../../banach-algebra.md#character-space-of-an-algebra) is Hausdorff, the continuous [bijection](../../../function.md#bijection) is a [homeomorphism](../../../topology.md#homeomorphism). This [boundary-analytic disk algebra with doubled character space](../../../banach-algebra.md#boundary-analytic-disk-algebra-with-doubled-character-space) has more [algebra characters](../../../banach-algebra.md#character-of-an-algebra) than evaluations on its original disk.

## 5

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For an element $a$ of a complex unital [Banach algebra](../../../banach-algebra.md), its [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) is

$$
\boxed{\sigma_A(a)=\{\lambda\in\mathbb C:\lambda1-a\text{ is not invertible in }A\}.}
$$

The [nonzero spectra of products in opposite orders](../../../banach-algebra.md#nonzero-spectra-of-products-in-opposite-orders) agree:

$$
\boxed{\sigma(ab)\setminus\{0\}=\sigma(ba)\setminus\{0\}.}
$$

For $\lambda\ne0$, if $R=(\lambda1-ab)^{-1}$ exists, direct multiplication on both sides verifies

$$
(\lambda1-ba)^{-1}=\lambda^{-1}(1+bRa).
$$

Interchanging $a,b$ proves the converse. Zero may differ. On the [Hilbert space](../../../hilbert-space.md) $\ell^2(\mathbb N_0)$, let $S$ be the [unilateral shift operator](../../../linear-operator-theory.md#unilateral-shift-operator) $Se_n=e_{n+1}$ and take $a=S^*$, $b=S$. Then $ab=S^*S=I$, whereas $ba=SS^*=I-P_0$, where $P_0$ is projection onto the first coordinate. Hence

$$
\boxed{\sigma(ab)=\{1\},\qquad\sigma(ba)=\{0,1\}.}
$$

Both values for the second operator occur on its two nonzero invariant summands; every other value has an inverse obtained separately on those summands.

We use the spectral definition of a [Positive element of a C-star algebra](../../../banach-algebra.md#positive-element-of-a-c-star-algebra): $h$ is positive when $h=h^*$ and $\sigma(h)\subseteq[0,\infty)$. The [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus), supplied by the [Commutative Gelfand--Naimark theorem](../../../banach-algebra.md#commutative-gelfand-naimark-theorem) for the algebra generated by a [Normal element of a C-star algebra](../../../banach-algebra.md#normal-element-of-a-c-star-algebra) and its adjoint, sends $F\in C(\sigma(h))$ to $F(h)$. It preserves products, sums, conjugation and the identity, is isometric, and satisfies $\sigma(F(h))=F(\sigma(h))$. For a self-adjoint element the spectrum is real, so real-valued functions produce self-adjoint elements.

For example, $F(t)=\sqrt t$ gives the [positive square root in a C-star algebra](../../../banach-algebra.md#positive-square-root-in-a-c-star-algebra) of a [Positive element of a C-star algebra](../../../banach-algebra.md#positive-element-of-a-c-star-algebra). It satisfies $(h^{1/2})^2=h$. Its uniqueness follows from the composition rule: if $d\geq0$ and $d^2=h$, then the [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus) in the algebra generated by $d$ gives $\sqrt{d^2}=d$. For positive invertible $h$, the functions $t^{-1}$ and $t^{-1/2}$ give positive inverses and inverse square roots. If $0\leq h$ and $r\geq\|h\|$, the function $r-t$ gives $r1-h\geq0$; the same calculus gives

$$
\|r1-h\|=\max_{t\in\sigma(h)}|r-t|\leq r.
$$

These transfer elementary scalar inequalities for functions of one element to the algebra. They do not justify applying a scalar inequality to arbitrary noncommuting elements.

To prove closure under addition without assuming an order theorem, let $a,b\geq0$, set $\alpha=\|a\|$, $\beta=\|b\|$ and $s=\alpha+\beta$. If $s=0$, both elements are zero. Otherwise,

$$
\|s1-(a+b)\|\leq\|\alpha1-a\|+\|\beta1-b\|\leq s.
$$

The element $a+b$ is self-adjoint, so any $\lambda\in\sigma(a+b)$ is real and satisfies $|s-\lambda|\leq s$. Thus $\lambda\geq0$, proving

$$
\boxed{a,b\geq0\Longrightarrow a+b\geq0.}
$$

We will also use that the positive cone is proper: if $h\geq0$ and $-h\geq0$, then $\sigma(h)\subseteq\{0\}$, and the norm formula for self-adjoint elements gives $h=0$.

We next prove $a^*a\geq0$ without presupposing that positivity is defined by such products. Put $h=a^*a$, which is self-adjoint, and form its negative part by the [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus):

$$
h_- =F(h),\qquad F(t)=\max\{-t,0\}.
$$

This is positive. Let $c=ah_-^{1/2}$. Since $h_-$ commutes with $h$,

$$
c^*c=h_-^{1/2}hh_-^{1/2}=-h_-^2\leq0.
$$

The nonzero product-spectrum identity proved above gives $\sigma(cc^*)\setminus\{0\}=\sigma(c^*c)\setminus\{0\}$. As $cc^*$ is self-adjoint, it too has spectrum in $(-\infty,0]$, so $cc^*\leq0$.

Write $c=u+iv$ with $u=u^*$ and $v=v^*$. The [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus) makes $u^2$ and $v^2$ positive, and the addition result gives

$$
c^*c+cc^*=2(u^2+v^2)\geq0.
$$

But both summands on the left are nonpositive, so their sum is also nonpositive. Properness of the cone forces $c^*c+cc^*=0$. Now $c^*c=-cc^*$ is positive as well as nonpositive, so $c^*c=0$. The [C-star identity](../../../banach-algebra.md#c-star-identity) gives $c=0$, whence $h_-^2=0$ and $h_-=0$. Thus $h$ has no negative spectral part:

$$
\boxed{a^*a\geq0\quad\hbox{for every }a\in A.}
$$

This proves the [positivity of adjoint products from spectral positivity](../../../banach-algebra.md#positivity-of-adjoint-products-from-spectral-positivity) and the equivalence with the usual definition by elements of the form $d^*d$: the reverse direction is the factorization $h=(h^{1/2})^*h^{1/2}$ for $h\geq0$.

Finally, if $a\geq0$ and $c\in A$, write

$$
c^*ac=(a^{1/2}c)^*(a^{1/2}c).
$$

The preceding result therefore proves

$$
\boxed{c^*ac\geq0.}
$$

In particular, [congruence preserves positivity in a C-star algebra](../../../banach-algebra.md#congruence-preserves-positivity-in-a-c-star-algebra), and $a\leq b$ implies $c^*ac\leq c^*bc$. These facts will justify the noncommutative order manipulations in the numbered parts.

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Since $a-1$ and $b-1=(b-a)+(a-1)$ are positive, their spectra are nonnegative. Translation of the [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) gives $\sigma(a),\sigma(b)\subseteq[1,\infty)$, so both elements are invertible. Their inverses and inverse square roots are positive by the [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus). Also $1-a^{-1}$ is positive because the scalar function $1-t^{-1}$ is nonnegative on $\sigma(a)$.

For the order reversal, set

$$
k=a^{-1/2}ba^{-1/2}=1+a^{-1/2}(b-a)a^{-1/2}\geq1.
$$

The inequality uses [congruence preserves positivity in a C-star algebra](../../../banach-algebra.md#congruence-preserves-positivity-in-a-c-star-algebra). [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus) gives $k^{-1}\leq1$. Since

$$
b^{-1}=a^{-1/2}k^{-1}a^{-1/2},
$$

another congruence shows

$$
a^{-1}-b^{-1}=a^{-1/2}(1-k^{-1})a^{-1/2}\geq0.
$$

Consequently

$$
\boxed{0<b^{-1}\leq a^{-1}\leq1.}
$$

Here $b^{-1}$ is strictly positive in the stronger invertible sense: $b^{-1}\geq\|b\|^{-1}1>0$, because its spectrum is the set of reciprocals of the positive spectral values of $b$. This is [inversion reverses the order of strictly positive elements](../../../banach-algebra.md#inversion-reverses-the-order-of-strictly-positive-elements); no commutativity of $a,b$ is required.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Although $ab$ need not be self-adjoint, it is similar to a [Positive element of a C-star algebra](../../../banach-algebra.md#positive-element-of-a-c-star-algebra). Namely,

$$
a^{-1/2}(ab)a^{1/2}=a^{1/2}ba^{1/2}=:d.
$$

By [congruence preserves positivity in a C-star algebra](../../../banach-algebra.md#congruence-preserves-positivity-in-a-c-star-algebra), $d\geq0$. In fact $b\geq1$ gives

$$
d-a=a^{1/2}(b-1)a^{1/2}\geq0,
$$

so $d\geq a\geq1$. Similar elements have the same [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element), because $s^{-1}(x-\lambda1)s$ is invertible exactly when $x-\lambda1$ is. Therefore the stronger conclusion is

$$
\boxed{\sigma(ab)=\sigma(d)\subseteq[1,\infty)\subseteq\mathbb R^+.}
$$

Positivity of the spectrum is being asserted, not positivity of the generally non-self-adjoint product itself.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Take the [C-star algebra](../../../banach-algebra.md#c-star-algebra) $M_2(\mathbb C)$ and choose

$$
a=\begin{pmatrix}1&0\\0&2\end{pmatrix},\qquad
b=\begin{pmatrix}2&1\\1&3\end{pmatrix}.
$$

Then $a-1=\operatorname{diag}(0,1)$ is positive, while

$$
b-a=\begin{pmatrix}1&1\\1&1\end{pmatrix}
$$

is positive, since its [quadratic form](../../../linear-algebra.md#quadratic-form) at $(x,y)$ is $|x+y|^2$. Thus $1\leq a\leq b$, as required. However,

$$
\boxed{b^2-a^2=\begin{pmatrix}4&5\\5&6\end{pmatrix}}
$$

has [determinant](../../../linear-algebra.md#determinant) $-1$ and [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $5\pm\sqrt{26}$, one of which is negative. Equivalently, its [quadratic form](../../../linear-algebra.md#quadratic-form) at the real vector $(5,-4)$ is $-4$. It is therefore not positive. This proves that [squaring is not order preserving in a C-star algebra](../../../banach-algebra.md#squaring-is-not-order-preserving-in-a-c-star-algebra), even for invertible elements bounded below by the identity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
