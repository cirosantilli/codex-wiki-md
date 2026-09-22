<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Baire category theorem](../../../../../baire-category-theorem.md) states that, in a nonempty [complete metric space](../../../../../complete-metric-space.md), a countable intersection of open dense sets is dense. Equivalently, a nonempty open set cannot be covered by countably many [nowhere dense sets](../../../../../nowhere-dense-set.md).

For the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md), let $X$ be a [Banach space](../../../../../banach-space-split.md), $Y$ a [normed vector space](../../../../../normed-vector-space.md), and $(T_\alpha)$ a family of [bounded linear operators](../../../../../continuous-linear-operator.md) for which $\sup_\alpha\|T_\alpha x\|<\infty$ for every $x\in X$. Put

$$
F_n=\{x\in X:\|T_\alpha x\|\le n\text{ for every }\alpha\}.
$$

Each $F_n$ is closed, being an intersection of inverse images of closed balls, and $X=\bigcup_nF_n$. By the [Baire category theorem](../../../../../baire-category-theorem.md), some $F_n$ has interior. Choose a closed ball $\overline B(x_0,r)\subseteq F_n$ with $r>0$. For $\|h\|\le r$, both $x_0$ and $x_0+h$ belong to $F_n$, and [linearity](../../../../../linearity.md) gives $\|T_\alpha h\|\le2n$. Scaling yields

$$
\boxed{\sup_\alpha\|T_\alpha\|\le\frac{2n}{r}<\infty.}
$$

Completeness is needed for the domain, not the codomain.

We next prove the [Silverman-Toeplitz theorem](../../../../../silverman-toeplitz-theorem.md). Write $c$ for the real [convergent sequence space](../../../../../convergent-sequence-space.md) with the [supremum norm](../../../../../supremum-norm.md). It is a [Banach space](../../../../../banach-space-split.md): the [l-infinity sequence space](../../../../../l-infinity-sequence-space.md) is complete by coordinatewise passage to limits of norm-Cauchy sequences, and $c$ is closed in it. Indeed, if $x^{(m)}\to x$ uniformly and each $x^{(m)}$ converges, approximate $x$ within $\varepsilon/3$ by one $x^{(m)}$ and make that sequence's tail oscillation smaller than $\varepsilon/3$. Then the tail of $x$ is Cauchy and therefore converges in $\mathbb R$.

Suppose $A$ is a [regular summability matrix](../../../../../regular-matrix-summability-method.md). Fix a row $i$ and consider the finite [bounded linear functionals](../../../../../continuous-linear-functional.md)

$$
S_{i,N}(x)=\sum_{j=1}^N a_{ij}x_j\qquad(x\in c).
$$

For every $x\in c$ their values converge, by the definition of regularity, and are therefore bounded. Their [operator norms](../../../../../operator-norm.md) are exactly $\sum_{j\le N}|a_{ij}|$: the upper bound is the triangle inequality, and the finite sign sequence $x_j=\operatorname{sgn}(a_{ij})$ for $j\le N$, zero afterwards, attains it. Applying the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) to this row shows $\sum_j|a_{ij}|<\infty$.

Consequently the full row functional $A_i:c\to\mathbb R$ is continuous and has norm $\sum_j|a_{ij}|$, using the same finite sign tests and then letting $N\to\infty$. Regularity makes $(A_i(x))_i$ convergent, hence bounded, for every $x\in c$. A second application of the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) gives a common row bound $M$. Testing regularity on a coordinate vector $e_j$ and on the constant-one sequence gives, respectively, convergence to zero down each column and convergence of row sums to one. Thus the necessary conditions are

$$
\sup_i\sum_j|a_{ij}|\le M<\infty,\qquad
 a_{ij}\longrightarrow0\ (j\text{ fixed}),\qquad
 s_i:=\sum_j a_{ij}\longrightarrow1.
$$

Conversely assume these conditions and let $x_j\to L$. The sequence is bounded, so every row sum defining $A_i(x)$ converges absolutely. Write

$$
A_i(x)-L=\sum_j a_{ij}(x_j-L)+L(s_i-1).
$$

Given $\varepsilon>0$, choose $N$ such that $|x_j-L|<\varepsilon/(M+1)$ for $j>N$. The tail of the first sum has modulus at most $M\varepsilon/(M+1)<\varepsilon$, uniformly in $i$. Its finite head tends to zero by columnwise convergence, and $L(s_i-1)\to0$. Since $\varepsilon$ is arbitrary, $A_i(x)\to L$. **The three conditions are necessary and sufficient for regularity.**

For the averaging matrix $B$, every absolute row sum and every row sum equals $1$. A fixed column eventually has entry $1/r\to0$. Thus $B$ is a [regular summability matrix](../../../../../regular-matrix-summability-method.md), and its transformed values are the [Cesaro means](../../../../../cesaro-mean.md). To exhibit a bounded sequence without a [Cesaro limit](../../../../../cesaro-convergence-of-a-sequence.md), put $N_0=0$, $N_m=2^{2^m}$ for $m\ge1$, and set

$$
w_j=(-1)^m\qquad(N_{m-1}<j\le N_m).
$$

At the end of the $m$th block,

$$
\left|\frac1{N_m}\sum_{j=1}^{N_m}w_j-(-1)^m\right|
\le\frac{2N_{m-1}}{N_m}\longrightarrow0.
$$

The averages at even block endpoints approach $1$, while those at odd endpoints approach $-1$. Hence **$w$ is bounded and has no $B$-limit**.

For an arbitrary [regular summability matrix](../../../../../regular-matrix-summability-method.md) $A$, use a [gliding hump argument](../../../../../gliding-hump-argument.md); this also handles negative entries. Put $N_0=0$ and $i_0=0$. Inductively choose $i_m>i_{m-1}$ so large that

$$
\sum_{j\le N_{m-1}}|a_{i_mj}|<\frac1{16},\qquad
\left|\sum_j a_{i_mj}\right|>\frac34.
$$

This is possible by the finite-column convergence and convergence of the row sums to one. Since the selected row is absolutely summable, choose $N_m>N_{m-1}$ with

$$
\sum_{j>N_m}|a_{i_mj}|<\frac1{16}.
$$

Define a single bounded sequence on the successive disjoint blocks by

$$
y_j=(-1)^m\operatorname{sgn}(a_{i_mj})\qquad(N_{m-1}<j\le N_m),
$$

using $\operatorname{sgn}(0)=0$. The row's absolute mass on its own block is greater than $3/4-1/8=5/8$, while all coordinates outside that block contribute a term of modulus less than $1/8$, irrespective of the signs subsequently assigned. Therefore

$$
(-1)^m A_{i_m}(y)>\frac12.
$$

Even and odd selected rows cannot tend to the same limit. Every row series does converge absolutely because $\|y\|_\infty\le1$. This proves **bounded divergence for every regular summability matrix**.

The row bound makes $T_A:\ell^\infty\to\ell^\infty$, $T_Ax=(A_i(x))_i$, a [bounded linear operator](../../../../../continuous-linear-operator.md) with $\|T_A\|\le M$. The [summability domain of a regular matrix](../../../../../summability-domain-of-a-regular-matrix.md) is

$$
E_A=T_A^{-1}(c).
$$

Since $c$ is closed, this is a [closed linear subspace](../../../../../closed-vector-subspace.md). It is proper by the constructed $y$. A proper [vector subspace](../../../../../vector-subspace.md) of a [normed vector space](../../../../../normed-vector-space.md) has empty interior: a ball in the subspace can be translated to a ball about zero, and scaling that ball would put every vector in the subspace. Thus

$$
\boxed{E_A\text{ is closed and nowhere dense in }\ell^\infty.}
$$

For a countable family of regular matrices, the [Baire category theorem](../../../../../baire-category-theorem.md) on the [Banach space](../../../../../banach-space-split.md) $\ell^\infty$ gives

$$
\ell^\infty\setminus\bigcup_{m\ge1}E_{A^{[m]}}\ne\varnothing.
$$

Any vector in this complement has none of the indicated matrix limits. The matrices in this clause must be regular, as in the preceding discussion; without that implicit qualification even a single zero matrix sums every bounded sequence to zero.

Finally take any [bounded sequence](../../../../../bounded-sequence.md) $x$. By the [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) it has a subsequence $x_{n_i}\to L$ with $n_i$ strictly increasing. Define the selector matrix

$$
a_{ij}=\begin{cases}1&j=n_i,\\0&j\ne n_i.\end{cases}
$$

Its absolute row sums and row sums are $1$, and each fixed column is eventually zero. The [Silverman-Toeplitz theorem](../../../../../silverman-toeplitz-theorem.md) makes it regular, while $A_i(x)=x_{n_i}\to L$. Thus **every bounded sequence is summable by some regular matrix depending on that sequence**. This is [subsequence selection as regular matrix summability](../../../../../subsequence-selection-as-regular-matrix-summability.md); it reverses the quantifier order of the impossibility result for a fixed matrix.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
