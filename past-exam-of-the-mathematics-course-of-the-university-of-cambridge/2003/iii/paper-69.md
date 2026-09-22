# Paper 69

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper69.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper69.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [a](#2/2/a)
      - [Solution](#2/2/a/solution)
    - [b](#2/2/b)
      - [Solution](#2/2/b/solution)
    - [c](#2/2/c)
      - [Solution](#2/2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [1](#5/1)
    - [Solution](#5/1/solution)
  - [2](#5/2)
    - [Solution](#5/2/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)

## 1

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [continuous function](../../../calculus.md#continuous-function) $f$ on $[0,1]$, its [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) is

$$
B_n(f,x)=\sum_{j=0}^n f(j/n)\binom njx^j(1-x)^{n-j}.
$$

The weights are nonnegative and, by the [binomial theorem](../../../combinatorics.md#binomial-theorem), sum to $(x+1-x)^n=1$. Thus $|B_n(f,x)|\le\sum_j|f(j/n)|\binom njx^j(1-x)^{n-j}\le\|f\|_\infty$ at every $x\in[0,1]$, including the endpoints. Taking the [supremum norm](../../../functional-analysis.md#supremum-norm) gives

$$
\boxed{\|B_nf\|_\infty\le\|f\|_\infty.}
$$

In particular, $B_n$ is a [linear operator](../../../vector-space.md#linear-operator) of norm one, since it preserves the constant function one.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At a sampling point $j/n$, the given [polynomial](../../../polynomial.md) has value $f_{nm}(j/n)=n^{-m}j^{\underline m}$, where $j^{\underline m}=j(j-1)\cdots(j-m+1)$ is a [falling factorial](../../../combinatorics.md#falling-factorial). It vanishes when $j<m$. The [binomial coefficient](../../../combinatorics.md#binomial-coefficient) identity $j^{\underline m}\binom nj=n^{\underline m}\binom{n-m}{j-m}$ therefore gives

$$
\begin{aligned}
B_n(f_{nm},x)&=\frac{n^{\underline m}}{n^m}\sum_{j=m}^n\binom{n-m}{j-m}x^j(1-x)^{n-j}\\
&=\frac{n^{\underline m}}{n^m}x^m\sum_{r=0}^{n-m}\binom{n-m}{r}x^r(1-x)^{n-m-r}\\
&=\boxed{f_{nm}(1)x^m}.
\end{aligned}
$$

The last step is the [binomial theorem](../../../combinatorics.md#binomial-theorem), and $n^{\underline m}/n^m=\prod_{r=0}^{m-1}(1-r/n)=f_{nm}(1)$. For $m=0$ the empty product is one and the identity is simply $B_n1=1$. This is the [Bernstein falling-factorial identity](../../../functional-analysis.md#bernstein-falling-factorial-identity).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix $m$ and take $n\ge m$. Comparing the two products defining $f_{nm}$ and the [monomial](../../../polynomial.md#monomial) $g_m(x)=x^m$, change one factor at a time. Every factor has absolute value at most one on $[0,1]$, so the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\|f_{nm}-g_m\|_\infty\le\sum_{r=0}^{m-1}\frac rn=\frac{m(m-1)}{2n},\qquad |f_{nm}(1)-1|\le\frac{m(m-1)}{2n}.
$$

The contraction proved in (a) and the [Bernstein falling-factorial identity](../../../functional-analysis.md#bernstein-falling-factorial-identity) from (b) now give

$$
\begin{aligned}
\|B_ng_m-g_m\|_\infty&\le\|B_n(g_m-f_{nm})\|_\infty+\|(f_{nm}(1)-1)g_m\|_\infty\\
&\le\boxed{\frac{m(m-1)}n\longrightarrow0}.
\end{aligned}
$$

This proves [uniform convergence](../../../real-analysis.md#uniform-convergence) for each fixed [monomial](../../../polynomial.md#monomial); [linearity](../../../vector-space.md#linearity) then gives it for every fixed [polynomial](../../../polynomial.md). The cases $m=0,1$ have zero error for every $n$.

## 2

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

Use degree-indexed [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) and [Fejér sums](../../../fourier-series.md#fejer-sum), as in this paper. For a $2\pi$-periodic [continuous function](../../../calculus.md#continuous-function), put

$$
\widehat f_k=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-ikt}\,dt,\qquad s_n(f,x)=\sum_{k=-n}^n\widehat f_ke^{ikx},\qquad \sigma_n(f)=\frac1{n+1}\sum_{j=0}^ns_j(f).
$$

Equivalently,

$$
\sigma_n(f,x)=\sum_{|k|\le n}\left(1-\frac{|k|}{n+1}\right)\widehat f_ke^{ikx}.
$$

These are [trigonometric polynomials](../../../fourier-series.md#trigonometric-polynomial) of degree at most $n$. Some treatments index the [Fejér sum](../../../fourier-series.md#fejer-sum) by the number of terms rather than its degree; the degree convention here is why the formulas below contain $\sigma_{2n-1}$ and $\sigma_{n-1}$.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/a">a</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/a/solution">Solution</h5>

↑ **Parent:** [A](#2/2/a)

For a [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) $t_n(x)=\sum_{|k|\le n}c_ke^{ikx}$, [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the exponential [Fourier modes](../../../fourier-analysis.md#fourier-mode) gives $s_j(t_n)=t_n$ whenever $j\ge n$. Every term in the [de la Vallée Poussin sum](../../../fourier-series.md#de-la-vallee-poussin-sum) has such an index, so

$$
\boxed{v_n(t_n)=\frac1n\sum_{j=n}^{2n-1}t_n=t_n.}
$$

Here and below $n\ge1$.

<h4 id="2/2/b">b</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/b/solution">Solution</h5>

↑ **Parent:** [B](#2/2/b)

Subtracting the two initial averages of [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) gives

$$
\boxed{v_n=2\sigma_{2n-1}-\sigma_{n-1}},
$$

because $2n\sigma_{2n-1}=\sum_{j=0}^{2n-1}s_j$ and $n\sigma_{n-1}=\sum_{j=0}^{n-1}s_j$. The positive normalized [Fejér kernel](../../../fourier-series.md#fejer-kernel) gives the [uniform-norm contraction of Fejér summation](../../../fourier-series.md#fejer-summation-is-a-uniform-norm-contraction), namely $\|\sigma_mf\|_\infty\le\|f\|_\infty$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) therefore gives

$$
\boxed{\|v_nf\|_\infty\le2\|\sigma_{2n-1}f\|_\infty+\|\sigma_{n-1}f\|_\infty\le3\|f\|_\infty.}
$$

<h4 id="2/2/c">c</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/c/solution">Solution</h5>

↑ **Parent:** [C](#2/2/c)

For any [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) $t_n$ of degree at most $n$, reproduction from (a) and the [operator norm](../../../continuous-dual-space.md#operator-norm) bound from (b) imply

$$
f-v_nf=(f-t_n)-v_n(f-t_n),\qquad \|f-v_nf\|_\infty\le4\|f-t_n\|_\infty.
$$

Taking the [infimum](../../../real-analysis.md#infimum) over $t_n$ gives

$$
\boxed{\|f-v_nf\|_\infty\le4E_n(f)}.
$$

This is the [polynomial reproduction error bound](../../../uniform-approximation.md#polynomial-reproduction-error-bound) with $\|v_n\|\le3$; attaining the [best uniform approximation](../../../uniform-approximation.md#best-uniform-approximation) is not needed for this inequality.

## 3

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $p\in A$, $r=f-p$, $E=\|r\|_\infty$ and $M=\{x\in[0,1]:|r(x)|=E\}$. The [Kolmogorov criterion for uniform approximation](../../../uniform-approximation.md#kolmogorov-criterion-for-uniform-approximation) says

$$
\boxed{p\text{ is best}\quad\Longleftrightarrow\quad\forall h\in A,\ \min_{x\in M}r(x)h(x)\le0.}
$$

If $E=0$, $p=f$ is already best and the criterion holds. Suppose $E>0$. If $q=p+h$ were strictly better, then $|r(x)-h(x)|<|r(x)|=E$ on $M$, which forces $r(x)h(x)>0$ there. Conversely, if a direction $h$ has $rh>0$ everywhere on $M$, [compactness](../../../topology.md#compact-space) gives a positive lower bound on this product. On a sufficiently small neighborhood of $M$, $r$ and $h$ therefore have matching signs with $|h|$ bounded away from zero and $|r|$ bounded away from zero. On its compact complement, $|r|\le E-\delta$ for some $\delta>0$. Choose $\varepsilon>0$ so small that $\varepsilon\|h\|_\infty<\delta$ and that subtracting $\varepsilon h$ does not cross zero on that neighborhood. Then $\|r-\varepsilon h\|_\infty<E$, so $p$ is not a [best uniform approximation](../../../uniform-approximation.md#best-uniform-approximation). This proves both directions.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Chebyshev alternation theorem](../../../uniform-approximation.md#equioscillation-theorem) states that $p\in\mathcal P_n$ is a [best uniform approximation](../../../uniform-approximation.md#best-uniform-approximation) to real $f$ precisely when there are $n+2$ increasingly ordered points $x_0<\cdots<x_{n+1}$ with

$$
f(x_i)-p(x_i)=\eta(-1)^iE,\qquad \eta\in\{-1,1\},\quad E=\|f-p\|_\infty.
$$

For sufficiency, an improving [polynomial](../../../polynomial.md) direction $h$ would have to share these alternating signs, by the [Kolmogorov criterion for uniform approximation](../../../uniform-approximation.md#kolmogorov-criterion-for-uniform-approximation). The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) would give at least $n+1$ distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) between consecutive points. A nonzero [polynomial](../../../polynomial.md) of degree at most $n$ cannot do that. If $E=0$, no improvement is possible anyway.

For necessity, suppose $E>0$ and the active set $M$ has no alternating sequence of length $n+2$. Its positive-error and negative-error subsets are disjoint [compact sets](../../../topology.md#compact-space), hence separated by a positive distance. Reading them from left to right splits $M$ into finitely many consecutive sign blocks. If there are $L$ blocks, choosing one point per block gives an alternating sequence, so $L\le n+1$. Choose $z_j$ in the gap between each consecutive pair of blocks. The [polynomial](../../../polynomial.md) $h(x)=C\prod_{j=1}^{L-1}(x-z_j)$ has degree at most $n$; choose the sign of $C$ to match the error on the first block. Its sign then matches the error on every block, and it is nonzero throughout $M$. Thus $rh>0$ on $M$, contradicting the [Kolmogorov criterion for uniform approximation](../../../uniform-approximation.md#kolmogorov-criterion-for-uniform-approximation). There must therefore be $n+2$ alternating extrema.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Choose a [best uniform approximation](../../../uniform-approximation.md#best-uniform-approximation) $p_n\in\mathcal P_n$. It exists because this [vector subspace](../../../vector-space.md#vector-subspace) is a [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) and a minimizing sequence $q_j$ is bounded: $\|q_j\|_\infty\le\|f\|_\infty+\|f-q_j\|_\infty$. [Finite-dimensional equivalence of norms](../../../functional-analysis.md#finite-dimensional-equivalence-of-norms) then supplies a convergent subsequence of coefficients. If $E_n(f)>0$, the [Chebyshev alternation theorem](../../../uniform-approximation.md#equioscillation-theorem) gives $n+2$ alternating error extrema. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies a zero $x_{n,k}$ of $f-p_n$ in each of the $n+1$ intervening open intervals. These [interpolation nodes](../../../numerical-analysis.md#interpolation-node) are distinct, and uniqueness of [polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) gives

$$
\boxed{\ell_n(f)=p_n,\qquad \|\ell_n(f)-f\|_\infty=E_n(f)\longrightarrow0}.
$$

The convergence follows from the [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem). If $E_n(f)=0$, choose any $n+1$ distinct nodes: the [polynomial interpolant](../../../numerical-analysis.md#lagrange-polynomial) is still $f=p_n$. This constructs [interpolation nodes from best uniform approximation](../../../numerical-analysis.md#interpolation-nodes-from-best-uniform-approximation); the nodes depend on $f$, and no universal node system for all [continuous functions](../../../calculus.md#continuous-function) is asserted.

## 4

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Periodicity and the [Hölder condition](../../../sobolev-space.md#holder-condition) give $|f(x-t)-f(x)|\le M|t|^\alpha$ for $|t|\le\pi$. The positive normalized [Fejér kernel](../../../fourier-series.md#fejer-kernel) therefore yields

$$
\|\sigma_{n-1}f-f\|_\infty\le\frac{2M}{\pi}\int_0^\pi t^\alpha F_{n-1}(t)\,dt.
$$

The exponential-sum representation of the kernel bounds $F_{n-1}(t)\le n/2$. Also $\sin(t/2)\ge t/\pi$ for $0\le t\le\pi$, so $F_{n-1}(t)\le\pi^2/(2nt^2)$. Splitting at $1/n$ and using $0<\alpha<1$ gives

$$
\begin{aligned}
\int_0^\pi t^\alpha F_{n-1}(t)\,dt&\le\frac n2\int_0^{1/n}t^\alpha\,dt+\frac{\pi^2}{2n}\int_{1/n}^\pi t^{\alpha-2}\,dt\\
&\le\left(\frac1{2(\alpha+1)}+\frac{\pi^2}{2(1-\alpha)}\right)n^{-\alpha}.
\end{aligned}
$$

Hence the [Hölder error bound for Fejér summation](../../../fourier-series.md#holder-error-bound-for-fejer-summation) is

$$
\boxed{\|\sigma_{n-1}f-f\|_\infty\le M\left(\frac1{\pi(\alpha+1)}+\frac\pi{1-\alpha}\right)n^{-\alpha}.}
$$

The constant depends on the [Hölder exponent](../../../sobolev-space.md#holder-exponent) and $M$, but not on $n$ or $f$ beyond its [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) bound.

## 5

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="5/1">1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/1/solution">Solution</h4>

↑ **Parent:** [1](#5/1)

The [Markov interlacing lemma](../../../polynomial.md#markov-interlacing-lemma) says that [differentiation](../../../calculus.md#differentiation) preserves [interlacing roots of polynomials](../../../polynomial.md#interlacing-roots-of-polynomials). More explicitly, if two degree-$d$ real [polynomials](../../../polynomial.md) have ordered real roots satisfying $a_1\le b_1\le a_2\le\cdots\le a_d\le b_d$, their $k$th [derivatives](../../../calculus.md#derivative) have ordered roots $a_j^{(k)},b_j^{(k)}$ satisfying

$$
a_1^{(k)}\le b_1^{(k)}\le a_2^{(k)}\le\cdots\le a_{d-k}^{(k)}\le b_{d-k}^{(k)},\qquad 0\le k<d.
$$

The analogous alternating order is preserved for [polynomials](../../../polynomial.md) of consecutive degrees. Common roots are allowed through weak inequalities; strictly interlacing simple roots give strict inequalities. When a derivative is constant, its root list is empty.

<h3 id="5/2">2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/2/solution">Solution</h4>

↑ **Parent:** [2](#5/2)

Order the [interpolation nodes](../../../numerical-analysis.md#interpolation-node) as $t_0<\cdots<t_n$, as required by their alternating nodal data. Write $w(x)=\prod_{j=0}^n(x-t_j)$ and $\ell_i(x)=w(x)/[(x-t_i)w'(t_i)]$ for the [Lagrange cardinal polynomials](../../../numerical-analysis.md#lagrange-cardinal-polynomial). Differentiating [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) gives

$$
p^{(k)}(x)=\sum_{i=0}^np(t_i)\ell_i^{(k)}(x),\qquad M_k(x)=\sum_{i=0}^n|\ell_i^{(k)}(x)|.
$$

The upper bound is the [triangle inequality](../../../topological-analysis.md#triangle-inequality); equality follows by choosing each independent nodal value to be the sign of its weight. Thus this is the [nodal derivative norm from Lagrange cardinal polynomials](../../../numerical-analysis.md#nodal-derivative-norm-from-lagrange-cardinal-polynomials).

To identify the maximizing signs, put $P_i=w/(x-t_i)$, a [monic polynomial](../../../polynomial.md#monic-polynomial) of degree $n$. Since $\operatorname{sign}w'(t_i)=(-1)^{n-i}$,

$$
(-1)^i\ell_i^{(k)}(x)=\frac{(-1)^nP_i^{(k)}(x)}{|w'(t_i)|}.
$$

For $0\le k<n$, let $\xi_{i,j}$ be the ordered roots of $P_i^{(k)}$, $1\le j\le n-k$. The roots of $P_i$ decrease componentwise as $i$ increases: deleting a later node replaces one retained node by an earlier one. The [monotonicity of polynomial critical points in their roots](../../../polynomial.md#monotonicity-of-polynomial-critical-points-in-their-roots), iterated $k$ times, therefore gives $\xi_{n,j}\le\cdots\le\xi_{0,j}$. Moreover, $P_n$ and $P_0$ weakly interlace, so the [Markov interlacing lemma](../../../polynomial.md#markov-interlacing-lemma) gives $\xi_{0,j}\le\xi_{n,j+1}$. Together,

$$
\xi_{n,j}\le\xi_{n-1,j}\le\cdots\le\xi_{0,j}\le\xi_{n,j+1}.
$$

These root bands have disjoint interiors. At a fixed $x$, all but at most one band lie wholly on one side of $x$. In the possible remaining band, $\xi_{i,j}$ moves monotonically as $i$ increases. Since the [leading coefficients](../../../polynomial.md#leading-coefficient-of-a-polynomial) of all $P_i^{(k)}$ are positive, the sequence $P_i^{(k)}(x)$ has at most one sign change after zero entries are ignored. The same holds for $(-1)^i\ell_i^{(k)}(x)$. If $k=n$, every $P_i^{(n)}=n!>0$, so the conclusion also holds.

The maximizing nodal signs can consequently be chosen as $\pm(-1)^i$ throughout, or as $\pm(-1)^i$ before one index $s$ and $\mp(-1)^i$ from that index onward. Zero weights can be assigned either sign to complete such a pattern. These are precisely the nodal values of $\pm p^*$ or $\pm q_s$, proving

$$
\boxed{M_k(x)=|p^{*\,(k)}(x)|\quad\text{or}\quad M_k(x)=|q_s^{(k)}(x)|\text{ for some }1\le s\le n}.
$$

The argument works for all real $x$, hence in particular for $[-1,1]$. For $k>n$ every derivative vanishes and the result is immediate.

## 6

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Assume the [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence) is ordered and its relevant support spans satisfy $t_{i+k}>t_i$. For distinct knots, the [divided difference](../../../numerical-analysis.md#divided-difference) is a finite linear combination of evaluations, so it commutes with integration. With $u\in[a,b]$,

$$
\int_a^b(u-t)_+^{k-1}\,dt=\int_a^u(u-t)^{k-1}\,dt=\frac{(u-a)^k}{k}.
$$

Taking the order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) in $u$ gives

$$
\boxed{\int_a^bM_i(t)\,dt=k[t_i,\ldots,t_{i+k}]\frac{(u-a)^k}{k}=1}.
$$

Indeed, the order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) of a degree-$k$ [polynomial](../../../polynomial.md) is its [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial), here $1/k$. This proves the [unit-integral normalization of a B-spline](../../../uniform-approximation.md#unit-integral-normalization-of-a-b-spline). Admissible repeated knots follow by coalescing knots, with the usual one-sided endpoint conventions.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Write $N_{i,k}$ for the order-$k$ [B-spline](../../../uniform-approximation.md#b-spline). At order one, $N_{i,1}=\mathbf1_{[t_i,t_{i+1})}$, and the finite sum is one on its basic knot interval. For larger order, the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) is

$$
N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t),
$$

with a zero-denominator term defined as zero. Sum over $i=1,\ldots,n$. For each interior lower-order index $j=2,\ldots,n$, the combined coefficient is

$$
\frac{t-t_j}{t_{j+k-1}-t_j}+\frac{t_{j+k-1}-t}{t_{j+k-1}-t_j}=1.
$$

The two unmatched lower-order terms have supports $[t_1,t_k]$ and $[t_{n+1},t_{n+k}]$, respectively, and vanish on the open basic interval $(t_k,t_{n+1})$. Induction therefore gives

$$
\boxed{\sum_{i=1}^nN_{i,k}(t)=1,\qquad t_k\le t\le t_{n+1}}.
$$

For simple knots and $k\ge2$, [continuity](../../../calculus.md#continuous-function) extends the identity to both endpoints. In the order-one case and at admissible repeated endpoint knots, use the one-sided value from the basic interval. Extending the knot sequence in both directions also proves the [subpartition of unity for B-splines](../../../uniform-approximation.md#subpartition-of-unity-for-b-splines), $0\le\sum_iN_i\le1$ everywhere: the finite sum is a subset of a nonnegative full partition. That weaker global inequality will be needed in Question 7(a).

## 7

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) condition is $(f-s^*,N_i)=0$ for all $i$. Since $M_i=kN_i/(t_{i+k}-t_i)$, it is equivalently

$$
Ga=b,\qquad G_{ij}=(M_i,N_j),\qquad b_i=(M_i,f).
$$

The [mixed-normalization spline Gram matrix](../../../uniform-approximation.md#mixed-normalization-spline-gram-matrix) is invertible: $G=D^{-1}H$, where $D_{ii}=(t_{i+k}-t_i)/k>0$ and $H_{ij}=(N_i,N_j)$ is the positive-definite ordinary [Gram matrix](../../../linear-algebra.md#gram-matrix) of the [basis](../../../vector-space.md#basis). Nonnegativity and the [unit-integral normalization of a B-spline](../../../uniform-approximation.md#unit-integral-normalization-of-a-b-spline) give $|b_i|\le\|f\|_\infty\int_0^1M_i=\|f\|_\infty$. The [subpartition of unity for B-splines](../../../uniform-approximation.md#subpartition-of-unity-for-b-splines) gives, on all of $[0,1]$,

$$
|s^*(t)|\le\sum_j|a_j|N_j(t)\le\|a\|_{\ell^\infty}.
$$

Consequently

$$
\|P_Sf\|_\infty\le\|a\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|b\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|f\|_\infty,
$$

so

$$
\boxed{\|P_S\|_\infty\le\|G^{-1}\|_{\ell^\infty}}.
$$

This is the [maximum-norm bound for spline projection](../../../uniform-approximation.md#maximum-norm-bound-for-spline-projection). Using a subpartition matters when the basic knot interval is a proper subinterval of $[0,1]$. As in the paper's assertion that the image lies in $C[0,1]$, the [spline](../../../uniform-approximation.md#spline-mathematics) space here must consist of [continuous functions](../../../calculus.md#continuous-function); order-one step splines or full-multiplicity interior knots do not have that property.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

For distinct ordered knots, put $h_i=t_{i+1}-t_i>0$. The linear [B-spline](../../../uniform-approximation.md#b-spline) $N_i$ is the triangular hat supported on $[t_i,t_{i+2}]$, equal to $(t-t_i)/h_i$ on its rising segment and $(t_{i+2}-t)/h_{i+1}$ on its falling segment. Its integral-normalized partner is $M_i=2N_i/(h_i+h_{i+1})$. Thus

$$
\int N_i^2=\frac{h_i+h_{i+1}}3,\qquad \int N_iN_{i-1}=\frac{h_i}6,\qquad \int N_iN_{i+1}=\frac{h_{i+1}}6.
$$

For example, the left overlap is $\int_0^{h_i}(u/h_i)(1-u/h_i)\,du=h_i/6$. Nonadjacent hats have disjoint interiors of their [supports](../../../function.md#support), so their [inner product](../../../linear-algebra.md#inner-product) is zero. The [linear-spline mixed Gram matrix](../../../uniform-approximation.md#linear-spline-mixed-gram-matrix) therefore has row

$$
\boxed{g_{ii}=\frac23,\quad g_{i,i-1}=\frac{h_i}{3(h_i+h_{i+1})},\quad g_{i,i+1}=\frac{h_{i+1}}{3(h_i+h_{i+1})},\quad g_{ij}=0\ (|i-j|\ge2)}.
$$

Retain only column indices in $1,\ldots,n$: the first or last row has no neighbor outside this range. Admissible repeated endpoint knots are obtained by a limit with zero spacings, provided $h_i+h_{i+1}>0$; a degenerate hat with zero support width is not a [basis](../../../vector-space.md#basis) element.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

The entries in (b) satisfy

$$
|g_{ii}|-\sum_{j\ne i}|g_{ij}|\ge\frac23-\frac{h_i+h_{i+1}}{3(h_i+h_{i+1})}=\frac13.
$$

Thus $G$ has [strict diagonal dominance](../../../vector-space.md#strictly-diagonally-dominant-matrix) with margin at least $1/3$. To prove the [inverse infinity-norm bound from diagonal dominance](../../../vector-space.md#inverse-infinity-norm-bound-from-diagonal-dominance) directly, choose $i$ with $|a_i|=\|a\|_{\ell^\infty}$. The [reverse triangle inequality](../../../topological-analysis.md#reverse-triangle-inequality) gives

$$
\|Ga\|_{\ell^\infty}\ge|(Ga)_i|\ge\left(|g_{ii}|-\sum_{j\ne i}|g_{ij}|\right)|a_i|\ge\frac13\|a\|_{\ell^\infty}.
$$

This also proves that the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is zero and hence that $G$ is invertible. Substituting $a=G^{-1}b$ and taking the [operator norm](../../../continuous-dual-space.md#operator-norm) gives

$$
\boxed{\|G^{-1}\|_{\ell^\infty}\le3}.
$$

Combined with (a), it yields $\|P_S\|_\infty\le3$ for linear [splines](../../../uniform-approximation.md#spline-mathematics), independently of the knot spacings. The diagonal-dominance argument already proves the required estimate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
