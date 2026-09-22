# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper15.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
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

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the uniform probability measure on the [Boolean hypercube](../../../combinatorics.md#boolean-hypercube). In the [Fourier-Walsh transform](../../../combinatorics.md#fourier-walsh-transform) convention $\chi_S(x)=(-1)^{\sum_{i\in S}x_i}$, write $f=\sum_S\alpha_S\chi_S$ with $\alpha_S=\mathbb E[f\chi_S]$. For the indicator $f$, [Parseval's identity](../../../fourier-analysis.md#parseval-identity) gives

$$
\alpha_\varnothing=t,\qquad\sum_S\alpha_S^2=t,\qquad\sum_{S\ne\varnothing}\alpha_S^2=t(1-t).
$$

The flip-probability [influence](../../../combinatorics.md#influence-of-a-variable) satisfies $\beta_i=4\sum_{S\ni i}\alpha_S^2$, and summing gives $\sum_{S\ne\varnothing}|S|\alpha_S^2=\frac14\sum_i\beta_i$.

For $p=1+\delta\in(1,2)$, [Beckner's inequality](../../../combinatorics.md#beckner-s-inequality) says $\|T_{\sqrt\delta}g\|_2\leq\|g\|_p$. Apply it to the [discrete derivative of a Boolean function](../../../combinatorics.md#discrete-derivative-of-a-boolean-function) in coordinate $i$, viewed on the other $n-1$ coordinates. Its nonzero magnitude is $1/2$ and occurs with probability $\beta_i$, so

$$
\sum_{S\ni i}\delta^{|S|-1}\alpha_S^2\leq\frac14\beta_i^{2/p}.
$$

Summing over $i$ gives the [hypercontractive weighted influence bound](../../../combinatorics.md#hypercontractive-weighted-influence-bound)

$$
\boxed{\sum_{S\ne\varnothing}|S|\delta^{|S|-1}\alpha_S^2\leq\frac14\sum_i\beta_i^{2/p}.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $\sum_i\beta_i\leq\sqrt{n\sum_i\beta_i^2}<\lambda$. The [total influence](../../../combinatorics.md#total-influence) identity in part (i) therefore gives $\boxed{\sum_{S\ne\varnothing}|S|\alpha_S^2<\lambda/4}$.

The [Holder inequality](../../../functional-analysis.md#holder-inequality) gives $\sum_i\beta_i^{2/p}\leq n^{1-1/p}(\sum_i\beta_i^2)^{1/p}<\lambda^{2/p}n^{1-2/p}$. Substitute this into the [hypercontractive weighted influence bound](../../../combinatorics.md#hypercontractive-weighted-influence-bound) and multiply by $\delta$ to obtain

$$
\sum_{S\ne\varnothing}|S|\delta^{|S|}\alpha_S^2<\frac\delta4\lambda^{2/p}n^{1-2/p}\leq\boxed{\frac14\lambda^{2/p}n^{1-2/p}},
$$

as required. The version with $\delta^{|S|-1}$ is slightly stronger and will also be useful below.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Put $v=t(1-t)$. The assertion is trivial when $v=0$. Otherwise suppose it fails and set $L=\log n$, $\lambda=vL$, $\gamma=3\log L/L$, $\delta=1-\gamma$, $p=2-\gamma$ and $b=L/3$, with natural logarithms. For large $n$ these parameters lie in their required ranges. The high-level [Fourier weight](../../../combinatorics.md#fourier-weight) is

$$
\sum_{|S|\geq b}\alpha_S^2\leq\frac1b\sum_S|S|\alpha_S^2<\frac\lambda{4b}=\frac34v.
$$

For $1\leq s<b$, let $M_n=\max[s\delta^{s-1}]^{-1}$. The logarithm of this expression is a convex function of real $s$, so its maximum on $[1,b]$ is at an endpoint. Also $\delta^{1-b}/b\to3$, since $-(b-1)\log(1-\gamma)=\log L+o(1)$. Hence $M_n$ is bounded. The stronger inequality in part (ii) gives

$$
\sum_{1\leq|S|<b}\alpha_S^2\leq\frac{M_n}4(vL)^{2/p}n^{1-2/p}.
$$

Divide by $v$. Because $0<v\leq1/4$ and $2/p>1$, the factor $v^{2/p-1}$ is at most one. The remaining factor is $L^{2/p}e^{-\gamma L/p}=L^{-1/2+o(1)}\to0$. Thus the low-level weight is $o(v)$ uniformly in $t$. Adding both parts contradicts $\sum_{S\ne\varnothing}\alpha_S^2=v$ for sufficiently large $n$. This proves the [squared-influence logarithmic lower bound](../../../combinatorics.md#squared-influence-logarithmic-lower-bound)

$$
\boxed{\sum_i\beta_i^2\geq\frac{t^2(1-t)^2(\log n)^2}{n}.}
$$

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [uniform cover inequality](../../../combinatorics.md#uniform-covers-theorem) states that for a positive-volume body $K\subset\mathbb R^n$ and a multiset $\mathcal A$ in which each coordinate occurs exactly $k$ times, $\boxed{|K|^k\leq\prod_{A\in\mathcal A}|K_A|}$, where $K_A$ is its coordinate projection and volumes use the corresponding dimensions.

To deduce the [box theorem](../../../combinatorics.md#box-theorem), maximize $\sum_i x_i$ subject to $\sum_{i\in A}x_i\leq\log|K_A|$ for every nonempty $A\subseteq[n]$. This [linear program](../../../mathematical-optimization.md#linear-programming) is feasible and bounded above by the full-set constraint. Its dual minimizes $\sum_A\lambda_A\log|K_A|$ over nonnegative weights with $\sum_{A\ni i}\lambda_A=1$. For rational weights, clearing denominators gives an exact uniform cover, so the [uniform cover inequality](../../../combinatorics.md#uniform-covers-theorem) bounds that dual objective below by $\log|K|$. The same holds for all feasible weights by density of rational points in the rational constraint polyhedron. [Strong duality](../../../mathematical-optimization.md#strong-duality) makes the primal optimum at least $\log|K|$, while the full-set constraint makes it at most that value. An optimal solution therefore gives $b_i=e^{x_i}>0$ with

$$
\boxed{\prod_i b_i=|K|,\qquad\prod_{i\in A}b_i\leq|K_A|\quad\text{for every }A.}
$$

The axis-aligned box with these side lengths has the required volume and projection volumes.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use the [lexicographic embedding of a sumset](../../../additive-combinatorics.md#lexicographic-embedding-of-a-sumset): choose the least tuple $(s_1,\ldots,s_n)\in\prod_iS_i$ representing each distinct sum, and let $B$ be the set of those tuples. Then $|B|=|S|$. If two projections onto $A$ had the same partial sum but different tuples, replacing the larger projected tuple by the smaller one inside its full representative would preserve that full sum and improve its lexicographic order. This is impossible. Thus the summation map is injective on the projection $B_A$, giving $|B_A|\leq|S_A|$.

Replace every integer tuple of $B$ by the closed unit cube centered there. Their interiors are disjoint, and each coordinate projection is a union of unit cubes indexed by $B_A$, so the resulting body has volume $|B|$ and projected volume $|B_A|$. Apply the [box theorem](../../../combinatorics.md#box-theorem) to obtain

$$
\boxed{|S|=\prod_i b_i,\qquad |S_A|\geq|B_A|\geq\prod_{i\in A}b_i.}
$$

The empty-set case uses $S_\varnothing=\{0\}$ and the empty product one.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Translate each two-element set by its smaller element to write $S_i=\{0,s_i\}$ with $s_i>0$. Translation does not affect any [sumset](../../../additive-combinatorics.md#sumset) cardinality. The pair-sum hypothesis forces the $s_i$ to be distinct, since equal values would give only three pair sums. Relabel so $s_1<\cdots<s_n$.

The [distinct-positive-integer subset-sum lower bound](../../../additive-combinatorics.md#distinct-positive-integer-subset-sum-lower-bound) has a short inductive proof. Suppose the first $n-1$ values have sum $P$, their largest subset sum. Adding $s_n$ creates the $n$ distinct sums $P+s_n$ and $P+s_n-s_i$ for $1\leq i<n$. They are all above $P$, since $s_n>s_i$, and hence are all new. Starting with one sum for no elements and adding $1,2,\ldots,n$ new sums gives

$$
\boxed{|S|\geq1+\frac{n(n+1)}2.}
$$

Equality is attained by $S_i=\{0,i\}$. Their subset sums fill every integer from zero to $n(n+1)/2$, by induction on $n$, and each pair of distinct positive values has four different pair sums. Thus **the bound is best possible for every $n$**.

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [Balister-Bollobas inequality](../../../information-theory.md#balister-bollobas-entropy-inequality) says that if $r_i$ is the coordinate multiplicity in a multiset $\mathcal A$, and $L_j=\{i:r_i\geq j\}$, then $\sum_jH(X_{L_j})\leq\sum_{A\in\mathcal A}H(X_A)$. More generally, each union-intersection compression decreases the entropy sum, by [entropy submodularity](../../../information-theory.md#entropy-submodularity).

For an exact $k$-cover define $A^-=[\min A-1]$ and $A^+=[\max A-1]\setminus A$. Compressing the family of $A\cup A^-$ gives the nested family of all $A^-$ together with $k$ full sets. Rearranging the resulting bound gives the upper [Madiman-Tetali inequality](../../../information-theory.md#madiman-tetali-entropy-inequality). Conversely, compressing the family of all $A^+$ together with $k$ full sets gives the nested family of $A\cup A^+$, yielding the lower bound. In conditional-entropy notation these are

$$
\boxed{\sum_{A\in\mathcal A}H(X_A\mid X_{A^+})\leq kH(X)\leq\sum_{A\in\mathcal A}H(X_A\mid X_{A^-}).}
$$

The coordinate multiplicities agree in each compression, because $\mathcal A$ is an exact $k$-cover. An equivalent proof expands the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) contributions $h_i=H(X_i\mid X_{[i-1]})$ and uses [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy). It also gives the upper inequality for arbitrary fractional covers and the lower inequality for fractional packings.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Choose an [independent set](../../../graph-theory.md#independent-set-graph-theory) uniformly and let $X_i$ indicate whether it contains vertex $i$. Then $H(X)=\log_2 i(G)$. Put $P_i=N(i)\cap[i-1]$ and $b_i=|P_i|$. Form a multiset containing every nonempty $P_i$ and $b_i$ copies of singleton $\{i\}$. Each coordinate $j$ occurs exactly $d_j$ times: in $d_j-b_j$ later-neighbor sets and in $b_j$ singleton copies.

For a set $A$ in this multiset, weight it by $1/\min_{j\in A}d_j$. These weights form a fractional cover, since each of the $d_j$ occurrences of $j$ has weight at least $1/d_j$. Apply the upper [Madiman-Tetali inequality](../../../information-theory.md#madiman-tetali-entropy-inequality). Since every $j\in P_i$ precedes $i$, one has $d_j\geq d_i$; enlarging that set's weight to $1/d_i$ and removing conditioning only enlarges its nonnegative contribution. For singleton terms retain the useful conditioning on $P_i$. Thus

$$
H(X)\leq\sum_i\frac1{d_i}\left[H(X_{P_i})+b_iH(X_i\mid X_{P_i})\right].
$$

For $b_i>0$, let $q_i=\mathbb P(X_{P_i}=0)$. Every nonzero neighbor assignment forces $X_i=0$, while the all-zero assignment allows at most two values. The [maximum entropy on a finite alphabet](../../../information-theory.md#maximum-entropy-on-a-finite-alphabet) gives

$$
H(X_{P_i})+b_iH(X_i\mid X_{P_i})\leq h_2(q_i)+(1-q_i)\log_2(2^{b_i}-1)+b_iq_i\leq\log_2(2^{b_i+1}-1).
$$

The last inequality is the binary entropy maximization formula, or the [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality), with group sizes $2^{b_i}$ and $2^{b_i}-1$. If $b_i=0$ the whole term is zero, also agreeing with the formula. Exponentiating proves the [degree-ordered independent-set entropy bound](../../../graph-theory.md#degree-ordered-independent-set-entropy-bound)

$$
\boxed{i(G)\leq\prod_i(2^{b_i+1}-1)^{1/d_i}.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Take **$G=K_{d,d}$ for any $d\geq1$**, ordering one part before the other. Every degree is $d$; the first $d$ vertices have $b_i=0$, the last $d$ have $b_i=d$. The bound is therefore $(2^{d+1}-1)^{d/d}=2^{d+1}-1$. An [independent set](../../../graph-theory.md#independent-set-graph-theory) lies entirely in one part, giving $2^d+2^d-1$ possibilities after subtracting the twice-counted empty set. Hence equality holds. Disjoint unions of such ordered components give further equality examples.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Choose $X$ uniformly among the $n$ vertices. For each covering graph use a proper binary coloring, and fill the color of an absent vertex with an independent random color having the same law as the color of a uniform vertex of that graph, as in the question's construction. Write $h_i$ for that color [information entropy](../../../information-theory.md#information-entropy), so $h_i\leq1$. The marginal distribution of $Y_i$ is precisely this color law, and the variables $Y_i$ are conditionally independent given $X$: present colors are deterministic and absent colors use independent dummy draws. Therefore

$$
H(Y_1,\ldots,Y_\ell\mid X)=\sum_i(1-|G_i|/n)h_i,\qquad H(Y_1,\ldots,Y_\ell)\leq\sum_i h_i.
$$

Any two distinct vertices are joined in some $G_i$ and have different forced colors there. They cannot both be compatible with the same observed color vector, so $H(X\mid Y_1,\ldots,Y_\ell)=0$. The [mutual information](../../../information-theory.md#mutual-information) identity now gives

$$
\log_2n\leq\frac1n\sum_i|G_i|h_i\leq\frac1n\sum_i|G_i|,
$$

and hence $\boxed{\sum_i|G_i|\geq n\log_2n}$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For each $G_i$, choose a proper coloring minimizing its color [information entropy](../../../information-theory.md#information-entropy) $h_i$, so its [coloring entropy weight](../../../graph-theory.md#coloring-entropy-weight) is $w(G_i)=|G_i|h_i$. A minimizing coloring exists: up to relabeling there are only finitely many partitions of its finite vertex set into color classes. Use independent dummy colors with the same marginal law as before. The marginal and conditional-entropy calculations in part (i) remain valid for any number of colors. Also any pair of vertices is joined in some covering graph and hence receives different forced colors there, so the full color vector still determines $X$. Thus

$$
\boxed{\sum_iw(G_i)\geq n\log_2n.}
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Use the same random variables for the edge cover of $G$. For a fixed color vector, any two compatible candidate vertices cannot be adjacent: an edge in a covering graph would force different colors at that coordinate. Thus the compatible candidates form an [independent set](../../../graph-theory.md#independent-set-graph-theory) and there are at most $\alpha$ of them. By the [maximum entropy on a finite alphabet](../../../information-theory.md#maximum-entropy-on-a-finite-alphabet), $H(X\mid Y_1,\ldots,Y_\ell)\leq\log_2\alpha$.

Consequently the [mutual information](../../../information-theory.md#mutual-information) is at least $\log_2n-\log_2\alpha$, while the marginal and conditional-entropy bounds from part (i) make it at most $n^{-1}\sum_iw(G_i)$. The [entropy weight of a graph cover](../../../graph-theory.md#entropy-weight-of-a-graph-cover) bound follows:

$$
\boxed{\sum_iw(G_i)\geq n\log_2(n/\alpha).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
