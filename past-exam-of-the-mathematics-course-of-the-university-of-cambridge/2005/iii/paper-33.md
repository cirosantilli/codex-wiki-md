# Paper 33

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper33.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper33.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use a fixed [logarithm](../../../calculus.md#logarithm) base $b>1$, and write $c=\log_b e=1/\ln b$. All [relative entropies](../../../probability-and-statistics.md#kullback-leibler-divergence) below use this same base. Adopt $0\log(0/q)=0$ and $p\log(p/0)=+\infty$ for $p>0$.

For [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality), if $q(x)=0<p(x)$ at some point, the [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) is infinite and the required conclusion is immediate. Otherwise let $S=\{x:p(x)>0\}$. The elementary inequality $\ln u\leq u-1$, with equality only at $u=1$, gives, for every $x\in S$,

$$
p(x)\log_b\frac{p(x)}{q(x)}\geq c\bigl(p(x)-q(x)\bigr).
$$

Consequently

$$
D(p\Vert q)\geq c\left(1-\sum_{x\in S}q(x)\right)\geq0.
$$

This argument applies to a countable [discrete probability distribution](../../../discrete-probability-distribution.md) too: the difference between the two sides of the pointwise inequality is nonnegative, and the negative part of the entropy summand is bounded by $cq(x)$, hence summable. Thus no subtraction of divergent series is involved. Equality forces both $\sum_Sq=1$ and equality in every pointwise inequality; hence $q(x)=p(x)$ on $S$ and $q=0=p$ off $S$. Conversely $p=q$ plainly gives zero. Therefore $\boxed{D(p\Vert q)\geq0,\quad D(p\Vert q)=0\iff p=q}$.

For the [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality), set $F=\sum_Af$, $G=\sum_Ag$, and normalize to the [probability distributions](../../../probability-theory.md#probability-distribution) $p_A=f/F$, $q_A=g/G$. When $A$ is nonempty, positivity ensures $F,G>0$, and direct expansion gives

$$
\sum_{x\in A}f(x)\log_b\frac{f(x)}{g(x)}
=F D(p_A\Vert q_A)+F\log_b\frac FG
\geq F\log_b\frac FG.
$$

Thus **normalization reduces the log-sum inequality to Gibbs inequality**. Equality holds exactly when $f/F=g/G$. The empty-set case is the zero identity under the usual zero-mass convention.

For the final bound, partition the alphabet using $A=\{x:p(x)>q(x)\}$ and put $a=p(A)$, $d=q(A)$. Since the total signed difference is zero,

$$
a-d=\sum_{x\in A}(p(x)-q(x))
=\frac12\sum_x|p(x)-q(x)|.
$$

Apply the [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality) separately to $A$ and its complement. The same normalization argument works for countable sets of finite total mass, using the countable [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) just proved. It yields the [binary partition bound for relative entropy](../../../probability-and-statistics.md#binary-partition-bound-for-relative-entropy)

$$
D(p\Vert q)\geq a\log_b\frac ad+(1-a)\log_b\frac{1-a}{1-d}.
$$

Zero block masses are interpreted by the stated conventions; a positive mass divided by zero makes the bound infinite. The given binary estimate now implies

$$
D(p\Vert q)\geq2c(a-d)^2
=\boxed{\frac{\log_b e}{2}\left(\sum_x|p(x)-q(x)|\right)^2}.
$$

This is [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality). Equivalently, for the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) $\|p-q\|_{\mathrm{TV}}=\frac12\sum_x|p(x)-q(x)|$, the bound is $D(p\Vert q)\geq2\log_b e\,\|p-q\|_{\mathrm{TV}}^2$. The factor $\log_b e$ keeps the statement valid for either bits or natural-logarithm units.

## 2

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For [discrete random variables](../../../random-variable.md#discrete-random-variable), write $p(u,v)$ for the joint [probability mass function](../../../probability-theory.md#probability-mass-function) and $p_U(u)$ for its marginal. The [conditional entropy](../../../information-theory.md#conditional-entropy) is the average of the entropies of the conditional distributions:

$$
h(V\mid U)=-\sum_{u:p_U(u)>0}\sum_vp(u,v)\log p(v\mid u),
\qquad p(v\mid u)=\frac{p(u,v)}{p_U(u)}.
$$

Conditional distributions at zero-probability values of $u$ can be chosen arbitrarily; they contribute nothing. Here $h$ denotes [Shannon entropy](../../../information-theory.md#information-entropy), with one common [logarithm](../../../calculus.md#logarithm) base and $0\log0=0$.

For $p(u,v)>0$, use $\log p(u,v)=\log p_U(u)+\log p(v\mid u)$ and sum with weight $-p(u,v)$. Summing out $v$ in the first term gives

$$
\boxed{h(U,V)=h(U)+h(V\mid U)}.
$$

For countable alphabets, the entropy contributions are nonnegative, so the equality remains valid with extended values by summing nonnegative terms. Applying this identity successively to the prefix $(X_1,\ldots,X_{i-1})$ and $X_i$ proves the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy):

$$
\boxed{h(X_1,\ldots,X_n)=\sum_{i=1}^n h(X_i\mid X_1,\ldots,X_{i-1})}.
$$

For $i=1$, the conditioning tuple is empty and the term is $h(X_1)$.

For the subset inequalities, first suppose the marginal entropies are finite, so all [joint entropies](../../../information-theory.md#joint-entropy) below are finite by the chain rule and the assumed [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy) property. Put $H=h(X_1,\ldots,X_n)$, and let $H_{-i}$ be the [joint entropy](../../../information-theory.md#joint-entropy) with coordinate $i$ omitted. Apply the two-variable chain rule in the order $(X_{[n]\setminus\{i\}},X_i)$ to get

$$
H-H_{-i}=h(X_i\mid X_{[n]\setminus\{i\}})
\leq h(X_i\mid X_1,\ldots,X_{i-1}).
$$

The inequality holds because the prefix conditioning set is contained in the set of all other coordinates. Summing over $i$ and using the chain rule gives

$$
nH-\sum_{i=1}^nH_{-i}\leq H,
\qquad\text{so}\qquad
\sum_{i=1}^nH_{-i}\geq(n-1)H.
$$

This proves [Han's entropy inequality](../../../probability-and-statistics.md#han-s-entropy-inequality). In terms of the [normalized subset entropy](../../../probability-and-statistics.md#normalized-subset-entropy), $h_n^{(n)}=H/n$ and $h_{n-1}^{(n)}=\sum_iH_{-i}/[n(n-1)]$, hence $\boxed{h_n^{(n)}\leq h_{n-1}^{(n)}}$ for $n\geq2$.

Apply the same result to each $k$-element coordinate set $S$. It gives

$$
(k-1)h(X_S)\leq\sum_{i\in S}h(X_{S\setminus\{i\}}).
$$

When this is summed over all $k$-subsets, each fixed $(k-1)$-subset $T$ occurs once for each possible added coordinate, namely $n-k+1$ times. Therefore

$$
(k-1)\sum_{|S|=k}h(X_S)
\leq(n-k+1)\sum_{|T|=k-1}h(X_T).
$$

Substitute $\sum_{|S|=k}h(X_S)=k\binom nk h_k^{(n)}$ and the analogous identity at $k-1$. The [binomial coefficient](../../../combinatorics.md#binomial-coefficient) identity $k\binom nk=(n-k+1)\binom n{k-1}$ cancels the common positive factor and gives

$$
\boxed{h_k^{(n)}\leq h_{k-1}^{(n)}\quad(2\leq k\leq n)}.
$$

This is the [monotonicity of normalized subset entropies](../../../probability-and-statistics.md#monotonicity-of-normalized-subset-entropies), obtained from the local $k$-coordinate inequality by explicit counting.

If some marginal entropy is infinite, each subset average contains at least one subset including that coordinate. The entropy of such a subset is at least that marginal entropy, by the nonnegative conditional-entropy chain rule, so every $h_k^{(n)}$ is infinite. The inequalities then hold in the extended sense. Otherwise the finite-entropy proof applies. For [independent random variables](../../../random-variable.md#independent-random-variables) the averages are all $n^{-1}\sum_i h(X_i)$; repeated copies of one variable instead give $h_k^{(n)}=h(X_1)/k$, illustrating the entropy reduction caused by redundancy.

## 3

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [binary block code](../../../coding-theory.md#binary-block-code) of length $N$ is a nonempty subset $C\subseteq\mathbb F_2^N$. Its size is $|C|$, the number of distinct [codewords](../../../coding-theory.md#codeword). The [Hamming distance](../../../coding-theory.md#hamming-distance) $d(x,y)$ counts coordinates at which two words differ. The code's [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) is $\min_{x\ne y\in C}d(x,y)$ when there are at least two words. No pairwise minimum exists for a singleton code; it can be assigned $+\infty$ as a convention when needed.

A [binary linear code](../../../coding-theory.md#binary-linear-code) is a [vector subspace](../../../vector-space.md#vector-subspace) of $\mathbb F_2^N$. If its [dimension](../../../vector-space.md#dimension-vector-space) is $k$, a [generator matrix](../../../coding-theory.md#generator-matrix) $G$ has a basis of $C$ as its $k$ rows, giving

$$
C=\{uG:u\in\mathbb F_2^k\},\qquad |C|=2^k.
$$

To match the coordinate-row convention, take a [parity-check matrix](../../../coding-theory.md#parity-check-matrix) $P$ of size $N\times(N-k)$, with independent columns, and define

$$
C=\{x\in\mathbb F_2^N:xP=0\}.
$$

The transpose $H=P^T$ is the usual [parity-check matrix](../../../coding-theory.md#parity-check-matrix) with one column per coordinate. By [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem), the displayed kernel has [dimension](../../../vector-space.md#dimension-vector-space) $k$. The two constructions agree when $GP=0$: the generator's row space lies in the parity-check kernel and has the same [dimension](../../../vector-space.md#dimension-vector-space), hence equals it. Conversely, for a given $C$, choose the columns of $P$ as a basis of its [dual code](../../../coding-theory.md#dual-code) $C^\perp$; orthogonality and the [dimension](../../../vector-space.md#dimension-vector-space) formula give exactly $C$ as the kernel.

For a nonzero [linear code](../../../coding-theory.md#linear-code), $x-y$ is a nonzero [codeword](../../../coding-theory.md#codeword) whenever $x,y$ are distinct [codewords](../../../coding-theory.md#codeword), and $d(x,y)=\operatorname{wt}(x-y)$. Conversely compare any nonzero [codeword](../../../coding-theory.md#codeword) with zero. Thus the [minimum Hamming distance of a linear code](../../../coding-theory.md#minimum-hamming-distance-of-a-linear-code) is the least nonzero [Hamming weight](../../../coding-theory.md#hamming-weight).

Write $P_i$ for the row associated with coordinate $i$. A nonzero binary vector $x$ is a [codeword](../../../coding-theory.md#codeword) exactly when

$$
xP=\sum_{i:x_i=1}P_i=0.
$$

Its nonzero coordinate positions therefore index a [linearly dependent](../../../vector-space.md#linear-dependence) set of rows. Conversely, a dependence among a set of rows has coefficients in $\mathbb F_2$, not all zero; putting these coefficients in the corresponding coordinates gives a nonzero [codeword](../../../coding-theory.md#codeword) of weight no greater than the number of rows in that set. Taking minima in both directions proves the [parity-check dependencies determine minimum distance](../../../coding-theory.md#parity-check-dependencies-determine-minimum-distance) criterion:

$$
\boxed{d(C)=\min\{|S|:(P_i)_{i\in S}\text{ is linearly dependent}\}}.
$$

Rows here are indexed by positions: equal row vectors at different positions are two distinct members of the indexed family. In the usual matrix convention, the same result refers to columns of $H=P^T$. For the zero code, neither a nonzero [codeword](../../../coding-theory.md#codeword) nor a dependent coordinate set exists, so both minima can consistently be interpreted as $+\infty$.

For the [Hamming code](../../../coding-theory.md#hamming-code), let $l\geq1$, set $N=2^l-1$, and let the rows of $P$ be all nonzero vectors of $\mathbb F_2^l$, each once. These rows include the standard basis, so $P$ has rank $l$ and the code has [dimension](../../../vector-space.md#dimension-vector-space) $N-l$ and size $2^{N-l}$. There is no dependence involving one row, because no row is zero, or two rows, because no rows are equal. For $l\geq2$, any two distinct nonzero vectors $a,b$ have a distinct nonzero sum $a+b$, which is another row. These three rows sum to zero. Thus $d(C)=3$ for $l\geq2$.

The [perfectness of a Hamming code](../../../coding-theory.md#perfectness-of-a-hamming-code) also has a direct decoding proof. Given any received word $y$, its [syndrome](../../../coding-theory.md#syndrome) is $yP\in\mathbb F_2^l$. A zero [syndrome](../../../coding-theory.md#syndrome) means $y\in C$. Otherwise it equals exactly one row $P_i$. The vector $y+e_i$ then has [syndrome](../../../coding-theory.md#syndrome) zero and is the unique [codeword](../../../coding-theory.md#codeword) obtainable by changing one coordinate. There is no other [codeword](../../../coding-theory.md#codeword) at distance at most one: its necessary correction would have to have the same [syndrome](../../../coding-theory.md#syndrome), and among zero and all single-coordinate errors the [syndromes](../../../coding-theory.md#syndrome) are precisely the distinct $2^l$ vectors of $\mathbb F_2^l$. Therefore the radius-one [Hamming balls](../../../coding-theory.md#hamming-ball) about [codewords](../../../coding-theory.md#codeword) partition $\mathbb F_2^N$.

Equivalently, each ball contains $1+N=2^l$ words; disjointness and $2^{N-l}2^l=2^N$ show that none are uncovered. Hence **every nondegenerate binary Hamming code is a perfect single-error-correcting code**. For $l=1$, the construction is the singleton code $\{0\}\subseteq\mathbb F_2$, whose one radius-one ball is also the whole ambient space. This deals with the degenerate boundary without falsely claiming its minimum distance is three.

## 4

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let the $r$ distinct [codewords](../../../coding-theory.md#codeword) be $x^{(1)},\ldots,x^{(r)}\in\mathbb F_2^N$. No [linearity](../../../vector-space.md#linearity) assumption is needed. Sum their [Hamming distances](../../../coding-theory.md#hamming-distance) over unordered distinct pairs:

$$
S=\sum_{1\leq i<j\leq r}d(x^{(i)},x^{(j)}).
$$

Each summand is at least the [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) $\delta$, so $S\geq\delta r(r-1)/2$.

For coordinate $a$, let $m_a$ be the number of [codewords](../../../coding-theory.md#codeword) whose $a$th bit is $1$. Exactly $m_a(r-m_a)$ unordered pairs differ at that coordinate. Summing coordinate contributions gives

$$
S=\sum_{a=1}^Nm_a(r-m_a)
\leq\sum_{a=1}^N\frac{r^2}{4}
=\frac{Nr^2}{4},
$$

since $m_a(r-m_a)=r^2/4-(m_a-r/2)^2$. Combining the two bounds and dividing by $r>0$ gives $2\delta(r-1)\leq Nr$, hence $r(2\delta-N)\leq2\delta$. Under $2\delta>N$, division is legitimate, proving the [Plotkin bound](../../../coding-theory.md#plotkin-bound)

$$
\boxed{r\leq\frac{2\delta}{2\delta-N}}.
$$

Because $r$ is an integer, it also satisfies the floor of the right-hand side. The binary alphabet is essential to the coordinate count; this proof applies to arbitrary [binary block codes](../../../coding-theory.md#binary-block-code), not just linear ones.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the homogeneous [weight enumerator](../../../coding-theory.md#weight-enumerator) convention

$$
W_C(s,t)=\sum_{x\in C}s^{\operatorname{wt}(x)}t^{N-\operatorname{wt}(x)}.
$$

Thus $s$ records ones, $t$ records zeros, and the ordinary [weight enumerator](../../../coding-theory.md#weight-enumerator) is $W_C(z,1)$. For a binary [linear code](../../../coding-theory.md#linear-code) $C$ of [dimension](../../../vector-space.md#dimension-vector-space) $k$ and its [dual code](../../../coding-theory.md#dual-code) $C^\perp$, the [MacWilliams identity](../../../coding-theory.md#macwilliams-identity) is

$$
\boxed{W_{C^\perp}(s,t)=\frac1{|C|}W_C(t-s,t+s)},
$$

or, equivalently, $W_C(s,t)=|C^\perp|^{-1}W_{C^\perp}(t-s,t+s)$. The second form applies the first to the dual and uses $(C^\perp)^\perp=C$.

One can verify the variable order directly from the character identity $\mathbf1_{C^\perp}(y)=|C|^{-1}\sum_{x\in C}(-1)^{x\cdot y}$. If $y$ is not orthogonal to $C$, translation by a [codeword](../../../coding-theory.md#codeword) having odd inner product pairs positive and negative terms, giving zero; otherwise all terms are one. After multiplying by $s^{\operatorname{wt}(y)}t^{N-\operatorname{wt}(y)}$ and summing over $y$, coordinate $j$ contributes $t+s$ when $x_j=0$, and $t-s$ when $x_j=1$. Their product is exactly the stated substitution.

For a [Hamming code](../../../coding-theory.md#hamming-code) with $N=2^l-1$, its dual is the [binary simplex code](../../../coding-theory.md#binary-simplex-code), generated by the $l$ rows of the usual [parity-check matrix](../../../coding-theory.md#parity-check-matrix) $H=P^T$. There are $2^l$ dual words. A nonzero message $a\in\mathbb F_2^l$ produces the evaluations $a\cdot v$ as $v$ runs over all nonzero vectors of $\mathbb F_2^l$. Exactly $2^{l-1}$ of them are one: the nonzero [linear functional](../../../linear-algebra.md#linear-functional) $v\mapsto a\cdot v$ takes each value equally often on the whole [vector space](../../../vector-space.md), and removing zero removes a zero value only. This proves the [constant weight of a binary simplex code](../../../coding-theory.md#constant-weight-of-a-binary-simplex-code).

Put $m=2^{l-1}$, so $N-m=m-1$. The dual enumerator is therefore $t^N+(2^l-1)s^m t^{m-1}$. Applying the [MacWilliams identity](../../../coding-theory.md#macwilliams-identity) gives the [Hamming code weight enumerator](../../../coding-theory.md#hamming-code-weight-enumerator)

$$
\boxed{W_C(s,t)=\frac1{2^l}\left[(s+t)^{2^l-1}+(2^l-1)(t-s)^{2^{l-1}}(t+s)^{2^{l-1}-1}\right]}.
$$

In one variable this is

$$
\boxed{W_C(z,1)=\frac{(1+z)^{2^l-1}+(2^l-1)(1-z)^{2^{l-1}}(1+z)^{2^{l-1}-1}}{2^l}}.
$$

For example, $l=3$ gives $1+7z^3+7z^4+z^7$; $l=2$ gives $1+z^3$. For $l=1$, the expression is $1$, agreeing with the singleton code. Setting $s=t=1$ in the homogeneous formula gives $2^{N-l}$, the correct number of [codewords](../../../coding-theory.md#codeword).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
