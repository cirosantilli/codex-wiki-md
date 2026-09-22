# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_24.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A strict [partial order](../../../set.md#partially-ordered-set) is a [well-founded relation](../../../set-theory.md#well-founded-relation) when every nonempty subset $Y\subseteq P$ has a minimal member:

$$
\boxed{\exists y\in Y\ \forall x\in Y\ \neg(x<_P y).}
$$

In [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) this is equivalent to the absence of an infinite descending sequence $p_0>_Pp_1>_P\cdots$. A descending sequence violates the minimal-member property; conversely, repeatedly choosing a predecessor from a subset with no minimal member constructs such a sequence using the [axiom of choice](../../../set-theory.md#axiom-of-choice).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For a [Sierpiński decomposition of the plane](../../../set-theory.md#sierpinski-decomposition-of-the-plane), $A,B$ partition $\mathbb R^2$, and one has countable vertical sections while the other has countable horizontal sections. With the orientation fixed as follows,

$$
\boxed{A\cap B=\varnothing,\quad A\cup B=\mathbb R^2,\quad
|\{y:(x,y)\in A\}|\leq\aleph_0,\quad
|\{x:(x,y)\in B\}|\leq\aleph_0}
$$

for every real $x,y$. Interchanging the coordinate directions and the names $A,B$ gives the equivalent convention. Here “countable” includes finite sets.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The relation of [eventual domination](../../../set-theory.md#eventual-domination) is

$$
f\leq^*g\quad\Longleftrightarrow\quad
\exists N\in\omega\ \forall n\geq N\ f(n)\leq g(n).
$$

A [dominating family](../../../set-theory.md#dominating-family) $C\subseteq\omega^\omega$ satisfies

$$
\boxed{\forall f\in\omega^\omega\ \exists g\in C\ (f\leq^*g).}
$$

It must dominate every function, and the exceptional finite initial interval may depend on both functions.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Use the [order completeness](../../../set.md#order-completeness) of $\mathbb R$ to define

$$
\boxed{\widetilde\varphi(x)=\sup\{\varphi(d):d\in D, d<x\}.}
$$

The set in this [supremum](../../../real-analysis.md#supremum) is nonempty and bounded above: choose $d_0,d_1\in D$ with $d_0<x<d_1$, using that $D$ is an [order-dense subset](../../../set.md#order-dense-subset). For $x\in D$, all its displayed values lie below $\varphi(x)$. If $y<\varphi(x)$, choose $e\in D$ with $y<e<\varphi(x)$; then $d=\varphi^{-1}(e)<x$. Thus the [supremum](../../../real-analysis.md#supremum) equals $\varphi(x)$.

The extension is strictly increasing. If $x<y$, choose $d,e\in D$ with $x<d<e<y$; then

$$
\widetilde\varphi(x)\leq\varphi(d)<\varphi(e)\leq\widetilde\varphi(y).
$$

Apply the same construction to $\varphi^{-1}$, obtaining $\psi$. For $d<x$, choose $e\in D$ with $d<e<x$; this gives $\varphi(d)<\widetilde\varphi(x)$. For $d>x$, a point of $D$ between $x$ and $d$ similarly gives $\varphi(d)>\widetilde\varphi(x)$. Hence

$$
\{e\in D:e<\widetilde\varphi(x)\}
=\{\varphi(d):d\in D, d<x\}.
$$

Taking inverse images and a [supremum](../../../real-analysis.md#supremum) shows $\psi(\widetilde\varphi(x))=x$. The symmetric argument gives $\widetilde\varphi(\psi(y))=y$, so the extension is an [order automorphism](../../../set.md#order-automorphism).

For uniqueness, any increasing extension $h$ has the same strict lower cut in $D$ at its value $h(x)$. Two distinct real numbers have different cuts in an [order-dense subset](../../../set.md#order-dense-subset), so $h(x)=\widetilde\varphi(x)$. **The extension exists and is unique.**

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

If two [order automorphisms](../../../set.md#order-automorphism) agree on $\mathbb Q$, their values at any real $x$ are the same [supremum](../../../real-analysis.md#supremum) of the common values at rational points below $x$. This is the uniqueness argument for [extension of an order automorphism from a dense subset](../../../set.md#extension-of-an-order-automorphism-from-a-dense-subset); it does not require either automorphism to carry $\mathbb Q$ onto itself.

Their restrictions belong to $\mathbb R^{\mathbb Q}$, whose [cardinality](../../../set-theory.md#cardinality) is

$$
(2^{\aleph_0})^{\aleph_0}=2^{\aleph_0}.
$$

This gives the upper bound. The translations $x\mapsto x+r$, one for each real $r$, are distinct [order automorphisms](../../../set.md#order-automorphism), giving the lower bound. Consequently

$$
\boxed{|\operatorname{Aut}(\mathbb R,<)|=2^{\aleph_0}.}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Write $\mathfrak c=2^{\aleph_0}$ and enumerate all nonidentity [order automorphisms](../../../set.md#order-automorphism) of the real line as $\langle h_\alpha:\alpha<\mathfrak c\rangle$. We construct sets of points to include and exclude, starting with $I_0=\mathbb Q$ and $E_0=\varnothing$.

At stage $\alpha$, each of $I_\alpha,E_\alpha$ has [cardinality](../../../set-theory.md#cardinality) less than $\mathfrak c$. Since $h_\alpha$ is a nonidentity increasing bijection, its moved points contain a nonempty open interval. Indeed if $h_\alpha(u)>u$, points between $u$ and $h_\alpha(u)$ are moved; the other direction is similar. There are therefore $\mathfrak c$ moved points. Choose one, $x_\alpha$, outside

$$
I_\alpha\cup E_\alpha\cup h_\alpha^{-1}[I_\alpha\cup E_\alpha].
$$

Then put $x_\alpha$ into $I$ and $h_\alpha(x_\alpha)$ into $E$. They are different, and the included and excluded sets remain disjoint. Take unions at limit stages. This recursion works even when $\mathfrak c$ is singular: before stage $\alpha$, only countably many initial points and at most $|\alpha|$ chosen pairs have been used.

Let $X=\mathbb Q\cup\{x_\alpha:\alpha<\mathfrak c\}$. It is an [order-dense subset](../../../set.md#order-dense-subset) of [cardinality](../../../set-theory.md#cardinality) $\mathfrak c$. Any nonidentity [order automorphism](../../../set.md#order-automorphism) of $X$ extends uniquely to some $h_\alpha$ of $\mathbb R$, but its value at $x_\alpha\in X$ is the excluded point $h_\alpha(x_\alpha)\notin X$, a contradiction. Thus **the resulting [rigid dense subset of the real line](../../../set.md#rigid-dense-subset-of-the-real-line) satisfies**

$$
\boxed{|X|=\mathfrak c,\qquad\operatorname{Aut}(X,<)=\{\mathrm{id}\}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On $[\kappa]^\omega$, declare $A\sim B$ when their [symmetric difference](../../../set.md#symmetric-difference) is finite. Use the [well-ordering theorem](../../../set-theory.md#well-ordering-theorem) to choose one representative $R_{[A]}$ from each equivalence class, and color by

$$
\boxed{c(A)=|A\triangle R_{[A]}|\pmod2.}
$$

Removing one point from a countably infinite set does not change its equivalence class and reverses this parity. For any $H\subseteq\kappa$ of order type $\omega$ and $x\in H$, both $H$ and $H\setminus\{x\}$ belong to $[H]^\omega$ and receive different colors. There is no homogeneous $H$ of [order type](../../../set-theory.md#order-type) $\omega$. This proves the negative [infinite-arity partition relation](../../../set-theory.md#infinite-arity-partition-relation)

$$
\boxed{\kappa\nrightarrow(\omega)^\omega_2.}
$$

The slashed arrow in the PDF is essential.

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A [Suslin line](../../../foundations-of-mathematics.md#suslin-line) is a [dense linear order without endpoints](../../../foundations-of-mathematics.md#dense-linear-order-without-endpoints) that is [order-complete](../../../set.md#order-completeness), has the [countable chain condition for a linear order](../../../set.md#countable-chain-condition-for-a-linear-order), and is not separable in its [order topology](../../../set.md#order-topology). Thus every disjoint family of nonempty open intervals is countable, but there is no countable [order-dense subset](../../../set.md#order-dense-subset). The completeness condition says that every nonempty bounded-above subset has a [supremum](../../../real-analysis.md#supremum). These requirements distinguish a [Suslin line](../../../foundations-of-mathematics.md#suslin-line) from the real line, which has the countable [order-dense subset](../../../set.md#order-dense-subset) $\mathbb Q$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

A [Kurepa tree](../../../set.md#kurepa-tree) is a [set-theoretic tree](../../../set.md#set-theoretic-tree) of height $\omega_1$, with every level countable, possessing at least $\aleph_2$ distinct [cofinal branches](../../../set.md#cofinal-branch). The predecessors of each node are well ordered; their [order type](../../../set-theory.md#order-type) is the node's height. A [cofinal branch](../../../set.md#cofinal-branch) is a maximal chain with nodes at unbounded heights below $\omega_1$, equivalently one node at every level after taking its predecessor closure.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

A [cofinal map](../../../set-theory.md#cofinal-map) $f:\delta\to\alpha$ has a range cofinal in $\alpha$:

$$
\boxed{\forall\xi<\alpha\ \exists\eta<\delta\ (\xi\leq f(\eta)).}
$$

For a limit $\alpha$, this is equivalent to $\sup f[\delta]=\alpha$. For a successor $\alpha$, its largest element must occur in the range. Monotonicity is an additional property and is not part of this definition. The [cofinality](../../../set-theory.md#cofinality) of $\alpha$ is the least [ordinal](../../../set-theory.md#ordinal) that admits such a [cofinal map](../../../set-theory.md#cofinal-map) into $\alpha$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

For clarity, each $\rho_\beta(\alpha)$ is an ordered finite sequence. Its [minimal walk along a club sequence](../../../set-theory.md#minimal-walk-along-a-club-sequence) is finite because its nodes strictly decrease until reaching $\alpha$, and an infinite strictly decreasing sequence of [ordinals](../../../set-theory.md#ordinal) cannot exist. At a step from $\delta>\alpha$, unboundedness of $C_\delta$ supplies $\min(C_\delta\setminus\alpha)$ in $[\alpha,\delta)$.

Compare the two [minimal walks along a club sequence](../../../set-theory.md#minimal-walk-along-a-club-sequence) to $\xi$ and to $\alpha$. As long as their current node is the same $\delta>\alpha$, their next nodes agree exactly when $C_\delta$ has no point in $[\xi,\alpha)$. At the first such point, the walk to $\xi$ moves to

$$
\min(C_\delta\setminus\xi)\in[\xi,\alpha),
$$

whereas the walk to $\alpha$ stays at or above $\alpha$. If this does not occur before the second walk terminates, the first walk reaches $\alpha$ with it and then makes its next step below $\alpha$.

Thus there is an index $j$, possibly the terminal index of the walk to $\alpha$, with

$$
\boxed{\beta_i^\xi=\beta_i^\alpha\ (i\leq j),\qquad
\xi\leq\beta_{j+1}^\xi<\alpha.}
$$

It is unique: after this step the first walk stays below $\alpha$, so it can never again coincide with a node of the walk to $\alpha$. This is the [first-divergence lemma for minimal walks](../../../set-theory.md#first-divergence-lemma-for-minimal-walks).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Let $j$ be the common-prefix index from the [first-divergence lemma for minimal walks](../../../set-theory.md#first-divergence-lemma-for-minimal-walks). If $j=n$, the walk to $\xi$ has followed the entire walk to $\alpha$ and must make at least one further step, contradicting the assumed equality of lengths. Hence $j<n$.

The current nodes agree, so put $\delta=\beta_j^\xi=\beta_j^\alpha$. Then $C_\delta\cap\xi$ is an initial segment of $C_\delta\cap\alpha$. It is proper because $\beta_{j+1}^\xi\in C_\delta\cap[\xi,\alpha)$. Therefore

$$
\boxed{C_{\beta_j^\xi}\cap\xi\text{ is a proper initial segment of }
C_{\beta_j^\alpha}\cap\alpha.}
$$

In particular, **each function $\rho_\beta$ is injective**: equality of two trace sequences would give equal lengths and then contradict this proper-initial-segment conclusion.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

There is a useful explicit reconstruction of a shorter trace from a longer one. Suppose

$$
\rho_\beta(\alpha)=\langle S_0,\ldots,S_{n-1}\rangle,
\qquad S_i=C_{\beta_i^\alpha}\cap\alpha,
$$

and fix $\xi<\alpha$. Let $j<n$ be the first index with $S_j\setminus\xi\ne\varnothing$, if it exists. Before that index, the walk to $\xi$ follows the walk to $\alpha$. At index $j$ it moves to $\delta=\min(S_j\setminus\xi)<\alpha$. Thus

$$
\rho_\beta(\xi)
=\langle S_i\cap\xi:i\leq j\rangle\mathbin{{}^\frown}\rho_\delta(\xi).
$$

When $\delta=\xi$, the appended trace is empty. If no such $j$ exists, the walk first reaches $\alpha$ and then continues toward $\xi$, giving

$$
\rho_\beta(\xi)
=\langle S_i\cap\xi:i<n\rangle\mathbin{{}^\frown}\rho_\alpha(\xi).
$$

Both formulas depend only on the displayed sequence, $\alpha,\xi$, and the fixed [club sequence](../../../set-theory.md#club-sequence). Equal traces $\rho_\beta(\alpha)=\rho_\gamma(\alpha)$ consequently reconstruct the same trace at every $\xi<\alpha$. This proves the [trace coherence lemma for minimal walks](../../../set-theory.md#trace-coherence-lemma-for-minimal-walks):

$$
\boxed{\rho_\beta\upharpoonright\alpha=\rho_\gamma\upharpoonright\alpha.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Take $\kappa=\omega_1$ and choose a [club sequence](../../../set-theory.md#club-sequence) on $\omega_2$, each $C_\delta$ of [order type](../../../set-theory.md#order-type) at most $\omega_1$. For a successor $\delta$ use its predecessor as a singleton; at a limit use a cofinal sequence of minimal length. Form the [minimal-walk tree](../../../set-theory.md#minimal-walk-tree)

$$
T_\alpha=\{\rho_\beta\upharpoonright\alpha:\alpha\leq\beta<\omega_2\},
\qquad T=\bigcup_{\alpha<\omega_2}T_\alpha,
$$

ordered by proper extension. Its height is $\omega_2$.

For $\xi<\delta$, the initial segment $C_\delta\cap\xi$ has [order type](../../../set-theory.md#order-type) strictly below $\omega_1$, and is countable. The strict inequality follows because a point of $C_\delta$ at or above $\xi$ occurs later in its enumeration. Hence every entry of every trace is countable. Under the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis), for $|\alpha|\leq\aleph_1$,

$$
|[\alpha]^{\leq\omega}|\leq\aleph_1^{\aleph_0}
=(2^{\aleph_0})^{\aleph_0}=\aleph_1.
$$

There are at most $\aleph_1$ finite sequences of such sets. The [trace coherence lemma for minimal walks](../../../set-theory.md#trace-coherence-lemma-for-minimal-walks) says that, for $\beta>\alpha$, the value $\rho_\beta(\alpha)$ determines $\rho_\beta\upharpoonright\alpha$. The case $\beta=\alpha$ adds at most one node. Thus $|T_\alpha|\leq\aleph_1$ for every level.

Suppose that $T$ had a [cofinal branch](../../../set.md#cofinal-branch), and take the union of its functions, $f$, with domain $\omega_2$. Every $\rho_\beta$ is injective by the proper-initial-segment argument, so $f$ is injective too. On the [stationary set](../../../set-theory.md#stationary-set)

$$
S=\{\alpha<\omega_2:\operatorname{cf}(\alpha)=\omega_1\},
$$

this set is stationary because the supremum of a strictly increasing $\omega_1$-sequence from any [club set](../../../set-theory.md#club-set) has cofinality $\omega_1$ and lies in that club. The union of the finitely many countable entries of $f(\alpha)$ is bounded below $\alpha$. Assign a strict upper bound below $\alpha$ to obtain a [regressive function](../../../set-theory.md#regressive-function). By [Fodor lemma](../../../set-theory.md#fodor-lemma), there is a stationary $S'\subseteq S$ and a single $\eta<\omega_2$ such that every entry of $f(\alpha)$ lies inside $\eta$ for $\alpha\in S'$. There are at most $\aleph_1$ such finite sequences by the same [cardinal arithmetic](../../../set-theory.md#cardinal-arithmetic), but $|S'|=\aleph_2$, contradicting injectivity.

Therefore **$T$ is an [aleph-two Aronszajn tree](../../../set.md#aleph-two-aronszajn-tree)**:

$$
\boxed{\operatorname{ht}(T)=\omega_2,\quad |T_\alpha|<\aleph_2,
\quad T\text{ has no cofinal branch}.}
$$

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The [diagonal intersection](../../../set-theory.md#diagonal-intersection) of the family is

$$
\boxed{\mathop{\triangle}_{\alpha<\delta}C_\alpha
=\{\beta<\delta:\forall\alpha<\beta\ (\beta\in C_\alpha)\}.}
$$

Membership at $\beta$ only tests the sets indexed below $\beta$, rather than every set of the family. At a regular uncountable $\delta$, a [diagonal intersection](../../../set-theory.md#diagonal-intersection) of [club sets](../../../set-theory.md#club-set) is again a [club set](../../../set-theory.md#club-set).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

[Fodor lemma](../../../set-theory.md#fodor-lemma) says that if $\lambda$ is a regular uncountable [cardinal](../../../set-theory.md#cardinal-number), $S\subseteq\lambda$ is stationary, and $f:S\to\lambda$ is regressive, then

$$
\boxed{\exists\xi<\lambda\quad\{\alpha\in S:f(\alpha)=\xi\}\text{ is stationary}.}
$$

Here a [regressive function](../../../set-theory.md#regressive-function) satisfies $f(\alpha)<\alpha$ at every nonzero $\alpha\in S$; removing $0$ has no effect on stationarity. Both regularity and stationarity are part of the hypotheses.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The [club principle](../../../set-theory.md#club-principle) $\clubsuit$ asserts that there is a sequence $\langle A_\delta:\delta\in\operatorname{Lim}(\omega_1)\rangle$ such that $A_\delta\subseteq\delta$ has [order type](../../../set-theory.md#order-type) $\omega$, is cofinal in $\delta$, and

$$
\boxed{\forall X\in[\omega_1]^{\omega_1}\ \exists\delta\in\operatorname{Lim}(\omega_1)\quad A_\delta\subseteq X.}
$$

It guesses a cofinal countable subset of an uncountable set, with inclusion as the guessing requirement.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Let $\langle D_\alpha:\alpha\in S\rangle$ witness the [stationary diamond principle](../../../set-theory.md#stationary-diamond-principle): for every $A\subseteq\omega_1$, the set of $\alpha\in S$ with $D_\alpha=A\cap\alpha$ is stationary. We construct a normal splitting [Suslin tree](../../../set.md#suslin-tree); this will be a nonspecial [Aronszajn tree](../../../set.md#aronszajn-tree).

Construct its levels by recursion. Start with one root, and give every node two immediate successors. At a countable limit $\alpha$, the constructed portion $T\upharpoonright\alpha$ is countable. Through each of its nodes choose a [cofinal branch](../../../set.md#cofinal-branch) of that portion, and put one new node above each chosen branch at level $\alpha$. This keeps the level countable and gives every earlier node an extension. Branches are identified by their predecessor chains, so nodes at a limit level are uniquely determined by their predecessors.

At a limit $\alpha\in S$, decode $D_\alpha$ as a candidate [tree antichain](../../../set.md#tree-antichain) $B$ of $T\upharpoonright\alpha$. If it is maximal, choose the branches just described to meet $B$. This is possible: for any node, maximality supplies a comparable member of $B$, and normality of the already constructed portion extends the larger of those two nodes to a [cofinal branch](../../../set.md#cofinal-branch) up to $\alpha$. Then every node at level $\alpha$, and every later node, lies above a member of $B$. This is [antichain sealing by diamond](../../../set-theory.md#antichain-sealing-by-diamond).

Here is a precise way to handle the coding. Give the countable level $\xi$ node codes in $[\omega\xi,\omega\xi+\omega)$. There is a [club set](../../../set-theory.md#club-set) of countable limit $\alpha$ with $\omega\alpha=\alpha$, and on this club the nodes below $\alpha$ have exactly the relevant codes below $\alpha$. Empty unused codes are ignored. Thus any subset of the entire tree has an ordinal code set to which the [stationary diamond principle](../../../set-theory.md#stationary-diamond-principle) applies.

Let $B$ now be any maximal [tree antichain](../../../set.md#tree-antichain) of the completed tree. There is a [club set](../../../set-theory.md#club-set) of $\alpha$ such that $B\cap(T\upharpoonright\alpha)$ is maximal in $T\upharpoonright\alpha$. Indeed, choose a comparable member of $B$ for each node; closure under the heights of these witnesses gives that club. Intersect it with the coding club. Stationary correct guessing supplies an $\alpha\in S$ on this intersection at which $B$ is sealed. A member of $B$ at or above level $\alpha$ would extend a member of $B$ below $\alpha$, contradicting the [tree antichain](../../../set.md#tree-antichain) property. So $B$ is contained in the countable portion below $\alpha$. Every [tree antichain](../../../set.md#tree-antichain) extends to a maximal one, hence every [tree antichain](../../../set.md#tree-antichain) is countable.

There is no [cofinal branch](../../../set.md#cofinal-branch) of length $\omega_1$. Otherwise, choosing at each successor level the other successor of its branch node would give an uncountable [tree antichain](../../../set.md#tree-antichain). Thus the resulting tree is a [Suslin tree](../../../set.md#suslin-tree). A [special Aronszajn tree](../../../set.md#special-aronszajn-tree) is a union of countably many [tree antichains](../../../set.md#tree-antichain); here those would all be countable and could not cover the $\aleph_1$ nodes. Therefore

$$
\boxed{\diamondsuit_S\ \Longrightarrow\ \text{a nonspecial Aronszajn tree exists}.}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The [diamond theorem in the constructible universe](../../../definable-power-set.md#diamond-theorem-in-the-constructible-universe) gives $L\models\diamondsuit$, and $L$ satisfies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Apply the preceding construction inside $L$ with $S=\omega_1^L$. It produces a normal splitting [Suslin tree](../../../set.md#suslin-tree).

For completeness, such a tree yields a [Suslin line](../../../foundations-of-mathematics.md#suslin-line). Order its nodes lexicographically using the two successors at every split, treating a node itself as a position between its two successor subtrees. Each node is thus a cut point between a left and a right subtree. This gives a [dense linear order without endpoints](../../../foundations-of-mathematics.md#dense-linear-order-without-endpoints). Every nonempty interval contains a whole cone above some node: for comparable endpoints use the successor cone of the descendant endpoint directed toward the other endpoint; for incomparable endpoints use the right-successor cone of the lower endpoint. Disjoint intervals therefore supply pairwise incomparable cone roots, so the order has the [countable chain condition for a linear order](../../../set.md#countable-chain-condition-for-a-linear-order). A countable collection of nodes has bounded heights; a cone based above that bound contains none of them, so it is not an [order-dense subset](../../../set.md#order-dense-subset). Passing to the [Dedekind completion](../../../set.md#dedekind-completion) using proper cuts, so that no endpoints are added, preserves density, the [countable chain condition for a linear order](../../../set.md#countable-chain-condition-for-a-linear-order), and nonseparability. For nonseparability, a countable dense set in the completion would give a countable dense set of original nodes by choosing one original node between each distinct pair of its points. This contradicts the preceding height-bound argument. The result is a [Suslin line](../../../foundations-of-mathematics.md#suslin-line).

Thus the [Suslin hypothesis](../../../foundations-of-mathematics.md#suslin-hypothesis) fails in $L$. The [constructible universe theorem](../../../definable-power-set.md#constructible-universe-theorem) is a theorem of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), so this is a relative-consistency argument, without an additional assumption that a transitive model exists:

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow
\operatorname{Con}(\mathrm{ZFC}+\neg\mathrm{SH}).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Choose $\aleph_2$ distinct [cofinal branches](../../../set.md#cofinal-branch) of the [Kurepa tree](../../../set.md#kurepa-tree) and regard them as subsets of its underlying set $\omega_1$. Let $\mathcal F$ be this family. Fix an ordinal $\alpha<\omega_1$. The countably many node codes below $\alpha$ have heights bounded by some $\delta<\omega_1$. A [cofinal branch](../../../set.md#cofinal-branch) meets level $\delta$, and its node there determines all its predecessors, hence all its nodes with codes below $\alpha$. Since level $\delta$ is countable,

$$
\boxed{|\mathcal F|=\aleph_2,\qquad
|\{X\cap\alpha:X\in\mathcal F\}|\leq\aleph_0\quad(\alpha<\omega_1).}
$$

This is the [Kurepa-family hypothesis](../../../set.md#kurepa-family-hypothesis). The given compatibility between the ordinal codes and the tree order ensures in particular that the branches are consistently viewed as subsets of $\omega_1$; boundedness of the heights of the countably many codes is what the argument uses.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Start with the [set-theoretic tree](../../../set.md#set-theoretic-tree) of initial characteristic functions

$$
T_\alpha=\{\chi_X\upharpoonright\alpha:X\in\mathcal F\},\qquad\alpha<\omega_1,
$$

ordered by extension. The [Kurepa-family hypothesis](../../../set.md#kurepa-family-hypothesis) makes each level countable, because its members are in one-to-one correspondence with the distinct traces $X\cap\alpha$. Every node extends to every higher level using an $X$ that witnesses it. Nodes at limit levels are uniquely determined by their predecessors, and the distinct $X$ give $\aleph_2$ distinct [cofinal branches](../../../set.md#cofinal-branch).

We can also ensure the splitting requirement in the definition of a [normal set-theoretic tree](../../../set.md#normal-set-theoretic-tree). Keep only nodes through which $\aleph_2$ of these branches pass. There are $\aleph_1$ nodes in total. For a discarded node, at most $\aleph_1$ of the selected branches pass through it, so at most $\aleph_1$ branches meet any discarded node. Remove those branches; $\aleph_2$ branches remain, and each retained node still has $\aleph_2$ remaining branches through it. It therefore has two different retained extensions at some later level, and has a retained extension at every higher level.

Choose increasing countable levels $\langle\delta_\xi:\xi<\omega_1\rangle$, starting at $0$, continuously at limits, so that all nodes at level $\delta_\xi$ split before level $\delta_{\xi+1}$. This is possible because each selected level is countable. Restrict to these levels and relabel them by $\xi$. The retained tree now has one root, extensions at every higher level, at least two immediate successors, and unique limits of predecessor chains. Distinct remaining branches stay distinct on this unbounded set of levels. Hence **the resulting [normal set-theoretic tree](../../../set.md#normal-set-theoretic-tree) is a [Kurepa tree](../../../set.md#kurepa-tree)**, with

$$
\boxed{\text{height }\omega_1,\quad\text{countable levels},\quad
\text{at least }\aleph_2\text{ cofinal branches}.}
$$

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

A [standard membership model of set theory](../../../set-theory.md#standard-membership-model-of-set-theory) has the actual membership relation:

$$
\boxed{E^M=\in\upharpoonright(M\times M),\qquad (M,\in)\models\mathrm{ZFC}.}
$$

When “standard model” is used with the transitive-model convention, one also requires $M$ to be transitive: $x\in y\in M$ implies $x\in M$. Under a convention where standard means only actual membership, this extra requirement defines a [transitive model](../../../set-theory.md#transitive-model). The [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) arguments below use transitive models of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), so that bounded quantification and [ordinals](../../../set-theory.md#ordinal) have their intended meaning.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) states that if $R$ is a well-founded extensional relation on a set $X$, then there is a unique transitive set $M$ and a unique bijection $\pi:X\to M$ such that

$$
\boxed{xRy\quad\Longleftrightarrow\quad\pi(x)\in\pi(y).}
$$

Extensionality means that distinct elements of $X$ have distinct predecessor sets. The collapse is characterized by the recursion

$$
\pi(y)=\{\pi(x):xRy\}.
$$

Well-founded recursion defines it, extensionality makes it injective, and its range is transitive. Uniqueness follows by [well-founded induction](../../../set-theory.md#well-founded-induction). For a class version, the relation must also be [set-like](../../../set-theory.md#set-like-relation); its predecessor sets must be sets.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

An [absolute formula](../../../set-theory.md#absolute-formula) has the same truth value in the structures under comparison for parameters common to them. For transitive models $M\subseteq N$ and $a_1,\ldots,a_n\in M$, the requirement is

$$
\boxed{M\models\varphi(a_1,\ldots,a_n)
\quad\Longleftrightarrow\quad
N\models\varphi(a_1,\ldots,a_n).}
$$

One specifies the relevant class of models, for example transitive models of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). A formula is upward absolute when the forward implication holds and downward absolute when the reverse implication holds. [Bounded formulas in set theory](../../../set-theory.md#bounded-formula-in-set-theory) are absolute between transitive membership structures: all their quantifiers range over the same elements of their parameter sets.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

**The rank characterization holds for a set relation, or a [set-like](../../../set-theory.md#set-like-relation) class relation.** For such a [well-founded relation](../../../set-theory.md#well-founded-relation), use [well-founded recursion](../../../set-theory.md#well-founded-recursion) to define

$$
\boxed{\rho(y)=\sup\{\rho(x)+1:xRy\}.}
$$

The predecessor set is a set, so the [supremum](../../../real-analysis.md#supremum) is an [ordinal](../../../set-theory.md#ordinal). For a [set-like](../../../set-theory.md#set-like-relation) class relation, the closure of the predecessors of any one point under finitely many predecessor steps is a set; perform the ordinary set recursion there. Uniqueness makes these local definitions agree, producing a class rank function. The formula immediately gives $xRy\Rightarrow\rho(x)<\rho(y)$.

Conversely, suppose such an ordinal-valued function exists. For any nonempty subset, or nonempty subclass in the class formulation, take an element whose rank is least among the ranks occurring. It has no predecessor in that subset or subclass, because a predecessor would have smaller rank. This proves well-foundedness.

There is a qualification in the printed class formulation. If well-founded class relations are defined to include [set-likeness](../../../set-theory.md#set-like-relation), it is already implicit and the assertion is correct. Under the minimal-element definition alone, it must be supplied. Without [set-likeness](../../../set-theory.md#set-like-relation), let $X=\operatorname{Ord}\cup\{u\}$, where $u=\{1\}$ is not an [ordinal](../../../set-theory.md#ordinal), and put every ordinal below $u$, with the usual ordinal order below it. Every nonempty subclass has a minimal element, so the relation is well founded. But [transfinite induction](../../../set-theory.md#transfinite-induction) forces $\rho(\alpha)\geq\alpha$ for all ordinals, whereas $\rho(u)$ would have to exceed every $\rho(\alpha)$. No such ordinal exists. Thus the unrestricted class assertion is false; **set-likeness is necessary for this standard rank proof**.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Let $M\subseteq N$ be transitive models of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) containing the set relation $R$ and its underlying set $X$. If $M$ judges $R$ well founded, it has an [ordinal rank function for a relation](../../../set-theory.md#ordinal-rank-function-for-a-relation) $\rho\in M$ by the preceding rank characterization. Being a function to [ordinals](../../../set-theory.md#ordinal) and satisfying

$$
\forall x,y\in X\ (xRy\Rightarrow\rho(x)<\rho(y))
$$

is absolute: the values are actual ordinals and the checks use only [bounded formulas in set theory](../../../set-theory.md#bounded-formula-in-set-theory). The same rank function exists in $N$, so $N$ judges $R$ well founded.

Conversely, if $M$ judged it not well founded, it would contain a nonempty set $Y$ with no $R$-minimal element. The property of this particular $Y$ is bounded and remains true in $N$, contradicting well-foundedness there. Thus

$$
\boxed{M\models\text{“}R\text{ is well founded”}
\iff N\models\text{“}R\text{ is well founded”}.}
$$

This is [absoluteness of well-foundedness](../../../set-theory.md#absoluteness-of-well-foundedness). The hypotheses that both models are transitive and satisfy [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) matter; a small transitive set without sufficient recursion axioms need not contain the required rank witness.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Put $\mathcal V=\langle V_\kappa,\in,R\rangle$. Because $\kappa$ is inaccessible, $|V_\xi|<\kappa$ for every $\xi<\kappa$, and $\kappa$ is regular. Choose one witness in $V_\kappa$ for every existential formula of this expanded language and every finite parameter tuple for which a witness exists. These are [Skolem functions](../../../mathematical-logic.md#skolem-function); they can be chosen in the ambient universe even when $R$ is not definable inside $V_\kappa$.

For each $\xi<\kappa$, the ranks of all chosen witnesses with parameters from $V_\xi$ have [supremum](../../../real-analysis.md#supremum) below $\kappa$: there are fewer than $\kappa$ such parameters and only countably many formulas. Choose $F(\xi)<\kappa$ strictly above those ranks. The limit closure points

$$
C=\{\alpha<\kappa:\alpha\text{ is limit and }\forall\xi<\alpha\ F(\xi)<\alpha\}
$$

form a [club set](../../../set-theory.md#club-set). At $\alpha\in C$, every existential assertion in $\mathcal V$ with parameters in $V_\alpha$ has a witness in $V_\alpha$. The [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test) yields

$$
\langle V_\alpha,\in,R\cap V_\alpha\rangle\prec\mathcal V.
$$

Thus the set $E$ of all such elementary levels is unbounded. It is also closed: the union at a limit of increasing elementary levels is an [elementary substructure](../../../mathematical-logic.md#elementary-substructure) by the [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem), and the union of their ranks is $V_\alpha$ with predicate $R\cap V_\alpha$. Therefore

$$
\boxed{E\text{ is closed and unbounded in }\kappa.}
$$

This is [club reflection below an inaccessible cardinal](../../../set-theory.md#club-reflection-below-an-inaccessible-cardinal).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

If $\kappa$ is a [Mahlo cardinal](../../../set-theory.md#mahlo-cardinal), its inaccessible ordinals form a [stationary set](../../../set-theory.md#stationary-set). For any $R\subseteq V_\kappa$, intersect that set with the [club set](../../../set-theory.md#club-set) of elementary levels from [club reflection below an inaccessible cardinal](../../../set-theory.md#club-reflection-below-an-inaccessible-cardinal). This supplies an inaccessible $\alpha<\kappa$ with the required [elementary substructure](../../../mathematical-logic.md#elementary-substructure).

Conversely, take an arbitrary [club set](../../../set-theory.md#club-set) $C\subseteq\kappa$ and use it as the predicate $R$. In $\langle V_\kappa,\in,C\rangle$, the sentence asserting that predicate-marked ordinals occur above every ordinal is true. Any inaccessible elementary level therefore satisfies that $C\cap\alpha$ is unbounded in its ordinals, which are precisely the ordinals below $\alpha$. Since $C$ is closed and $\alpha$ is a limit ordinal, $\alpha\in C$. The assumed reflection property consequently gives an inaccessible ordinal in every [club set](../../../set-theory.md#club-set). Hence the inaccessible ordinals are stationary and

$$
\boxed{\kappa\text{ is Mahlo}\iff
\text{every predicate has an inaccessible elementary rank level below }\kappa.}
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

First express inaccessibility by universally excluding witnesses to its failure. Besides $\kappa$ being an ordinal greater than $\omega$, require that for every $\alpha<\kappa$ there is no function from $\alpha$ cofinal in $\kappa$, and no injection from $\kappa$ into $\mathcal P(\alpha)$. The first condition gives regular cardinalhood; the second says that $\kappa$ is a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal). Under the [axiom of choice](../../../set-theory.md#axiom-of-choice) these are exactly the conditions for a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal).

These are [Pi-one formulas modulo ZF](../../../set-theory.md#pi-one-formula-modulo-zf): the only unbounded quantifiers universally range over possible functions. Being a function of the specified domain, having bounded or cofinal range in $\kappa$, and being an injection whose values are subsets of $\alpha$ can all be written with [bounded formulas in set theory](../../../set-theory.md#bounded-formula-in-set-theory), without using a power-set object as an unbounded existential witness. Consequently inaccessibility is downward absolute to a transitive [inner model](../../../set-theory.md#inner-model) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice).

Now suppose $\kappa$ is Mahlo in $V$. It is inaccessible in the [constructible universe](../../../definable-power-set.md#constructible-universe) $L$, and every $V$-inaccessible ordinal below it is also inaccessible in $L$. Let $C\in L$ be any set that $L$ regards as a [club set](../../../set-theory.md#club-set) in $\kappa$. Closure and unboundedness are absolute properties of this fixed set of ordinals, so $C$ is also a [club set](../../../set-theory.md#club-set) in $V$. By Mahloness in $V$, it contains an ordinal that is inaccessible in $V$, hence in $L$. Every $L$-club therefore meets the $L$-inaccessible ordinals below $\kappa$. Thus **[Mahloness is downward absolute to the constructible universe](../../../set-theory.md#mahloness-is-downward-absolute-to-the-constructible-universe)**:

$$
\boxed{L\models\text{“}\kappa\text{ is Mahlo”}.}
$$

## 5

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Use the [countable-condition collapse](../../../forcing.md#countable-condition-collapse)

$$
\boxed{\mathbb P=\operatorname{Col}(\omega_1,\kappa)
=\{p:p\text{ is a countable partial function from }\omega_1\text{ to }\kappa\},}
$$

ordered by reverse inclusion: an extension of a function is a stronger condition. All sizes and conditions here are computed in the ground model $M$.

This forcing is [countably closed](../../../forcing.md#countably-closed-forcing): the union of a descending countable sequence is a countable partial function. Thus it adds no countable ordinal sequences and preserves $\omega_1$. For each $\xi<\omega_1$, the conditions whose domains contain $\xi$ are dense; for each $\eta<\kappa$, those whose ranges contain $\eta$ are dense. The union of the [generic filter](../../../forcing.md#generic-filter) is therefore a surjection from $\omega_1$ onto $\kappa$, and $|\kappa|^{M[G]}=\aleph_1$.

Inaccessibility gives $\kappa^{\aleph_0}=\kappa$: every countable sequence is bounded below the regular $\kappa$, and the [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) property bounds the number of sequences at each bound below $\kappa$. Hence $|\mathbb P|=\kappa$. The forcing satisfies the $\kappa^+$-[chain condition for forcing](../../../forcing.md#chain-condition-for-forcing), so it preserves every cardinal above $\kappa$. **This gives precisely the requested collapse and preservation.** The assertion that $\kappa$ is collapsed to $\aleph_1$ concerns its new cardinality; the ordinal $\kappa$ itself does not change.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

**For an arbitrary ground model, this alternative needs an additional arithmetic hypothesis.** The requested countable-cover property already prevents any collapse of an infinite ground-model cardinal. If a cardinal $\theta$ were collapsed, there would be a surjection $f:\alpha\to\theta$ with $|\alpha|^M<\theta$. The asserted ground-model $F$ would cover $\theta$ by the union of $|\alpha|^M$ countable sets, a ground-model set of size at most $\max(\aleph_0,|\alpha|^M)<\theta$, a contradiction. Thus all infinite cardinals are preserved.

Put $\lambda=(\aleph_3)^M$, which must then remain $\aleph_3$. If the extension has continuum $\lambda$, it has

$$
\lambda^{\aleph_0}=(2^{\aleph_0})^{\aleph_0}=\lambda.
$$

The ground-model functions from $\omega$ into $\lambda$ remain present and their cardinality cannot be collapsed. Necessarily

$$
\boxed{M\models\lambda^{\aleph_0}=\lambda.}
$$

For example, a ground model with continuum larger than $\aleph_3$ cannot satisfy the printed request. This is a genuine missing hypothesis, rather than a forcing construction that works for every $M$.

Under the necessary hypothesis, use [Cohen forcing](../../../forcing.md#cohen-forcing) to add $\lambda$ reals:

$$
\mathbb P=\operatorname{Fn}(\lambda\times\omega,2,{<}\omega).
$$

The [delta-system lemma](../../../set-theory.md#delta-system-lemma) shows that it has the [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing): an uncountable family of finite conditions has an uncountable subfamily whose domains form a delta-system and whose values agree on its root, so any two of that subfamily are compatible. It therefore preserves cardinals. Its $\lambda$ coordinate reals are pairwise distinct by dense disagreement requirements. Conversely each [nice forcing name](../../../forcing.md#nice-forcing-name) for a real uses countably many countable [antichains in a forcing order](../../../forcing.md#antichain-in-a-forcing-order), so the number of such names is at most $\lambda^{\aleph_0}=\lambda$. Hence

$$
\boxed{M[G]\models2^{\aleph_0}=\aleph_3.}
$$

For any ordinal-valued function name, choose for each $\xi<\alpha$ a maximal [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) deciding its value. The [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing) makes the set $F(\xi)$ of possible ordinal values countable in $M$. Pad it with $\omega$ if needed to make it countably infinite. The [possible-values lemma for chain-condition forcing](../../../forcing.md#possible-values-lemma-for-chain-condition-forcing) gives the stronger pointwise covering statement

$$
\boxed{f(\xi)\in F(\xi)\quad(\xi<\alpha),}
$$

which implies the requested range inclusion. When a condition only forces that the name is such a function, make these choices below that condition; it belongs to the generic filter witnessing the actual function.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Use [diamond-sequence forcing](../../../forcing.md#diamond-sequence-forcing). A condition is a sequence

$$
p=\langle A_\xi:\xi\leq\delta_p\rangle,qquad
\delta_p<\omega_1,\quad A_\xi\subseteq\xi,
$$

ordered by end extension. Its countable descending chains have lower bounds: take their union and, if their lengths approach a new limit, add an arbitrary subset at that last index. Hence it is [countably closed](../../../forcing.md#countably-closed-forcing) and preserves $\omega_1$. The union of the [generic filter](../../../forcing.md#generic-filter) supplies $\langle A_\xi:\xi<\omega_1\rangle$.

To prove the [diamond principle](../../../set-theory.md#diamond-principle), let a condition force that $\dot X\subseteq\omega_1$ and that $\dot C$ is a [club set](../../../set-theory.md#club-set). Below any such condition build $p_n$ and strictly increasing countable ordinals $\delta_n$ so that $\delta_n>\delta_{p_n}$, $p_{n+1}$ forces $\delta_n\in\dot C$, decides $\dot X\cap\delta_n$, and has length past $\delta_n$. Unboundedness supplies $\delta_n$; countable closure allows deciding all the bits below it. The construction can be carried out in $M$.

Let $\delta=\sup_n\delta_n=\sup_n\delta_{p_n}$. The union of the conditions has entries exactly below $\delta$ and decides a ground-model set $x=\dot X\cap\delta$. Extend that union by setting $A_\delta=x$. This condition forces $\delta\in\dot C$ by closure, and $A_\delta=\dot X\cap\delta$. The conditions giving a correct guess inside any named [club set](../../../set-theory.md#club-set) are therefore dense. Thus

$$
\boxed{M[G]\models\diamondsuit.}
$$

No ground-model [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis) is needed; this forcing is allowed to collapse higher cardinals.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Fix [forcing names](../../../forcing.md#forcing-name) $\tau,\tau_1,\ldots,\tau_n\in M$ for the set $w$ and the parameters. Define a name

$$
\sigma=\{(\eta,p):\exists q\ ((\eta,q)\in\tau,\ p\leq q,
\ p\Vdash\varphi(\eta,\tau,\tau_1,\ldots,\tau_n))\}.
$$

Only $\eta$ appearing in $\tau$ and $p\in\mathbb P$ are needed, so this is a subset of a ground-model set. The [forcing definability lemma](../../../forcing.md#forcing-definability-lemma) makes its defining predicate a formula of $M$. Ground-model [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) therefore gives $\sigma\in M$.

If $(\eta,p)\in\sigma$ with $p\in G$, the accompanying $q\geq p$ belongs to $G$, so $\eta_G\in\tau_G$. The [forcing theorem](../../../forcing.md#forcing-theorem) gives $\varphi(\eta_G,\tau_G,(\tau_1)_G,\ldots,(\tau_n)_G)$.

Conversely, if $u\in\tau_G$ satisfies this formula, choose $(\eta,q)\in\tau$ with $q\in G$ and $\eta_G=u$. The [forcing truth lemma](../../../forcing.md#forcing-truth-lemma) supplies $r\in G$ forcing the formula for these names. Directedness gives $p\in G$ with $p\leq q,r$. Then $(\eta,p)\in\sigma$, and $u\in\sigma_G$. Thus

$$
\boxed{\sigma_G=\{u\in w:\varphi(u,w,v_1,\ldots,v_n)\}.}
$$

This proves the instance of the [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) in the [generic extension](../../../forcing.md#generic-extension), without assuming that instance there in order to construct the name.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

Countability of the forcing and uncountability of $Y$ are understood internally in $M$ and $M[G]$, respectively. This matters because the model itself is externally countable. Choose a name $\dot Y\in M$ and a ground-model set $A\in M$ containing every ground-model element that can occur in $Y$. Such an $A$ exists: the rank of $\dot Y$ bounds the ranks of its values, so a sufficiently high $V_\theta^M$ contains $Y\subseteq M$.

For $p\in P$, ground-model [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) and the [forcing definability lemma](../../../forcing.md#forcing-definability-lemma) give

$$
X_p=\{a\in A:p\Vdash\check a\in\dot Y\}\in M.
$$

By the [forcing truth lemma](../../../forcing.md#forcing-truth-lemma),

$$
Y=\bigcup_{p\in G}X_p.
$$

If every $X_p$ for $p\in G$ were countable in $M$, it would remain countable in $M[G]$, where $G\subseteq P$ is countable. Then $Y$ would be countable, contrary to the hypothesis. Thus some $p\in G$ has $X_p$ uncountable in $M$; otherwise its ground-model enumeration would still enumerate it in the extension. Let $X=X_p$. Every one of its members is forced by $p$ into $Y$, so

$$
\boxed{X\in M,\quad M\models|X|>\aleph_0,\quad
M[G]\models X\subseteq Y.}
$$

The [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing) also preserves its uncountability. Separativity is not needed for this particular argument. This is the [ground-model uncountable subset lemma for countable forcing](../../../forcing.md#ground-model-uncountable-subset-lemma-for-countable-forcing).

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

The finite binary-function [Cohen forcing](../../../forcing.md#cohen-forcing) $\operatorname{Fn}(\omega,2,{<}\omega)$ is countable in $M$. It preserves $\omega_1$, and the countable levels, height, and normal extensions of the ground-model tree remain unchanged.

If the extension contained an uncountable [tree antichain](../../../set.md#tree-antichain), apply the [ground-model uncountable subset lemma for countable forcing](../../../forcing.md#ground-model-uncountable-subset-lemma-for-countable-forcing) to obtain an uncountable $X\in M$ contained in it. Incomparability in the fixed ground-model tree is absolute, so $M$ already regards $X$ as an uncountable [tree antichain](../../../set.md#tree-antichain), contradicting that $T$ is Suslin in $M$. Similarly, a new [cofinal branch](../../../set.md#cofinal-branch) has an uncountable ground-model subset. Comparability is absolute, so this would be an uncountable chain in the ground-model tree, again impossible.

Therefore **[countable forcing preserves Suslin trees](../../../forcing.md#countable-forcing-preserves-suslin-trees)**, and in particular

$$
\boxed{M[G]\models\text{“}T\text{ is a Suslin tree”}.}
$$

## 6

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

The forcing is [cardinal-preserving](../../../forcing.md#cardinal-preserving-forcing) over $M$ when every ground-model cardinal remains a cardinal in every [generic extension](../../../forcing.md#generic-extension):

$$
\boxed{\forall G\text{ generic over }M\ \forall\kappa\in M\quad
M\models\text{“}\kappa\text{ is a cardinal”}
\Rightarrow M[G]\models\text{“}\kappa\text{ is a cardinal”}.}
$$

[Forcing preserves ordinals](../../../forcing.md#forcing-preserves-ordinals), and an ordinal that was not a cardinal already has a ground-model bijection with a smaller ordinal, which persists. Thus this definition gives equality of the cardinal ordinals in the two models.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

The [forcing definability lemma](../../../forcing.md#forcing-definability-lemma) states that for each formula $\varphi(v_1,\ldots,v_n)$ there is a first-order formula $\mathrm{Force}_\varphi$, depending on $\varphi$ but not on the chosen names, such that for $p\in P$ and [forcing names](../../../forcing.md#forcing-name) $\tau_i\in M$,

$$
\boxed{p\Vdash_M\varphi(\tau_1,\ldots,\tau_n)
\iff M\models\mathrm{Force}_\varphi(p,\tau_1,\ldots,\tau_n,\mathbb P).}
$$

The order relation of $\mathbb P$ is included in its set code. Thus each instance of the forcing relation is definable inside the ground model, allowing the uses of ground-model [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) and replacement in the forcing arguments.

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

The forcing is $\kappa$-closed in $M$ when every descending sequence of conditions of length less than $\kappa$, belonging to $M$, has a lower bound in $M$:

$$
\boxed{\delta<\kappa,\quad p_\eta\leq p_\xi\ (\xi<\eta<\delta)
\ \Longrightarrow\ \exists q\in P\ \forall\xi<\delta\ q\leq p_\xi.}
$$

We use the convention that $q\leq p$ means that $q$ is stronger. In particular, $\omega_1$-[closed forcing](../../../forcing.md#closed-forcing) is [countably closed](../../../forcing.md#countably-closed-forcing). Internal quantification over the sequences is essential when $M$ is externally countable.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

This is the [Rasiowa–Sikorski lemma](../../../forcing.md#rasiowa-sikorski-lemma). Put $p_0=p$ and recursively choose

$$
p_{n+1}\leq p_n,\qquad p_{n+1}\in D_n,
$$

using density. Set

$$
\boxed{G=\{q\in P:\exists n\ p_n\leq q\}.}
$$

It contains $p$, is upward closed toward weaker conditions, and is directed: if $p_i\leq q$ and $p_j\leq r$, then $p_{\max(i,j)}$ is a common stronger condition in $G$. It meets each $D_n$ through $p_{n+1}$. Thus $G$ is the required [generic filter](../../../forcing.md#generic-filter) for the prescribed countable family of dense sets. For a [countable transitive model](../../../forcing.md#countable-transitive-model), externally enumerate its dense sets to obtain a generic filter over the model by this same argument.

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

The PDF's middle equality is **$(\omega^2)^M=(\omega^2)^{M[G]}$**, concerning ordinal exponentiation. The TeX incorrectly turns the exponent into a subscript; preserving $\omega_2$ would be incompatible with forcing CH over many ground models.

Let $A=(\mathcal P(\omega))^M$ and use the [countable-condition collapse](../../../forcing.md#countable-condition-collapse) of $A$ onto $\omega_1$:

$$
\boxed{\mathbb P=\{p:p\text{ is a countable partial function }\omega_1\to A\},}
$$

ordered by extension. Countable unions give lower bounds, so [closed forcing adds no short ordinal sequences](../../../forcing.md#closed-forcing-adds-no-short-ordinal-sequences); in particular it adds no reals and preserves $\omega_1$. Dense requirements ensure that the union of the [generic filter](../../../forcing.md#generic-filter) is a total surjection $g:\omega_1\to A$. Thus

$$
\boxed{\aleph_1^M=\aleph_1^{M[G]},\qquad
\mathcal P(\omega)^{M[G]}=\mathcal P(\omega)^M,\qquad
\operatorname{ran}(g)=\mathcal P(\omega)^{M[G]}.}
$$

Finally [forcing preserves ordinals](../../../forcing.md#forcing-preserves-ordinals), and the recursion defining ordinal multiplication and exponentiation is absolute. Both models compute $\omega^2$ as the same order type of $\omega$ successive copies of $\omega$. This proves the printed middle equality too. Higher cardinals may collapse, which is allowed by the actual PDF.

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

In the [generic extension](../../../forcing.md#generic-extension) from the preceding construction, a surjection from $\omega_1$ onto all reals gives $2^{\aleph_0}\leq\aleph_1$. [Cantor theorem](../../../set.md#cantor-s-theorem) gives the reverse inequality, so the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis) holds.

For the exact consistency-strength statement, existence of a [countable transitive model](../../../forcing.md#countable-transitive-model) is stronger than bare consistency of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). One can formalize the forcing proof syntactically, or use the [constructible universe theorem](../../../definable-power-set.md#constructible-universe-theorem): [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) proves that its [constructible universe](../../../definable-power-set.md#constructible-universe) satisfies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) and the [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis). If there is any model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), its internal constructible universe is therefore a model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) with CH. By the [Godel completeness theorem](../../../mathematical-logic.md#godel-s-completeness-theorem),

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow
\operatorname{Con}(\mathrm{ZFC}+\mathrm{CH}).}
$$

This deduction does not silently replace consistency by existence of a transitive model.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

For each $\xi<\kappa$, choose a maximal [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) below $p$ deciding a witness $\eta>\xi$ in $\dot C$. Write the decided values as $\eta_{\xi,q}$, one for each condition $q$ in that antichain. The $\kappa$-[chain condition for forcing](../../../forcing.md#chain-condition-for-forcing) gives fewer than $\kappa$ possible values. Since $\kappa$ is regular in $M$, choose

$$
g(\xi)=\sup\{\eta_{\xi,q}+1:q\text{ is in the chosen antichain}\}<\kappa.
$$

The [possible-values lemma for chain-condition forcing](../../../forcing.md#possible-values-lemma-for-chain-condition-forcing) ensures

$$
p\Vdash\exists\eta\in\dot C\ (\xi<\eta<g(\xi)).
$$

In $M$ take the [club set](../../../set-theory.md#club-set) of limit closure points

$$
\boxed{D=\{\delta<\kappa:\delta\text{ is limit and }
\forall\xi<\delta\ g(\xi)<\delta\}.}
$$

It is unbounded by repeatedly closing any starting ordinal under $g$ for countably many steps, and closed by taking increasing limits. For $\delta\in D$, the forced displayed property gives points of $\dot C$ arbitrarily high below $\delta$. Its forced closedness yields $\delta\in\dot C$. Therefore

$$
\boxed{D\in M\text{ is club},\qquad p\Vdash\check D\subseteq\dot C.}
$$

This proves the [ground-model club containment lemma](../../../forcing.md#ground-model-club-containment-lemma). The name on the right is $\dot C$, as printed in the PDF.

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

Fix $p$ and a name $\dot f$ such that $p$ forces a two-coloring of $[\lambda]^{<\omega}$. For each ground-model finite set $a\subseteq\lambda$, record its full [forcing decision pattern](../../../forcing.md#forcing-decision-pattern)

$$
F(a)(q)=\begin{cases}
0,&q\leq p\text{ and }q\Vdash\dot f(\check a)=0,\\
1,&q\leq p\text{ and }q\Vdash\dot f(\check a)=1,\\
2,&\text{otherwise}.
\end{cases}
$$

There are at most $3^{|\mathbb P|}<\lambda$ such patterns, since $\lambda$ is a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) and $|\mathbb P|<\lambda$. For finite $\mathbb P$ the number of patterns is finite, also below $\lambda$. Encode the patterns by an ordinal $\beta<\lambda$ and apply the assumed [finite-subset partition property](../../../set-theory.md#finite-subset-partition-property) to obtain $H\subseteq\lambda$ of size $\lambda$ such that $F$ is constant on $[H]^n$ for every $n<\omega$.

For each $n$, choose one $a_n\in[H]^n$. Conditions below $p$ deciding $\dot f(a_n)$ are dense. Whenever one such condition decides the value, equality of patterns means it forces that same value at every $a\in[H]^n$. A [generic filter](../../../forcing.md#generic-filter) containing $p$ meets this dense set for each $n$, so $f$ is constant on each $[H]^n$ in the extension. The constants may differ with $n$, exactly as required.

The forcing has size below the regular $\lambda$, hence satisfies the $\lambda$-[chain condition for forcing](../../../forcing.md#chain-condition-for-forcing) and preserves its cardinality. The ground-model set $H$ consequently still has size $\lambda$. Since the argument works for every name and condition,

$$
\boxed{\Vdash_{\mathbb P}\lambda\rightarrow(\lambda)^{<\omega}_2.}
$$

This is [small forcing preservation of finite-subset partition properties](../../../set-theory.md#small-forcing-preservation-of-finite-subset-partition-properties); no closure assumption on the forcing is required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
