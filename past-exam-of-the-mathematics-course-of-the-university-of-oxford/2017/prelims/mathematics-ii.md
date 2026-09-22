# Mathematics II

↑ **Parent:** [Prelims](../prelims.md)

Source: [released examination PDF, bundle pages 58–62](https://www.whatdotheyknow.com/request/bsc_mathematics_prelims_and_part/response/2784209/attach/3/202409%20817%20annex.pdf#page=58).

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
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
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
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

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [infimum](../../../real-analysis.md#infimum) of $A$ is its greatest [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set): $\alpha=\inf A$ means that $\alpha\leq x$ for every $x\in A$, and that every [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) $l$ of $A$ satisfies $l\leq\alpha$. The [supremum](../../../real-analysis.md#supremum) is its least [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set): $\beta=\sup A$ means that $x\leq\beta$ for every $x\in A$, and every [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) $u$ satisfies $\beta\leq u$. The [completeness of the real numbers](../../../sequence-and-series.md#completeness-of-the-real-numbers) ensures that both exist for a nonempty bounded [set](../../../set.md) of [real numbers](../../../arithmetic.md#real-number).

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Put $s=\sup(-A)$. For every $x\in A$, $-x\leq s$, hence $-s\leq x$, so $-s$ is a [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) of $A$. If $l$ is any [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) of $A$, then $-x\leq-l$ for every $x\in A$, making $-l$ an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) of $-A$. The definition of [supremum](../../../real-analysis.md#supremum) gives $s\leq-l$, or $l\leq-s$. Thus $-s$ is the greatest [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set), and

$$
\boxed{\inf A=-\sup(-A).}
$$

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Let $M=\max\{\sup A,\sup B\}$. Every element of the [union](../../../set.md#set-union) $A\cup B$ is at most $M$, so $M$ is an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set). Conversely, every [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) of $A\cup B$ is an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) of each of $A$ and $B$, hence is at least both [suprema](../../../real-analysis.md#supremum) and therefore at least $M$. Consequently

$$
\boxed{\sup(A\cup B)=\max\{\sup A,\sup B\}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

**True.** Write $s=\sup A$ and $u=\sup\{\sup R_m:m\geq1\}$. All these [suprema](../../../real-analysis.md#supremum) exist in $[0,1]$. Since $R_m\subseteq A$, we have $\sup R_m\leq s$ for every $m$, hence $u\leq s$. Conversely, every $x_{m,n}\leq\sup R_m\leq u$, so $u$ is an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) of $A$ and $s\leq u$. Thus the [iterated extrema of an array](../../../real-analysis.md#iterated-extrema-of-an-array) satisfy

$$
\boxed{\sup A=\sup_{m\geq1}\sup_{n\geq1}x_{m,n}.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

**True.** Set $l=\inf A$ and $v=\inf\{\inf R_m:m\geq1\}$. Because $R_m\subseteq A$, every row [infimum](../../../real-analysis.md#infimum) satisfies $\inf R_m\geq l$, so $v\geq l$. But $x_{m,n}\geq\inf R_m\geq v$ for all $m,n$, making $v$ a [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) of $A$. Therefore $v\leq l$, and

$$
\boxed{\inf A=\inf_{m\geq1}\inf_{n\geq1}x_{m,n}.}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

**True.** For every $m,n$,

$$
\inf C_n\leq x_{m,n}\leq\sup R_m.
$$

Fix $m$. The number $\sup R_m$ is an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) for every column [infimum](../../../real-analysis.md#infimum), so $\sup_n\inf C_n\leq\sup R_m$. This holds for every $m$, making $\sup_n\inf C_n$ a [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) of the row [suprema](../../../real-analysis.md#supremum). Taking their [infimum](../../../real-analysis.md#infimum) gives the [weak minimax inequality](../../../real-analysis.md#weak-minimax-inequality)

$$
\boxed{\sup_{n\geq1}\inf_{m\geq1}x_{m,n}\leq\inf_{m\geq1}\sup_{n\geq1}x_{m,n}.}
$$

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

**False.** Take $x_{1,n}=0$ for every $n$, and $x_{m,n}=1$ for every $m\geq2$ and every $n$. Each row is constant, so its [infimum](../../../real-analysis.md#infimum) and [supremum](../../../real-analysis.md#supremum) coincide. Nevertheless,

$$
\boxed{\inf_m\sup R_m=0<1=\sup_m\inf R_m.}
$$

The two outer [extrema](../../../mathematical-optimization.md#maximum-and-minimum) can select different rows.

## 2

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [sequence](../../../sequence-and-series.md#sequence) $(a_n)$ has [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) $L$ if

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall n\geq N:\quad |a_n-L|<\varepsilon.
$$

For the reciprocal rule, the required condition is $\boxed{L\ne0}$. Indeed, eventually $|a_n-L|<|L|/2$, so $|a_n|\geq|L|/2>0$. The reciprocals are then defined on this tail, and

$$
\left|\frac1{a_n}-\frac1L\right|=\frac{|a_n-L|}{|a_n||L|}\leq\frac{2|a_n-L|}{|L|^2}\longrightarrow0.
$$

A finite number of zero initial terms does not affect this tail [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence); if a reciprocal [sequence](../../../sequence-and-series.md#sequence) is required at every index, those terms must be excluded or assigned arbitrary values separately.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Rewrite the [recurrence relation](../../../sequence-and-series.md#recurrence-relation) as

$$
a_{n+1}=\frac12\left(a_n+\frac c{a_n}\right).
$$

Since $a_0=1>0$ and $c>0$, a positive $a_n$ gives a positive $a_{n+1}$. [Mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) therefore proves $\boxed{a_n>0\text{ for all }n\geq0}$, and also shows that every division in the [recurrence relation](../../../sequence-and-series.md#recurrence-relation) is defined.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For every $n\geq0$, direct algebra gives

$$
a_{n+1}^2-c=\frac{(a_n^2+c)^2-4ca_n^2}{4a_n^2}=\frac{(a_n^2-c)^2}{4a_n^2}\geq0.
$$

Thus $\boxed{a_n^2\geq c\text{ for every }n\geq1}$. This identity is the key estimate in [Newton iteration for a square root](../../../mathematical-optimization.md#newton-iteration-for-a-square-root).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

For $n\geq1$, the preceding parts give a positive denominator and a nonpositive numerator in

$$
a_{n+1}-a_n=\frac{c-a_n^2}{2a_n}.
$$

Hence $\boxed{a_{n+1}\leq a_n\text{ for every }n\geq1}$. The restriction $n\geq1$ matters: if $c>1$, then $a_1=(1+c)/2>a_0$.

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The tail $(a_n)_{n\geq1}$ is a [monotone sequence](../../../sequence-and-series.md#monotone-sequence) bounded below by zero. The [bounded monotone sequence theorem](../../../sequence-and-series.md#bounded-monotone-sequence-theorem) therefore gives $a_n\to L\geq0$. Taking the [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) in $a_n^2\geq c$ yields $L^2\geq c>0$, so $L>0$. The reciprocal rule from part (a) permits passage to the [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) in the [recurrence relation](../../../sequence-and-series.md#recurrence-relation):

$$
L=\frac12\left(L+\frac cL\right).
$$

Multiplication by $2L$ gives

$$
\boxed{L>0,\qquad L^2=c.}
$$

This proves existence of the positive [square root](../../../algebra.md#square-root) without assuming that existence when constructing the [sequence](../../../sequence-and-series.md#sequence).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

**Only (ii) is necessarily true.** Every real $a_n$ satisfies $a_n^2\geq0>c$, so (ii) holds automatically. For a single counterexample to (i) and (iii), choose $c=-3$ and $a_0=1$. The [recurrence relation](../../../sequence-and-series.md#recurrence-relation) then gives the nonzero periodic [sequence](../../../sequence-and-series.md#sequence)

$$
a_{2j}=1,\qquad a_{2j+1}=-1\qquad(j\geq0).
$$

Here $a_1<0$, disproving (i), and $a_2>a_1$, disproving (iii). This counterexample satisfies the requirement that no iterate is zero.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Write $d=-c>0$. Suppose, for a contradiction, that only finitely many sign changes occur. Since every $a_n\ne0$, the sign is then constant for $n\geq N$. Set $b_n=|a_n|>0$ on that tail. Multiplying the [recurrence relation](../../../sequence-and-series.md#recurrence-relation) by this constant sign gives

$$
b_{n+1}=\frac12\left(b_n-\frac d{b_n}\right)>0,
\qquad 0<b_{n+1}<\frac12b_n.
$$

Consequently $b_{N+j}<2^{-j}b_N$ for $j\geq1$, and $b_n\to0$ by comparison with a [geometric sequence](../../../sequence-and-series.md#geometric-progression). But positivity of $b_{n+1}$ requires $b_n^2>d$ at every step, which is incompatible with $b_n\to0$. Thus the [negative-parameter square-root iteration changes sign infinitely often](../../../mathematical-optimization.md#negative-parameter-square-root-iteration-changes-sign-infinitely-often).

## 3

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A real or complex [sequence](../../../sequence-and-series.md#sequence) $(a_n)$ is a [Cauchy sequence](../../../sequence-and-series.md#cauchy-sequence) if

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall m,n\geq N:\quad |a_m-a_n|<\varepsilon.
$$

For $z_n=x_n+iy_n$, the [complex modulus](../../../complex-analysis.md#complex-modulus) gives

$$
|x_m-x_n|\leq|z_m-z_n|,\qquad |y_m-y_n|\leq|z_m-z_n|.
$$

Thus the same $N$ works for both coordinate [Cauchy sequences](../../../sequence-and-series.md#cauchy-sequence). Conversely, if both real coordinate [Cauchy sequences](../../../sequence-and-series.md#cauchy-sequence) converge to $x$ and $y$, then $|z_n-(x+iy)|\leq|x_n-x|+|y_n-y|\to0$. This proves the needed completeness for [complex numbers](../../../complex-analysis.md#complex-number) from the assumed [completeness of the real numbers](../../../sequence-and-series.md#completeness-of-the-real-numbers).

Now suppose $\sum_{n\geq0}|z_n|$ converges. Its real [partial sums](../../../sequence-and-series.md#partial-sum) form a [Cauchy sequence](../../../sequence-and-series.md#cauchy-sequence). Given $\varepsilon>0$, sufficiently late tails therefore satisfy $\sum_{k=n+1}^m|z_k|<\varepsilon$. For $s_m=\sum_{k=0}^mz_k$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) yields

$$
|s_m-s_n|\leq\sum_{k=n+1}^m|z_k|<\varepsilon\qquad(m>n\geq N).
$$

The complex [partial sums](../../../sequence-and-series.md#partial-sum) are a [Cauchy sequence](../../../sequence-and-series.md#cauchy-sequence), hence converge by the coordinate argument. Therefore **[absolute convergence](../../../sequence-and-series.md#absolute-convergence) implies convergence** for a complex [series](../../../sequence-and-series.md#series-mathematics).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Define the [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) of the [power series](../../../sequence-and-series.md#power-series) by

$$
R=\sup\left\{|w|:w\in\mathbb C,\ \sum_{n=0}^{\infty}a_nw^n\text{ converges}\right\}\in[0,\infty],
$$

with $R=\infty$ when this [set](../../../set.md) is unbounded. It is nonempty because the [power series](../../../sequence-and-series.md#power-series) converges at zero.

If $|z|<R$, the definition of [supremum](../../../real-analysis.md#supremum) supplies a point $w$ of convergence with $|z|<|w|$. The terms $a_nw^n$ of a convergent [series](../../../sequence-and-series.md#series-mathematics) tend to zero and are bounded, say $|a_nw^n|\leq M$. Therefore

$$
|a_nz^n|\leq M\left(\frac{|z|}{|w|}\right)^n.
$$

The right-hand side has a convergent [geometric series](../../../sequence-and-series.md#geometric-series), since $|z|/|w|<1$. The [comparison test](../../../sequence-and-series.md#direct-comparison-test) proves [absolute convergence](../../../sequence-and-series.md#absolute-convergence) at $z$.

If $|z|>R$ and the [power series](../../../sequence-and-series.md#power-series) converged at $z$, then $|z|$ would belong to the [set](../../../set.md) whose [supremum](../../../real-analysis.md#supremum) is $R$, an immediate contradiction. Thus

$$
\boxed{|z|<R\Rightarrow\text{absolute convergence},\qquad |z|>R\Rightarrow\text{divergence}.}
$$

No assertion about the boundary $|z|=R$ follows from this argument. If $R=0$ the first assertion is vacuous; if $R=\infty$ the second is vacuous.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

For fixed $z\ne0$, the ratio of successive [absolute values](../../../real-analysis.md#absolute-value) is

$$
\frac{|z|^{n+1}/(n+1)!}{|z|^n/n!}=\frac{|z|}{n+1}\longrightarrow0.
$$

The [ratio test](../../../sequence-and-series.md#ratio-test) says that a [series](../../../sequence-and-series.md#series-mathematics) converges absolutely when this ratio has a [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) strictly below one. Thus this [power series](../../../sequence-and-series.md#power-series) converges absolutely for every complex $z$; at zero the conclusion is immediate. Its [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) is $\boxed{R=\infty}$.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Split the [power series](../../../sequence-and-series.md#power-series) into even and odd indices:

$$
\sum_{n=0}^{\infty}a_nz^n=\sum_{j=0}^{\infty}\left(\frac z2\right)^{2j}+\sum_{j=0}^{\infty}\frac{z^{2j+1}}{(2j+1)^2},
$$

whenever the two [series](../../../sequence-and-series.md#series-mathematics) converge absolutely. If $|z|<1$, the even part is a convergent [geometric series](../../../sequence-and-series.md#geometric-series), while the odd part is bounded termwise in [absolute value](../../../real-analysis.md#absolute-value) by $\sum_j|z|^{2j+1}$, also a convergent [geometric series](../../../sequence-and-series.md#geometric-series). Hence there is [absolute convergence](../../../sequence-and-series.md#absolute-convergence) throughout $|z|<1$.

If $|z|>1$, the odd terms have [absolute values](../../../real-analysis.md#absolute-value) $|z|^{2j+1}/(2j+1)^2$. Their successive ratio tends to $|z|^2>1$, so these terms grow eventually and do not tend to zero. The [term test for divergence](../../../sequence-and-series.md#term-test-for-divergence) therefore forces divergence of the original [power series](../../../sequence-and-series.md#power-series). Consequently its [radius of convergence](../../../sequence-and-series.md#radius-of-convergence) is

$$
\boxed{R=1.}
$$

## 4

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

If $x\ne y$, one of $x<y$ and $y<x$ holds. Since $f$ is [strictly increasing](../../../calculus.md#strictly-increasing-function), the corresponding values are strictly ordered, so $f(x)\ne f(y)$. Thus $f$ is an [injection](../../../algebra.md#injective-function). Every element of the [image of a function](../../../set-theory.md#image-of-a-function) $f([a,b])$ equals $f(x)$ for some $x\in[a,b]$, which is precisely [surjectivity](../../../algebra.md#surjective-function) onto that [image of a function](../../../set-theory.md#image-of-a-function). Hence $f:[a,b]\to f([a,b])$ is a **[bijection](../../../function.md#bijection)**.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Let $u<v$ lie in $f([a,b])$, and put $x=g(u)$ and $y=g(v)$. Equality $x=y$ would imply $u=v$. If $x>y$, strict [monotonicity](../../../calculus.md#monotonic-function) of $f$ would give $u=f(x)>f(y)=v$. Both are impossible, so $x<y$. Therefore the [inverse function](../../../function.md#inverse-function) $g$ is **[strictly increasing](../../../calculus.md#strictly-increasing-function)**.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $x_0>a$, define

$$
l=\sup\{f(t):a\leq t<x_0\}.
$$

This nonempty [set](../../../set.md) is bounded above by $f(x_0)$, so $l\leq f(x_0)$. Given $\varepsilon>0$, the [supremum](../../../real-analysis.md#supremum) property supplies $s<x_0$ with $l-\varepsilon<f(s)\leq l$. Whenever $s<t<x_0$, [monotonicity](../../../calculus.md#monotonic-function) gives

$$
l-\varepsilon<f(s)\leq f(t)\leq l.
$$

This proves the left-hand [one-sided limit](../../../calculus.md#one-sided-limit) $f^-(x_0)=l$.

For $x_0<b$, define

$$
r=\inf\{f(t):x_0<t\leq b\}.
$$

Here $r\geq f(x_0)$. Choose $u>x_0$ with $r\leq f(u)<r+\varepsilon$, using the [infimum](../../../real-analysis.md#infimum) property. For $x_0<t<u$, [monotonicity](../../../calculus.md#monotonic-function) gives $r\leq f(t)\leq f(u)<r+\varepsilon$, proving the right-hand [one-sided limit](../../../calculus.md#one-sided-limit) $f^+(x_0)=r$. Thus

$$
\boxed{f^-(x_0)\leq f(x_0)\leq f^+(x_0)}
$$

where the relevant [one-sided limits](../../../calculus.md#one-sided-limit) exist, including the indicated single [one-sided limit](../../../calculus.md#one-sided-limit) at each endpoint.

At an interior point, [continuity](../../../calculus.md#continuous-function) implies both [one-sided limits](../../../calculus.md#one-sided-limit) equal $f(x_0)$. Conversely, equality $f^-(x_0)=f^+(x_0)$ and the displayed inequalities force both to equal $f(x_0)$, giving [continuity](../../../calculus.md#continuous-function). Therefore

$$
\boxed{f\text{ continuous at }x_0\in(a,b)\iff f^-(x_0)=f^+(x_0).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

If $f$ is a [continuous function](../../../calculus.md#continuous-function), the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) ensures that every value between $f(a)$ and $f(b)$ is attained. [Monotonicity](../../../calculus.md#monotonic-function) excludes values outside that range, so $f([a,b])=[f(a),f(b)]$.

Conversely, suppose this equality of [sets](../../../set.md) holds. At an interior point, if $f^-(x_0)<f(x_0)$, any $y$ strictly between these two numbers lies in $[f(a),f(b)]$. Yet inputs below $x_0$ have values at most $f^-(x_0)$ and inputs at or above $x_0$ have values at least $f(x_0)$, so no input attains $y$. This contradicts [surjectivity](../../../algebra.md#surjective-function). The same argument excludes $f(x_0)<f^+(x_0)$, so part (b) gives [continuity](../../../calculus.md#continuous-function) at every interior point.

At $a$, a strict gap $f(a)<f^+(a)$ likewise leaves every value between them unattained; hence $f^+(a)=f(a)$, giving right [continuity](../../../calculus.md#continuous-function). At $b$, the corresponding argument gives $f^-(b)=f(b)$ and left [continuity](../../../calculus.md#continuous-function). These are the appropriate endpoint notions on $[a,b]$. Hence

$$
\boxed{f\text{ continuous on }[a,b]\iff f([a,b])=[f(a),f(b)].}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

With the strict [monotonicity](../../../calculus.md#monotonic-function) assumed at the start of the question, parts (a) and (c) give a [strictly increasing](../../../calculus.md#strictly-increasing-function) [inverse function](../../../function.md#inverse-function)

$$
g:[f(a),f(b)]\longrightarrow[a,b],\qquad g(f(a))=a,\quad g(f(b))=b.
$$

Its [image of a function](../../../set-theory.md#image-of-a-function) is exactly the [interval](../../../real-analysis.md#interval-mathematics) between its endpoint values. Apply part (c) to $g$, with domain $[f(a),f(b)]$, to conclude that **$g$ is a [continuous function](../../../calculus.md#continuous-function)**, including at both endpoints.

If the word “increasing” in this subpart were interpreted as merely [nondecreasing](../../../calculus.md#nondecreasing-function), an [inverse function](../../../function.md#inverse-function) need not exist: a constant [function](../../../function.md) is a counterexample. The preceding strict hypothesis supplies the required [injectivity](../../../algebra.md#injective-function).

## 5

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [sequence](../../../sequence-and-series.md#sequence) $(f_n)$ converges by [uniform convergence](../../../sequence-and-series.md#uniform-convergence) to $f$ on $E$ if

$$
\forall\varepsilon>0\ \exists M\in\mathbb N\ \forall n\geq M\ \forall x\in E:\quad |f_n(x)-f(x)|<\varepsilon.
$$

The index $M$ must work simultaneously for every $x\in E$.

Given $\varepsilon>0$, choose $m\geq N$ so large that $|f_m(x)-f(x)|<\varepsilon/3$ for every $x\in E$. The [continuity](../../../calculus.md#continuous-function) of this one fixed $f_m$ at $x_0$ gives $\delta>0$ such that $x\in E$ and $|x-x_0|<\delta$ imply $|f_m(x)-f_m(x_0)|<\varepsilon/3$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) then gives

$$
|f(x)-f(x_0)|\leq|f(x)-f_m(x)|+|f_m(x)-f_m(x_0)|+|f_m(x_0)-f(x_0)|<\varepsilon.
$$

Thus **$f$ is continuous at $x_0$**, with [continuity](../../../calculus.md#continuous-function) understood relative to $E$. This is the pointwise form of the [uniform limit theorem](../../../sequence-and-series.md#uniform-limit-theorem).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

**No.** Let $E=\mathbb R$, $x_0=0$ and

$$
f_n(x)=\frac1n\mathbf1_{\{0\}}(x),\qquad f(x)=0.
$$

The [supremum norm](../../../normed-vector-space.md#supremum-norm) satisfies $\|f_n-f\|_\infty=1/n\to0$, so there is [uniform convergence](../../../sequence-and-series.md#uniform-convergence) to the [continuous function](../../../calculus.md#continuous-function) $f$. But every $f_n$ is [discontinuous](../../../calculus.md#discontinuity-of-a-function) at zero: $f_n(0)=1/n$ whereas $f_n(x)=0$ for every $x\ne0$. No tail consists of [functions](../../../function.md) continuous at $x_0$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

At $x=0$, $f_n(x)=0$. For fixed $x>0$,

$$
0\leq f_n(x)=\frac{nx}{1+n^2x^2}\leq\frac1{nx}\longrightarrow0.
$$

Thus the [pointwise limit](../../../sequence-and-series.md#pointwise-limit) is zero everywhere on $[0,1]$. However, with $t=nx$, the inequality $1+t^2\geq2t$ gives $f_n(x)\leq1/2$, and equality occurs at $x=1/n\in[0,1]$. Hence

$$
\boxed{\|f_n\|_\infty=\frac12\quad\text{for every }n\geq1,}
$$

so there is **no [uniform convergence](../../../sequence-and-series.md#uniform-convergence)**. The moving evaluation point $1/n$ captures a peak missed by each fixed positive input.

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

The finite [geometric series](../../../sequence-and-series.md#geometric-series) identity gives, for each $|x|<1$,

$$
f_n(x)=\frac{x(1-x^n)}{1-x}\longrightarrow f(x)=\frac{x}{1-x},\qquad f(x)-f_n(x)=\frac{x^{n+1}}{1-x}.
$$

For every fixed $n$, the [absolute value](../../../real-analysis.md#absolute-value) of this error tends to infinity as $x\to1^-$. Thus

$$
\boxed{\sup_{-1<x<1}|f(x)-f_n(x)|=\infty,}
$$

and there is **no [uniform convergence](../../../sequence-and-series.md#uniform-convergence)** on $(-1,1)$.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

**Yes.** By [uniform convergence](../../../sequence-and-series.md#uniform-convergence), choose $N$ so that $|p_n(x)-f(x)|<1$ for every $n\geq N$ and every $x\in\mathbb R$. Then

$$
|p_n(x)-p_N(x)|<2\qquad(n\geq N,\ x\in\mathbb R).
$$

The [polynomial](../../../polynomial.md) $p_n-p_N$ is bounded on the whole [real line](../../../real-analysis.md#real-line). The supplied growth property of nonconstant [polynomials](../../../polynomial.md) implies that this difference must be constant; write $p_n=p_N+c_n$. Evaluating at zero gives $c_n=p_n(0)-p_N(0)\to c=f(0)-p_N(0)$. For each $x$, take the [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) in $p_n(x)=p_N(x)+c_n$ to obtain

$$
\boxed{f(x)=p_N(x)+c\quad\text{for every }x\in\mathbb R.}
$$

This is a [polynomial](../../../polynomial.md). The [uniform limits of polynomials on the real line](../../../sequence-and-series.md#uniform-limits-of-polynomials-on-the-real-line) therefore have a tail in which all nonconstant coefficients have already stabilized; only the constant coefficients may continue to change.

## 6

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [function](../../../function.md) $f$ is [differentiable](../../../analysis.md#differentiable-function) at $c$ if the finite [limit of a function](../../../calculus.md#limit-of-a-function)

$$
f'(c)=\lim_{x\to c,\ x\ne c}\frac{f(x)-f(c)}{x-c}
$$

exists. If it exists, put $L=f'(c)$ and define

$$
\epsilon(x)=\begin{cases}\dfrac{f(x)-f(c)}{x-c}-L,&x\ne c,\\0,&x=c.\end{cases}
$$

The definition of [derivative](../../../calculus.md#derivative) gives $\epsilon(x)\to0$ as $x\to c$. For $x\ne c$, rearrangement gives the desired [local linear approximation](../../../calculus.md#local-linear-approximation)

$$
f(x)=f(c)+L(x-c)+\epsilon(x)(x-c).
$$

At $x=c$, this identity holds because both terms containing $x-c$ vanish. Conversely, if such an identity holds, then for $x\ne c$ its [difference quotient](../../../calculus.md#difference-quotient) is $L+\epsilon(x)\to L$. Hence $f$ is [differentiable](../../../analysis.md#differentiable-function) at $c$, and necessarily $\boxed{L=f'(c)}$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Use the [local linear approximation](../../../calculus.md#local-linear-approximation) from part (a), with $L=f'(c)$. Since $x_n\leq c\leq y_n$ and $x_n\ne y_n$, we have $y_n-x_n>0$, and subtraction gives

$$
\frac{f(y_n)-f(x_n)}{y_n-x_n}-L=\frac{\epsilon(y_n)(y_n-c)+\epsilon(x_n)(c-x_n)}{y_n-x_n}.
$$

The coefficients $(y_n-c)/(y_n-x_n)$ and $(c-x_n)/(y_n-x_n)$ are nonnegative and sum to one. Therefore

$$
\left|\frac{f(y_n)-f(x_n)}{y_n-x_n}-L\right|\leq\max\{|\epsilon(x_n)|,|\epsilon(y_n)|\}\longrightarrow0.
$$

Here $\epsilon(c)=0$ handles any endpoint of a secant that happens to equal $c$. Thus [secants straddling a differentiability point](../../../analysis.md#secants-straddling-a-differentiability-point) satisfy

$$
\boxed{\lim_{n\to\infty}\frac{f(y_n)-f(x_n)}{y_n-x_n}=f'(c).}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

**No.** On $(-1,1)$ take $c=0$ and

$$
f(x)=\begin{cases}x^2\sin(1/x),&x\ne0,\\0,&x=0.\end{cases}
$$

At zero, its [difference quotient](../../../calculus.md#difference-quotient) has [absolute value](../../../real-analysis.md#absolute-value) $|x\sin(1/x)|\leq|x|\to0$, so $f'(0)=0$. Away from zero, the [product rule](../../../calculus.md#product-rule) and [chain rule](../../../calculus.md#chain-rule) apply. Define

$$
A_n=2\pi n,\qquad B_n=\begin{cases}\pi/2,&n\text{ even},\\3\pi/2,&n\text{ odd},\end{cases}\qquad x_n=\frac1{A_n},\quad y_n=\frac1{A_n+B_n}\qquad(n\geq1).
$$

These are distinct positive inputs tending to zero. Since $\sin A_n=0$ and $\sin(A_n+B_n)=\sin B_n$,

$$
\frac{f(y_n)-f(x_n)}{y_n-x_n}=-\frac{\sin B_n}{B_n}\frac{A_n}{A_n+B_n}.
$$

The even-indexed [subsequence](../../../sequence-and-series.md#subsequence) tends to $-2/\pi$, whereas the odd-indexed [subsequence](../../../sequence-and-series.md#subsequence) tends to $2/(3\pi)$. Thus the [limit of a sequence](../../../sequence-and-series.md#limit-of-a-sequence) does not exist. The two points lie on the same side of $c$, so the nonnegative-weight estimate in part (b) is unavailable. This is a concrete instance of [differentiability does not imply continuity of the derivative](../../../analysis.md#differentiability-does-not-imply-continuity-of-the-derivative).

## 7

↑ **Parent:** [Mathematics II](mathematics-ii.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

By the [Heine-Cantor theorem](../../../topological-analysis.md#heine-cantor-theorem), a [continuous function](../../../calculus.md#continuous-function) on the [compact interval](../../../real-analysis.md#compact-interval) $[a,b]$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity). Given $\varepsilon>0$, choose $\delta>0$ such that $|f(s)-f(t)|<\varepsilon$ whenever $s,t\in[a,b]$ and $|s-t|<\delta$.

Choose a finite [partition of an interval](../../../real-analysis.md#partition-of-an-interval) $a=t_0<t_1<\cdots<t_m=b$ with every width below $\delta$. Define the [step function](../../../measure-theory.md#step-function)

$$
\phi(t)=f(t_{j-1})\quad(t_{j-1}\leq t<t_j),\qquad\phi(b)=f(b).
$$

For each $t<b$, its distance from the chosen left endpoint is below $\delta$, so $|f(t)-\phi(t)|<\varepsilon$; at $b$ the error is zero. Hence

$$
\boxed{|f(t)-\phi(t)|<\varepsilon\quad\text{for every }t\in[a,b].}
$$

A [step function](../../../measure-theory.md#step-function) may have separately assigned values at its finitely many partition points; these values do not affect its [Riemann integral](../../../real-analysis.md#riemann-integral). If $a=b$, simply take $\phi=f$ on that singleton.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Put $E_n=\sup_{t\in[a,b]}|f(t)-\phi_n(t)|\to0$, so the hypothesis is [uniform convergence](../../../sequence-and-series.md#uniform-convergence). Every [step function](../../../measure-theory.md#step-function) is bounded and [Riemann integrable](../../../real-analysis.md#riemann-integrable-function): away from its finitely many partition points it is constant, and those exceptional points can be covered by [intervals](../../../real-analysis.md#interval-mathematics) of arbitrarily small total length. A [partition of an interval](../../../real-analysis.md#partition-of-an-interval) containing their boundaries makes the difference of its [upper Darboux sum](../../../real-analysis.md#upper-darboux-sum) and [lower Darboux sum](../../../real-analysis.md#lower-darboux-sum) arbitrarily small.

Choose one $n$ with $E_n<\infty$. Boundedness of $\phi_n$ and $|f|\leq|\phi_n|+E_n$ show that $f$ is a [bounded function](../../../function.md#bounded-function). Assume $a<b$, since for $a=b$ all the [integrals](../../../integral.md) are zero. Given $\eta>0$, choose $n$ so that $2E_n(b-a)<\eta/2$, and then a [partition of an interval](../../../real-analysis.md#partition-of-an-interval) $P$ such that $U(\phi_n,P)-L(\phi_n,P)<\eta/2$. On every partition subinterval, $|f-\phi_n|\leq E_n$ gives

$$
U(f,P)\leq U(\phi_n,P)+E_n(b-a),\qquad L(f,P)\geq L(\phi_n,P)-E_n(b-a).
$$

Thus

$$
U(f,P)-L(f,P)\leq U(\phi_n,P)-L(\phi_n,P)+2E_n(b-a)<\eta.
$$

The [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion) proves that $f$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function). Finally, [linearity of the integral](../../../integral.md#linearity-of-integration) and [monotonicity of the Riemann integral](../../../real-analysis.md#monotonicity-of-the-riemann-integral) give

$$
\left|\int_a^bf(t)\,dt-\int_a^b\phi_n(t)\,dt\right|\leq\int_a^b|f(t)-\phi_n(t)|\,dt\leq(b-a)E_n\longrightarrow0.
$$

Therefore

$$
\boxed{\int_a^bf(t)\,dt=\lim_{n\to\infty}\int_a^b\phi_n(t)\,dt.}
$$

This proves the relevant case of [uniform convergence preserves integrals on a compact interval](../../../sequence-and-series.md#uniform-convergence-preserves-integrals-on-a-compact-interval).

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

**The printed assertion needs an endpoint qualification:** the enumeration includes zero, but $\mathbf1_{[0,0)}$ is identically zero. In fact $f$ is continuous at zero; the claimed [discontinuities](../../../calculus.md#discontinuity) occur at every $r_j>0$.

Define the finite [step function](../../../measure-theory.md#step-function) sums

$$
\phi_N(t)=\sum_{k=1}^N\frac1{k^2}\mathbf1_{[0,r_k)}(t).
$$

The assumed convergence of $\sum_k1/k^2$ and the bound on each [indicator function](../../../measure-theory.md#indicator-function) give

$$
0\leq f(t)-\phi_N(t)\leq\sum_{k>N}\frac1{k^2},\qquad\|f-\phi_N\|_\infty\leq\sum_{k>N}\frac1{k^2}\longrightarrow0.
$$

Thus the defining [series](../../../sequence-and-series.md#series-mathematics) converges everywhere and has [uniform convergence](../../../sequence-and-series.md#uniform-convergence). Part (b) proves that **$f$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function)**; it also gives, if desired,

$$
\boxed{\int_0^1f(t)\,dt=\sum_{k=1}^{\infty}\frac{r_k}{k^2}.}
$$

For $r_j>0$ and $0\leq t<r_j$, every [indicator function](../../../measure-theory.md#indicator-function) is [nonincreasing](../../../calculus.md#nonincreasing-function), and the $j$th drops by one between $t$ and $r_j$. Hence

$$
f(t)-f(r_j)=\sum_{k\geq1}\frac{\mathbf1_{[0,r_k)}(t)-\mathbf1_{[0,r_k)}(r_j)}{k^2}\geq\frac1{j^2}.
$$

Taking inputs from the left tending to $r_j$ proves a [discontinuity](../../../calculus.md#discontinuity) there.

For completeness, [continuity](../../../calculus.md#continuous-function) at zero follows directly from a finite-head and tail argument. Given $\varepsilon>0$, choose $N$ with $\sum_{k>N}1/k^2<\varepsilon$. Choose $\delta>0$ below every positive $r_k$ with $k\leq N$. For $0\leq t<\delta$, the first $N$ [indicator functions](../../../measure-theory.md#indicator-function) have exactly their values at zero; the one with $r_k=0$, if present, is always zero. Thus $|f(t)-f(0)|\leq\sum_{k>N}1/k^2<\varepsilon$. This confirms that the endpoint exception is real. Replacing the printed enumeration of $[0,1)$ by one of $(0,1)$ would remove it.

Finally, the [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers) supplies a positive rational $r_j$ in every nonempty open subinterval of $[0,1]$. Thus **a [Riemann integrable](../../../real-analysis.md#riemann-integrable-function) [function](../../../function.md) can have a [discontinuity](../../../calculus.md#discontinuity) in every open subinterval**: [dense jumps do not prevent Riemann integrability](../../../real-analysis.md#dense-jumps-do-not-prevent-riemann-integrability).

## ↑ Ancestors (9)

1. [Prelims](../prelims.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Oxford](../../../past-exam-of-the-mathematics-course-of-the-university-of-oxford.md)
4. [Mathematics course of the University of Oxford](../../../university-of-oxford.md#mathematics-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../../university-of-oxford.md)
8. [List of universities](../../../README.md#list-of-universities)
9. [Codex Wiki](../../../README.md)
