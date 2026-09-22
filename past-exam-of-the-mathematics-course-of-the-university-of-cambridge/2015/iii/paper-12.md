# Paper 12

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_12.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_12.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $Z$ be a real [random variable](../../../random-variable.md) with finite [expectation](../../../probability-theory.md#expected-value) $m$ and finite [variance](../../../variance.md) $\sigma^2$. **The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) is**

$$
\boxed{\mathbb P(|Z-m|\geq t)\leq\frac{\sigma^2}{t^2}\quad(t>0).}
$$

The proof is the pointwise comparison

$$
t^2\mathbf1_{\{|Z-m|\geq t\}}\leq(Z-m)^2.
$$

Taking [expectations](../../../probability-theory.md#expected-value) and using the definition of [variance](../../../variance.md) gives

$$
t^2\mathbb P(|Z-m|\geq t)\leq\mathbb E(Z-m)^2=\sigma^2.
$$

Division by the positive number $t^2$ proves the [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality), including the case $\sigma^2=0$. Equivalently, this is the [Markov inequality](../../../probability-inequality.md#markov-inequality) applied to the nonnegative [random variable](../../../random-variable.md) $(Z-m)^2$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Write $p=p(n)$ and let $T$ be the [triangle count in a binomial random graph](../../../graph-theory.md#triangle-count-in-a-binomial-random-graph). For every three-element [set](../../../set.md) $S$ of [vertices](../../../graph.md#vertex-graph-theory), let $I_S$ be the [indicator random variable](../../../probability-theory.md#indicator-random-variable) that its three [edges](../../../graph-theory.md#edge-of-a-graph) are present. Then

$$
T=\sum_{|S|=3}I_S,\qquad \mu=\mathbb ET=\binom n3p^3.
$$

For two distinct triples $S,R$, their [indicator random variables](../../../probability-theory.md#indicator-random-variable) are [independent random variables](../../../random-variable.md#independent-random-variables) unless they share an [edge](../../../graph-theory.md#edge-of-a-graph). Sharing just one [vertex](../../../graph.md#vertex-graph-theory) still leaves the sets of relevant [edges](../../../graph-theory.md#edge-of-a-graph) disjoint. If they share an [edge](../../../graph-theory.md#edge-of-a-graph), their union has five [edges](../../../graph-theory.md#edge-of-a-graph), and therefore

$$
\operatorname{Cov}(I_S,I_R)=p^5-p^6.
$$

There are $\binom n2\binom{n-2}2$ unordered pairs of distinct [triangles in a graph](../../../graph.md#triangle-in-a-graph) sharing an [edge](../../../graph-theory.md#edge-of-a-graph): choose that [edge](../../../graph-theory.md#edge-of-a-graph), and then choose their two additional [vertices](../../../graph.md#vertex-graph-theory). The [variance of a sum](../../../variance.md#variance-of-a-sum) consequently gives the exact formula

$$
\operatorname{Var}T=\binom n3(p^3-p^6)+2\binom n2\binom{n-2}2(p^5-p^6).
$$

For sufficiently large $n$, the hypothesis $np\to\infty$ ensures $p>0$, so $\mu>0$. Dropping negative terms and simplifying the [binomial coefficients](../../../combinatorics.md#binomial-coefficient),

$$
\frac{\operatorname{Var}T}{\mu^2}\leq\frac{1}{\binom n3p^3}+\frac{18(n-3)}{n(n-1)(n-2)p}
=O\!\left(\frac1{(np)^3}+\frac1{n^2p}\right)\longrightarrow0.
$$

Here $n^2p=n(np)\to\infty$ as well. The event $T\geq2\mu$ implies $|T-\mu|\geq\mu$. Applying the [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) from part (i) gives the requested conclusion:

$$
\boxed{\mathbb P\!\left(T\geq2p^3\binom n3\right)\leq\frac{\operatorname{Var}T}{\mu^2}\longrightarrow0.}
$$

Thus the [triangle count](../../../graph.md#triangle-count) is concentrated around its [expectation](../../../probability-theory.md#expected-value) throughout this range of the [binomial random graph](../../../graph-theory.md#binomial-random-graph).

## 2

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use [normalized Fourier analysis on a finite abelian group](../../../additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group), identifying $A$ with its [indicator function](../../../measure-theory.md#indicator-function) $a=\mathbf1_A$ on the [cyclic group](../../../group.md#cyclic-group) $\mathbb Z_n$. The conventions are

$$
\mathbb E_xh(x)=\frac1n\sum_{x\in\mathbb Z_n}h(x),\qquad
\widehat h(r)=\mathbb E_xh(x)\omega^{-rx},\qquad
(h*k)(x)=\mathbb E_yh(y)k(x-y).
$$

The last operation is [normalized convolution on a finite group](../../../additive-combinatorics.md#normalized-convolution-on-a-finite-group). With these conventions the [Fourier coefficients on a finite abelian group](../../../additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group) use a normalized average, while sums over frequencies use counting measure.

Expanding the [normalized convolution on a finite group](../../../additive-combinatorics.md#normalized-convolution-on-a-finite-group) and putting $z=x-y$ gives

$$
\widehat f(r)=\mathbb E_x\mathbb E_y a(y)a(x-y)\omega^{-rx}
=\bigl(\mathbb E_y a(y)\omega^{-ry}\bigr)\bigl(\mathbb E_z a(z)\omega^{-rz}\bigr)
=\widehat a(r)^2.
$$

For the [translation of a function](../../../function.md#translation-of-a-function) $g(x)=f(x-u)$, putting $z=x-u$ yields

$$
\widehat g(r)=\mathbb E_z f(z)\omega^{-r(z+u)}=\omega^{-ru}\widehat f(r).
$$

**The two transforms are therefore**

$$
\boxed{\widehat f(r)=\widehat A(r)^2,\qquad \widehat g(r)=\omega^{-ru}\widehat A(r)^2.}
$$

The negative sign in the translation factor follows from the negative sign in our [Fourier coefficient on a finite abelian group](../../../additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group) convention.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Since $a$ is an [indicator function](../../../measure-theory.md#indicator-function) of [density of a finite subset](../../../additive-combinatorics.md#density-of-a-finite-subset) $\alpha$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $|\widehat a(r)|\leq\mathbb E_xa(x)=\alpha$ for every frequency. Also, [character orthogonality](../../../representation-theory.md#character-orthogonality) and the [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) give

$$
\sum_r|\widehat a(r)|^2=\mathbb E_x|a(x)|^2=\alpha.
$$

For completeness, the [character orthogonality](../../../representation-theory.md#character-orthogonality) used here is

$$
\sum_{r\in\mathbb Z_n}\omega^{r(y-x)}=
\begin{cases}n,&x=y,\\0,&x\ne y,\end{cases}
$$

which follows by summing a finite [geometric series](../../../real-analysis.md#geometric-series). Expanding the squared [Fourier coefficients on a finite abelian group](../../../additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group) and using this identity proves the displayed [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) directly.

Combining the uniform bound with that identity gives the **fourth-moment bound**

$$
\boxed{\|\widehat A\|_4^4=\sum_r|\widehat a(r)|^4\leq\alpha^2\sum_r|\widehat a(r)|^2=\alpha^3.}
$$

In particular, the [Lp norm](../../../real-analysis.md#lp-norm) on the frequency side here is a sum, not a normalized average. This is the [fourth Fourier moment bound for an indicator function](../../../additive-combinatorics.md#fourth-fourier-moment-bound-for-an-indicator-function).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For the physical-space [L2 norm](../../../real-analysis.md#l2-norm) use $\|h\|_2^2=\mathbb E_x|h(x)|^2$. By part (i) and the [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group),

$$
\|f-g\|_2^2=\sum_r|1-\omega^{-ru}|^2|\widehat a(r)|^4.
$$

Split this sum into the [large spectrum](../../../additive-combinatorics.md#large-spectrum) $K$ and its complement. Because $u$ belongs to the [Bohr set](../../../additive-combinatorics.md#bohr-set) in the question, for $r\in K$,

$$
|1-\omega^{-ru}|=|1-\omega^{ru}|\leq\varepsilon.
$$

Consequently the contribution from $K$ is at most $\varepsilon^2\sum_r|\widehat a(r)|^4\leq\varepsilon^2\alpha^3$ by part (ii). Outside $K$, $|\widehat a(r)|<\theta$, and $|1-\omega^{-ru}|\leq2$. Thus that contribution is at most

$$
4\theta^2\sum_{r\notin K}|\widehat a(r)|^2\leq4\theta^2\alpha.
$$

Adding the estimates proves

$$
\boxed{\|f-g\|_2^2\leq\varepsilon^2\alpha^3+4\theta^2\alpha.}
$$

The argument also covers empty $A$ or empty $K$. As usual the radius and threshold are nonnegative; a negative radius makes the premise empty whenever $K$ is nonempty. The estimate expresses [Bohr-set almost periodicity of a convolution](../../../additive-combinatorics.md#bohr-set-almost-periodicity-of-a-convolution): a [translation of a function](../../../function.md#translation-of-a-function) by an element of the [Bohr set](../../../additive-combinatorics.md#bohr-set) barely changes the large [Fourier coefficients on a finite abelian group](../../../additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group), while the small ones have little total energy.

## 3

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An additive form of the [Plünnecke inequality](../../../additive-combinatorics.md#plunnecke-inequality) is the following. If $A,B$ are nonempty finite subsets of an [abelian group](../../../group.md#abelian-group) and $|A+B|\leq K|A|$, then there is one nonempty $X\subseteq A$ such that, simultaneously for every integer $m\geq0$,

$$
\boxed{|X+mB|\leq K^m|X|.}
$$

Here $mB$ is an [iterated sumset](../../../additive-combinatorics.md#iterated-sumset) and $0B=\{0\}$. In particular, its [Plünnecke-Ruzsa inequality](../../../additive-combinatorics.md#plunnecke-ruzsa-inequality) consequence is

$$
\boxed{|kB-\ell B|\leq K^{k+\ell}|A|\qquad(k,\ell\geq0).}
$$

We prove both statements, so that the [sumset](../../../additive-combinatorics.md#sumset) and [difference set](../../../additive-combinatorics.md#difference-set) formulations are covered.

Choose a nonempty $X\subseteq A$ minimizing the ratio $|X+B|/|X|$, and denote this minimum by $\kappa$. Such a minimizer exists because $A$ is finite, and $\kappa\leq K$. Every $Z\subseteq X$ satisfies $|Z+B|\geq\kappa|Z|$, with the empty case also valid. We first prove the [Petridis minimal-growth lemma](../../../additive-combinatorics.md#petridis-minimal-growth-lemma)

$$
|X+B+C|\leq\kappa|X+C|
$$

for every finite nonempty $C$.

List $C=\{c_1,\ldots,c_t\}$. Let $U_i=X+\{c_1,\ldots,c_i\}$ and $U_0=\varnothing$. Define

$$
X_i=\{x\in X:x+c_i\notin U_{i-1}\},\qquad Z_i=X\setminus X_i.
$$

The new points of $U_i$ are exactly $X_i+c_i$, so $|X+C|=\sum_i|X_i|$. Since $Z_i+c_i\subseteq U_{i-1}$, the [sumset](../../../additive-combinatorics.md#sumset) $Z_i+B+c_i$ is already contained in $U_{i-1}+B$. It follows that the new points introduced into $U_i+B$ are contained in

$$
\bigl((X+B)\setminus(Z_i+B)\bigr)+c_i.
$$

As $Z_i+B\subseteq X+B$, their number is at most

$$
|X+B|-|Z_i+B|\leq\kappa|X|-\kappa|Z_i|=\kappa|X_i|.
$$

Summing these increments proves the [Petridis minimal-growth lemma](../../../additive-combinatorics.md#petridis-minimal-growth-lemma). Taking $C=(m-1)B$ for $m\geq1$ and iterating now gives

$$
|X+mB|\leq\kappa|X+(m-1)B|\leq\kappa^m|X|\leq K^m|X|.
$$

This proves the [Plünnecke inequality](../../../additive-combinatorics.md#plunnecke-inequality) with the same minimizing set $X$ for every $m$.

To obtain the [difference set](../../../additive-combinatorics.md#difference-set) bound, we also prove the required [Ruzsa triangle inequality](../../../additive-combinatorics.md#ruzsa-triangle-inequality). For finite $U,V,Z$ with $Z\ne\varnothing$, choose one representation $d=u_d-v_d$ of each $d\in U-V$. The map

$$
(U-V)\times Z\longrightarrow(U-Z)\times(Z-V),\qquad
(d,z)\longmapsto(u_d-z,z-v_d)
$$

is an [injection](../../../algebra.md#injective-function): the sum of the output coordinates recovers $d$, and the first coordinate then recovers $z$ because $u_d$ was fixed. Thus

$$
|U-V|\,|Z|\leq|U-Z|\,|Z-V|.
$$

Use $U=kB$, $V=\ell B$, and $Z=-X$. The already proved [Plünnecke inequality](../../../additive-combinatorics.md#plunnecke-inequality) yields

$$
|kB-\ell B|\leq\frac{|X+kB|\,|X+\ell B|}{|X|}
\leq\kappa^{k+\ell}|X|\leq K^{k+\ell}|A|.
$$

This finishes the proof of the stated [Plünnecke-Ruzsa inequality](../../../additive-combinatorics.md#plunnecke-ruzsa-inequality). The use of an [abelian group](../../../group.md#abelian-group) is essential in commuting the translates and [sumsets](../../../additive-combinatorics.md#sumset) in the minimal-growth argument.

## 4

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

We derive the [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma) from the permitted [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma), then turn a [corner in an integer grid](../../../additive-combinatorics.md#corner-in-an-integer-grid) into a [triangle in a graph](../../../graph.md#triangle-in-a-graph).

The [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma) says that for every $\eta>0$ there are $\rho>0$ and $N_0$ such that a [graph](../../../graph.md) on $N\geq N_0$ [vertices](../../../graph.md#vertex-graph-theory) with fewer than $\rho N^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) can be made [triangle-free](../../../graph.md#triangle-free-graph) by deleting at most $\eta N^2$ [edges](../../../graph-theory.md#edge-of-a-graph). Here [triangles in a graph](../../../graph.md#triangle-in-a-graph) are unordered triples of distinct [vertices](../../../graph.md#vertex-graph-theory). We prove this consequence with the necessary quantitative dependence.

We may assume $0<\eta<1$. Put $d=\eta/4$, choose an integer $m_0\geq4/\eta$, and choose

$$
0<\varepsilon\leq\min\{\eta/8,d/4,1/4\}.
$$

Apply the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma) to obtain an exceptional class $V_0$ of size at most $\varepsilon N$ and equal-sized classes $V_1,\ldots,V_k$ of size $L$, where $m_0\leq k\leq M$, and at most $\varepsilon k^2$ pairs are not [regular pairs of vertex sets](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets). The constant $M$ depends only on these chosen parameters. Delete all [edges](../../../graph-theory.md#edge-of-a-graph) incident with $V_0$, all [edges](../../../graph-theory.md#edge-of-a-graph) within a class, all [edges](../../../graph-theory.md#edge-of-a-graph) between irregular pairs, and all [edges](../../../graph-theory.md#edge-of-a-graph) between pairs whose [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) is less than $d$. The respective costs are at most

$$
\varepsilon N^2,\qquad \frac{N^2}{2m_0},\qquad \varepsilon N^2,\qquad \frac d2N^2.
$$

Their sum is at most $\eta N^2/2$, hence certainly at most $\eta N^2$.

If a [triangle in a graph](../../../graph.md#triangle-in-a-graph) survives, it lies in three distinct classes whose three pairs are $\varepsilon$-[regular pairs of vertex sets](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) of [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) at least $d$ in the original [graph](../../../graph.md). We now check the needed [regular triangle counting lemma](../../../probabilistic-combinatorics.md#regular-triangle-counting-lemma). In the first class all but at most $2\varepsilon L$ [vertices](../../../graph.md#vertex-graph-theory) have at least $(d-\varepsilon)L$ neighbours in each of the other two classes; otherwise the definition of a [regular pair of vertex sets](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) would be violated. For each such [vertex](../../../graph.md#vertex-graph-theory) $v$, its two neighbour sets each have size at least $\varepsilon L$, so their mutual [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) is at least $d-\varepsilon$. It follows that the original three classes contain at least

$$
(1-2\varepsilon)(d-\varepsilon)^3L^3\geq\frac{d^3}{8}L^3
$$

[triangles in a graph](../../../graph.md#triangle-in-a-graph). The elementary lower bound holds because $\varepsilon\leq1/4$ and $\varepsilon\leq d/4$. Also $L=(N-|V_0|)/k\geq N/(2M)$. Thus a surviving [triangle in a graph](../../../graph.md#triangle-in-a-graph) implies at least $d^3N^3/(64M^3)$ original [triangles in a graph](../../../graph.md#triangle-in-a-graph). Set $\rho=d^3/(128M^3)$ and take $N_0$ large enough for the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma). Fewer than $\rho N^3$ original [triangles in a graph](../../../graph.md#triangle-in-a-graph) force the cleaned [graph](../../../graph.md) to be [triangle-free](../../../graph.md#triangle-free-graph), proving the [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma).

Now suppose $0<\delta\leq1$ and $A\subseteq[n]^2$. Use the [tripartite graph encoding of a grid](../../../graph.md#tripartite-graph-encoding-of-a-grid) to construct a [tripartite graph](../../../graph.md#tripartite-graph) with disjoint labelled classes

$$
X=[n],\qquad Y=[n],\qquad Z=[2n].
$$

For each $(a,b)\in A$, put in the three [edges](../../../graph-theory.md#edge-of-a-graph) joining $a\in X$, $b\in Y$, and $a+b\in Z$. These yield $|A|$ canonical [triangles in a graph](../../../graph.md#triangle-in-a-graph). They are pairwise [edge-disjoint triangles](../../../graph.md#edge-disjoint-triangles): an $XY$ [edge](../../../graph-theory.md#edge-of-a-graph) determines $(a,b)$ directly, an $XZ$ [edge](../../../graph-theory.md#edge-of-a-graph) determines $b=z-a$, and a $YZ$ [edge](../../../graph-theory.md#edge-of-a-graph) determines $a=z-b$. Any deletion making the [graph](../../../graph.md) [triangle-free](../../../graph.md#triangle-free-graph) must therefore remove at least $|A|$ [edges](../../../graph-theory.md#edge-of-a-graph).

On the other hand, an arbitrary [triangle in a graph](../../../graph.md#triangle-in-a-graph) with labels $(x,y,z)$ gives three points of $A$:

$$
(x,y),\qquad(x,z-x),\qquad(z-y,y).
$$

Writing $d=z-x-y$, these are $(x,y),(x,y+d),(x+d,y)$. If $d\ne0$, they form the required [corner in an integer grid](../../../additive-combinatorics.md#corner-in-an-integer-grid). If there is no such [corner in an integer grid](../../../additive-combinatorics.md#corner-in-an-integer-grid), every [triangle in a graph](../../../graph.md#triangle-in-a-graph) is canonical, and the total number is precisely $|A|\leq n^2$.

Apply the [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma) with $\eta=\delta/32$. The constructed [graph](../../../graph.md) has $N=4n$ [vertices](../../../graph.md#vertex-graph-theory). For sufficiently large $n$, $N\geq N_0$ and

$$
n^2<\rho(4n)^3.
$$

In the absence of a [corner in an integer grid](../../../additive-combinatorics.md#corner-in-an-integer-grid), the [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma) would destroy all [triangles in a graph](../../../graph.md#triangle-in-a-graph) by deleting at most

$$
\eta(4n)^2=\frac\delta2n^2<\delta n^2\leq|A|
$$

[edges](../../../graph-theory.md#edge-of-a-graph), contradicting the pairwise [edge-disjoint triangles](../../../graph.md#edge-disjoint-triangles). **Every sufficiently large grid therefore has the asserted [corner in an integer grid](../../../additive-combinatorics.md#corner-in-an-integer-grid) in every subset of positive fixed [density of a finite subset](../../../additive-combinatorics.md#density-of-a-finite-subset).** For $\delta>1$ there is no eligible subset, so the assertion is vacuous. This proves the [corners theorem](../../../additive-combinatorics.md#corners-theorem), including the stipulated nonzero displacement; no positivity of $d$ was required.

## 5

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Apply the [polynomial method in combinatorics](../../../combinatorics.md#polynomial-method-in-combinatorics) to the [finite-field Kakeya set](../../../vector-space.md#finite-field-kakeya-set) $A$. We will actually obtain the stronger estimate

$$
\boxed{|A|\geq\binom{p+n-1}{n}\geq\frac{p^n}{n!}.}
$$

Let $\mathcal P$ be the [vector space](../../../vector-space.md) over the [prime field](../../../algebra.md#prime-field) $\mathbb F_p$ of [multivariate polynomials](../../../polynomial.md#multivariate-polynomial) in $n$ variables of [total degree of a polynomial](../../../polynomial.md#total-degree-of-a-polynomial) at most $p-1$. By the [dimension of a bounded-total-degree polynomial space](../../../polynomial.md#dimension-of-a-bounded-total-degree-polynomial-space), its [monomial](../../../polynomial.md#monomial) basis consists of $x_1^{a_1}\cdots x_n^{a_n}$ with $a_i\geq0$ and $\sum_i a_i\leq p-1$. Adding a slack exponent gives $n+1$ nonnegative exponents summing to $p-1$; the [stars and bars](../../../combinatorics.md#stars-and-bars-combinatorics) count shows that

$$
\dim\mathcal P=\binom{p+n-1}{n}.
$$

If $|A|<\dim\mathcal P$, the evaluation [linear map](../../../vector-space.md#linear-map) $\mathcal P\to\mathbb F_p^A$ has a nonzero element in its [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map). Thus there is a nonzero [polynomial](../../../polynomial.md) $P$ of [total degree of a polynomial](../../../polynomial.md#total-degree-of-a-polynomial) $d\leq p-1$ vanishing at every point of $A$. Its degree cannot be zero, since $A$ contains a line and is nonempty. Write $P_d$ for its nonzero top [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) part.

For every nonzero $v\in\mathbb F_p^n$, the directional hypothesis supplies an [affine line in a vector space](../../../vector-space.md#affine-line-in-a-vector-space)

$$
\{a_v+tv:t\in\mathbb F_p\}\subseteq A.
$$

Directions are one-dimensional [vector subspaces](../../../vector-space.md#vector-subspace); rescaling a representative does not change this line. The univariate [polynomial](../../../polynomial.md) $P(a_v+tv)$ has degree at most $d<p$ and vanishes for all $p$ values of $t$. The [root bound for a polynomial](../../../polynomial.md#lagrange-root-bound-over-a-field) makes it the zero [polynomial](../../../polynomial.md). Its coefficient of $t^d$ is exactly $P_d(v)$, so $P_d(v)=0$ for every nonzero $v$. Because $d>0$, $P_d(0)=0$ too.

To finish, we prove the relevant [polynomial nonvanishing below the field size](../../../combinatorics.md#polynomial-nonvanishing-below-the-field-size). A [polynomial](../../../polynomial.md) over $\mathbb F_p$ of degree at most $p-1$ in each variable cannot vanish on all of $\mathbb F_p^n$ unless it is zero. Induct on $n$. The one-variable case is the [root bound for a polynomial](../../../polynomial.md#lagrange-root-bound-over-a-field). For more variables, write

$$
Q(x_1,\ldots,x_n)=\sum_{j=0}^{p-1}Q_j(x_1,\ldots,x_{n-1})x_n^j.
$$

Fixing the first $n-1$ coordinates gives a univariate [polynomial](../../../polynomial.md) with $p$ [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), so all its coefficients are zero. Hence every $Q_j$ vanishes on $\mathbb F_p^{n-1}$, and the induction hypothesis makes every $Q_j$ zero. Applying this to $P_d$, whose [total degree of a polynomial](../../../polynomial.md#total-degree-of-a-polynomial) is less than $p$, contradicts its choice as nonzero.

Therefore $|A|\geq\dim\mathcal P$. Finally,

$$
\binom{p+n-1}{n}=\frac{p(p+1)\cdots(p+n-1)}{n!}\geq\frac{p^n}{n!},
$$

which proves the requested lower bound. The crucial observation in the [finite-field Kakeya polynomial bound](../../../vector-space.md#finite-field-kakeya-polynomial-bound) is that complete lines force the highest [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) part to vanish in every direction.

## 6

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use the part-preserving [bipartite four-cycle density](../../../probabilistic-combinatorics.md#bipartite-four-cycle-density) convention

$$
t_4(G)=\frac1{n^4}\sum_{x,x'\in X}\sum_{y,y'\in Y}
G(x,y)G(x,y')G(x',y)G(x',y').
$$

Here $G(x,y)$ is the [indicator function](../../../measure-theory.md#indicator-function) of adjacency, and repeated labels are allowed. This is the [homomorphism density](../../../graph-theory.md#homomorphism-density) convention appropriate to the [four-cycle norm](../../../additive-combinatorics.md#box-norm). We derive the needed counting and [operator norm](../../../continuous-dual-space.md#operator-norm) facts directly.

Let $M=(G(x,y))$ be the $n$-by-$n$ [biadjacency matrix](../../../graph-theory.md#biadjacency-matrix), let $\mathbf1$ be the all-ones [vector](../../../vector-space.md#vector), let $J=\mathbf1\mathbf1^{\mathsf T}$, and put $H=M-\delta J$. The degree hypothesis says

$$
M\mathbf1=\delta n\mathbf1,\qquad M^{\mathsf T}\mathbf1=\delta n\mathbf1,
$$

so the centered [matrix](../../../vector-space.md#matrix) $H$ annihilates $\mathbf1$ on both sides. In particular, $HJ=JH^{\mathsf T}=0$, and

$$
MM^{\mathsf T}=\delta^2nJ+HH^{\mathsf T}.
$$

The two terms have zero products in either order. Expanding the [matrix trace](../../../linear-algebra.md#matrix-trace) directly counts four adjacency factors:

$$
\operatorname{tr}\bigl((MM^{\mathsf T})^2\bigr)
=\sum_{x,x',y,y'}M_{xy}M_{x'y}M_{x'y'}M_{xy'}=n^4t_4(G).
$$

Since $J^2=nJ$ and $\operatorname{tr}J=n$, we obtain

$$
n^4t_4(G)=\delta^4n^4+\operatorname{tr}\bigl((HH^{\mathsf T})^2\bigr).
$$

The given upper bound therefore implies

$$
\operatorname{tr}\bigl((HH^{\mathsf T})^2\bigr)\leq c^4\delta^4n^4.
$$

This computation proves the [centered four-cycle identity for a biregular graph](../../../graph-theory.md#centered-four-cycle-identity-for-a-biregular-graph), rather than assuming a [four-cycle norm](../../../additive-combinatorics.md#box-norm) identity.

The [matrix](../../../vector-space.md#matrix) $Q=HH^{\mathsf T}$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). By the [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) it has nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_j$, and

$$
\lambda_{\max}^2\leq\sum_j\lambda_j^2=\operatorname{tr}(Q^2).
$$

Moreover, for the [Euclidean norm](../../../functional-analysis.md#euclidean-norm),

$$
\|H\|_{\mathrm{op}}^2=\lambda_{\max}(HH^{\mathsf T}).
$$

Indeed $\|H^{\mathsf T}v\|_2^2=v^{\mathsf T}Qv$, whose maximum on unit [vectors](../../../vector-space.md#vector) is $\lambda_{\max}$; the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) characterization $\|H\|_{\mathrm{op}}=\sup_{\|u\|_2=\|v\|_2=1}|u^{\mathsf T}Hv|$ also shows that $H$ and $H^{\mathsf T}$ have the same [operator norm](../../../continuous-dual-space.md#operator-norm). Taking fourth roots thus gives

$$
\|H\|_{\mathrm{op}}\leq c\delta n,
$$

where the error parameter $c$ is nonnegative, as in the claimed bound.

Finally use the [indicator vectors](../../../measure-theory.md#indicator-vector) $a=\mathbf1_A$, $b=\mathbf1_B$. Their [Euclidean norms](../../../functional-analysis.md#euclidean-norm) are $\sqrt{|A|}$ and $\sqrt{|B|}$, so the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the [operator norm](../../../continuous-dual-space.md#operator-norm) estimate yield

$$
\begin{aligned}
|e(A,B)-\delta|A||B||
&=|a^{\mathsf T}Hb|\\
&\leq\|a\|_2\|H\|_{\mathrm{op}}\|b\|_2\\
&\leq c\delta n\sqrt{|A||B|}
=c\delta\sqrt{\alpha\beta}\,n^2.
\end{aligned}
$$

**This is the required discrepancy bound.** It also holds when either subset is empty or $\delta=0$. In fact, because $H$ annihilates constants, replacing $a,b$ by $a-\alpha\mathbf1,b-\beta\mathbf1$ gives the stronger bound $c\delta n^2\sqrt{\alpha(1-\alpha)\beta(1-\beta)}$. This is the [spectral discrepancy bound for a biregular graph](../../../graph-theory.md#spectral-discrepancy-bound-for-a-biregular-graph).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
