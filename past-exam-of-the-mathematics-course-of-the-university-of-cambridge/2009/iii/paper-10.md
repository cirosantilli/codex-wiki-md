# Paper 10

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper10.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper10.pdf)

**Table of contents**

- [1](#1)
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
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)

## 1

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose $M$ with $|f|\leq M$ on $U$, and fix $r=(1-\|x\|)/4>0$. We prove a local [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) bound, which gives more than [continuity](../../../calculus.md#continuous-function). Let $u,v\in B(x,r)$, put $d=\|v-u\|$, and suppose $d>0$. The point $w=u+(2r/d)(v-u)$ lies in $B(x,3r)\subset U$, while $d<2r$ and

$$
v=\left(1-\frac d{2r}\right)u+\frac d{2r}w.
$$

By [convexity](../../../real-analysis.md#convex-function), $f(v)-f(u)\leq[d/(2r)](f(w)-f(u))\leq Md/r$. Interchanging $u,v$ gives

$$
\boxed{|f(v)-f(u)|\leq\frac Mr\|v-u\|\qquad(u,v\in B(x,r)).}
$$

The case $d=0$ is immediate. Every point has such a neighborhood, so **$f$ is locally Lipschitz and therefore continuous throughout $U$**. This is the [bounded convex functions are locally Lipschitz on an open ball](../../../real-analysis.md#bounded-convex-functions-are-locally-lipschitz-on-an-open-ball) argument; no finite-dimensional assumption is needed.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Fix $y\in E$, and take $t>0$ sufficiently small that $x+ty\in U$. For $0<s<t$, [convexity](../../../real-analysis.md#convex-function) along the line segment gives

$$
\frac{f(x+sy)-f(x)}s\leq\frac{f(x+ty)-f(x)}t.
$$

Thus the positive secant slopes are nondecreasing in their parameter, and have a limit as the parameter decreases to zero. The local [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) from part (a) bounds their absolute values by $L\|y\|$, where $L=M/r$. Hence the [directional derivative](../../../calculus.md#directional-derivative) exists as a finite real number and

$$
\boxed{|D_yf(x)|\leq L\|y\|.}
$$

For $y=0$ it is zero.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $p(y)=D_yf(x)$. Rescaling the parameter in the [directional derivative](../../../calculus.md#directional-derivative) gives $p(ay)=ap(y)$ for $a>0$, and $p(0)=0$ handles $a=0$. For sufficiently small $t>0$, [convexity](../../../real-analysis.md#convex-function) gives

$$
f(x+t(y+z))\leq\tfrac12f(x+2ty)+\tfrac12f(x+2tz).
$$

Subtract $f(x)$, divide by $t$, and let $t\downarrow0$. The finite limits from part (b) give

$$
\boxed{p(y+z)\leq p(y)+p(z),\qquad p(ay)=ap(y)\quad(a\geq0).}
$$

These are exactly the defining conditions of a [sublinear functional](../../../functional-analysis.md#sublinear-function). In particular, a [directional derivative of a convex function is sublinear](../../../calculus.md#directional-derivative-of-a-convex-function-is-sublinear); it need not be linear.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The dominated real form of the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) extends the zero [linear functional](../../../linear-algebra.md#linear-functional) on $\{0\}$ to a [linear functional](../../../linear-algebra.md#linear-functional) $l:E\to\mathbb R$ with $l(y)\leq p(y)$ everywhere. If $x+z\in U$, [convexity](../../../real-analysis.md#convex-function) of the ball puts the whole segment in $U$. Its increasing secant slopes give

$$
p(z)=\lim_{t\downarrow0}\frac{f(x+tz)-f(x)}t\leq f(x+z)-f(x).
$$

Therefore

$$
\boxed{f(x+z)\geq f(x)+l(z)\qquad(x+z\in U).}
$$

This constructs a supporting [affine minorant](../../../real-analysis.md#affine-minorant) at $x$. Part (e) shows that it is a [continuous supporting functional for a locally bounded convex function](../../../real-analysis.md#continuous-supporting-functional-for-a-locally-bounded-convex-function).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The bound in part (b) and domination $l\leq p$ give $l(y)\leq L\|y\|$. Applying the same bound to $-y$, and using linearity, gives $-l(y)=l(-y)\leq L\|y\|$. Consequently

$$
\boxed{|l(y)|\leq L\|y\|,\qquad\|l\|\leq L.}
$$

A [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) is continuous, so $l$ belongs to the [continuous dual space](../../../continuous-dual-space.md) $E'$. The domination by a [sublinear functional](../../../functional-analysis.md#sublinear-function) alone was algebraic; the local [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) supplies the needed boundedness.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

By part (a), $f$ is a bounded [continuous function](../../../calculus.md#continuous-function), hence is Borel measurable and integrable for the given [probability measure](../../../probability-theory.md#probability-measure). By part (e), $l\in E'$, and its restriction to the unit ball is also bounded and integrable. For every $u\in U$, the supporting inequality says $f(u)\geq f(x)+l(u)-l(x)$. Taking [expectations](../../../probability-theory.md#expected-value) and using the [barycentre](../../../topological-vector-space.md#barycenter) hypothesis for this particular $l$ gives

$$
\mathbb E f\geq f(x)+\mathbb E l-l(x)=f(x).
$$

Thus **$\boxed{\mathbb E f\geq f(x)}$**, the [Jensen inequality](../../../real-analysis.md#jensen-s-inequality). This proof only uses the stated weak [barycentre](../../../topological-vector-space.md#barycenter) identity; a vector-valued integral for the identity map is not needed.

## 2

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [completely regular Hausdorff space](../../../topology.md#completely-regular-hausdorff-space) is a [Hausdorff space](../../../topology.md#hausdorff-space) in which each point $x$ outside a [closed set](../../../topology.md#closed-set) $F$ is separated from $F$ by a [continuous function](../../../calculus.md#continuous-function) $u:X\to[0,1]$ with $u(x)=1$ and $u|_F=0$. Put $E=C_b(X)$ and define the [evaluation character](../../../banach-algebra.md#evaluation-character) by $\delta_x(g)=g(x)$. The [weak-star topology](../../../weak-topology.md#weak-star-topology) on $E'$ is the topology of pointwise convergence on $E$: its coordinate maps $p\mapsto p(g)$ are continuous, and generate the topology. It is [Hausdorff](../../../topology.md#hausdorff-space), and the dual unit ball is compact in it by the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem).

For nonempty $X$, $\|\delta_x\|=1$ by the [supremum norm](../../../functional-analysis.md#supremum-norm) bound and the constant function $1$. All the coordinates of $x\mapsto\delta_x$ are continuous, so $\delta$ is continuous. Complete regularity separates distinct points, proving injectivity. To prove [continuity](../../../calculus.md#continuous-function) of the inverse onto its image, let $x\in O$ with $O$ open in $X$. Separating $x$ from $X\setminus O$ gives a bounded continuous $u$ with

$$
\delta_x\in\{p:p(u)>1/2\},\qquad\delta^{-1}\{p:p(u)>1/2\}\subseteq O.
$$

Such neighborhoods prove that **$\delta$ is a [homeomorphism](../../../topology.md#homeomorphism) onto $\delta(X)$**. This qualification is essential: it is not onto the whole dual, since the zero functional is not an evaluation on a nonempty space.

Define the [Stone-Čech compactification](../../../physics.md#stone-cech-compactification) to be

$$
\boxed{\beta X=\overline{\delta(X)}^{\,w^*}\subseteq B_{E'}.}
$$

The [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) makes this a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space), with $X$ identified with its dense evaluation copy. For $g\in C_b(X)$, the coordinate function $\widetilde g(p)=p(g)$ is a continuous extension. Density gives $\|\widetilde g\|_\infty=\|g\|_\infty$. Conversely any $h\in C(\beta X)$ restricts to an element $g$ of $C_b(X)$, and $h=\widetilde g$ because they agree on the [dense subset](../../../topology.md#dense-set) $X$. Restriction and coordinate extension are inverse linear isometries, hence

$$
\boxed{C(\beta X)\cong C_b(X)\quad\text{isometrically}.}
$$

They also preserve products: the corresponding [continuous functions](../../../calculus.md#continuous-function) agree on $X$ and hence everywhere.

For the universal extension property, let $f:X\to K$ be continuous and $K$ a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space). Pullback defines a bounded [linear operator](../../../vector-space.md#linear-operator) $T:C(K)\to C_b(X)$ by $Tg=g\circ f$. Its dual map $T':E'\to C(K)'$ is weak-star continuous, since $(T'p)(g)=p(Tg)$. Evaluation $\delta_K:K\to C(K)'$ is a [homeomorphism](../../../topology.md#homeomorphism) onto a compact, thus closed, subset: a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) is completely regular, by the [Urysohn lemma](../../../topology.md#urysohn-s-lemma). Now $T'\delta_x=\delta_K(f(x))$, so

$$
T'(\beta X)\subseteq\overline{\delta_K(f(X))}\subseteq\delta_K(K).
$$

Therefore $\overline f=\delta_K^{-1}\circ T'|_{\beta X}$ is the required continuous extension. Two continuous maps into the [Hausdorff space](../../../topology.md#hausdorff-space) $K$ agreeing on the [dense subset](../../../topology.md#dense-set) $X$ agree everywhere, proving uniqueness.

If $X$ is open in $\beta X$, then it is a [locally compact space](../../../topology.md#locally-compact-space): around any $x$, regularity of the [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) $\beta X$ gives an open neighborhood whose closure is compact and lies in $X$. Conversely, suppose $X$ is locally compact. Choose an open neighborhood $U$ of $x$ in $X$ with compact closure $C\subseteq X$. There is an open $O\subseteq\beta X$ with $O\cap X=U$. Density of $X$ implies $O\subseteq\overline U^{\beta X}$, while compactness of $C$ makes it closed in $\beta X$, so $\overline U^{\beta X}\subseteq C$. Thus $x\in O\subseteq X$. This proves

$$
\boxed{X\text{ is open in }\beta X\iff X\text{ is locally compact}.}
$$

The empty-space cases are immediate.

The final printed assertion, for an arbitrary subset of $\beta X$, is false. Take the infinite [discrete space](../../../topology.md#discrete-space) $X=\mathbb N$. It is not compact, so its [compactification](../../../physics.md#compactification-physics) has a point $p\in\beta\mathbb N\setminus\mathbb N$. The singleton $\{p\}$ is closed, hence equals its own closure. It is not open, since every nonempty open subset of $\beta\mathbb N$ meets the dense copy of $\mathbb N$. This is a counterexample.

The valid result holds for subsets $D\subseteq X$, and more generally for open subsets of $\beta X$. For $D\subseteq X$, its indicator is bounded continuous because $X$ is discrete. Its extension $\widetilde{\mathbf1_D}$ is still idempotent by density, so it takes only the values zero and one. The set $H=\{\widetilde{\mathbf1_D}=1\}$ is clopen and has $H\cap X=D$. Density then gives $H=\overline D^{\beta X}$. If $O$ is open in $\beta X$, the set $O\cap X$ is dense in $O$, so $\overline O=\overline{O\cap X}$ is clopen by the result just proved. Consequently **$\beta X$ is extremally disconnected**, which means the closure of every [open set](../../../topology.md#open-set) is open. This is the [discrete Stone-Čech compactifications are extremally disconnected](../../../physics.md#discrete-stone-cech-compactifications-are-extremally-disconnected) theorem, with the essential open-set qualification.

## 3

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Positivity of the [linear functional](../../../linear-algebra.md#linear-functional) gives monotonicity. For any $g\in C(K)$, the pointwise bounds $-\|g\|_\infty1\leq g\leq\|g\|_\infty1$ therefore imply

$$
|\phi(g)|\leq\phi(1)\|g\|_\infty.
$$

Thus the [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional) is bounded, hence continuous, and its [operator norm](../../../continuous-dual-space.md#operator-norm) is at most $\phi(1)$. Evaluating on the constant function $1$, which has [supremum norm](../../../functional-analysis.md#supremum-norm) one when $K$ is nonempty, gives the reverse inequality. Hence

$$
\boxed{\|\phi\|=\phi(1).}
$$

For empty $K$ the function space and functional are zero, so the same conclusion holds. This is the [norm of a positive functional on C(K)](../../../continuous-dual-space.md#norm-of-a-positive-functional-on-c-k) identity.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $c=\|\phi\|=\phi(1)\geq0$. If $c=0$, the [linear functional](../../../linear-algebra.md#linear-functional) is zero and is positive. Otherwise, for a nonzero $g\geq0$ let $h=g/\|g\|_\infty$. Then $0\leq h\leq1$ and $\|1-h\|_\infty\leq1$, so boundedness gives

$$
\phi(h)=c-\phi(1-h)\geq c-|\phi(1-h)|\geq0.
$$

Positive rescaling gives $\phi(g)\geq0$. Thus **$\phi$ is a [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional)**. This is the scalar form of the [unital contraction positivity criterion](../../../continuous-dual-space.md#unital-contraction-positivity-criterion).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

We construct the [Jordan decomposition of a bounded functional on C(K)](../../../continuous-dual-space.md#jordan-decomposition-of-a-bounded-functional-on-c-k) directly, without assuming a measure representation. For $f\geq0$, define

$$
P(f)=\sup\{\phi(g):g\in C(K),\ 0\leq g\leq f\}.
$$

This is finite, nonnegative, and positively homogeneous, since $0$ is allowed and $|\phi(g)|\leq\|\phi\|\|f\|_\infty$. If $f,h\geq0$, separately chosen approximate maximizers add to an admissible function for $P(f+h)$, giving $P(f+h)\geq P(f)+P(h)$. For the converse, any $0\leq g\leq f+h$ splits into the [continuous functions](../../../calculus.md#continuous-function)

$$
g_1=\min(g,f),\qquad g_2=g-g_1=\max(g-f,0),
$$

with $0\leq g_1\leq f$ and $0\leq g_2\leq h$. Hence $\phi(g)\leq P(f)+P(h)$ and $P$ is additive on the positive cone.

Extend it to a [linear functional](../../../linear-algebra.md#linear-functional) by $\phi^+(u-v)=P(u)-P(v)$ for $u,v\geq0$. This is well defined: two decompositions satisfy $u+v'=u'+v$, and additivity gives the same difference. Every continuous real function has such a decomposition, for example into its pointwise positive and negative parts. The extension is positive. Define $\phi^-=\phi^+-\phi$; for $f\geq0$, the choice $g=f$ shows $P(f)\geq\phi(f)$, so $\phi^-$ is also positive. Part (a) makes both [positive linear functionals](../../../continuous-dual-space.md#positive-linear-functional) continuous.

Their [operator norms](../../../continuous-dual-space.md#operator-norm) satisfy

$$
\|\phi^+\|+\|\phi^-\|=2P(1)-\phi(1)
=\sup_{0\leq g\leq1}\phi(2g-1)
=\sup_{\|h\|_\infty\leq1}\phi(h)=\|\phi\|.
$$

The last equality uses symmetry of the real unit ball. Therefore

$$
\boxed{\phi=\phi^+-\phi^-,\qquad\|\phi\|=\|\phi^+\|+\|\phi^-\|.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write $\phi(g)=a+ib$ with $a,b\in\mathbb R$, where $g$ is real valued. The normalization and the [operator norm](../../../continuous-dual-space.md#operator-norm) bound imply, for every real $t$,

$$
|1+it\phi(g)|^2\leq\|1+itg\|_\infty^2=1+t^2\|g\|_\infty^2.
$$

The left side is $(1-tb)^2+t^2a^2$, so

$$
-2tb+t^2(a^2+b^2-\|g\|_\infty^2)\leq0.
$$

Divide by $t>0$ and let $t\downarrow0$ to obtain $b\geq0$. Divide by $t<0$, reversing the inequality, and let $t\uparrow0$ to obtain $b\leq0$. Thus **$\boxed{\operatorname{Im}\phi(g)=0}$** for every real-valued $g$. The first-order term in $t$ is what forces reality; this is the complex-functional step in the [unital contraction positivity criterion](../../../continuous-dual-space.md#unital-contraction-positivity-criterion).

## 4

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The two [algebras](../../../algebra.md) have the same identity, so an inverse in $A$ is also an inverse in $B$. Therefore **$G(A)\subseteq G_B(A)$**.

For strictness, take $B=C_{\mathbb C}(\mathbb T)$, where $\mathbb T$ is the unit circle, and let $A$ be the uniform closure of the [polynomials](../../../polynomial.md) in the coordinate function $z$. This is a closed unital subalgebra of the [Banach algebra](../../../banach-algebra.md) $B$. The coordinate $z$ has inverse $\overline z$ in $B$. But $\overline z$ cannot belong to $A$: for every [polynomial](../../../polynomial.md) $p$,

$$
\frac1{2\pi}\int_0^{2\pi} e^{it}p(e^{it})\,dt=0,
$$

and the same identity holds for every element of $A$ by [uniform convergence](../../../real-analysis.md#uniform-convergence). It fails for $\overline z$, since $z\overline z=1$. Thus **$z\in G_B(A)\setminus G(A)$**. This [algebra](../../../algebra.md) is the boundary realization of the [disk algebra](../../../banach-algebra.md#disk-algebra).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Because $A$ is a closed subalgebra of a [Banach algebra](../../../banach-algebra.md), it is itself complete. If $\|a-1\|<1$, the [Neumann series](../../../banach-algebra.md#neumann-series) converges in $A$:

$$
\boxed{a^{-1}=\sum_{n=0}^{\infty}(1-a)^n.}
$$

Multiplying the partial sums by $a$ on either side gives $1-(1-a)^{N+1}$, which tends to $1$. Thus every such $a$ is invertible in $A$, and **$1$ is an interior point of $G(A)$**.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $a\in G(A)$, any $b\in A$ with $\|a^{-1}\|\|b-a\|<1$ has the factorization

$$
b=a\bigl(1+a^{-1}(b-a)\bigr).
$$

The second factor has a [Neumann series](../../../banach-algebra.md#neumann-series) inverse in $A$, so $b\in G(A)$. Hence the [group of invertible elements of a Banach algebra](../../../banach-algebra.md#group-of-invertible-elements-of-a-banach-algebra) $G(A)$ is open in $A$.

For $a\in G_B(A)$ use its inverse in $B$ instead. The same small-perturbation argument proves invertibility of $b$ in $B$ whenever $b\in A$ and $\|a^{-1}\|_B\|b-a\|_B<1$. Therefore **both $G(A)$ and $G_B(A)$ are open subsets of $A$**; in the second argument the inverse need not lie in $A$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $c=(1-ab)^{-1}\in A$. From the two inverse identities we have $cab=c-1=abc$. The candidate inverse is

$$
\boxed{(1-ba)^{-1}=1+bca.}
$$

Indeed

$$
(1-ba)(1+bca)=1+b(c-1-abc)a=1,
$$

and

$$
(1+bca)(1-ba)=1+b(c-1-cab)a=1.
$$

Both products have been checked, so this is valid in a noncommutative [Banach algebra](../../../banach-algebra.md). It is the identity underlying the [nonzero spectra of products in opposite orders](../../../banach-algebra.md#nonzero-spectra-of-products-in-opposite-orders) result.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Suppose the inverse norms did not tend to infinity. Some subsequence would satisfy $\|a_n^{-1}\|\leq C$. Since $a_n\to a$, for its large indices $\|a_n^{-1}(a-a_n)\|<1$. Then

$$
a=a_n\bigl(1+a_n^{-1}(a-a_n)\bigr)
$$

is invertible in $A$ by the [Neumann series](../../../banach-algebra.md#neumann-series), contradicting the hypothesis. Hence **$\boxed{\|a_n^{-1}\|\to\infty}$**, the [inverse norm divergence at noninvertible boundary points](../../../banach-algebra.md#inverse-norm-divergence-at-noninvertible-boundary-points) property.

If $a$ were invertible in $B$, then [continuity of inversion in a Banach algebra](../../../banach-algebra.md#continuity-of-inversion-in-a-banach-algebra) would give $a_n^{-1}\to a^{-1}$ in $B$. Explicitly, the same factorization around $a$ gives a [Neumann series](../../../banach-algebra.md#neumann-series) and the bound $\|a_n^{-1}-a^{-1}\|\leq\|a_n^{-1}\|\|a-a_n\|\|a^{-1}\|$, with the inverse norms locally bounded in $B$. Since every $a_n^{-1}$ belongs to the closed subalgebra $A$, so would $a^{-1}$. That would make $a\in G(A)$, again a contradiction. Therefore **$a\notin G_B(A)$**.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Part (c) makes $G(A)$ relatively open in $G_B(A)$. It is also relatively closed: if a sequence in $G(A)$ converges to $a\in G_B(A)$, part (e) forbids $a\notin G(A)$. Sequences detect closure here because the topology comes from a norm.

Intersecting this clopen subset with any [connected component](../../../geometry-and-topology.md#connected-component) $C$ of $G_B(A)$ gives a clopen subset of the connected space $C$. It is therefore either empty or all of $C$. Thus **$G(A)$ is the union of those [connected components](../../../geometry-and-topology.md#connected-component) of $G_B(A)$ that it meets**. This is [connected-component permanence of subalgebra invertibility](../../../banach-algebra.md#connected-component-permanence-of-subalgebra-invertibility); it does not require [connected components](../../../geometry-and-topology.md#connected-component) to be path connected.

## 5

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem) says that a nonzero complex unital [Banach algebra](../../../banach-algebra.md) in which every nonzero element is invertible is isomorphic to $\mathbb C$ by the scalar map $\lambda\mapsto\lambda1$. With the usual normalization $\|1\|=1$, that isomorphism is isometric. Commutativity need not be assumed in the theorem; it follows from the conclusion.

**Every complex Banach division [algebra](../../../algebra.md) is the scalar [field](../../../algebra.md#field).** We use complex scalars throughout this question, including for $C^1[0,1]$; the complex-[algebra character](../../../banach-algebra.md#character-of-an-algebra) and spectrum conclusions depend on that convention.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The assertion requires a proper [ideal](../../../commutative-algebra.md#ideal). If $I=A$, no proper [ideal](../../../commutative-algebra.md#ideal) can contain it, so the literal statement without that restriction is false.

Let $I$ be proper, and consider the partially ordered collection of proper [ideals](../../../commutative-algebra.md#ideal) containing $I$. It is nonempty. The union of a chain is an [ideal](../../../commutative-algebra.md#ideal), because any two of its elements belong together to some member of the chain. It is still proper: if it contained $1$, some member of the chain would contain $1$ and equal $A$. Thus every chain has an upper bound in the collection. The [Zorn lemma](../../../set-theory.md#zorn-s-lemma) gives a maximal member, and any proper [ideal](../../../commutative-algebra.md#ideal) containing it still belongs to the collection. Hence this is a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) of $A$.

Therefore **every proper [ideal](../../../commutative-algebra.md#ideal) is contained in a maximal proper [ideal](../../../commutative-algebra.md#ideal)**. This algebraic argument only needs a nonzero unital commutative [ring](../../../commutative-algebra.md#ring); the [Banach algebra](../../../banach-algebra.md) assumptions become important for closedness of [maximal ideals](../../../commutative-algebra.md#maximal-ideal) in part (c).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

A [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is a nonzero multiplicative complex [linear functional](../../../linear-algebra.md#linear-functional) $\phi:A\to\mathbb C$. Nonzeroness and multiplicativity force $\phi(1)=1$, so it is onto $\mathbb C$. Its kernel is an [ideal](../../../commutative-algebra.md#ideal), and the quotient is the [field](../../../algebra.md#field) $\mathbb C$, making the kernel maximal.

[Continuity](../../../calculus.md#continuous-function) is automatic. The element $a-\phi(a)1$ cannot be invertible, since applying $\phi$ to an inverse equation would give $0=1$. On the other hand $a-\lambda1$ is invertible whenever $|\lambda|>\|a\|$, by the [Neumann series](../../../banach-algebra.md#neumann-series). Hence $|\phi(a)|\leq\|a\|$, the [automatic continuity of characters](../../../banach-algebra.md#automatic-continuity-of-characters) bound.

Conversely let $M$ be a [maximal ideal](../../../commutative-algebra.md#maximal-ideal). Its closure is an [ideal](../../../commutative-algebra.md#ideal), because multiplication is continuous. That closure is proper: otherwise there would be $m\in M$ with $\|1-m\|<1$, making $m$ invertible by the [Neumann series](../../../banach-algebra.md#neumann-series) and forcing $M=A$. Maximality gives $\overline M=M$. The quotient $A/M$ is consequently a [Banach algebra](../../../banach-algebra.md). It is a division [algebra](../../../algebra.md): for any $a\notin M$, the larger [ideal](../../../commutative-algebra.md#ideal) $M+Aa$ equals $A$, so the class of $a$ has an inverse. By the [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem), $A/M\cong\mathbb C$, and its quotient map gives a continuous [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) with kernel $M$.

If two [algebra characters](../../../banach-algebra.md#character-of-an-algebra) have the same kernel, then $a-\phi(a)1$ lies in the second kernel, giving $\psi(a)=\phi(a)$ for every $a$. Thus

$$
\boxed{\Phi_A\longrightarrow\mathcal M_A,\qquad\phi\longmapsto\ker\phi}
$$

is a bijection. This proves that [maximal ideals of a commutative complex unital Banach algebra are character kernels](../../../banach-algebra.md#maximal-ideals-of-a-commutative-complex-unital-banach-algebra-are-character-kernels).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

For every [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) $\phi$, the element $a-\phi(a)1$ cannot be invertible, so $\phi(a)\in\sigma_A(a)$. Conversely, if $\lambda\in\sigma_A(a)$, the principal [ideal](../../../commutative-algebra.md#ideal) $A(a-\lambda1)$ is proper: otherwise $b(a-\lambda1)=1$ for some $b$, which in this commutative [algebra](../../../algebra.md) gives an inverse. Part (b) puts that [ideal](../../../commutative-algebra.md#ideal) inside a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $M$, and the corresponding [algebra character](../../../banach-algebra.md#character-of-an-algebra) from part (c) has $\phi(a)=\lambda$. Therefore

$$
\boxed{\sigma_A(a)=\{\phi(a):\phi\in\Phi_A\}=\widehat a(\Phi_A).}
$$

Here $\widehat a(\phi)=\phi(a)$ is the [Gelfand transform](../../../banach-algebra.md#gelfand-representation). The [spectrum equals character values in a commutative Banach algebra](../../../banach-algebra.md#spectrum-equals-character-values-in-a-commutative-banach-algebra) result does not require the [Gelfand transform](../../../banach-algebra.md#gelfand-representation) to be injective: the [algebra](../../../algebra.md) need not be semisimple.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Take complex-valued functions. Pointwise multiplication is associative and commutative, with identity the constant function $1$, whose norm is one. The [product rule](../../../calculus.md#product-rule) gives

$$
\|fg\|_\infty+\|(fg)'\|_\infty
\leq\|f\|_\infty\|g\|_\infty+\|f'\|_\infty\|g\|_\infty+\|f\|_\infty\|g'\|_\infty
\leq\|f\|\|g\|.
$$

To prove completeness, let $(f_n)$ be a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in this norm. The functions and their derivatives converge uniformly to [continuous functions](../../../calculus.md#continuous-function) $f,g$. Passing to the limit in $f_n(t)-f_n(0)=\int_0^tf_n'(s)\,ds$ gives $f(t)-f(0)=\int_0^tg(s)\,ds$. The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) yields $f'=g$, including the one-sided endpoint derivatives. Thus $f\in C^1[0,1]$ and $f_n\to f$ in the stated norm. Consequently **$A$ is a unital commutative [Banach algebra](../../../banach-algebra.md)**.

Let $u(t)=t$. If $\lambda\notin[0,1]$, then $(u-\lambda1)^{-1}(t)=1/(t-\lambda)$ belongs to $C^1[0,1]$. If $\lambda\in[0,1]$, the function $u-\lambda1$ vanishes somewhere and cannot have a pointwise inverse. Thus $\sigma_A(u)=[0,1]$. Every [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) satisfies $\phi(u)=t_0$ for some $t_0\in[0,1]$, by part (d), and therefore $\phi(p(u))=p(t_0)$ for every [polynomial](../../../polynomial.md) $p$.

[Polynomials](../../../polynomial.md) are dense in this stronger norm, not just the [supremum norm](../../../functional-analysis.md#supremum-norm). By the [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem), approximate the real and imaginary parts of $f'$ uniformly by [polynomials](../../../polynomial.md), combining them into $q_n\to f'$. Put $p_n(t)=f(0)+\int_0^tq_n(s)\,ds$. Then $p_n$ is a [polynomial](../../../polynomial.md) and

$$
\|p_n'-f'\|_\infty\to0,\qquad\|p_n-f\|_\infty\leq\|q_n-f'\|_\infty\to0.
$$

[Continuity](../../../calculus.md#continuous-function) of the [algebra character](../../../banach-algebra.md#character-of-an-algebra) now gives $\phi(f)=\lim p_n(t_0)=f(t_0)$. Conversely each point evaluation is a continuous [algebra character](../../../banach-algebra.md#character-of-an-algebra). Hence the [character space of C1 on a compact interval](../../../banach-algebra.md#character-space-of-c1-on-a-compact-interval) consists exactly of the evaluation functionals, and part (c) gives

$$
\boxed{\mathcal M_A=\{M_t:t\in[0,1]\},\qquad M_t=\{f\in C^1[0,1]:f(t)=0\}.}
$$

Distinct points give distinct [maximal ideals](../../../commutative-algebra.md#maximal-ideal), since the coordinate function separates them.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
