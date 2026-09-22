# Mathematics II

↑ **Parent:** [Prelims](../prelims.md)

Source: [released examination PDF, bundle pages 48–52](https://www.whatdotheyknow.com/request/bsc_mathematics_prelims_and_part/response/2784209/attach/3/202409%20817%20annex.pdf#page=48).

Original solutions to all seven questions and all 42 lettered or Roman subparts of the ordinary sitting on 24 June 2015.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
    - [iv](#2/a/iv)
      - [Solution](#2/a/iv/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
    - [v](#2/b/v)
      - [Solution](#2/b/v/solution)
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
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
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
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)

## 1

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Call $k$ a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) when $a_k\geq a_m$ for every $m>k$. If there are infinitely many [peaks of a sequence](../../../sequence-and-series.md#peak-of-a-sequence), list their indices in increasing order, $k_1<k_2<\cdots$. Since $k_{r+1}>k_r$,

$$
\boxed{a_{k_1}\geq a_{k_2}\geq\cdots.}
$$

This is a decreasing [subsequence](../../../sequence-and-series.md#subsequence); throughout this argument, a decreasing [monotone sequence](../../../sequence-and-series.md#monotone-sequence) may have equal successive terms.

If there are only finitely many [peaks of a sequence](../../../sequence-and-series.md#peak-of-a-sequence), choose $N$ beyond all their indices; take $N=1$ if there are none. Every $n\geq N$ fails to be a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence), so some $m>n$ satisfies $a_m>a_n$. Starting with $n_1=N$, choose such an $n_{r+1}>n_r$ recursively. This gives

$$
\boxed{a_{n_1}<a_{n_2}<\cdots.}
$$

The two cases prove the [monotone subsequence theorem](../../../sequence-and-series.md#monotone-subsequence-theorem) without any boundedness hypothesis.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [Bolzano-Weierstrass theorem](../../../sequence-and-series.md#bolzano-weierstrass-theorem) states: **every [bounded sequence](../../../sequence-and-series.md#bounded-sequence) of [real numbers](../../../arithmetic.md#real-number) has a [convergent subsequence](../../../real-analysis.md#convergent-subsequence).**

By the [monotone subsequence theorem](../../../sequence-and-series.md#monotone-subsequence-theorem) proved in the preceding part, a [bounded sequence](../../../sequence-and-series.md#bounded-sequence) $(a_n)$ has a [monotone subsequence](../../../sequence-and-series.md#monotone-subsequence) $(b_r)$. It inherits the bounds of $(a_n)$. For completeness, the [bounded monotone sequence theorem](../../../sequence-and-series.md#bounded-monotone-sequence-theorem) follows directly from [completeness of the real numbers](../../../sequence-and-series.md#completeness-of-the-real-numbers). If $(b_r)$ is increasing, let $L=\sup\{b_r:r\geq1\}$. For every $\varepsilon>0$, the definition of [supremum](../../../real-analysis.md#supremum) supplies $r_0$ with $L-\varepsilon<b_{r_0}\leq L$. Then

$$
r\geq r_0\quad\Longrightarrow\quad L-\varepsilon<b_{r_0}\leq b_r\leq L,
$$

so $b_r\to L$. If $(b_r)$ is decreasing, apply the increasing case to $(-b_r)$, or use its [infimum](../../../real-analysis.md#infimum). Thus in either case

$$
\boxed{\text{some }n_1<n_2<\cdots\text{ and }L\in\mathbb R\text{ satisfy }a_{n_r}\longrightarrow L.}
$$

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

It is useful to prove the [contrapositive](../../../mathematical-logic.md#contrapositive). Suppose $k$ is a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) $(a_n)$ and $m$ is a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) $(-a_n)$. The second condition says $a_j\geq a_m$ for every $j>m$. Hence

$$
j>\max\{k,m\}\quad\Longrightarrow\quad a_m\leq a_j\leq a_k.
$$

Only finitely many earlier terms remain, and their [absolute values](../../../real-analysis.md#absolute-value) have a finite [maximum](../../../set.md#maximum-of-a-subset-of-a-total-order). Together these give a bound for every term, so $(a_n)$ is a [bounded sequence](../../../sequence-and-series.md#bounded-sequence). Consequently,

$$
\boxed{(a_n)\text{ unbounded}\ \Longrightarrow\ (a_n)\text{ or }(-a_n)\text{ has no peaks}.}
$$

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

If $a_n\to L$, every [subsequence](../../../sequence-and-series.md#subsequence) also has [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) $L$: its increasing indices eventually exceed any prescribed threshold. This applies in particular to every [monotone subsequence](../../../sequence-and-series.md#monotone-subsequence).

Conversely, suppose $(a_n)$ is a [bounded sequence](../../../sequence-and-series.md#bounded-sequence) and all its [monotone subsequences](../../../sequence-and-series.md#monotone-subsequence) converge to the same $L$. At least one exists by the [monotone subsequence theorem](../../../sequence-and-series.md#monotone-subsequence-theorem). If $a_n$ did not tend to $L$, there would be $\varepsilon_0>0$ and a [subsequence](../../../sequence-and-series.md#subsequence) $(a_{n_j})$ such that

$$
|a_{n_j}-L|\geq\varepsilon_0\qquad(j\geq1).
$$

Apply the [monotone subsequence theorem](../../../sequence-and-series.md#monotone-subsequence-theorem) to $(a_{n_j})$. The resulting further [subsequence](../../../sequence-and-series.md#subsequence) is also a [monotone subsequence](../../../sequence-and-series.md#monotone-subsequence) of $(a_n)$, so it tends to $L$, contradicting the displayed bound. Therefore

$$
\boxed{a_n\to L\ \Longleftrightarrow\ \text{every monotone subsequence tends to }L.}
$$

The [bounded monotone sequence theorem](../../../sequence-and-series.md#bounded-monotone-sequence-theorem) ensures that these [subsequences](../../../sequence-and-series.md#subsequence) have finite [limits of sequences](../../../sequence-and-series.md#limit-of-a-sequence); the hypothesis requires those values to agree.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Choose the [sequence](../../../sequence-and-series.md#sequence)

$$
\boxed{a_n=(-1)^n\qquad(n\geq1).}
$$

Every even index is a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) $(a_n)$, since its value is $1$ and all later values are at most $1$. Every odd index is a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) $(-a_n)$ for the same reason. Both [sets](../../../set.md) of indices are infinite.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Choose the [sequence](../../../sequence-and-series.md#sequence)

$$
\boxed{b_n=(-1)^n n\qquad(n\geq1).}
$$

After every index there are positive terms arbitrarily large and negative terms arbitrarily small. Thus every term has both a larger later term and a smaller later term. The former excludes a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) $(b_n)$, and the latter excludes a [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) $(-b_n)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Choose $N$ beyond every [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) of both $(a_n)$ and $(-a_n)$. Every term with index at least $N$ has a strictly larger later term and a strictly smaller later term.

Suppose for a contradiction that $a_n\to L$. Starting at $a_N$, recursively select a strictly increasing [subsequence](../../../sequence-and-series.md#subsequence) and a strictly decreasing [subsequence](../../../sequence-and-series.md#subsequence). Both must have [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) $L$. If their second terms are $u>a_N$ and $v<a_N$, respectively, passage to their [limits of sequences](../../../sequence-and-series.md#limit-of-a-sequence) gives

$$
L\geq u>a_N,\qquad L\leq v<a_N,
$$

a contradiction. Hence **$(a_n)$ does not converge.** This argument includes the possibility that either [set](../../../set.md) of [peaks of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) is empty.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Enumerate both [sets](../../../set.md) of [peaks of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) in increasing order of index. If $a_n\to L$, the two selected [subsequences](../../../sequence-and-series.md#subsequence) both tend to $L$.

For the converse, suppose $a_{k_r}\to L$ and $a_{m_r}\to L$. Given $\varepsilon>0$, choose $r$ large enough that both selected terms differ from $L$ by less than $\varepsilon$. For every $n>\max\{k_r,m_r\}$, the two [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) conditions imply

$$
\boxed{L-\varepsilon<a_{m_r}\leq a_n\leq a_{k_r}<L+\varepsilon.}
$$

The lower bound comes from the [peak of a sequence](../../../sequence-and-series.md#peak-of-a-sequence) of $(-a_n)$ at $m_r$. This is precisely the definition of $a_n\to L$. Thus **convergence is equivalent to a common finite [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) for the upper and lower peak [subsequences](../../../sequence-and-series.md#subsequence).**

## 2

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A [sequence](../../../sequence-and-series.md#sequence) $(a_n)$ of [real numbers](../../../arithmetic.md#real-number) is a [convergent sequence](../../../sequence-and-series.md#convergent-sequence) with [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) $\ell$ when

$$
\boxed{\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall n\geq N:\quad |a_n-\ell|<\varepsilon.}
$$

Divergence to positive [infinity](../../../mathematics.md#infinity) means

$$
\boxed{\forall M\in\mathbb R\ \exists N\in\mathbb N\ \forall n\geq N:\quad a_n>M.}
$$

In both definitions the same $N$ must control every later term. The second condition is not convergence to a [real number](../../../arithmetic.md#real-number).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Suppose $a_n\to\ell$. With tolerance $1$, choose $N$ such that $|a_n-\ell|<1$ whenever $n\geq N$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $|a_n|\leq|a_n-\ell|+|\ell|<1+|\ell|$ for these terms. Set

$$
\boxed{B=1+|\ell|+\sum_{j=1}^{N-1}|a_j|.}
$$

An empty sum is zero. This finite $B$ satisfies $|a_n|\leq B$ for every $n$, so every [convergent sequence](../../../sequence-and-series.md#convergent-sequence) is a [bounded sequence](../../../sequence-and-series.md#bounded-sequence).

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

Put $u=c^{-1}-1>0$, so $c=(1+u)^{-1}$. By [Bernoulli's inequality](../../../algebra.md#bernoulli-s-inequality), $(1+u)^n\geq1+nu$, and hence

$$
\boxed{0<c^n\leq\frac1{1+nu}\longrightarrow0.}
$$

More explicitly, for $\varepsilon>0$ choose an [integer](../../../integer.md) $N>1/(u\varepsilon)$. For $n\geq N$, the right-hand side is less than $\varepsilon$. Thus the [geometric sequence](../../../sequence-and-series.md#geometric-progression) has [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) zero, either directly by the definition or by the [squeeze theorem](../../../calculus.md#squeeze-theorem).

<h4 id="2/a/iv">iv</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/a/iv)

Given $\varepsilon>0$, the two assumed [limits of sequences](../../../sequence-and-series.md#limit-of-a-sequence) supply thresholds $N_1,N_2$ such that $|a_n-\ell|<\varepsilon$ for $n\geq N_1$ and $|c_n-\ell|<\varepsilon$ for $n\geq N_2$. For $n\geq\max\{N_1,N_2\}$,

$$
\ell-\varepsilon<a_n\leq b_n\leq c_n<\ell+\varepsilon.
$$

Thus $|b_n-\ell|<\varepsilon$ eventually, proving the [squeeze theorem](../../../calculus.md#squeeze-theorem):

$$
\boxed{b_n\longrightarrow\ell.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

**False.** Take the positive [sequence](../../../sequence-and-series.md#sequence) $\boxed{a_n=n}$. Then

$$
\frac{a_{n+1}}{a_n}=\frac{n+1}{n}=1+\frac1n\longrightarrow1,
$$

but $a_n\to+\infty$, so it has no finite [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence). Successive ratios close to one do not prevent cumulative growth.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**False.** Take the positive [geometric sequence](../../../sequence-and-series.md#geometric-progression) $\boxed{a_n=2^{-n}}$. It tends to zero, while

$$
\boxed{\frac{a_{n+1}}{a_n}=\frac12\not\longrightarrow1.}
$$

A positive [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) would make the claim true since $a_{n+1}/a_n$ would then tend to $\ell/\ell=1$, but positivity of each individual term does not exclude a zero [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

**True.** Since $a_n^n\to2$, there is $N_0$ such that $1<a_n^n<3$ for $n\geq N_0$. Positivity then gives $a_n>1$ on this tail.

Fix $\varepsilon>0$. If $a_n\geq1+\varepsilon$, [Bernoulli's inequality](../../../algebra.md#bernoulli-s-inequality) gives

$$
a_n^n\geq(1+\varepsilon)^n\geq1+n\varepsilon.
$$

For $n>2/\varepsilon$, this contradicts $a_n^n<3$. Therefore eventually $1<a_n<1+\varepsilon$, proving

$$
\boxed{a_n\longrightarrow1.}
$$

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

**True.** Choose $N$ such that $\ell/2<a_n<3\ell/2$ for every $n\geq N$. All the finitely many preceding terms are also positive. Define the positive [minimum](../../../set.md#minimum-of-a-subset-of-a-total-order) and finite [maximum](../../../set.md#maximum-of-a-subset-of-a-total-order)

$$
\eta=\min\bigl(\{\ell/2\}\cup\{a_j:1\leq j<N\}\bigr)>0,
\qquad
B=\max\bigl(\{3\ell/2\}\cup\{a_j:1\leq j<N\}\bigr)<\infty.
$$

Every term lies between $\eta$ and $B$, so every ratio is at most $B/\eta$. Consequently the required [supremum](../../../real-analysis.md#supremum) satisfies

$$
\boxed{\sup\{a_n/a_m:m,n\in\mathbb N\}\leq B/\eta<\infty.}
$$

<h4 id="2/b/v">v</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/v/solution">Solution</h5>

↑ **Parent:** [V](#2/b/v)

**False.** Choose the positive [sequence](../../../sequence-and-series.md#sequence)

$$
\boxed{a_n=1+\frac1{\sqrt n}.}
$$

It has [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) one, but [Bernoulli's inequality](../../../algebra.md#bernoulli-s-inequality) gives

$$
a_n^n=\left(1+\frac1{\sqrt n}\right)^n\geq1+\sqrt n\longrightarrow+\infty.
$$

Thus $(a_n^n)$ is not a [bounded sequence](../../../sequence-and-series.md#bounded-sequence).

## 3

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

For a [series](../../../sequence-and-series.md#series-mathematics) of [complex numbers](../../../complex-analysis.md#complex-number), form the [partial sums](../../../sequence-and-series.md#partial-sum) $S_N=\sum_{n=1}^Na_n$. The [series](../../../sequence-and-series.md#series-mathematics) converges when these [partial sums](../../../sequence-and-series.md#partial-sum) have a finite [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) $S\in\mathbb C$:

$$
\boxed{\forall\varepsilon>0\ \exists N_0\ \forall N\geq N_0:\quad |S_N-S|<\varepsilon.}
$$

The [series](../../../sequence-and-series.md#series-mathematics) has [absolute convergence](../../../sequence-and-series.md#absolute-convergence) when $\sum_{n=1}^{\infty}|a_n|$ converges as a [series](../../../sequence-and-series.md#series-mathematics) of nonnegative [real numbers](../../../arithmetic.md#real-number). A [series](../../../sequence-and-series.md#series-mathematics) beginning at $n=0$ uses the same definitions with that starting index.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Let $T_N=\sum_{n=1}^N|a_n|$ and $S_N=\sum_{n=1}^Na_n$. If $(T_N)$ converges, it is a [Cauchy sequence](../../../sequence-and-series.md#cauchy-sequence). Thus, for every $\varepsilon>0$, some $N$ makes

$$
\left|S_q-S_p\right|=\left|\sum_{n=p+1}^qa_n\right|\leq\sum_{n=p+1}^q|a_n|=T_q-T_p<\varepsilon
\qquad(q>p\geq N),
$$

where the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives the bound. Therefore $(S_N)$ is a [Cauchy sequence](../../../sequence-and-series.md#cauchy-sequence) in the [complex numbers](../../../complex-analysis.md#complex-number). These form a [complete metric space](../../../topological-analysis.md#complete-metric-space), so $(S_N)$ has a finite [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence). Equivalently, apply the [Cauchy criterion for series](../../../sequence-and-series.md#cauchy-criterion-for-series). Hence **[absolute convergence](../../../sequence-and-series.md#absolute-convergence) implies convergence.**

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The finite [geometric series](../../../sequence-and-series.md#geometric-series) identity, obtained by subtracting $t$ times the sum from the sum itself, gives

$$
S_N=\sum_{n=0}^Nt^n=\frac{1-t^{N+1}}{1-t}.
$$

For $0<t<1$, the [geometric sequence](../../../sequence-and-series.md#geometric-progression) $t^{N+1}$ tends to zero by Question 2(a)(iii). Therefore

$$
\boxed{\sum_{n=0}^{\infty}t^n=\frac1{1-t}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) of a [power series](../../../sequence-and-series.md#power-series) $\sum_{n=0}^{\infty}a_nz^n$ is the number $R\in[0,\infty]$ such that the [series](../../../sequence-and-series.md#series-mathematics) has [absolute convergence](../../../sequence-and-series.md#absolute-convergence) for $|z|<R$ and diverges for $|z|>R$. Equivalently,

$$
\boxed{R=\sup\left\{r\geq0:\ \sum_{n=0}^{\infty}|a_n|r^n<\infty\right\}.}
$$

Use $r^0=1$, including at $r=0$. The [supremum](../../../real-analysis.md#supremum) may be $+\infty$. There is no general conclusion at $|z|=R$: boundary convergence depends on the [coefficients](../../../vector-space.md#coefficient). If $R=0$, only the centre is guaranteed; if $R=\infty$, every finite $z$ lies inside the [disk of convergence](../../../sequence-and-series.md#disk-of-convergence).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The [comparison test for series](../../../sequence-and-series.md#comparison-test-for-series) states that, for $0\leq u_n\leq v_n$ eventually, convergence of $\sum v_n$ implies convergence of $\sum u_n$. Equivalently, divergence of $\sum u_n$ implies divergence of $\sum v_n$.

For $|z|<1$, the coefficient bound gives

$$
\sum_{n=1}^{\infty}|a_nz^n|\leq M\sum_{n=1}^{\infty}|z|^n<\infty
$$

by the [geometric series](../../../sequence-and-series.md#geometric-series) formula and the [comparison test for series](../../../sequence-and-series.md#comparison-test-for-series). The single term $a_0$ does not affect convergence. For $|z|\geq1$,

$$
|a_nz^n|>m|z|^n\geq m>0\qquad(n\geq1),
$$

so the terms do not tend to zero. The fact that [terms of a convergent series tend to zero](../../../sequence-and-series.md#terms-of-a-convergent-series-tend-to-zero) excludes convergence there. Thus

$$
\boxed{R=1.}
$$

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

If $z_0=0$, there is no $z$ with $|z|<|z_0|$, so the claim is vacuous. Suppose $z_0\ne0$. Convergence of $\sum a_nz_0^n$ implies $a_nz_0^n\to0$, because [terms of a convergent series tend to zero](../../../sequence-and-series.md#terms-of-a-convergent-series-tend-to-zero). In particular this is a [bounded sequence](../../../sequence-and-series.md#bounded-sequence), so $|a_nz_0^n|\leq C$ for some finite $C$ and every $n$.

For $|z|<|z_0|$, put $q=|z|/|z_0|<1$. Then

$$
|a_nz^n|=|a_nz_0^n|q^n\leq Cq^n.
$$

The [geometric series](../../../sequence-and-series.md#geometric-series) and [comparison test for series](../../../sequence-and-series.md#comparison-test-for-series) prove

$$
\boxed{\sum_{n=0}^{\infty}|a_nz^n|<\infty.}
$$

Thus convergence at one point gives [absolute convergence](../../../sequence-and-series.md#absolute-convergence) at every point strictly closer to the centre.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

All three examples below have positive [integer](../../../integer.md) [coefficients](../../../vector-space.md#coefficient), so they work under either convention for whether $0\in\mathbb N$.

For $R=1$, take $\boxed{a_n=1}$. This is the [geometric series](../../../sequence-and-series.md#geometric-series): it converges for $|z|<1$, and its terms fail to tend to zero for $|z|\geq1$.

For $R=0$, take $\boxed{a_n=n!}$, using the [factorial](../../../combinatorics.md#factorial) and $0!=1$. For every fixed $z\ne0$, the [absolute values](../../../real-analysis.md#absolute-value) of successive terms have ratio $(n+1)|z|$. This eventually exceeds two, so the terms grow without bound and the [series](../../../sequence-and-series.md#series-mathematics) cannot converge. At $z=0$ it is finite, giving [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) zero.

For $R=1/\sqrt2$, take

$$
\boxed{a_n=2^{\lfloor n/2\rfloor},}
$$

using the [floor function](../../../calculus.md#floor-function). The [coefficients](../../../vector-space.md#coefficient) satisfy

$$
\frac{(\sqrt2)^n}{\sqrt2}\leq a_n\leq(\sqrt2)^n.
$$

The upper bound and the [comparison test for series](../../../sequence-and-series.md#comparison-test-for-series) give [absolute convergence](../../../sequence-and-series.md#absolute-convergence) when $\sqrt2|z|<1$. The lower bound prevents the terms tending to zero when $\sqrt2|z|\geq1$. Hence the [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) is exactly $1/\sqrt2$.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Use the [ceiling function](../../../calculus.md#ceiling-function) to choose positive [integer](../../../integer.md) [coefficients](../../../vector-space.md#coefficient)

$$
\boxed{a_n=\lceil\alpha^{-n}\rceil\qquad(n\geq0).}
$$

Because $0<\alpha<1$, we have $\alpha^{-n}\geq1$ and

$$
\alpha^{-n}\leq a_n<\alpha^{-n}+1\leq2\alpha^{-n}.
$$

For $|z|<\alpha$, the [comparison test for series](../../../sequence-and-series.md#comparison-test-for-series) with the [geometric series](../../../sequence-and-series.md#geometric-series) gives

$$
\sum_{n=0}^{\infty}|a_nz^n|\leq2\sum_{n=0}^{\infty}\left(\frac{|z|}{\alpha}\right)^n<\infty.
$$

For $|z|\geq\alpha$, we instead have $|a_nz^n|\geq(|z|/\alpha)^n\geq1$, so the terms do not tend to zero. Thus **the [power series](../../../sequence-and-series.md#power-series) has [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) exactly $\alpha$.**

## 4

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

A [function](../../../function.md) $f:E\to\mathbb R$ is [continuous](../../../calculus.md#continuous-function) on $E$ if it is [continuous](../../../calculus.md#continuous-function) at every $p\in E$, meaning

$$
\boxed{\forall p\in E\ \forall\varepsilon>0\ \exists\delta>0\ \forall x\in E:\quad |x-p|<\delta\ \Longrightarrow\ |f(x)-f(p)|<\varepsilon.}
$$

The [function](../../../function.md) has [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $E$ when

$$
\boxed{\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in E:\quad |x-y|<\delta\ \Longrightarrow\ |f(x)-f(y)|<\varepsilon.}
$$

For [continuity](../../../calculus.md#continuous-function), $\delta$ may depend on both $p$ and $\varepsilon$. For [uniform continuity](../../../topological-analysis.md#uniform-continuity), one $\delta$ must work for every pair of points in $E$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Suppose the [continuous function](../../../calculus.md#continuous-function) $f$ did not have [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $[a,b]$. Negating its definition gives $\varepsilon_0>0$ such that for every $n\geq1$ there are $x_n,y_n\in[a,b]$ with

$$
|x_n-y_n|<1/n,\qquad |f(x_n)-f(y_n)|\geq\varepsilon_0.
$$

The [Bolzano-Weierstrass theorem](../../../sequence-and-series.md#bolzano-weierstrass-theorem), which states that every [bounded sequence](../../../sequence-and-series.md#bounded-sequence) of [real numbers](../../../arithmetic.md#real-number) has a [convergent subsequence](../../../real-analysis.md#convergent-subsequence), gives $x_{n_k}\to p$. The inequalities $a\leq x_{n_k}\leq b$ imply $p\in[a,b]$. By the [triangle inequality](../../../topological-analysis.md#triangle-inequality),

$$
|y_{n_k}-p|\leq|y_{n_k}-x_{n_k}|+|x_{n_k}-p|\longrightarrow0.
$$

Since [continuous functions preserve convergent sequences](../../../calculus.md#continuous-functions-preserve-convergent-sequences), both $f(x_{n_k})$ and $f(y_{n_k})$ tend to $f(p)$. Their difference therefore tends to zero, contradicting its [absolute value](../../../real-analysis.md#absolute-value) being at least $\varepsilon_0$. This proves the [Heine-Cantor theorem](../../../topological-analysis.md#heine-cantor-theorem) in the required setting: **$f$ has [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $[a,b]$.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For any $x,y\in\mathbb R$, rationalizing the difference of [square roots](../../../algebra.md#square-root) gives

$$
|g(x)-g(y)|=\frac{|f(x)-f(y)|}{\sqrt{f(x)}+\sqrt{f(y)}}\leq\frac12|f(x)-f(y)|,
$$

since $f(x),f(y)\geq1$. Given $\varepsilon>0$, use [uniform continuity](../../../topological-analysis.md#uniform-continuity) of $f$ with tolerance $2\varepsilon$ to obtain $\delta>0$. Whenever $|x-y|<\delta$, the displayed estimate yields $|g(x)-g(y)|<\varepsilon$. Thus **$g$ has [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $\mathbb R$.** The [square root](../../../algebra.md#square-root) [function](../../../function.md) is in fact [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) with constant $1/2$ on $[1,\infty)$.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Take

$$
\boxed{g(x)=1+|x|,\qquad f(x)=(1+|x|)^2.}
$$

Both [functions](../../../function.md) have values in $[1,\infty)$. The [reverse triangle inequality](../../../topological-analysis.md#reverse-triangle-inequality) gives $|g(x)-g(y)|\leq|x-y|$, so $g$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) and hence has [uniform continuity](../../../topological-analysis.md#uniform-continuity).

For $x_n=n$ and $y_n=n+1/n$, the distances satisfy $|x_n-y_n|=1/n\to0$, whereas

$$
|f(y_n)-f(x_n)|=2\frac{n+1}{n}+\frac1{n^2}>2.
$$

In particular tolerance $\varepsilon=1$ defeats every proposed $\delta$: choose $n$ with $1/n<\delta$. Thus **$f$ does not have [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $\mathbb R$.**

## 5

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Write the [partial sums](../../../sequence-and-series.md#partial-sum) as $S_N(x)=\sum_{n=1}^Nf_n(x)$. The [series](../../../sequence-and-series.md#series-mathematics) has [uniform convergence](../../../sequence-and-series.md#uniform-convergence) to $s:E\to\mathbb R$ if

$$
\boxed{\forall\varepsilon>0\ \exists N_0\in\mathbb N\ \forall N\geq N_0\ \forall x\in E:\quad |S_N(x)-s(x)|<\varepsilon.}
$$

The same threshold $N_0$ must control every point of $E$. Equivalently, the [supremum error](../../../sequence-and-series.md#supremum-error) $\sup_{x\in E}|S_N(x)-s(x)|$ tends to zero, for nonempty $E$.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) states: if [functions](../../../function.md) $f_n:E\to\mathbb R$ or $\mathbb C$ satisfy

$$
|f_n(x)|\leq M_n\quad\text{for every }x\in E,
\qquad M_n\geq0,
\qquad\sum_{n=1}^{\infty}M_n<\infty,
$$

then $\sum f_n$ has [uniform convergence](../../../sequence-and-series.md#uniform-convergence) and [absolute convergence](../../../sequence-and-series.md#absolute-convergence) on $E$. In fact $\sum|f_n|$ also has [uniform convergence](../../../sequence-and-series.md#uniform-convergence), since every tail is bounded by the corresponding tail of $\sum M_n$:

$$
\boxed{\sup_{x\in E}\sum_{n=N+1}^{\infty}|f_n(x)|\leq\sum_{n=N+1}^{\infty}M_n\longrightarrow0.}
$$

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Take $0\leq r<R$. At the point $r$, the [power series](../../../sequence-and-series.md#power-series) has [absolute convergence](../../../sequence-and-series.md#absolute-convergence), so $\sum_{n=0}^{\infty}|a_n|r^n<\infty$. On the whole [interval](../../../real-analysis.md#interval-mathematics) $[-r,r]$,

$$
|a_nx^n|\leq|a_n|r^n.
$$

The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) with $M_n=|a_n|r^n$ proves **[uniform convergence](../../../sequence-and-series.md#uniform-convergence) on $[-r,r]$.** It also gives the explicit tail estimate

$$
\boxed{\sup_{|x|\leq r}\left|\sum_{n=N+1}^{\infty}a_nx^n\right|\leq\sum_{n=N+1}^{\infty}|a_n|r^n\longrightarrow0.}
$$

For $r=0$ the [interval](../../../real-analysis.md#interval-mathematics) consists only of zero, and all positive-degree terms vanish. If $R=\infty$, the same argument applies to every finite $r$; if $R=0$, there is no $r\geq0$ with $r<R$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $S_N=\sum_{n=1}^Nf_n$ and let $s$ be its [uniform limit](../../../sequence-and-series.md#uniform-limit). Choose a finite $B\geq0$ with $|g(x)|\leq B$ for all $x\in E$. The [partial sums](../../../sequence-and-series.md#partial-sum) of the multiplied [series](../../../sequence-and-series.md#series-mathematics) are $gS_N$, and

$$
|g(x)S_N(x)-g(x)s(x)|\leq B|S_N(x)-s(x)|.
$$

For any $\varepsilon>0$, [uniform convergence](../../../sequence-and-series.md#uniform-convergence) supplies $N_0$ making $|S_N(x)-s(x)|<\varepsilon/(B+1)$ for all $N\geq N_0$ and $x\in E$. The displayed estimate then gives an error less than $\varepsilon$. Thus

$$
\boxed{\sum_{n=1}^{\infty}f_n(x)g(x)=g(x)s(x)\quad\text{uniformly on }E.}
$$

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Choose the unbounded [function](../../../function.md) $\boxed{g(x)=1/x}$ on $E=(0,1/2]$. It is unbounded because $g(1/k)=k$ for all [integers](../../../integer.md) $k\geq2$. For each $x\in E$, the [geometric series](../../../sequence-and-series.md#geometric-series) gives the sum and its remainder after degree $N$:

$$
\sum_{n=0}^{\infty}x^ng(x)=\frac1{x(1-x)},
\qquad
\frac1{x(1-x)}-\sum_{n=0}^Nx^{n-1}=\frac{x^N}{1-x}.
$$

Since $0<x\leq1/2$,

$$
\boxed{\sup_{x\in E}\left|\frac1{x(1-x)}-\sum_{n=0}^Nx^{n-1}\right|\leq2^{1-N}\longrightarrow0.}
$$

This proves [uniform convergence](../../../sequence-and-series.md#uniform-convergence). Although the first term $1/x$ and the sum are unbounded, the late tails have a bound tending to zero independently of $x$. [Uniform convergence](../../../sequence-and-series.md#uniform-convergence) concerns those tails and does not require the individual [functions](../../../function.md) to be bounded.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

For real-valued [functions](../../../function.md), the [Uniform Cauchy criterion](../../../sequence-and-series.md#uniform-cauchy-criterion) applied to [partial sums](../../../sequence-and-series.md#partial-sum) says that $\sum u_n$ has [uniform convergence](../../../sequence-and-series.md#uniform-convergence) exactly when

$$
\forall\varepsilon>0\ \exists N\ \forall q>p\geq N\ \forall x\in E:\quad\left|\sum_{n=p+1}^q u_n(x)\right|<\varepsilon.
$$

Sufficiency uses [completeness of the real numbers](../../../sequence-and-series.md#completeness-of-the-real-numbers).

Let $M$ be a common bound for the [uniformly bounded family of functions](../../../topological-analysis.md#uniformly-bounded-family-of-functions) $(g_n)$; increase it if necessary so that $M>0$. The assumed [uniform absolute convergence](../../../sequence-and-series.md#uniform-absolute-convergence) of $\sum f_n$ gives $N$ such that

$$
\sum_{n=p+1}^q|f_n(x)|<\frac{\varepsilon}{M+1}
\qquad(q>p\geq N,\ x\in E).
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) now yields

$$
\boxed{\left|\sum_{n=p+1}^q f_n(x)g_n(x)\right|\leq M\sum_{n=p+1}^q|f_n(x)|<\varepsilon.}
$$

The [Uniform Cauchy criterion](../../../sequence-and-series.md#uniform-cauchy-criterion) therefore proves **[uniform convergence](../../../sequence-and-series.md#uniform-convergence) of $\sum f_ng_n$.** The same estimate with $|f_ng_n|$ proves [uniform absolute convergence](../../../sequence-and-series.md#uniform-absolute-convergence) as well.

## 6

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

A [function](../../../function.md) $f:(a,b)\to\mathbb R$ is [differentiable](../../../analysis.md#differentiable-function) on $(a,b)$ when, at each $c\in(a,b)$, its [difference quotient](../../../calculus.md#difference-quotient) has a finite [limit of a function](../../../calculus.md#limit-of-a-function):

$$
\boxed{f'(c)=\lim_{h\to0}\frac{f(c+h)-f(c)}h\in\mathbb R.}
$$

Here $h\ne0$ and $c+h\in(a,b)$.

For sufficiently small nonzero $h$, the [difference quotient](../../../calculus.md#difference-quotient) has [absolute value](../../../real-analysis.md#absolute-value) at most $|f'(c)|+1$, because it tends to $f'(c)$. Consequently

$$
|f(c+h)-f(c)|\leq|h|\bigl(|f'(c)|+1\bigr)\longrightarrow0.
$$

This is [continuity](../../../calculus.md#continuous-function) at $c$. Since $c$ was arbitrary, **[differentiability](../../../analysis.md#differentiability) implies [continuity](../../../calculus.md#continuous-function) on $(a,b)$.**

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

On $(0,1)$, the [product rule](../../../calculus.md#product-rule) and [chain rule](../../../calculus.md#chain-rule) give $f'(x)=2x\sin(1/x)-\cos(1/x)$. On $(-1,0)$, the [function](../../../function.md) is constant and has [derivative](../../../calculus.md#derivative) zero. At zero,

$$
\frac{f(h)-f(0)}h=\begin{cases}h\sin(1/h),&h>0,\\0,&h<0.\end{cases}
$$

Its [absolute value](../../../real-analysis.md#absolute-value) is at most $|h|$, so the [squeeze theorem](../../../calculus.md#squeeze-theorem) gives $f'(0)=0$. Therefore

$$
\boxed{f'(x)=\begin{cases}2x\sin(1/x)-\cos(1/x),&0<x<1,\\0,&-1<x\leq0.\end{cases}}
$$

For $x_n=1/(2\pi n)$, we have $x_n\to0$ but $f'(x_n)=-1$ for every $n$. This differs from $f'(0)=0$, so $f'$ is not [continuous](../../../calculus.md#continuous-function) at zero. Indeed, $y_n=1/((2n+1)\pi)$ gives $f'(y_n)=1$, so the right-hand [limit of a function](../../../calculus.md#limit-of-a-function) does not exist. Thus **$f$ is [differentiable](../../../analysis.md#differentiable-function) everywhere on $(-1,1)$, while $f'$ is discontinuous at zero.**

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

Fix $d$ strictly between $f'(a)$ and $f'(b)$, and set $F(x)=f(x)-dx$. The [function](../../../function.md) $F$ is [continuous](../../../calculus.md#continuous-function) on $[a,b]$: interior [differentiability](../../../analysis.md#differentiability) gives interior [continuity](../../../calculus.md#continuous-function), and the finite one-sided [derivatives](../../../calculus.md#derivative) give [continuity](../../../calculus.md#continuous-function) at the endpoints. The [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) therefore gives a point $c$ where $F$ attains its [minimum](../../../set.md#minimum-of-a-subset-of-a-total-order).

Since $F'_+(a)=f'(a)-d<0$, for sufficiently small $h>0$ we have $F(a+h)<F(a)$, so $a$ cannot be a minimizing point. Since $F'_-(b)=f'(b)-d>0$, the quotient $(F(b-h)-F(b))/(-h)$ is positive for sufficiently small $h>0$, giving $F(b-h)<F(b)$. Thus $b$ cannot be a minimizing point either, and $c\in(a,b)$.

[Fermat's theorem on stationary points](../../../calculus.md#fermat-s-theorem-on-stationary-points) states that a [differentiable function](../../../analysis.md#differentiable-function) at an interior [local minimum](../../../analysis.md#local-minimum) or [local maximum](../../../analysis.md#local-maximum) has [derivative](../../../calculus.md#derivative) zero there. Applying it to $F$ gives

$$
\boxed{0=F'(c)=f'(c)-d,\qquad f'(c)=d.}
$$

This proves the relevant case of [Darboux's theorem](../../../calculus.md#darboux-s-theorem-analysis); the argument uses [continuity](../../../calculus.md#continuous-function) of $f$, with no assumption of [continuity](../../../calculus.md#continuous-function) of $f'$.

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Choose $h_n=\min\{1/n,(b-c)/2\}>0$. Then $h_n\to0$ and $[c,c+h_n]\subset(a,b)$. The [mean value theorem](../../../calculus.md#mean-value-theorem) states that a [continuous function](../../../calculus.md#continuous-function) on a [closed interval](../../../real-analysis.md#closed-real-interval), [differentiable](../../../analysis.md#differentiable-function) in its interior, has an interior [derivative](../../../calculus.md#derivative) equal to its endpoint [difference quotient](../../../calculus.md#difference-quotient). It gives $x_n\in(c,c+h_n)$ with

$$
f'(x_n)=\frac{f(c+h_n)-f(c)}{h_n}.
$$

Here $x_n\ne c$, $x_n\to c$, and the right-hand side tends to $f'(c)$ by [differentiability](../../../analysis.md#differentiability) at $c$. If $L=\lim_{x\to c}f'(x)$ exists, the same values $f'(x_n)$ must tend to $L$. Uniqueness of the [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) gives

$$
\boxed{\lim_{x\to c}f'(x)=f'(c).}
$$

Thus a [derivative](../../../calculus.md#derivative) cannot have a [removable discontinuity](../../../calculus.md#removable-discontinuity) at a point where the original [function](../../../function.md) is [differentiable](../../../analysis.md#differentiable-function). The proof also excludes an infinite [limit of a function](../../../calculus.md#limit-of-a-function) there, since the displayed [difference quotients](../../../calculus.md#difference-quotient) have a finite [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence).

## 7

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

The [continuous function](../../../calculus.md#continuous-function) $|h|$ attains a finite [maximum](../../../set.md#maximum-of-a-subset-of-a-total-order) $M$ on $[a,b]$ by the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem). Additivity and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the [Riemann integral](../../../real-analysis.md#riemann-integral) imply, for any $x,y\in[a,b]$,

$$
\boxed{|H(y)-H(x)|=\left|\int_x^yh(t)\,dt\right|\leq M|y-x|.}
$$

For reversed endpoints, reverse the orientation of the [integral](../../../integral.md) before taking its [absolute value](../../../real-analysis.md#absolute-value). Given $\varepsilon>0$, choose $\delta=\varepsilon/(M+1)$. Then $|x-y|<\delta$ implies $|H(x)-H(y)|<\varepsilon$. Thus **$H$ is [continuous](../../../calculus.md#continuous-function) on $[a,b]$**, including one-sided [continuity](../../../calculus.md#continuous-function) at the endpoints; it is even [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). If $a=b$, the [function](../../../function.md) is defined on one point and the conclusion is immediate.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Write $G=\int_a^bg(t)\,dt\geq0$ and $I=\int_a^bf(t)g(t)\,dt$. By the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem), $f$ attains a [minimum](../../../set.md#minimum-of-a-subset-of-a-total-order) $m$ and a [maximum](../../../set.md#maximum-of-a-subset-of-a-total-order) $M$ on $[a,b]$. Because $g\geq0$, the [monotonicity of the Riemann integral](../../../real-analysis.md#monotonicity-of-the-riemann-integral) gives

$$
mG\leq I\leq MG.
$$

If $G=0$, this forces $I=0$, and every $c\in[a,b]$ satisfies the required identity. This includes $a=b$.

If $G>0$, divide to obtain $m\leq I/G\leq M$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem), applied between points where the [continuous function](../../../calculus.md#continuous-function) $f$ attains $m$ and $M$, supplies $c\in[a,b]$ with $f(c)=I/G$. Hence the [weighted mean value theorem for integrals](../../../real-analysis.md#weighted-mean-value-theorem-for-integrals) gives

$$
\boxed{\int_a^bf(t)g(t)\,dt=f(c)\int_a^bg(t)\,dt.}
$$

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Again let $G=\int_a^bg(t)\,dt\geq0$ and $I=\int_a^bf(t)g(t)\,dt$. Since $f$ is a nondecreasing [monotonic function](../../../calculus.md#monotonic-function), $f(a)\leq f(t)\leq f(b)$ on $[a,b]$. The condition $g\geq0$ and the [monotonicity of the Riemann integral](../../../real-analysis.md#monotonicity-of-the-riemann-integral) give

$$
f(a)G\leq I\leq f(b)G.
$$

Set $H(x)=\int_a^xg(t)\,dt$. By part (a), $H$ is [continuous](../../../calculus.md#continuous-function). Therefore the [function](../../../function.md)

$$
K(x)=f(a)H(x)+f(b)\bigl(G-H(x)\bigr)
$$

is [continuous](../../../calculus.md#continuous-function) on $[a,b]$. Its endpoint values are $K(a)=f(b)G$ and $K(b)=f(a)G$, which enclose $I$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) provides $d\in[a,b]$ with $K(d)=I$, so

$$
\boxed{\int_a^bf(t)g(t)\,dt=f(a)\int_a^dg(t)\,dt+f(b)\int_d^bg(t)\,dt.}
$$

If the two endpoint values coincide, the preceding bounds force $I$ to equal that common value and either endpoint works. Thus the proof also covers $G=0$, $f(a)=f(b)$ and $a=b$, without dividing by any possibly zero quantity.

## ↑ Ancestors (9)

1. [Prelims](../prelims.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Oxford](../../../past-exam-of-the-mathematics-course-of-the-university-of-oxford.md)
4. [Mathematics course of the University of Oxford](../../../university-of-oxford.md#mathematics-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../../university-of-oxford.md)
8. [List of universities](../../../README.md#list-of-universities)
9. [Codex Wiki](../../../README.md)
