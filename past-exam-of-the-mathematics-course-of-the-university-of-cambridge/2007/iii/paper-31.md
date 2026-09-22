# Paper 31

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper31.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper31.pdf)

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
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take $m\ge2$, as required for the lower bound in this part. A binary [Huffman code](../../../information-theory.md#huffman-code) has a [full binary tree](../../../computer-science.md#full-binary-tree): every merge has two children, and all [codewords](../../../coding-theory.md#codeword) are leaves. More generally an optimal [prefix code](../../../coding-theory.md#prefix-code) for positive-probability symbols cannot have an internal vertex with only one child, since suppressing that vertex shortens its descendant [codewords](../../../coding-theory.md#codeword) and reduces the expected length.

Choose a leaf of maximum depth $s$. Its sibling must also be a leaf, since an internal sibling would have a descendant deeper than $s$. These two leaves give the [deepest sibling property of an optimal prefix code](../../../information-theory.md#deepest-sibling-property-of-an-optimal-prefix-code), and there are only $m$ leaves altogether. Therefore

$$
\boxed{2\le n_s\le m.}
$$

For the degenerate singleton alphabet, an empty [codeword](../../../coding-theory.md#codeword) suffices and $n_s=1$; the stated lower bound consequently excludes $m=1$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

If all leaves of a [full binary tree](../../../computer-science.md#full-binary-tree) have depth $s$, all binary paths of length $s$ end in leaves. Thus it has exactly $2^s$ leaves and $m=2^s$. Equivalently, equality in the [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) gives $m2^{-s}=1$.

Conversely, when $m=2^k$ a complete depth-$k$ tree is a [prefix code](../../../coding-theory.md#prefix-code) with mean length $k$. For any prefix lengths $s_i$, convexity gives

$$
2^{-L}\le\frac1m\sum_{i=1}^m2^{-s_i}\le\frac1m,\qquad L=\frac1m\sum_i s_i,
$$

so $L\ge\log_2m=k$. The complete tree is optimal. A [Huffman code](../../../information-theory.md#huffman-code) attains this optimum, and equality in the strictly convex first inequality forces all its lengths to equal $k$. Hence, for $m\ge2$,

$$
\boxed{n_s=m\quad\Longleftrightarrow\quad m\text{ is a power of two}.}
$$

This also proves that ties in the Huffman construction do not change the conclusion.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the balancing fact proved by the exchange argument in part d: every leaf of an optimal tree has depth $s-1$ or $s$. A [full binary tree](../../../computer-science.md#full-binary-tree) with this property has all $2^{s-1}$ possible vertices at level $s-1$; at least one of these is split into two deepest leaves. Thus

$$
2^{s-1}<m\le2^s.
$$

These inequalities characterize the maximum [codeword length](../../../coding-theory.md#codeword-length) exactly:

$$
\boxed{s=\lceil\log_2m\rceil.}
$$

In the suggested notation $m=a2^k$, $1\le a<2$, this is $s=k$ for $a=1$ and $s=k+1$ for $1<a<2$. The distinction at a power of two is important.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Suppose a leaf has depth $t\le s-2$. By part a there is a sibling pair of leaves at depth $s$. These leaves are disjoint from the shallow leaf and its descendants, since a leaf has no descendants. Modify the [prefix tree of a code](../../../coding-theory.md#prefix-tree-of-a-code) by splitting the shallow leaf into two leaves at depth $t+1$ and replacing the deepest sibling pair by their parent as one leaf at depth $s-1$. The number of leaves remains $m$, so assign the equiprobable source letters bijectively to the new leaves.

The sum of depths for the three affected leaves changes from $t+2s$ to $2(t+1)+(s-1)$. The change is

$$
2(t+1)+(s-1)-(t+2s)=t-s+1\le-1.
$$

All other depths are unchanged. Since probabilities are equal, this strictly decreases the [expected codeword length](../../../information-theory.md#expected-codeword-length), contradicting the optimality of the [Huffman code](../../../information-theory.md#huffman-code). This is the [balancing exchange for a uniform optimal prefix code](../../../information-theory.md#balancing-exchange-for-a-uniform-optimal-prefix-code). There is therefore no leaf of depth at most $s-2$, proving

$$
\boxed{s_i\in\{s-1,s\}\text{ for every }i,\qquad n_{s-1}+n_s=m.}
$$

The argument applies to every optimal binary prefix tree for the uniform source, independently of how Huffman ties are resolved.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

A [full binary tree](../../../computer-science.md#full-binary-tree) has Kraft sum one. For example, place mass one at the root and divide each internal vertex's mass equally between its children; a leaf at depth $l$ receives $2^{-l}$, and the total mass on leaves remains one. Using part d gives the two equations

$$
n_{s-1}+n_s=m,\qquad \frac{n_{s-1}}{2^{s-1}}+\frac{n_s}{2^s}=1.
$$

Multiplying the second equation by $2^s$ and subtracting the first gives the [uniform-source Huffman length distribution](../../../information-theory.md#uniform-source-huffman-length-distribution)

$$
\boxed{n_{s-1}=2^s-m,\qquad n_s=2m-2^s,\qquad s=\lceil\log_2m\rceil.}
$$

If $m=2^s$, the first number is zero and every [codeword](../../../coding-theory.md#codeword) has length $s$. Otherwise both levels occur. The corresponding mean length is $L=s-(2^s-m)/m$.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

For the uniform 27-symbol model, $s=\lceil\log_2 27\rceil=5$. The [uniform-source Huffman length distribution](../../../information-theory.md#uniform-source-huffman-length-distribution) gives

$$
\boxed{n_4=32-27=5,\qquad n_5=54-32=22.}
$$

Thus five symbols receive four-bit [codewords](../../../coding-theory.md#codeword) and the other 22 receive five-bit [codewords](../../../coding-theory.md#codeword). To realize these lengths, start with all 32 binary words of length five and collapse any five disjoint sibling pairs into their four-bit parents. This leaves exactly five leaves at depth four and 22 at depth five. All source letters have the same probability, so which five letters receive the shorter [codewords](../../../coding-theory.md#codeword) is arbitrary.

The [expected codeword length](../../../information-theory.md#expected-codeword-length) is

$$
\boxed{L=\frac{5\cdot4+22\cdot5}{27}=\frac{130}{27}\approx4.815\text{ bits per symbol}.}
$$

The 27 symbols may represent 26 letters and a space, but this idealization keeps them equiprobable; it is not an empirical frequency model of English.

## 2

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use base-two logarithms and put $H=H(U_1)=-\sum_i p_i\log_2p_i$, with $0\log_2 0=0$. Zero-probability letters can be omitted. The random variables $I_j=-\log_2p_{U_j}$ are [self-information](../../../information-theory.md#information-content) values, are IID, and have finite mean $H$ because the alphabet is finite. Independence gives

$$
-\log_2 P(U_1=u_1,\ldots,U_n=u_n)=\sum_{j=1}^n-\log_2p_{u_j}.
$$

For an arbitrary $\delta>0$, define the [typical set](../../../information-theory.md#typical-set)

$$
T_{n,\delta}=\left\{u^{(n)}:P(u^{(n)})>0,\ \left|-\frac1n\log_2P(u^{(n)})-H\right|\le\delta\right\}.
$$

The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) implies $P(T_{n,\delta})\to1$. Every string in this set satisfies

$$
2^{-n(H+\delta)}\le P(u^{(n)})\le2^{-n(H-\delta)}.
$$

This is the [asymptotic equipartition property](../../../information-theory.md#asymptotic-equipartition-property) for the given finite IID source, here obtained directly from the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers).

For the upper bound, summing the lower bound on typical-string probabilities yields $|T_{n,\delta}|\le2^{n(H+\delta)}$. For sufficiently large $n$, its probability is at least $1-\varepsilon$, so it is an admissible set in the definition of $M(n,\varepsilon)$. Hence

$$
\limsup_{n\to\infty}\frac1n\log_2M(n,\varepsilon)\le H+\delta.
$$

For the lower bound, let $A$ be any admissible set and write $\eta_n=P(T_{n,\delta}^c)\to0$. Then

$$
P(A\cap T_{n,\delta})\ge1-\varepsilon-\eta_n.
$$

Each member of this intersection has probability at most $2^{-n(H-\delta)}$. Therefore, for all sufficiently large $n$,

$$
|A|\ge(1-\varepsilon-\eta_n)2^{n(H-\delta)}\ge\frac{1-\varepsilon}{2}\,2^{n(H-\delta)}.
$$

This applies in particular to a minimum-size admissible set, giving a liminf at least $H-\delta$. Letting $\delta\downarrow0$ proves both existence and the value of the [minimal high-probability source-set exponent](../../../information-theory.md#minimal-high-probability-source-set-exponent):

$$
\boxed{\lim_{n\to\infty}\frac1n\log_2M(n,\varepsilon)=H(U_1)\qquad(0<\varepsilon<1).}
$$

For a deterministic source, $H=0$ and $M(n,\varepsilon)=1$, consistent with the formula.

For coding, label the strings in an admissible set with distinct binary indices of length $\lceil\log_2M(n,\varepsilon)\rceil$. A decoder reconstructs those strings exactly and may fail outside the set. Thus asymptotically $H$ bits per source symbol describe any fixed fraction $1-\varepsilon$ of the probability mass. More strongly, every rate $R>H$ permits block codes with error tending to zero: choose $\delta<R-H$, encode the typical strings individually and reserve one index for all other strings. The required number of indices is at most $2^{n(H+\delta)}+1\le2^{nR}$ for large $n$.

Conversely, a block encoder with at most $2^{nR}$ outputs can reconstruct at most that many distinct input strings correctly. If $R<H$, choose $0<\delta<H-R$. Its success probability is at most

$$
\eta_n+2^{nR}2^{-n(H-\delta)}\longrightarrow0.
$$

This gives the [strong converse for fixed-rate source coding](../../../information-theory.md#strong-converse-for-fixed-rate-source-coding). It is the operational significance of the [information entropy](../../../information-theory.md#information-entropy) limit for [reliable source encoding at a rate](../../../information-theory.md#reliable-source-encoding-at-a-rate). The allowance of a small reconstruction error matters: a fixed-length code that must encode every possible string without error generally needs the larger rate $\log_2|\{i:p_i>0\}|$.

## 3

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We give the bounds for an alphabet of size $q\ge2$, including the binary case $q=2$. Let $C$ be a length-$n$ code with $M$ [codewords](../../../coding-theory.md#codeword) and [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) at least $d$, where $1\le d\le n$. Write $A_q(n,d)$ for the [maximum code size at a given distance](../../../coding-theory.md#maximum-code-size-at-a-given-distance) and

$$
V_q(n,t)=\sum_{j=0}^t\binom nj(q-1)^j
$$

for the number of words in a [Hamming ball](../../../coding-theory.md#hamming-ball) of radius $t$. The $j$th term chooses the changed coordinates and the $q-1$ alternative symbols in each.

For the [Hamming bound](../../../coding-theory.md#hamming-bound), put $t=\lfloor(d-1)/2\rfloor$. Balls of radius $t$ around distinct [codewords](../../../coding-theory.md#codeword) are disjoint: a common point would, by the [triangle inequality](../../../topological-analysis.md#triangle-inequality), make their distance at most $2t<d$. Counting those balls inside the $q^n$ ambient words proves

$$
\boxed{M V_q\!\left(n,\left\lfloor\frac{d-1}{2}\right\rfloor\right)\le q^n,\qquad A_q(n,d)\le\frac{q^n}{V_q(n,\lfloor(d-1)/2\rfloor)}.}
$$

No linearity is needed. For a [linear code](../../../coding-theory.md#linear-code) of [dimension](../../../vector-space.md#dimension-vector-space) $k$ over $\mathbb F_q$, replace $M$ by $q^k$.

For the [Gilbert–Varshamov bound](../../../coding-theory.md#gilbert-varshamov-bound), construct a code greedily, adding any word at distance at least $d$ from all previously selected words, until none remains. The process terminates because the space is finite. Its maximality implies that the radius-$(d-1)$ balls around its [codewords](../../../coding-theory.md#codeword) cover the whole space: an uncovered word could have been added. These balls may overlap, but the size of their union is at most the sum of their sizes. Hence the constructed code has $M V_q(n,d-1)\ge q^n$, proving the existence bound

$$
\boxed{A_q(n,d)\ge\frac{q^n}{V_q(n,d-1)}.}
$$

One may take the ceiling on the right because code size is integral.

For completeness, the sharper linear version is the [Varshamov bound for linear codes](../../../coding-theory.md#varshamov-bound-for-linear-codes). When $q$ is a prime power and $d\ge2$, an $[n,k,\ge d]$ [linear code](../../../coding-theory.md#linear-code) exists provided

$$
\boxed{\sum_{j=0}^{d-2}\binom{n-1}{j}(q-1)^j<q^{n-k}.}
$$

Set $r=n-k$ and choose $n$ columns of an $r\times n$ [parity-check matrix](../../../coding-theory.md#parity-check-matrix) in order. When choosing column $l$, exclude all combinations of at most $d-2$ earlier columns, including the zero combination. There are at most $\sum_{j=0}^{d-2}\binom{l-1}{j}(q-1)^j$ forbidden vectors, smaller than $q^r$ by the assumed inequality. A column can therefore be chosen. Inductively every set of at most $d-1$ chosen columns is independent: a relation involving the newest one would express it as a combination of at most $d-2$ earlier columns. The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) has [dimension](../../../vector-space.md#dimension-vector-space) at least $n-r=k$ and [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) at least $d$, since a low-weight [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) vector would be such a column relation. If its [dimension](../../../vector-space.md#dimension-vector-space) is larger than $k$, take a $k$-dimensional subspace. This proves the stated linear existence claim; it does not assume the greedy nonlinear code was linear.

To derive the asymptotic bounds, define the [q-ary entropy](../../../information-theory.md#entropy-function-for-a-q-ary-alphabet)

$$
H_q(x)=x\log_q(q-1)-x\log_qx-(1-x)\log_q(1-x),
$$

with the continuous endpoint conventions. Its derivative is $\log_q((q-1)(1-x)/x)$, so it is increasing on $[0,1-1/q]$ and has maximum one at $1-1/q$. [Stirling's formula](../../../real-analysis.md#stirling-formula) gives, uniformly for integer $0\le j\le n$,

$$
\log_q\left[\binom nj(q-1)^j\right]=nH_q(j/n)+O(\log(n+1)).
$$

The sum defining $V_q$ is between its largest summand and $(n+1)$ times that summand. For radius fractions tending to $\rho\le1-1/q$, monotonicity of $H_q$ makes the largest exponent tend to $H_q(\rho)$. Consequently the [Hamming ball volume exponent](../../../coding-theory.md#hamming-ball-volume-exponent) is

$$
\boxed{\frac1n\log_qV_q(n,t_n)\longrightarrow H_q(\rho)\quad\text{if }t_n/n\to\rho\in[0,1-1/q].}
$$

For $\rho>1-1/q$, the exponent is one: use a radius fraction just below $1-1/q$ for a lower bound and $V_q\le q^n$ for an upper bound.

Set $d_n=\max\{1,\lceil\delta n\rceil\}$ and define the [asymptotic rate-distance function](../../../coding-theory.md#asymptotic-rate-distance-function) by

$$
\alpha_q(\delta)=\limsup_{n\to\infty}\frac1n\log_qA_q(n,d_n),\qquad0\le\delta\le1.
$$

The [code rate](../../../coding-theory.md#code-rate) is $n^{-1}\log_qM$ and the [relative minimum distance](../../../coding-theory.md#relative-minimum-distance-of-a-code) is $d/n$. A limsup suffices; no unproved existence of a limit for optimal code sizes is required. The packing radii have fraction tending to $\delta/2$, so the finite [Hamming bound](../../../coding-theory.md#hamming-bound) and the volume exponent give the [asymptotic Hamming bound](../../../coding-theory.md#asymptotic-hamming-bound)

$$
\boxed{\alpha_q(\delta)\le1-H_q(\delta/2)\qquad(0\le\delta\le1).}
$$

The covering radii have fraction tending to $\delta$, giving the [asymptotic Gilbert–Varshamov bound](../../../coding-theory.md#asymptotic-gilbert-varshamov-bound)

$$
\boxed{\alpha_q(\delta)\ge1-H_q(\delta)\qquad(0\le\delta\le1-1/q).}
$$

For larger $\delta$, this covering argument gives only the trivial lower bound zero, not the expression obtained by extending the decreasing [information entropy](../../../information-theory.md#information-entropy) function beyond its maximum.

The asymptotic lower bound is also achievable by [linear codes](../../../coding-theory.md#linear-code) over a [finite field](../../../algebra.md#finite-field). For $\delta>0$ and sufficiently large $n$, take redundancy $r_n=\lfloor\log_qV_q(n-1,d_n-2)\rfloor+1$, so $q^{r_n}>V_q(n-1,d_n-2)$. The linear existence condition produces [dimension](../../../vector-space.md#dimension-vector-space) at least $n-r_n$; its rate has liminf at least $1-H_q(\delta)$. At $\delta=0$, use the whole space, of rate one. In particular, for binary codes the bounds reduce to

$$
\boxed{1-h_2(\delta)\le\alpha_2(\delta)\le1-h_2(\delta/2)\qquad(0\le\delta\le1/2),}
$$

where $h_2$ is the [binary entropy](../../../information-theory.md#binary-entropy) function.

## 4

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use binary codes, so the [polynomial](../../../polynomial.md) modulus is $f(X)=X^N+1=X^N-1$ in $\mathbb F_2[X]$. A [cyclic code](../../../coding-theory.md#cyclic-code) $C$ is a linear subspace of $\mathbb F_2^N$ invariant under the cyclic shift $(a_0,\ldots,a_{N-1})\mapsto(a_{N-1},a_0,\ldots,a_{N-2})$. Identify a word with $a(X)=\sum_{i=0}^{N-1}a_iX^i$. Addition is coefficientwise, and multiplication is [polynomial](../../../polynomial.md) multiplication reduced modulo $f$. In the [quotient ring](../../../commutative-algebra.md#quotient-ring)

$$
R=\mathbb F_2[X]/(f),
$$

multiplication by $X$ is exactly that cyclic shift. Closure under this map and linear combinations gives closure under multiplication by every [polynomial](../../../polynomial.md), so a [cyclic code](../../../coding-theory.md#cyclic-code) is an [ideal](../../../commutative-algebra.md#ideal) of $R$. Conversely, an [ideal](../../../commutative-algebra.md#ideal) is a linear subspace closed under multiplication by $X$, proving the correspondence.

Take the inverse image of $C$ in $\mathbb F_2[X]$. This is an [ideal](../../../commutative-algebra.md#ideal) containing $(f)$. The [polynomial division algorithm](../../../polynomial.md#polynomial-division) shows directly that it has a unique monic generator $g$: choose a nonzero [polynomial](../../../polynomial.md) of least [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) and divide any other member by it; the remainder is in the [ideal](../../../commutative-algebra.md#ideal) and has smaller [polynomial degree](../../../polynomial.md#degree-of-a-polynomial), so must vanish. If two monic generators existed, mutual divisibility would make them equal. Because $f$ belongs to the [ideal](../../../commutative-algebra.md#ideal), $g\mid f$. Conversely every monic divisor of $f$ defines an [ideal](../../../commutative-algebra.md#ideal) of $R$. Thus the [generator polynomial of a cyclic code](../../../coding-theory.md#generator-polynomial-of-a-cyclic-code) satisfies

$$
\boxed{C=(g)\subseteq R,\qquad g\mid X^N+1.}
$$

For a nonzero code, $g$ is its nonzero [polynomial](../../../polynomial.md) representative of least [polynomial degree](../../../polynomial.md#degree-of-a-polynomial). For the zero code, use $g=f$, whose residue in $R$ is zero; this standard convention covers that endpoint despite its having no nonzero [codeword](../../../coding-theory.md#codeword).

Let $r=\deg g$ and $k=N-r$, and put $h=f/g$. Every [codeword](../../../coding-theory.md#codeword) has a unique representation $bg$ with $\deg b<k$: dividing an arbitrary multiplier by $h$ does not change its product with $g$ modulo $f$. The words $g,Xg,\ldots,X^{k-1}g$ have distinct leading degrees below $N$ and are independent. Consequently

$$
\boxed{\dim C=N-\deg g=k.}
$$

The statement remains valid for the zero code, with an empty basis, and the full code, with $g=1$.

For length 16, characteristic two gives $X^{16}+1=(X+1)^{16}$. Its only monic divisors are $(X+1)^j$ for $0\le j\le16$. Hence all [binary cyclic codes of length a power of two](../../../coding-theory.md#binary-cyclic-codes-of-length-a-power-of-two) in this case are

$$
\boxed{C_j=((X+1)^j),\qquad\dim C_j=16-j,\qquad0\le j\le16.}
$$

There are exactly 17 codes, forming the chain $C_{16}\subset C_{15}\subset\cdots\subset C_0$. This is a [repeated-root cyclic code](../../../coding-theory.md#repeated-root-cyclic-code) situation, so it would be incorrect to count just square-free factors. Their canonical [check polynomials of a cyclic code](../../../coding-theory.md#check-polynomial-of-a-cyclic-code) are $(X+1)^{16-j}$. An explicit expansion of each generator is $\prod_{b:\,\text{bit }b\text{ of }j\text{ is }1}(1+X^{2^b})$.

The canonical [check polynomial of a cyclic code](../../../coding-theory.md#check-polynomial-of-a-cyclic-code) is

$$
\boxed{h(X)=\frac{X^N+1}{g(X)},\qquad g(X)h(X)=X^N+1.}
$$

Indeed $ah\equiv0\pmod f$ means $f\mid ah$. Since $f=gh$, cancellation in the [polynomial ring](../../../commutative-algebra.md#polynomial-ring) gives $g\mid a$, exactly code membership. No coprimality of $g$ and $h$ is needed, including for length 16.

There is a normalization qualification in the printed definition. The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) condition alone does not force the supplied [polynomial](../../../polynomial.md) $\widetilde h$ to equal this canonical $h$. If $d=\gcd(f,\widetilde h)$, write $f=df_1$ and $\widetilde h=dh_1$ with $\gcd(f_1,h_1)=1$. Then $f\mid a\widetilde h$ holds exactly when $f_1\mid a$, so its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is the [ideal](../../../commutative-algebra.md#ideal) generated by $f/d$. Therefore

$$
\boxed{\ker(a\mapsto a\widetilde h\bmod f)=C\quad\Longleftrightarrow\quad\gcd(f,\widetilde h)=f/g.}
$$

Equivalently $\widetilde h=h u$ with $\gcd(u,g)=1$. Requiring the monic divisor of $f$ selects the canonical [check polynomial of a cyclic code](../../../coding-theory.md#check-polynomial-of-a-cyclic-code). For example $Xh$ gives the same [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) as $h$, since $X$ is a unit modulo $f$, but is generally a different [polynomial](../../../polynomial.md). Given any permitted $\widetilde h$, taking $\gcd(f,\widetilde h)$ recovers the canonical $h$.

To construct a [parity-check matrix](../../../coding-theory.md#parity-check-matrix), write the canonical $h=\sum_{l=0}^k h_lX^l$ and its [reciprocal polynomial](../../../polynomial.md#reciprocal-polynomial) $h^*(X)=X^kh(X^{-1})$. Take coefficient vectors, padded to length $N$, of

$$
\boxed{h^*,\ Xh^*,\ldots,X^{r-1}h^*}
$$

as the $r$ rows of $H$. Here $h_0=1$ because $h\mid f$, so these rows have successive leading degrees $k,k+1,\ldots,N-1$ and are independent. For a word $a$, row $j$ has dot product $\sum_{l=0}^k h_{k-l}a_{j+l}$, the coefficient of $X^{k+j}$ in the ordinary product $ah$. If $a\in C$, then $ah=bf$ with $\deg b<k$. This product has no terms in degrees $k,\ldots,N-1$, so $Ha^T=0$. The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of $H$ has [dimension](../../../vector-space.md#dimension-vector-space) $N-r=k$, the same as $C$, proving $\ker H=C$. This proves the [reciprocal-polynomial parity-check matrix](../../../coding-theory.md#reciprocal-polynomial-parity-check-matrix) construction and identifies its rows as a basis for the [dual of a cyclic code](../../../coding-theory.md#dual-of-a-cyclic-code).

Alternatively, a supplied [check polynomial of a cyclic code](../../../coding-theory.md#check-polynomial-of-a-cyclic-code) reduced modulo $f$, $\widetilde h=\sum_{l=0}^{N-1}\widetilde h_lX^l$, gives the [polynomial multiplication parity-check matrix](../../../coding-theory.md#polynomial-multiplication-parity-check-matrix)

$$
B_{ti}=\widetilde h_{\,t-i\bmod N}\qquad(0\le t,i<N).
$$

This circulant matrix represents multiplication by $\widetilde h$ modulo $f$, so its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $C$ and its [matrix rank](../../../vector-space.md#matrix-rank) is $r$. Selecting independent rows yields a rank-$r$ [parity-check matrix](../../../coding-theory.md#parity-check-matrix) even without initially normalizing the supplied [polynomial](../../../polynomial.md).

The [syndrome](../../../coding-theory.md#syndrome) $s(y)=Hy^T$ labels the [coset](../../../group-theory.md#coset) $C+y$. Indeed $s(y)=s(z)$ if and only if $H(y-z)^T=0$, equivalently $y-z\in C$. There are $2^r$ [cosets](../../../group-theory.md#coset), each with $2^k$ words, and the [syndrome classification of code cosets](../../../coding-theory.md#syndrome-classification-of-code-cosets) gives a bijection between them and $\mathbb F_2^r$. If $y=c+e$ is a transmitted [codeword](../../../coding-theory.md#codeword) plus an error, then $s(y)=s(e)$: the [syndrome](../../../coding-theory.md#syndrome) determines the error [coset](../../../group-theory.md#coset). Choosing a minimum-weight [coset leader](../../../coding-theory.md#coset-leader) and subtracting it performs [minimum-distance decoding](../../../coding-theory.md#minimum-distance-decoding). The error itself need not be uniquely identified, but it is unique when its weight is at most $\lfloor(d-1)/2\rfloor$, since the corresponding error-correction balls are disjoint.

For the [repetition code](../../../coding-theory.md#repetition-code), the nonzero [codeword](../../../coding-theory.md#codeword) is the all-ones word, so

$$
\boxed{g_{\mathrm{rep}}(X)=1+X+\cdots+X^{N-1},\qquad h_{\mathrm{rep}}(X)=X+1.}
$$

Their product is $X^N+1$, and the generator [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) $N-1$ gives [dimension](../../../vector-space.md#dimension-vector-space) one. For the [single parity-check code](../../../coding-theory.md#single-parity-check-code), membership is $a(1)=0$, equivalent to divisibility by $X+1$. Thus

$$
\boxed{g_{\mathrm{par}}(X)=X+1,\qquad h_{\mathrm{par}}(X)=1+X+\cdots+X^{N-1}.}
$$

Its [dimension](../../../vector-space.md#dimension-vector-space) is $N-1$; it is the even-weight code.

Finally, factor the binary length-seven modulus:

$$
X^7+1=(X+1)(X^3+X+1)(X^3+X^2+1).
$$

A standard cyclic realization of the [Hamming code of length seven](../../../coding-theory.md#hamming-code-of-length-seven) uses

$$
\boxed{g(X)=X^3+X+1,\qquad h(X)=(X+1)(X^3+X^2+1)=X^4+X^2+X+1.}
$$

Its [dimension](../../../vector-space.md#dimension-vector-space) is four. The reciprocal-check construction gives

$$
H=\begin{pmatrix}1&0&1&1&1&0&0\\0&1&0&1&1&1&0\\0&0&1&0&1&1&1\end{pmatrix}.
$$

Its columns are exactly the seven distinct nonzero vectors of $\mathbb F_2^3$, so no word of weight one or two is in its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). The generator itself has weight three, so the [minimum Hamming distance](../../../coding-theory.md#minimum-distance-of-a-code) is exactly three; this is the $[7,4,3]$ [Hamming code](../../../coding-theory.md#hamming-code). Reversing the cyclic coordinate order gives the equally valid reciprocal choice

$$
\boxed{g(X)=X^3+X^2+1,\qquad h(X)=X^4+X^3+X^2+1.}
$$

The [polynomial](../../../polynomial.md) answer therefore depends on the cyclic coordinate convention, while the resulting codes are equivalent.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
