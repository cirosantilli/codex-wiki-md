<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We give the bounds for an alphabet of size $q\ge2$, including the binary case $q=2$. Let $C$ be a length-$n$ code with $M$ [codewords](../../../../../codeword.md) and [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) at least $d$, where $1\le d\le n$. Write $A_q(n,d)$ for the [maximum code size at a given distance](../../../../../maximum-code-size-at-a-given-distance.md) and

$$
V_q(n,t)=\sum_{j=0}^t\binom nj(q-1)^j
$$

for the number of words in a [Hamming ball](../../../../../hamming-ball.md) of radius $t$. The $j$th term chooses the changed coordinates and the $q-1$ alternative symbols in each.

For the [Hamming bound](../../../../../hamming-bound.md), put $t=\lfloor(d-1)/2\rfloor$. Balls of radius $t$ around distinct [codewords](../../../../../codeword.md) are disjoint: a common point would, by the [triangle inequality](../../../../../triangle-inequality.md), make their distance at most $2t<d$. Counting those balls inside the $q^n$ ambient words proves

$$
\boxed{M V_q\!\left(n,\left\lfloor\frac{d-1}{2}\right\rfloor\right)\le q^n,\qquad A_q(n,d)\le\frac{q^n}{V_q(n,\lfloor(d-1)/2\rfloor)}.}
$$

No linearity is needed. For a [linear code](../../../../../linear-code.md) of [dimension](../../../../../dimension-vector-space.md) $k$ over $\mathbb F_q$, replace $M$ by $q^k$.

For the [Gilbert–Varshamov bound](../../../../../gilbert-varshamov-bound.md), construct a code greedily, adding any word at distance at least $d$ from all previously selected words, until none remains. The process terminates because the space is finite. Its maximality implies that the radius-$(d-1)$ balls around its [codewords](../../../../../codeword.md) cover the whole space: an uncovered word could have been added. These balls may overlap, but the size of their union is at most the sum of their sizes. Hence the constructed code has $M V_q(n,d-1)\ge q^n$, proving the existence bound

$$
\boxed{A_q(n,d)\ge\frac{q^n}{V_q(n,d-1)}.}
$$

One may take the ceiling on the right because code size is integral.

For completeness, the sharper linear version is the [Varshamov bound for linear codes](../../../../../varshamov-bound-for-linear-codes.md). When $q$ is a prime power and $d\ge2$, an $[n,k,\ge d]$ [linear code](../../../../../linear-code.md) exists provided

$$
\boxed{\sum_{j=0}^{d-2}\binom{n-1}{j}(q-1)^j<q^{n-k}.}
$$

Set $r=n-k$ and choose $n$ columns of an $r\times n$ [parity-check matrix](../../../../../parity-check-matrix.md) in order. When choosing column $l$, exclude all combinations of at most $d-2$ earlier columns, including the zero combination. There are at most $\sum_{j=0}^{d-2}\binom{l-1}{j}(q-1)^j$ forbidden vectors, smaller than $q^r$ by the assumed inequality. A column can therefore be chosen. Inductively every set of at most $d-1$ chosen columns is independent: a relation involving the newest one would express it as a combination of at most $d-2$ earlier columns. The [kernel](../../../../../kernel-of-a-linear-map.md) has [dimension](../../../../../dimension-vector-space.md) at least $n-r=k$ and [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) at least $d$, since a low-weight [kernel](../../../../../kernel-of-a-linear-map.md) vector would be such a column relation. If its [dimension](../../../../../dimension-vector-space.md) is larger than $k$, take a $k$-dimensional subspace. This proves the stated linear existence claim; it does not assume the greedy nonlinear code was linear.

To derive the asymptotic bounds, define the [q-ary entropy](../../../../../entropy-function-for-a-q-ary-alphabet.md)

$$
H_q(x)=x\log_q(q-1)-x\log_qx-(1-x)\log_q(1-x),
$$

with the continuous endpoint conventions. Its derivative is $\log_q((q-1)(1-x)/x)$, so it is increasing on $[0,1-1/q]$ and has maximum one at $1-1/q$. [Stirling's formula](../../../../../stirling-formula.md) gives, uniformly for integer $0\le j\le n$,

$$
\log_q\left[\binom nj(q-1)^j\right]=nH_q(j/n)+O(\log(n+1)).
$$

The sum defining $V_q$ is between its largest summand and $(n+1)$ times that summand. For radius fractions tending to $\rho\le1-1/q$, monotonicity of $H_q$ makes the largest exponent tend to $H_q(\rho)$. Consequently the [Hamming ball volume exponent](../../../../../hamming-ball-volume-exponent.md) is

$$
\boxed{\frac1n\log_qV_q(n,t_n)\longrightarrow H_q(\rho)\quad\text{if }t_n/n\to\rho\in[0,1-1/q].}
$$

For $\rho>1-1/q$, the exponent is one: use a radius fraction just below $1-1/q$ for a lower bound and $V_q\le q^n$ for an upper bound.

Set $d_n=\max\{1,\lceil\delta n\rceil\}$ and define the [asymptotic rate-distance function](../../../../../asymptotic-rate-distance-function.md) by

$$
\alpha_q(\delta)=\limsup_{n\to\infty}\frac1n\log_qA_q(n,d_n),\qquad0\le\delta\le1.
$$

The [code rate](../../../../../code-rate.md) is $n^{-1}\log_qM$ and the [relative minimum distance](../../../../../relative-minimum-distance-of-a-code.md) is $d/n$. A limsup suffices; no unproved existence of a limit for optimal code sizes is required. The packing radii have fraction tending to $\delta/2$, so the finite [Hamming bound](../../../../../hamming-bound.md) and the volume exponent give the [asymptotic Hamming bound](../../../../../asymptotic-hamming-bound.md)

$$
\boxed{\alpha_q(\delta)\le1-H_q(\delta/2)\qquad(0\le\delta\le1).}
$$

The covering radii have fraction tending to $\delta$, giving the [asymptotic Gilbert–Varshamov bound](../../../../../asymptotic-gilbert-varshamov-bound.md)

$$
\boxed{\alpha_q(\delta)\ge1-H_q(\delta)\qquad(0\le\delta\le1-1/q).}
$$

For larger $\delta$, this covering argument gives only the trivial lower bound zero, not the expression obtained by extending the decreasing [information entropy](../../../../../information-entropy.md) function beyond its maximum.

The asymptotic lower bound is also achievable by [linear codes](../../../../../linear-code.md) over a [finite field](../../../../../finite-field.md). For $\delta>0$ and sufficiently large $n$, take redundancy $r_n=\lfloor\log_qV_q(n-1,d_n-2)\rfloor+1$, so $q^{r_n}>V_q(n-1,d_n-2)$. The linear existence condition produces [dimension](../../../../../dimension-vector-space.md) at least $n-r_n$; its rate has liminf at least $1-H_q(\delta)$. At $\delta=0$, use the whole space, of rate one. In particular, for binary codes the bounds reduce to

$$
\boxed{1-h_2(\delta)\le\alpha_2(\delta)\le1-h_2(\delta/2)\qquad(0\le\delta\le1/2),}
$$

where $h_2$ is the [binary entropy](../../../../../binary-entropy.md) function.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
