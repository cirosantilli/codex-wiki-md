# Paper 6

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper6.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper6.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

We first prove the stronger compact-square form, in which all the one-variable functions are continuous. There are five fixed pairs of [continuous functions](../../../calculus.md#continuous-function) $a_q,b_q$ on the unit interval such that every real $f\in C([0,1]^2)$ has a representation

$$
\boxed{f(x,y)=\sum_{q=1}^5G_q\big(a_q(x)+b_q(y)\big),}
$$

with continuous one-variable $G_q$. We construct the inner functions and then prove convergence of the outer functions, rather than assume the [Kolmogorov-Arnold representation theorem](../../../uniform-approximation.md#kolmogorov-arnold-representation-theorem).

**Constructing separating inner functions.** Work in the [Banach space](../../../banach-space.md) $\mathcal X=C([0,1])^{10}$ with the maximum of the ten [supremum norms](../../../functional-analysis.md#supremum-norm). For each positive integer $n$, let $U_n$ consist of tuples $(a_q,b_q)_{q=1}^5$ for which there are, for each $q$, finite families of closed intervals $I_{qi}$ and $J_{qj}$ of length less than $1/n$, satisfying two conditions. Each point of the unit interval belongs to at least four of the five unions $\bigcup_iI_{qi}$, and likewise for the $J$ families. Within each fixed $q$, the compact sets

$$
K_{qij}=a_q(I_{qi})+b_q(J_{qj})
$$

are pairwise disjoint for distinct pairs $(i,j)$. Each $K_{qij}$ is a closed interval, by [continuity](../../../calculus.md#continuous-function) and the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem). These are [grid-separated additive coordinates](../../../uniform-approximation.md#grid-separated-additive-coordinates).

The set $U_n$ is open: for a tuple and its finitely many witnessing intervals, the distinct compact image intervals have a positive minimum separation. A sufficiently small uniform change in the inner functions preserves that separation, while the interval-cover conditions do not change.

To prove density, start with any ten [continuous functions](../../../calculus.md#continuous-function) and any positive approximation tolerance. Choose a common fine partition so that each original function oscillates by less than a small fraction of the tolerance on a partition cell and its immediate neighbours; choose its mesh smaller than $1/(2n)$. Near every internal division point put five small, pairwise disjoint open gaps, one for each $q$. Use these gaps to divide the interval into closed towns for family $q$, including the two endpoints in towns. Gaps from different families are disjoint, so any point misses at most one family; every town has length less than $1/n$ if the gaps are sufficiently small. Do this for both coordinates.

Approximate $a_q$ and $b_q$ by functions which are constant on their respective towns, and interpolate linearly across the gaps. The towns lie near single partition cells, so [uniform continuity](../../../topological-analysis.md#uniform-continuity) makes these approximations as close to the original functions as desired. For each $q$, perturb the finitely many town values $\alpha_{qi},\beta_{qj}$ arbitrarily slightly so that all sums $\alpha_{qi}+\beta_{qj}$ are distinct. This is possible because each unwanted equality between distinct pairs is a proper [affine hyperplane](../../../vector-space.md#affine-hyperplane) in the [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) of values; finitely many such hyperplanes cannot fill any [open ball](../../../topology.md#open-ball). Interpolating the perturbed values still approximates the original functions, and the rectangle images are now distinct singleton sets. Thus $U_n$ is dense.

By the [Baire category theorem](../../../topological-analysis.md#baire-category-theorem), choose one tuple in $\bigcap_{n\geq1}U_n$. To recall why completeness suffices here, start inside any [open ball](../../../topology.md#open-ball) and successively choose [closed balls](../../../topological-analysis.md#closed-ball) of positive radii tending to zero, each contained in the preceding ball and in the next dense open $U_n$. Their centers form a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), and its limit belongs to every ball, hence every $U_n$. Fix this tuple once and for all: it does not depend on $f$.

**A quantitative approximation step.** Let a continuous residual $r$ have [supremum norm](../../../functional-analysis.md#supremum-norm) $M>0$. Choose $n$ large enough that the oscillation of $r$ on any rectangle of side lengths below $1/n$ is at most $M/20$. For each rectangle $I_{qi}\times J_{qj}$ choose a sample point $(x_{qi},y_{qj})$. Define a one-variable $h_q$ to have constant value $r(x_{qi},y_{qj})/3$ on $K_{qij}$. The image intervals are disjoint, so interpolate linearly in their gaps and extend constantly beyond the outermost ones. Then $h_q$ is continuous on the real line and

$$
\|h_q\|_\infty\leq M/3.
$$

At a given $(x,y)$, at most one family fails to contain $x$ in an $I$ town and at most one fails to contain $y$ in a $J$ town. Thus the point belongs to rectangles in $k$ families, where $3\leq k\leq5$. For each of these families the summand differs from $r(x,y)/3$ by at most $M/60$. Each remaining summand has absolute value at most $M/3$. Consequently

$$
\begin{aligned}
\left|r(x,y)-\sum_{q=1}^5h_q(a_q(x)+b_q(y))\right|
&\leq\left(\frac{k-3}{3}+\frac{5-k}{3}\right)M+\frac{kM}{60}\\
&\leq\frac23M+\frac1{12}M=\frac34M.
\end{aligned}
$$

This proves a strict contraction uniformly over the square, including points in gaps.

**Summing the corrections.** Set $r_0=f$ and apply that step repeatedly, subtracting the five summands at each stage. The residuals satisfy $\|r_m\|_\infty\leq(3/4)^m\|f\|_\infty$, and the corresponding corrections satisfy $\|h_{qm}\|_\infty\leq(3/4)^m\|f\|_\infty/3$. If a residual is zero, take all subsequent corrections to be zero. The series

$$
G_q=\sum_{m=0}^{\infty}h_{qm}
$$

converges uniformly on the real line to a [continuous function](../../../calculus.md#continuous-function). The residuals tend uniformly to zero, proving the boxed representation. An affine change of each coordinate treats any compact rectangle.

**Removing a restriction to a compact domain.** For a continuous real function $f$ on the whole plane, set

$$
M(t)=\max_{x^2+y^2\leq t}|f(x,y)|\quad(t\geq0).
$$

Choose a positive continuous one-variable $A$ by linear interpolation of $A(n)=(n+2)(1+M(n+1))$ at nonnegative integers. Since these values increase, for $n\leq t\leq n+1$ we have $A(t)\geq(n+2)(1+M(n+1))\geq(1+t)(1+M(t))$. Therefore

$$
b(x,y)=\frac{f(x,y)}{A(x^2+y^2)}
\quad\text{satisfies}\quad |b(x,y)|\leq\frac1{1+x^2+y^2}.
$$

Let $\sigma(x)=\tfrac12+\pi^{-1}\arctan x$. Transport $b$ to the open square by $\widetilde b(s,t)=b(\tan(\pi(s-1/2)),\tan(\pi(t-1/2)))$, and set it to zero on the square's boundary. The displayed decay estimate proves [continuity](../../../calculus.md#continuous-function) at every boundary point, including the corners. Apply the compact-square representation to $\widetilde b$ and substitute $s=\sigma(x)$, $t=\sigma(y)$ to obtain $b$ using continuous one-variable functions and [addition](../../../arithmetic.md#addition).

Finally multiply this expression by $A(x^2+y^2)$. Multiplication itself uses only [addition](../../../arithmetic.md#addition) and one-variable functions, because

$$
uv=\frac{(u+v)^2-(u-v)^2}{4}.
$$

Squaring, negation and scaling are one-variable operations, as are $A$ and $\sigma$. Thus the [whole-plane reduction for continuous superposition](../../../uniform-approximation.md#whole-plane-reduction-for-continuous-superposition) gives a finite expression of the required kind for every continuous $f$ on the plane, without a boundedness assumption. For a complex-valued $f$, apply the argument to its real and imaginary parts and combine them using [addition](../../../arithmetic.md#addition) and the one-variable map $z\mapsto iz$. **All the constituent one-variable functions can be taken continuous.**

## 2

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem) states that an arbitrary product of [compact spaces](../../../topology.md#compact-space), with the [product topology](../../../geometry-and-topology.md#product-topology), is compact; no [Hausdorff](../../../topology.md#hausdorff-space) hypothesis is necessary. We prove it using [Zorn's lemma](../../../set-theory.md#zorn-s-lemma) and the [axiom of choice](../../../set-theory.md#axiom-of-choice).

First, every proper [filter on a set](../../../set-theory.md#filter-set-theory) extends to an [ultrafilter](../../../set-theory.md#ultrafilter). Order its proper extensions by inclusion. The union of a chain is again a proper filter: any finite collection of its members occurs in one member of the chain, and the empty set occurs in none. [Zorn's lemma](../../../set-theory.md#zorn-s-lemma) gives a maximal proper filter $\mathcal U$. If $A\notin\mathcal U$, adjoining $A$ must destroy properness, so some $F\in\mathcal U$ has $F\cap A=\varnothing$, and hence $X\setminus A\in\mathcal U$. This proves the decision property of an [ultrafilter](../../../set-theory.md#ultrafilter).

Next prove the [ultrafilter characterization of compactness](../../../topology.md#ultrafilter-characterization-of-compactness). In a [compact space](../../../topology.md#compact-space) the [closed sets](../../../topology.md#closed-set) $\overline F$, for $F\in\mathcal U$, have the [finite intersection property](../../../topology.md#finite-intersection-property), so their intersection contains a point $x$. Every open neighbourhood $O$ of $x$ belongs to $\mathcal U$: otherwise its closed complement belongs to $\mathcal U$ and contains $x$, a contradiction. Thus the ultrafilter converges to $x$. Conversely, if an open cover has no finite subcover, the closed complements have the [finite intersection property](../../../topology.md#finite-intersection-property) and generate a proper filter. Extend it to an ultrafilter. A limit point lies in some member $O$ of the cover, so both $O$ and its complement would belong to the ultrafilter. This is impossible. These arguments also prove the closed-set form of [compactness](../../../topology.md#compact-space) directly by taking complements.

Now let $X=\prod_{j\in J}X_j$. If a factor is empty, the product is empty and compact. Otherwise the [axiom of choice](../../../set-theory.md#axiom-of-choice) makes $X$ nonempty. For an [ultrafilter](../../../set-theory.md#ultrafilter) $\mathcal U$ on $X$, its coordinate image

$$
\mathcal U_j=\{A\subseteq X_j:\pi_j^{-1}(A)\in\mathcal U\}
$$

is an ultrafilter. [Compactness](../../../topology.md#compact-space) of $X_j$ supplies at least one limit $x_j$; use the [axiom of choice](../../../set-theory.md#axiom-of-choice) to choose one for every $j$. A basic open neighbourhood of $x=(x_j)_j$ restricts finitely many coordinates. Each corresponding inverse image belongs to $\mathcal U$, so their finite intersection also does. Hence $\mathcal U$ converges to $x$ in the [product topology](../../../geometry-and-topology.md#product-topology). The ultrafilter criterion proves the theorem. The explicit choices and the maximal-filter argument are exactly the places where choice enters.

The [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) states that the closed [unit ball](../../../functional-analysis.md#unit-ball) of the [continuous dual space](../../../continuous-dual-space.md) $V^*$ of a real or complex [normed vector space](../../../functional-analysis.md#normed-vector-space) $V$ is compact in the [weak-star topology](../../../weak-topology.md#weak-star-topology) $\sigma(V^*,V)$. Completeness of $V$ is not required.

For each $v\in V$, let $D_v=\{z\in\mathbb K:|z|\leq\|v\|\}$, a compact scalar disk or interval. By the [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem), $P=\prod_{v\in V}D_v$ is compact. Inside $P$, impose the equations

$$
z_{u+v}=z_u+z_v,\qquad z_{\alpha v}=\alpha z_v
\quad(u,v\in V,\ \alpha\in\mathbb K).
$$

Each equation defines a closed subset, since it concerns continuous coordinate projections into a [Hausdorff](../../../topology.md#hausdorff-space) scalar [field](../../../algebra.md#field). Their intersection $K$ is therefore compact. A point in $K$ defines a [linear functional](../../../linear-algebra.md#linear-functional) $\ell(v)=z_v$, and the coordinate bounds give $|\ell(v)|\leq\|v\|$. Conversely, every $\ell\in V^*$ with $\|\ell\|\leq1$ gives such a point. Thus $K$ is exactly the image of the dual [unit ball](../../../functional-analysis.md#unit-ball) under $\ell\mapsto(\ell(v))_{v\in V}$. The induced [product topology](../../../geometry-and-topology.md#product-topology) is precisely pointwise convergence on $V$, which is the [weak-star topology](../../../weak-topology.md#weak-star-topology). This proves

$$
\boxed{\{\ell\in V^*:\|\ell\|\leq1\}\text{ is weak-star compact}.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

This proof uses neither the [axiom of choice](../../../set-theory.md#axiom-of-choice) nor a preliminary choice of points in all the given sets. For each nonempty $A_j$, form a disjoint union $X_j=A_j\sqcup\{\infty_j\}$ with a distinguished added point, and give it the [topology](../../../topology.md)

$$
\tau_j=\{\varnothing,A_j,\{\infty_j\},X_j\}.
$$

The original set $A_j$ has the indiscrete subspace topology, and is [clopen](../../../topology.md#clopen-set). Any open cover of $X_j$ either contains $X_j$, or contains both $A_j$ and $\{\infty_j\}$, so it has a subcover of at most two members. Thus $X_j$ is compact by a proof requiring no choices. No [Hausdorff](../../../topology.md#hausdorff-space) restriction is imposed in this question, and these generally non-Hausdorff spaces are allowed.

The product $X=\prod_{j\geq1}X_j$ has the explicitly given all-infinity point, so it is nonempty without choice. By the assumed countable-product [compactness](../../../topology.md#compact-space) it is compact. For each $j$ let

$$
F_j=\{x\in X:x_j\in A_j\}.
$$

The coordinate projection is continuous and $A_j$ is closed in $X_j$, so $F_j$ is closed. Any finite intersection of the $F_j$ is nonempty: pick an element of each of those finitely many nonempty sets and put $\infty_k$ in every other coordinate. Finite choice follows by induction in ordinary set theory without assuming the [axiom of choice](../../../set-theory.md#axiom-of-choice).

[Compactness](../../../topology.md#compact-space) and the [finite intersection property](../../../topology.md#finite-intersection-property) now give $\bigcap_{j\geq1}F_j\ne\varnothing$. Choose one point $x$ from this single nonempty set. The function $f(j)=x_j$ satisfies $f(j)\in A_j$ for every $j$, proving the [axiom of countable choice](../../../set-theory.md#axiom-of-countable-choice).

**The implication holds in choice-free set theory:** [countable product compactness implies countable choice](../../../set-theory.md#countable-product-compactness-implies-countable-choice). The printed lower index zero is inconsistent with the stated positive-integer index set; indexing from one merely relabels this argument and changes no conclusion.

## 3

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For $x,y\in B$, write $L_x(y)=xy$ and $R_y(x)=xy$. Separate [continuity](../../../calculus.md#continuous-function) and [linearity](../../../vector-space.md#linearity) make both maps [bounded linear operators](../../../topological-vector-space.md#continuous-linear-operator). For each fixed $y$,

$$
\sup_{\|x\|\leq1}\|L_x y\|=\sup_{\|x\|\leq1}\|R_yx\|\leq\|R_y\|<\infty.
$$

The [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) therefore gives $C<\infty$ such that $\|L_x\|\leq C$ whenever $\|x\|\leq1$. Scaling yields

$$
\|xy\|\leq C\|x\|\|y\|.
$$

For completeness, the relevant [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) follows from the [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) as follows. For a pointwise bounded family $\mathcal T$ of [bounded linear operators](../../../topological-vector-space.md#continuous-linear-operator) on a [Banach space](../../../banach-space.md), the [closed sets](../../../topology.md#closed-set) $E_m=\{y:\sup_{T\in\mathcal T}\|Ty\|\leq m\}$ cover the space. One $E_m$ contains an [open ball](../../../topology.md#open-ball) $B(y_0,r)$. Subtracting the bounds for $y_0$ and $y_0+h$, with $\|h\|<r$, gives $\sup_T\|Th\|\leq2m$. Applying this to $h=(r/2)u$, $\|u\|\leq1$, bounds every [operator norm](../../../continuous-dual-space.md#operator-norm) by $4m/r$.

Define the new [norm](../../../functional-analysis.md#norm) by

$$
\boxed{\|x\|_* =\|L_x\|.}
$$

It is a [norm](../../../functional-analysis.md#norm) because $L_xe=x$, so $L_x=0$ implies $x=0$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) and scalar homogeneity follow from those of the [operator norm](../../../continuous-dual-space.md#operator-norm). Moreover,

$$
\frac{\|x\|}{\|e\|}\leq\|L_x\|\leq C\|x\|,
$$

so it is equivalent to the original [norm](../../../functional-analysis.md#norm) and remains complete. By [associativity](../../../group.md#associative-property), $L_{xy}=L_xL_y$, and the [submultiplicativity](../../../banach-algebra.md#submultiplicativity) of the [operator norm](../../../continuous-dual-space.md#operator-norm) proves

$$
\boxed{\|xy\|_*\leq\|x\|_*\|y\|_*.}
$$

This is [renorming a separately continuous Banach algebra](../../../banach-algebra.md#renorming-a-separately-continuous-banach-algebra). It even gives $\|e\|_*=1$. If the algebra is the zero space, the conclusion is immediate separately.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

A complex [Banach algebra](../../../banach-algebra.md) is an associative complex algebra with a complete [norm](../../../functional-analysis.md#norm) satisfying [submultiplicativity](../../../banach-algebra.md#submultiplicativity), $\|ab\|\leq\|a\|\|b\|$. A [field](../../../algebra.md#field) has a nonzero identity $e$, and every nonzero element is invertible. We derive the [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem) from these facts.

If $\|z\|<1$, the series $e+z+z^2+\cdots$ converges in the complete algebra. Multiplying its partial sums by $e-z$ and passing to the limit proves the [Neumann series](../../../banach-algebra.md#neumann-series) inverse. In particular, for any $x\in B$ and $|\lambda|>\|x\|$,

$$
R(\lambda)=(\lambda e-x)^{-1}
=\frac{e}{\lambda}+\sum_{n=1}^{\infty}\frac{x^n}{\lambda^{n+1}}.
$$

This [resolvent of an element](../../../banach-algebra.md#resolvent-of-an-element) tends to zero in [norm](../../../functional-analysis.md#norm) at infinity; the estimate follows from the geometric bound on $\|x^n\|$.

We next prove that the [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) cannot be empty. Suppose every $\lambda e-x$ were invertible. At each $\lambda_0$, write

$$
\lambda e-x=(\lambda_0e-x)\big(e+(\lambda-\lambda_0)R(\lambda_0)\big).
$$

The [Neumann series](../../../banach-algebra.md#neumann-series) on a small disk about $\lambda_0$ proves that $R$ is analytic there. Consequently, for each [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) $\ell:B\to\mathbb C$, the function $\lambda\mapsto\ell(R(\lambda))$ is entire. It is bounded outside a large disk by the estimate above and bounded on that disk by [continuity](../../../calculus.md#continuous-function). The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) makes it constant; its zero limit at infinity makes the constant zero.

Continuous complex [linear functionals](../../../linear-algebra.md#linear-functional) separate points of $B$. Here is the needed consequence of the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem): for $z\ne0$, define $g(tz)=t\|z\|$ on the real span of $z$ and extend it as a bounded real [linear functional](../../../linear-algebra.md#linear-functional) of [norm](../../../functional-analysis.md#norm) one. Then $\ell(w)=g(w)-ig(iw)$ is complex linear and continuous, and $\operatorname{Re}\ell(z)=\|z\|\ne0$. The real extension theorem is proved explicitly in Question 4(i) below. Thus $\ell(R(\lambda))=0$ for every $\ell$ forces $R(\lambda)=0$, contradicting $(\lambda e-x)R(\lambda)=e\ne0$. This proves the [nonemptiness of the Banach-algebra spectrum](../../../banach-algebra.md#nonemptiness-of-the-banach-algebra-spectrum).

Choose $\lambda\in\sigma_B(x)$. Since $B$ is a [field](../../../algebra.md#field), the noninvertible element $x-\lambda e$ must be zero. Hence every $x\in B$ is a scalar multiple of $e$. The map

$$
\boxed{\Phi:\mathbb C\longrightarrow B,\qquad\Phi(\lambda)=\lambda e}
$$

is therefore a bijective unital complex-algebra homomorphism. It and its inverse are bounded, since $\|\lambda e\|=|\lambda|\|e\|$. Thus it is an isomorphism of [Banach algebras](../../../banach-algebra.md). If the usual normalization $\|e\|=1$ is included in the definition, it is an isometry; without that normalization, it is still the required continuous algebra isomorphism.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

**The first algebra exists.** Let $A=L^1(0,1)$ with truncated [convolution](../../../fourier-analysis.md#convolution)

$$
(f*g)(t)=\int_0^t f(s)g(t-s)\,ds.
$$

The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) gives

$$
\|f*g\|_1\leq\int_{s,u\geq0,\ s+u\leq1}|f(s)||g(u)|\,ds\,du
\leq\|f\|_1\|g\|_1.
$$

[Commutativity](../../../algebra.md#commutativity) follows by replacing $s$ with $t-s$; [associativity](../../../group.md#associative-property) follows from the [Fubini theorem](../../../measure-theory.md#fubini-s-theorem) applied to the simplex $s,u\geq0$, $s+u\leq t$. Together with completeness of $L^1$, this makes $A$ a commutative [Banach algebra](../../../banach-algebra.md), not necessarily unital. Adjoin an identity using [unitization](../../../banach-algebra.md#unitization-of-an-algebra):

$$
B=\mathbb C\oplus A,\quad
(\alpha,f)(\beta,g)=(\alpha\beta,\alpha g+\beta f+f*g),\quad
\|(\alpha,f)\|=|\alpha|+\|f\|_1.
$$

This [norm](../../../functional-analysis.md#norm) is complete and submultiplicative by the preceding bound, and $e=(1,0)$ is the identity. This is the [Volterra convolution algebra on a finite interval](../../../banach-algebra.md#volterra-convolution-algebra-on-a-finite-interval) with an identity adjoined.

Take $x=(0,\mathbf1)$, where $\mathbf1(t)=1$. Direct induction under [convolution](../../../fourier-analysis.md#convolution) gives

$$
x^n=(0,t^{n-1}/(n-1)!),\qquad
\|x^n\|=\frac1{n!}>0.
$$

Thus no power vanishes. For every $\lambda\ne0$ the series

$$
\frac e\lambda+\sum_{n=1}^{\infty}\frac{x^n}{\lambda^{n+1}}
$$

converges absolutely, since its [norms](../../../functional-analysis.md#norm) have factorial denominators. Multiplication by $\lambda e-x$ telescopes to $e$, so it is an inverse. On the other hand $x$ cannot be invertible: its scalar coordinate is zero, and scalar coordinates multiply, so $xy$ can never equal $e$. Hence

$$
\boxed{\sigma_B(x)=\{0\},\qquad \rho(x)=0,\qquad x^n\ne0\text{ for every }n\geq1.}
$$

This explicitly exhibits a nonnilpotent [quasinilpotent element](../../../banach-algebra.md#quasinilpotent-element) without assuming a spectral-radius formula.

**The second algebra does not exist.** Suppose it did, and choose a nonscalar $y$. Nonemptiness of its [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element), together with $\rho(y)=0$, gives $\sigma_B(y)=\{0\}$. But $y+e$ is still nonscalar: if $y+e=\alpha e$, then $y=(\alpha-1)e$. By [translation of the spectrum by a scalar](../../../banach-algebra.md#translation-of-the-spectrum-by-a-scalar),

$$
\sigma_B(y+e)=1+\sigma_B(y)=\{1\},\qquad\rho(y+e)=1.
$$

This contradicts the required zero [spectral radius](../../../analysis.md#spectral-radius) for every nonscalar element. The contradiction already uses the spectral condition alone; the nonvanishing-power condition cannot remedy it.

## 4

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $p$ be the [Minkowski functional](../../../topological-vector-space.md#minkowski-functional) of $E$:

$$
p(v)=\inf\{t>0:v\in tE\}.
$$

The contained ball makes $E$ absorbing, so $p$ is finite, nonnegative and satisfies $p(v)\leq\|v\|/\epsilon$. It is positively homogeneous. To check subadditivity, if $v\in sE$ and $w\in tE$, the defining property of a [convex set](../../../mathematical-optimization.md#convex-set) gives $(v+w)/(s+t)\in E$, whence $p(v+w)\leq s+t$; let $s,t$ decrease to the respective infima. Thus $p$ is a [sublinear functional](../../../functional-analysis.md#sublinear-function). We have $p(e)\leq1$ for every $e\in E$. Also $p(x)\geq1$: otherwise $x\in tE$ for some $0<t<1$, which would put $x$ in $E$ because $E$ is a [convex set](../../../mathematical-optimization.md#convex-set) and $0\in E$.

We prove the dominated form of the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) needed here. Suppose $g$ is linear on a subspace $M$ and $g\leq p$ there. To extend it to $M+\mathbb Rv$ with $v\notin M$, choose the value $c$ at $v$ between

$$
\sup_{m\in M}\{g(m)-p(m-v)\}
\quad\text{and}\quad
\inf_{n\in M}\{p(n+v)-g(n)\}.
$$

Every lower candidate is at most every upper candidate, because

$$
g(m)+g(n)=g(m+n)\leq p(m+n)\leq p(m-v)+p(n+v).
$$

Taking $m=n=0$ among the candidates shows the two endpoints are finite: the lower supremum is at least $-p(-v)$ and at most $p(v)$, and the upper infimum lies between them and $p(v)$. Define $\widetilde g(m+tv)=g(m)+tc$. For $t>0$, the upper inequality applied to $m/t$ gives domination by $p(m+tv)$. For $t<0$, apply the lower inequality to $m/(-t)$ and multiply by $-t$. At $t=0$ domination already holds. Hence this is a dominated one-dimensional extension.

Order all dominated extensions by inclusion of their domains. Chain unions preserve linearity and domination, so [Zorn's lemma](../../../set-theory.md#zorn-s-lemma) gives a maximal extension. The one-dimensional argument shows its domain is the whole vector space. This proves the requisite dominated [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem), rather than invoking an unproved separation form.

On the line $\mathbb Rx$, start with $g(tx)=tp(x)$. For $t\geq0$ this equals $p(tx)$; for $t<0$ it is nonpositive and therefore at most $p(tx)$. Extend it to $T\leq p$ on $V$. Then

$$
Tx=p(x)\geq1,\qquad Te\leq p(e)\leq1\quad(e\in E).
$$

Applying domination to $v$ and $-v$ also gives

$$
|Tv|\leq\frac{\|v\|}{\epsilon}.
$$

Thus $T$ is a [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional), and

$$
\boxed{Tx\geq1\geq Te\quad\text{for every }e\in E.}
$$

This proves [separation from an absorbing convex set](../../../functional-analysis.md#separation-from-an-absorbing-convex-set) with no closedness assumption on $E$. The proof also gives the norm-preserving real extension theorem used earlier: take $p(v)=C\|v\|$ when the original functional has [norm](../../../functional-analysis.md#norm) at most $C$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

If $F$ is empty, the zero [linear functional](../../../linear-algebra.md#linear-functional) satisfies the conclusion vacuously. Otherwise choose one $f_0\in F$, put $\delta=\epsilon/2$, and form the [convex set](../../../mathematical-optimization.md#convex-set)

$$
E=F+B(0,\delta)-f_0.
$$

It contains $B(0,\delta)$ because $f_0\in F$. The point $x=-f_0$ is outside $E$: membership would imply $0=f+u$ for some $f\in F$ with $\|u\|<\delta$, contradicting the assumed absence of points of $F$ in $B(0,\epsilon)$.

Apply part (i). There is a [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) $T$ with $T(-f_0)\geq1$ and $T(f+u-f_0)\leq1$ for every $f\in F$, $\|u\|<\delta$. Thus $T\ne0$ and

$$
Tf+Tu\leq1+Tf_0\leq0.
$$

For fixed $f$, take the supremum of $Tu$ over this [open ball](../../../topology.md#open-ball); it is $\delta\|T\|$. Consequently $Tf\leq-\delta\|T\|$ for every $f\in F$. The normalization

$$
\boxed{S=-\frac{T}{\delta\|T\|}}
$$

is a [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) satisfying $Sf\geq1$ for every $f\in F$. No [compactness](../../../topology.md#compact-space), closedness or attainment of the supremum on the [open ball](../../../topology.md#open-ball) is needed.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $F$ be the [convex hull](../../../mathematical-optimization.md#convex-hull) of all terms of the sequence, meaning the set of their finite [convex combinations](../../../mathematical-optimization.md#convex-combination). Suppose $B(0,\epsilon)\cap F=\varnothing$. Part (ii) then gives a [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) $S$ with $Sf\geq1$ for every $f\in F$. In particular $Sf_n\geq1$ for every $n$, contradicting $Sf_n\to0$. Therefore the ball meets $F$.

A point of that intersection is a finite combination $\sum_{k=1}^m\alpha_kf_{n_k}$ with nonnegative coefficients summing to one. Set $N=\max_k n_k$, combine repeated indices and insert zero coefficients for omitted indices. This gives

$$
\boxed{\lambda_j\geq0,\quad\sum_{j=1}^N\lambda_j=1,\qquad
\left\|\sum_{j=1}^N\lambda_j f_j\right\|<\epsilon.}
$$

Thus **zero lies in the [norm](../../../functional-analysis.md#norm) closure of the convex hull**. The same argument applies to every tail of the sequence and, by choosing errors tending to zero, also gives the usual [Mazur lemma](../../../hilbert-space.md#mazur-s-lemma). Completeness of $V$ is not required for this conclusion.

The hypothesis needed is precisely convergence to zero against every [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional), namely [weak convergence](../../../weak-topology.md#weak-convergence). The PDF says only “continuous” for the testing maps. If that is interpreted as including arbitrary nonlinear continuous maps, the constant map $T\equiv1$ makes the hypothesis impossible. The proof above establishes the substantive conclusion under the intended, weaker linear-testing hypothesis, and therefore also the implication under the literal stronger wording.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
