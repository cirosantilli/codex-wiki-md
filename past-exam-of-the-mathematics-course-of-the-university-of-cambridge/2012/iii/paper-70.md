# Paper 70

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_70.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_70.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [1](#6/b/1)
      - [Solution](#6/b/1/solution)
    - [2](#6/b/2)
      - [Solution](#6/b/2/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $\Delta_t^2f(x)=f(x+t)-2f(x)+f(x-t)$, and use the [second modulus of smoothness](../../../uniform-approximation.md#second-modulus-of-smoothness) $\omega_2(f,h)=\sup_{|t|\le h}\|\Delta_t^2f\|_\infty$. The [Jackson kernel](../../../uniform-approximation.md#jackson-kernel) is even, nonnegative and has unit integral. Pairing the two halves of its [convolution](../../../fourier-analysis.md#convolution) therefore gives

$$
j_nf(x)-f(x)=\frac12\int_{-\pi}^{\pi}\Delta_t^2f(x)J_n(t)\,dt.
$$

We need a weighted moment estimate rather than just concentration of the [Jackson kernel](../../../uniform-approximation.md#jackson-kernel). For $|t|\le\pi$, the bounds $|\sin(t/2)|\ge |t|/\pi$ and $|\sin(nt/2)|\le\min(n|\sin(t/2)|,1)$ imply

$$
0\le J_n(t)\le C\min\{n,n^{-3}|t|^{-4}\}.
$$

Consequently, splitting the integral at $1/n$ gives

$$
\int_{-\pi}^{\pi}t^2J_n(t)\,dt
\le 2C\left(n\int_0^{1/n}t^2\,dt+n^{-3}\int_{1/n}^{\pi}t^{-2}\,dt\right)\le C'n^{-2}.
$$

The [second modulus of smoothness](../../../uniform-approximation.md#second-modulus-of-smoothness) satisfies $\omega_2(f,t)\le(1+t/h)^2\omega_2(f,h)$ for $t\ge0$. To see this, choose $q=\lceil t/h\rceil$ when $t>0$, put $u=t/q$, and factor the [function translation](../../../function.md#translation-of-a-function) difference $T_t-I=(T_u-I)\sum_{r=0}^{q-1}T_u^r$. Squaring gives at most $q^2$ translated second differences of step $u$. Each [function translation](../../../function.md#translation-of-a-function) is an [isometry](../../../riemannian-geometry.md#isometry) in the [supremum norm](../../../functional-analysis.md#supremum-norm), and centered and forward second differences have the same [supremum norm](../../../functional-analysis.md#supremum-norm). This proves the stated scaling bound.

Taking $h=1/n$, using $(1+n|t|)^2\le2+2n^2t^2$, and integrating against the [Jackson kernel](../../../uniform-approximation.md#jackson-kernel) now proves

$$
\|j_nf-f\|_\infty\le\frac12\omega_2(f,1/n)\int_{-\pi}^{\pi}(1+n|t|)^2J_n(t)\,dt\le C''\omega_2(f,1/n).
$$

Thus **the Jackson operator estimate is uniform in both $f$ and $n$**.

For the requested degree-$n$ [best uniform approximation](../../../uniform-approximation.md#best-uniform-approximation), note that the [Jackson kernel](../../../uniform-approximation.md#jackson-kernel), and hence $j_mf$, has [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) degree at most $2(m-1)$. Indeed the fourth power in the [Jackson kernel](../../../uniform-approximation.md#jackson-kernel) is the squared modulus of a squared sum of $m$ consecutive complex exponentials. Choose $m=\lfloor n/2\rfloor+1$, so $2(m-1)\le n$ and $m\ge n/2$. The [second-difference integral formula](../../../uniform-approximation.md#second-difference-integral-formula) gives

$$
\Delta_t^2f(x)=\int_{-|t|}^{|t|}(|t|-|u|)f''(x+u)\,du,
\qquad \omega_2(f,h)\le h^2\|f''\|_\infty.
$$

Applying the [Jackson operator estimate](../../../uniform-approximation.md#jackson-operator-estimate) with this $m$ yields the concise answer

$$
\boxed{E_n(f)\le \|j_mf-f\|_\infty\le \frac{4C''}{n^2}\|f''\|_\infty\quad(n\ge1).}
$$

The change of index is essential: $j_nf$ itself generally has degree $2n-2$, exceeding the permitted degree.

## 2

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) is the positive weighted average

$$
B_n(f,x)=\sum_{k=0}^n f(k/n)b_{n,k}(x),\qquad b_{n,k}(x)=\binom nkx^k(1-x)^{n-k}.
$$

For $0\le x\le1$, the [Bernstein basis](../../../functional-analysis.md#bernstein-basis) weights are nonnegative and the [binomial theorem](../../../combinatorics.md#binomial-theorem) gives $\sum_{k=0}^nb_{n,k}(x)=1$. Hence $|B_n(f,x)|\le\sum_k\|f\|_\infty b_{n,k}(x)=\|f\|_\infty$. In particular,

$$
\boxed{\|B_n(f)\|_\infty\le\|f\|_\infty.}
$$

This is the contraction property of the [positive linear operator on continuous functions](../../../topological-vector-space.md#positive-linear-operator-on-continuous-functions) defined by the [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [integer](../../../number-theory.md#integer) endpoint hypothesis is important. Let $r_{n,k}=\binom nk f(k/n)-\lfloor\binom nk f(k/n)\rfloor$. The [floor function](../../../calculus.md#floor-function) gives $0\le r_{n,k}<1$, while $r_{n,0}=r_{n,n}=0$ because $f(0)$ and $f(1)$ are [integers](../../../number-theory.md#integer). Therefore the [rounded Bernstein polynomial](../../../functional-analysis.md#rounded-bernstein-polynomial) satisfies

$$
0\le B_n(f,x)-B_n^*(f,x)\le S_n(x):=\sum_{k=1}^{n-1}x^k(1-x)^{n-k}.
$$

For $0\le x\le1/4$, the successive terms have ratio $x/(1-x)\le1/3$, so the [geometric series](../../../real-analysis.md#geometric-series) estimate gives

$$
S_n(x)\le\frac32x(1-x)^{n-1}\le\frac{3}{2n}.
$$

The last inequality follows by maximizing $x(1-x)^{n-1}$ at $x=1/n$. The same bound holds on $[3/4,1]$ by reflection. On $[1/4,3/4]$, each factor $x$ and $1-x$ is at most $3/4$, giving $S_n(x)\le(n-1)(3/4)^n$. Thus

$$
\boxed{\|B_n(f)-B_n^*(f)\|_\infty\le\max\left\{\frac{3}{2n},(n-1)(3/4)^n\right\}\longrightarrow0.}
$$

Here $n\ge2$; for $n=1$ the difference vanishes. Without the [integer](../../../number-theory.md#integer) endpoint hypothesis the claim would fail: at $x=0$ the error is $f(0)-\lfloor f(0)\rfloor$, independently of $n$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

First prove necessity. If [polynomials](../../../polynomial.md) with [integer](../../../number-theory.md#integer) [coefficients](../../../vector-space.md#coefficient) converge to $f$ in the [supremum norm](../../../functional-analysis.md#supremum-norm), their values at $0$ and $1$ are convergent sequences of [integers](../../../number-theory.md#integer). Each such sequence is eventually constant, since a convergent sequence is [Cauchy](../../../real-analysis.md#cauchy-sequence) and two distinct [integers](../../../number-theory.md#integer) are at distance at least one. Its limit is an [integer](../../../number-theory.md#integer). Thus $f(0),f(1)\in\mathbb Z$.

For sufficiency we also need [uniform convergence](../../../real-analysis.md#uniform-convergence) of the [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) to $f$. Here is a direct argument. For $X\sim\operatorname{Bin}(n,x)$, write $B_n(f,x)=\mathbb E f(X/n)$. The [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) has $\mathbb E(X/n)=x$ and $\operatorname{Var}(X/n)=x(1-x)/n\le1/(4n)$. For every $\delta>0$, [uniform continuity](../../../topological-analysis.md#uniform-continuity) of $f$ and the [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) give

$$
|B_n(f,x)-f(x)|\le\omega(f,\delta)+2\|f\|_\infty\mathbb P(|X/n-x|>\delta)
\le\omega(f,\delta)+\frac{\|f\|_\infty}{2n\delta^2}.
$$

First make $\delta$ small and then $n$ large; the bound is uniform in $x$. Hence $\|B_n(f)-f\|_\infty\to0$.

If the endpoints are [integers](../../../number-theory.md#integer), part (b) gives $\|B_n^*(f)-B_n(f)\|_\infty\to0$. Each coefficient multiplying $x^k(1-x)^{n-k}$ in $B_n^*$ is an [integer](../../../number-theory.md#integer). Expanding $(1-x)^{n-k}$ by the [binomial theorem](../../../combinatorics.md#binomial-theorem) therefore gives [integer](../../../number-theory.md#integer) [coefficients](../../../vector-space.md#coefficient) in the ordinary monomial [basis](../../../vector-space.md#basis). The [triangle inequality](../../../topological-analysis.md#triangle-inequality) proves $\|B_n^*(f)-f\|_\infty\to0$. Thus **the [integer](../../../number-theory.md#integer) endpoint condition is necessary and sufficient** for [integer-coefficient polynomial approximation](../../../uniform-approximation.md#integer-coefficient-polynomial-approximation).

## 3

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use real-valued [continuous functions](../../../calculus.md#continuous-function) and real [trigonometric polynomials](../../../fourier-series.md#trigonometric-polynomial). The [trigonometric Chebyshev alternation theorem](../../../uniform-approximation.md#trigonometric-chebyshev-alternation-theorem) says that $p\in\mathcal T_n$ is the unique [best uniform approximation](../../../uniform-approximation.md#best-uniform-approximation) to $f$ if and only if there are distinct points, ordered within one period,

$$
x_0<x_1<\cdots<x_{2n+1}<x_0+2\pi,
\qquad f(x_j)-p(x_j)=\varepsilon(-1)^j\|f-p\|_\infty,
\quad\varepsilon\in\{-1,1\}.
$$

Thus **the required number of alternating extrema is $2n+2$**. When the error is zero, the assertion is interpreted trivially and $p=f$ is unique. The count reflects $\dim\mathcal T_n=2n+1$ and the fact that a nonzero degree-$n$ [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) has at most $2n$ zeros in one period. In particular a strictly better candidate would force its difference from $p$ to have alternating signs at these points and hence at least $2n+2$ zeros, counting the closing interval around the circle. The [trigonometric Chebyshev alternation theorem](../../../uniform-approximation.md#trigonometric-chebyshev-alternation-theorem) also gives necessity and uniqueness.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) gives [uniform convergence](../../../real-analysis.md#uniform-convergence) and [continuity](../../../calculus.md#continuous-function) of the series. For the proposed [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial), set $q=5^{m+1}$ and $A=\sum_{k=m+1}^\infty a_k$. The tail satisfies

$$
r(x):=f(x)-t_n(x)=\sum_{k=m+1}^\infty a_k\cos(5^kx),\qquad \|r\|_\infty\le A.
$$

At $x_j=j\pi/q$, for $j=0,\ldots,2q-1$, the [integer](../../../number-theory.md#integer) $5^k/q$ is odd for every omitted frequency. Thus $\cos(5^kx_j)=(-1)^j$ and $r(x_j)=(-1)^jA$. In particular $\|r\|_\infty=A$.

Since $n<q$, these $2q$ points include at least $2n+2$ consecutive alternating extrema in a single period. Also $5^m\le n$, so $t_n\in\mathcal T_n$. The [trigonometric Chebyshev alternation theorem](../../../uniform-approximation.md#trigonometric-chebyshev-alternation-theorem) proves that **the proposed partial sum is the unique best approximant**, with

$$
\boxed{E_n(f)=\sum_{k=m+1}^\infty a_k\qquad(5^m\le n<5^{m+1}).}
$$

This is an instance of [positive lacunary trigonometric series](../../../uniform-approximation.md#positive-lacunary-trigonometric-series): all omitted odd frequency ratios align their extrema.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [geometric series](../../../real-analysis.md#geometric-series) formula and part (b) give

$$
E_n(f)=\sum_{k=m+1}^\infty3^{-k}=\frac12\,3^{-m},\qquad 5^m\le n<5^{m+1}.
$$

Put $\alpha=\log 3/\log 5$. Then $5^\alpha=3$, so $n^\alpha<3^{m+1}$ and

$$
\boxed{E_n(f)\le\frac{3}{2}n^{-\log 3/\log 5}.}
$$

This is the **largest possible decay exponent**: at $n=5^m$, an estimate with exponent $\beta>\alpha$ would require $\frac12\le c(3/5^\beta)^m$, whose right side tends to zero. Any smaller exponent also gives a valid weaker estimate. In fact $\frac12n^{-\alpha}\le E_n(f)<\frac32n^{-\alpha}$ for every $n\ge1$.

## 4

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the usual strictly increasing [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence), and initially assume $k\ge2$. The explicit formula for the order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) gives

$$
M_i(t)=k\sum_{j=i}^{i+k}\frac{(t_j-t)_+^{k-1}}{\prod_{\substack{\ell=i\\\ell\ne j}}^{i+k}(t_j-t_\ell)}.
$$

Each summand is a [truncated power function](../../../polynomial.md#truncated-power-function) in $t$, with its junction at $t_j$. It is a [piecewise polynomial function](../../../polynomial.md#piecewise-polynomial-function) of degree at most $k-1$ and has $k-2$ [continuous](../../../calculus.md#continuous-function) [derivatives](../../../calculus.md#derivative). Finite summation preserves these properties.

For $t\ge t_{i+k}$ all summands vanish. For $t\le t_i$, all [spline knot](../../../uniform-approximation.md#spline-knot) data come from the [polynomial](../../../polynomial.md) $u\mapsto(u-t)^{k-1}$. An order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) annihilates a [polynomial](../../../polynomial.md) of smaller degree, so $M_i(t)=0$ there too. Thus the [support](../../../function.md#support) is contained in $[t_i,t_{i+k}]$.

On the last open [spline knot](../../../uniform-approximation.md#spline-knot) interval only the $j=i+k$ term survives; it is a nonzero multiple of $(t_{i+k}-t)^{k-1}$. On the first open [spline knot](../../../uniform-approximation.md#spline-knot) interval, compare the truncated [spline knot](../../../uniform-approximation.md#spline-knot) data with the untruncated [polynomial](../../../polynomial.md) data: only the $j=i$ value differs. Since the untruncated [divided difference](../../../numerical-analysis.md#divided-difference) is zero, the result is a nonzero multiple of $(t_i-t)^{k-1}$. Consequently both outer pieces are nonzero, giving exact closed [support](../../../function.md#support). The [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) used below also proves positivity throughout the open [support](../../../function.md#support). Therefore

$$
\boxed{M_i\in C^{k-2}(\mathbb R),\qquad\operatorname{supp}M_i=[t_i,t_{i+k}],\qquad\deg\text{ each piece}\le k-1.}
$$

This is [simple-knot B-spline regularity](../../../uniform-approximation.md#simple-knot-b-spline-regularity). For $k=1$ the [B-splines](../../../uniform-approximation.md#b-spline) are interval indicators; they are piecewise constant and need not be [continuous](../../../calculus.md#continuous-function). The notation $C^{k-2}$ should then be read as no [continuity](../../../calculus.md#continuous-function) requirement, not as a classical negative-order differentiability space.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [divided difference](../../../numerical-analysis.md#divided-difference) is a finite linear combination of [spline knot](../../../uniform-approximation.md#spline-knot) values, so it commutes with the finite integral. For every [spline knot](../../../uniform-approximation.md#spline-knot) $t_j$ in the defining interval,

$$
\int_{t_i}^{t_{i+k}}(t_j-t)_+^{k-1}\,dt=\frac{(t_j-t_i)^k}{k}.
$$

It follows that

$$
\int_{t_i}^{t_{i+k}}M_i(t)\,dt=[t_i,\ldots,t_{i+k}](u-t_i)^k=1,
$$

because the order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) of a monic degree-$k$ [polynomial](../../../polynomial.md) is its leading coefficient. This proves the [unit-integral normalization of a B-spline](../../../uniform-approximation.md#unit-integral-normalization-of-a-b-spline).

For the [partition of unity](../../../differential-geometry.md#partition-of-unity), let $N_{i,r}$ denote the partition-normalized order-$r$ [B-spline](../../../uniform-approximation.md#b-spline). The [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) is

$$
N_{i,r}(t)=\frac{t-t_i}{t_{i+r-1}-t_i}N_{i,r-1}(t)+\frac{t_{i+r}-t}{t_{i+r}-t_{i+1}}N_{i+1,r-1}(t).
$$

It follows by substituting the explicit [divided difference](../../../numerical-analysis.md#divided-difference) formula into both sides and collecting each [truncated power function](../../../polynomial.md#truncated-power-function). The starting case is $N_{i,1}=\mathbf1_{[t_i,t_{i+1})}$, with endpoint conventions irrelevant when $r\ge2$. The two weights are nonnegative wherever their respective lower-order [B-splines](../../../uniform-approximation.md#b-spline) are nonzero. Induction therefore gives $N_{i,r}\ge0$ and strict positivity in its open [support](../../../function.md#support).

Extend the finite [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence) strictly in both directions, with no finite accumulation. At each point only finitely many [B-splines](../../../uniform-approximation.md#b-spline) are nonzero. For the full extended family the sum is one for order one. Summing the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula), the combined coefficient of $N_{j,r-1}$ is

$$
\frac{t-t_j}{t_{j+r-1}-t_j}+\frac{t_{j+r-1}-t}{t_{j+r-1}-t_j}=1.
$$

Induction gives a full [partition of unity](../../../differential-geometry.md#partition-of-unity) at every order. On $t_k<t<t_{n+1}$, all extended order-$k$ [functions](../../../function.md) with index $i\le0$ or $i\ge n+1$ vanish by their supports. Hence

$$
\boxed{\sum_{i=1}^nN_i(t)=1\quad(t_k<t<t_{n+1}),\qquad\int M_i=1.}
$$

The same argument gives the useful global [subpartition of unity for B-splines](../../../uniform-approximation.md#subpartition-of-unity-for-b-splines), $0\le\sum_{i=1}^nN_i(t)\le1$, including outside the basic [spline knot](../../../uniform-approximation.md#spline-knot) interval.

## 5

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) has range $\mathcal S$, not all of $C[0,1]$: the latter is an [infinite-dimensional vector space](../../../vector-space.md#infinite-dimensional-vector-space) whereas $\mathcal S$ is a [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space). For a concrete counterexample, $e^x$ cannot belong to any finite-degree piecewise polynomial space, since all its [derivatives](../../../calculus.md#derivative) are nonzero on every open interval. For $k\ge2$, the [B-splines](../../../uniform-approximation.md#b-spline) are [continuous](../../../calculus.md#continuous-function), so the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) is a map $C[0,1]\to\mathcal S\subset C[0,1]$. For order one it instead has a generally discontinuous piecewise constant range. For example, a single interval indicator on $[1/4,3/4)$ is the projection of the constant [function](../../../function.md) one onto its span, and is not [continuous](../../../calculus.md#continuous-function).

Write $s^*=\sum_ja_jN_j$. Since $M_i$ is a positive [scalar multiple](../../../vector-space.md#scalar-multiple) of $N_i$, the [operator normal equations](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) $\langle f-s^*,N_i\rangle=0$ are equivalent to

$$
Ga=b,\qquad b_i=\langle M_i,f\rangle.
$$

The [mixed-normalization spline Gram matrix](../../../uniform-approximation.md#mixed-normalization-spline-gram-matrix) is invertible: $G=DH$ where $D_{ii}=k/(t_{i+k}-t_i)>0$ and $H_{ij}=\langle N_i,N_j\rangle$ is the ordinary [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) of [inner products](../../../linear-algebra.md#inner-product) of a linearly independent [basis](../../../vector-space.md#basis). The positivity and [unit-integral normalization of a B-spline](../../../uniform-approximation.md#unit-integral-normalization-of-a-b-spline) give $|b_i|\le\|f\|_\infty$. The [subpartition of unity for B-splines](../../../uniform-approximation.md#subpartition-of-unity-for-b-splines) gives

$$
|s^*(t)|\le\|a\|_{\ell^\infty}\sum_jN_j(t)\le\|a\|_{\ell^\infty}.
$$

Here the [operator norm](../../../continuous-dual-space.md#operator-norm) of a [matrix](../../../vector-space.md#matrix) on $\ell^\infty$ is its maximum absolute row sum. Consequently,

$$
\|P_{\mathcal S}f\|_\infty\le\|a\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|b\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|f\|_\infty,
\qquad\boxed{\|P_{\mathcal S}\|_\infty\le\|G^{-1}\|_{\ell^\infty}.}
$$

This proves the [maximum-norm bound for spline projection](../../../uniform-approximation.md#maximum-norm-bound-for-spline-projection).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For $k=2$ on an equidistant [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence), $N_i$ is the triangular hat with value one at $t_{i+1}$ and [support](../../../function.md#support) $[t_i,t_{i+2}]$. Its slopes on the two pieces are $1/h$ and $-1/h$, and $M_i=N_i/h$. Direct integration gives

$$
\int N_i^2=2\int_0^h(u/h)^2\,du=\frac{2h}{3},\qquad
\int N_iN_{i+1}=\int_0^h(u/h)(1-u/h)\,du=\frac h6.
$$

Nonadjacent hats have disjoint interiors of their supports, so their [inner product](../../../linear-algebra.md#inner-product) vanishes. Dividing by $h$ therefore gives

$$
\boxed{g_{ij}=\begin{cases}2/3,&i=j,\\1/6,&|i-j|=1,\\0,&|i-j|\ge2.\end{cases}}
$$

This [linear-spline mixed Gram matrix](../../../uniform-approximation.md#linear-spline-mixed-gram-matrix) is [tridiagonal](../../../vector-space.md#tridiagonal-matrix). Every diagonal entry is $2/3$, including the first and last: the distinct-knot hats have their full supports inside $[0,1]$. End rows simply lack one off-diagonal neighbor; there are no repeated endpoint [spline knots](../../../uniform-approximation.md#spline-knot) here.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

A [strict diagonal dominance](../../../vector-space.md#strictly-diagonally-dominant-matrix) argument proves the estimate even on a nonuniform strictly increasing [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence). Put $h_i=t_{i+1}-t_i>0$. Then $N_i$ has a rising piece of length $h_i$ and a falling piece of length $h_{i+1}$, while $M_i=2N_i/(h_i+h_{i+1})$. The same integrations as in part (b) give the [linear-spline mixed Gram matrix](../../../uniform-approximation.md#linear-spline-mixed-gram-matrix)

$$
g_{ii}=\frac23,\qquad g_{i,i-1}=\frac{h_i}{3(h_i+h_{i+1})},\qquad
g_{i,i+1}=\frac{h_{i+1}}{3(h_i+h_{i+1})}.
$$

Only entries with indices in $1,\ldots,n$ are present. Thus $\sum_{j\ne i}|g_{ij}|\le1/3$ in every row.

For $Ga=b$, choose an index $i$ with $|a_i|=\|a\|_{\ell^\infty}$. The [reverse triangle inequality](../../../topological-analysis.md#reverse-triangle-inequality) then yields

$$
|b_i|\ge g_{ii}|a_i|-\sum_{j\ne i}|g_{ij}||a_j|
\ge\left(\frac23-\frac13\right)\|a\|_{\ell^\infty}.
$$

Hence $\|a\|_{\ell^\infty}\le3\|b\|_{\ell^\infty}$. Applying this to every $b$ proves

$$
\boxed{\|G^{-1}\|_{\ell^\infty}\le3,\qquad\|P_{\mathcal S}\|_\infty\le3\quad(k=2).}
$$

This is the [inverse infinity-norm bound from diagonal dominance](../../../vector-space.md#inverse-infinity-norm-bound-from-diagonal-dominance); no total positivity theorem is needed. The proof also gives invertibility directly by taking $b=0$.

## 6

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

An [orthonormal](../../../linear-algebra.md#orthonormal-set) [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis) consists of [closed subspaces of a Hilbert space](../../../hilbert-space.md#closed-subspace-of-a-hilbert-space) $(V_j)_{j\in\mathbb Z}$ of the [Hilbert space](../../../hilbert-space.md) $L^2(\mathbb R)$ such that

$$
V_j\subset V_{j+1},\qquad\overline{\bigcup_jV_j}=L^2(\mathbb R),\qquad\bigcap_jV_j=\{0\},\qquad
g\in V_j\ \Longleftrightarrow\ g(2\cdot)\in V_{j+1}.
$$

There is a [scaling function](../../../fourier-analysis.md#scaling-function) $\phi$ whose [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_0$. Consequently $\phi_{j,k}(x)=2^{j/2}\phi(2^jx-k)$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_j$; in particular $V_0$ is invariant under [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function).

Let $W_j=V_{j+1}\ominus V_j$ be the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of $V_j$ in $V_{j+1}$. Nesting, density and the trivial intersection imply the [orthogonal direct sum](../../../vector-space.md#orthogonal-direct-sum)

$$
L^2(\mathbb R)=\bigoplus_{j\in\mathbb Z}W_j.
$$

For example, telescoping $V_{J+1}=V_L\oplus\bigoplus_{j=L}^JW_j$ and letting $L\to-\infty$, $J\to\infty$ gives this decomposition; the corresponding [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) converge strongly to zero and the identity by the intersection and density properties.

To construct the [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet), use $\phi\in V_1$ to write the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) $\phi=\sum_na_n\phi(2\cdot-n)$, with $a\in\ell^2$ and $\sum_n|a_n|^2=2$. Put $m(t)=\frac12\sum_na_ne^{-int}$. The [orthonormal translates and Fourier periodization](../../../fourier-analysis.md#orthonormal-translates-and-fourier-periodization) criterion proved in part (b), applied to the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation), yields

$$
1=\sum_k|\widehat\phi(2t+2\pi k)|^2
=|m(t)|^2\sum_\ell|\widehat\phi(t+2\pi\ell)|^2+|m(t+\pi)|^2\sum_\ell|\widehat\phi(t+\pi+2\pi\ell)|^2
=|m(t)|^2+|m(t+\pi)|^2.
$$

This is the [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) identity. Define

$$
q(t)=-e^{-it}\overline{m(t+\pi)},\qquad b_n=(-1)^n\overline{a_{1-n}},\qquad
\psi(x)=\sum_nb_n\phi(2x-n).
$$

The [Fourier series](../../../fourier-series.md) of $q$ is $\frac12\sum_nb_ne^{-int}$, and $\widehat\psi(2t)=q(t)\widehat\phi(t)$. The two rows $(m(t),m(t+\pi))$ and $(q(t),q(t+\pi))$ form a unitary $2\times2$ [matrix](../../../vector-space.md#matrix) almost everywhere: both have squared [norm](../../../functional-analysis.md#norm) one and their [inner product](../../../linear-algebra.md#inner-product) is zero. This [wavelet completion of a multiresolution filter](../../../fourier-analysis.md#wavelet-completion-of-a-multiresolution-filter) proves not just orthogonality but completeness. Splitting a finer-scale coefficient [Fourier series](../../../fourier-series.md) into its values at $t$ and $t+\pi$, this invertible two-channel matrix resolves it into a coarse-scale channel and its complementary channel. Thus the [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) of $\psi$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $W_0$.

The dilated [functions](../../../function.md) $\psi_{j,k}(x)=2^{j/2}\psi(2^jx-k)$ therefore form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of each $W_j$. The [orthogonal direct sum](../../../vector-space.md#orthogonal-direct-sum) proves the conclusion: **every [orthonormal](../../../linear-algebra.md#orthonormal-set) multiresolution analysis produces an [orthonormal](../../../linear-algebra.md#orthonormal-set) wavelet [basis](../../../vector-space.md#basis)** $\{\psi_{j,k}:j,k\in\mathbb Z\}$ of $L^2(\mathbb R)$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/1">1</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/1/solution">Solution</h5>

↑ **Parent:** [1](#6/b/1)

Use the printed [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat\phi(t)=\int\phi(x)e^{-ixt}\,dx$, interpreted by the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) when $\phi$ is only square integrable. By the scaling and [function translation](../../../function.md#translation-of-a-function) rules,

$$
\widehat{\phi(2\cdot-n)}(t)=\frac12e^{-int/2}f(t/2).
$$

Taking the [Fourier transform](../../../analysis.md#fourier-transform) of the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) gives $f(t)=m(t/2)f(t/2)$, or equivalently

$$
\boxed{f(2t)=m(t)f(t),\qquad m(t)=\frac12\sum_na_ne^{-int}.}
$$

Conversely this identity, the same scaling rule and injectivity of the [Fourier transform](../../../analysis.md#fourier-transform) recover the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation).

For infinite filters, these statements are equalities in $L^2$, with [Fourier series](../../../fourier-series.md) understood in $L^2[0,2\pi]$. Under the accompanying [orthonormality](../../../linear-algebra.md#orthonormal-set) condition, $\{\sqrt2\phi(2\cdot-n)\}$ is an [orthonormal sequence](../../../hilbert-space.md#orthonormal-sequence), so the refinement series converges in $L^2$ precisely for $a\in\ell^2$. Moreover the condition in part (b)(2) makes multiplication by $f$ an [isometry](../../../riemannian-geometry.md#isometry) from periodic $L^2$ symbols into $L^2(\mathbb R)$:

$$
\int_{\mathbb R}|m(t)f(t)|^2\,dt=\int_0^{2\pi}|m(t)|^2\sum_k|f(t+2\pi k)|^2\,dt=\int_0^{2\pi}|m(t)|^2\,dt.
$$

Applying this to finite filter truncations justifies passage to the limit in both directions. Thus the two paired assertions have a rigorous equivalent interpretation without requiring absolute integrability of $\phi$.

<h4 id="6/b/2">2</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/2/solution">Solution</h5>

↑ **Parent:** [2](#6/b/2)

Let $F(t)=\sum_{k\in\mathbb Z}|f(t+2\pi k)|^2$. By the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem), $F$ is integrable on $[0,2\pi]$, since its integral is $\int_{\mathbb R}|f|^2<\infty$. The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) and periodization give

$$
\langle\phi(\cdot-n),\phi(\cdot-m)\rangle
=\frac1{2\pi}\int_{\mathbb R}|f(t)|^2e^{i(m-n)t}\,dt
=\frac1{2\pi}\int_0^{2\pi}F(t)e^{i(m-n)t}\,dt.
$$

Consequently, if $F=1$ almost everywhere these [inner products](../../../linear-algebra.md#inner-product) are $\delta_{mn}$, proving [orthonormality](../../../linear-algebra.md#orthonormal-set). Conversely [orthonormality](../../../linear-algebra.md#orthonormal-set) says that every [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) of $F-1$ is zero. The [uniqueness of Fourier coefficients in L1](../../../fourier-series.md#uniqueness-of-fourier-coefficients-in-l1) implies $F-1=0$ almost everywhere. Hence

$$
\boxed{\{\phi(\cdot-n)\}_{n\in\mathbb Z}\text{ is orthonormal}\quad\Longleftrightarrow\quad\sum_k|f(t+2\pi k)|^2=1\text{ a.e.}}
$$

This proves [orthonormal translates and Fourier periodization](../../../fourier-analysis.md#orthonormal-translates-and-fourier-periodization), including both directions and the normalization constant associated with the printed [Fourier transform](../../../analysis.md#fourier-transform).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The half-open translates $[-\pi,\pi)+2\pi k$ partition the real line. Exactly one summand is therefore nonzero in the periodization of $|f|^2$, giving $\sum_k|f(t+2\pi k)|^2=1$.

Choose the [Shannon scaling mask](../../../fourier-analysis.md#shannon-scaling-mask) to be the $2\pi$-periodic extension of $\mathbf1_{[-\pi/2,\pi/2)}$. On the [support](../../../function.md#support) of $f$, its product with $f$ is $\mathbf1_{[-\pi/2,\pi/2)}(t)=f(2t)$; outside that [support](../../../function.md#support) both sides vanish. Thus the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) holds in frequency. The [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) give its precise filter normalization:

$$
a_n=\frac1\pi\int_{-\pi/2}^{\pi/2}e^{int}\,dt
=\begin{cases}1,&n=0,\\\dfrac{2\sin(n\pi/2)}{\pi n},&n\ne0.\end{cases}
$$

These [coefficients](../../../vector-space.md#coefficient) are square summable, so the interpretation in part (b) applies.

The [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) gives the [Shannon scaling function](../../../fourier-analysis.md#shannon-scaling-function)

$$
\phi(x)=\frac1{2\pi}\int_{-\pi}^{\pi}e^{ixt}\,dt,
\qquad\boxed{\phi(x)=\frac{\sin(\pi x)}{\pi x}\ (x\ne0),\qquad\phi(0)=1.}
$$

This is the normalized [sinc function](../../../analysis.md#sinc-function). Its [Fourier transform](../../../analysis.md#fourier-transform) is taken in the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) sense: the [Shannon scaling function](../../../fourier-analysis.md#shannon-scaling-function) belongs to $L^2$ but not $L^1$, so its Fourier integral is not absolutely convergent. The inverse integral above is an ordinary integral because the rectangular transform belongs to $L^1$. The resulting refinement spaces are exactly the $L^2$ [functions](../../../function.md) with [Fourier transform](../../../analysis.md#fourier-transform) supported in $[-2^j\pi,2^j\pi]$; their union is [dense](../../../topology.md#dense-set) and their intersection is zero. Thus this example also gives a full [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
