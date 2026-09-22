# Paper 124

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_124.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_124.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [additive arithmetic function](../../../number-theory.md#additive-function-number-theory) satisfies $f(mn)=f(m)+f(n)$ for [coprime integers](../../../number-theory.md#coprime-integers) $m,n$; a [completely additive arithmetic function](../../../number-theory.md#completely-additive-arithmetic-function) satisfies this for all positive $m,n$. In either case $f(1)=0$. The [Fundamental theorem of arithmetic](../../../number-theory.md#fundamental-theorem-of-arithmetic) gives $f(n)=\sum_{p^k\parallel n}f(p^k)$, where $p^k\parallel n$ means that the [prime valuation](../../../number-theory.md#prime-valuation) of $n$ at $p$ is exactly $k$.

Under the [discrete uniform distribution](../../../discrete-probability-distribution.md#discrete-uniform-distribution) on $[N]$, the [expectation](../../../probability-theory.md#expected-value) of the [indicator function](../../../measure-theory.md#indicator-function) of $p^k\parallel n$ is

$$
\frac1N\left(\left\lfloor\frac N{p^k}\right\rfloor-\left\lfloor\frac N{p^{k+1}}\right\rfloor\right)=\frac1{p^k}\left(1-\frac1p\right)+O(N^{-1}).
$$

The formula remains valid when $p^{k+1}>N$. Applying [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) to the finite [prime power](../../../number-theory.md#prime-power) decomposition proves **the required mean formula**:

$$
\boxed{\mathbb E_N f=\sum_{p^k\le N}\frac{f(p^k)}{p^k}\left(1-\frac1p\right)+O\left(\frac1N\sum_{p^k\le N}|f(p^k)|\right).}
$$

For the last assertion, write the [excess prime-factor multiplicity](../../../number-theory.md#excess-prime-factor-multiplicity) directly as a sum of nonnegative [indicator functions](../../../measure-theory.md#indicator-function):

$$
\Omega(n)-\omega(n)=\sum_p\sum_{k\ge2}\mathbf1_{p^k\mid n}.
$$

Here $\omega$ is the [prime omega function](../../../number-theory.md#prime-omega-function) and $\Omega$ is the [total number of prime factors](../../../number-theory.md#total-number-of-prime-factors). The [expectation](../../../probability-theory.md#expected-value) is bounded independently of $N$, since

$$
\mathbb E_N(\Omega-\omega)\le\sum_p\sum_{k\ge2}\frac1{p^k}=\sum_p\frac1{p(p-1)}\le\sum_{m=2}^\infty\frac1{m(m-1)}=1.
$$

Thus [Markov inequality](../../../probability-inequality.md#markov-inequality) gives **vanishing probability on every diverging scale**:

$$
\boxed{\mathbb P_N(\Omega-\omega\ge t(N))\le\frac1{t(N)}\longrightarrow0.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Möbius function](../../../number-theory.md#mobius-function) has $\mu(1)=1$, $\mu(n)=0$ when $n$ is divisible by a [prime](../../../number-theory.md#prime-number) square, and $\mu(n)=(-1)^r$ when $n$ is a product of $r$ distinct [primes](../../../number-theory.md#prime-number). The [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) is initially the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) $\zeta(s)=\sum_{n\ge1}n^{-s}$ for $\sigma=\Re s>1$. Both this [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) and $\sum\mu(n)n^{-s}$ have [absolute convergence](../../../real-analysis.md#absolute-convergence), because $|\mu(n)|\le1$ and $\sum n^{-\sigma}<\infty$.

For a finite set of [primes](../../../number-theory.md#prime-number) $p\le y$, multiplication of absolutely convergent [geometric series](../../../real-analysis.md#geometric-series) and [unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) give

$$
\prod_{p\le y}(1-p^{-s})^{-1}=\sum_{\substack{n\ge1\\p\mid n\Rightarrow p\le y}}n^{-s}.
$$

Every omitted integer has a [prime factor](../../../number-theory.md#prime-factor) exceeding $y$, so it exceeds $y$. The difference from $\zeta(s)$ has absolute value at most $\sum_{n>y}n^{-\sigma}\to0$. This proves the [Euler product](../../../analytic-number-theory.md#euler-product), with the product interpreted as the limit of its finite products:

$$
\boxed{\zeta(s)=\prod_p(1-p^{-s})^{-1}\qquad(\Re s>1).}
$$

For the reciprocal identity, [absolute convergence](../../../real-analysis.md#absolute-convergence) justifies multiplying and regrouping the two [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) by their product index. Their [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution) coefficient at $m$ is

$$
\sum_{d\mid m}\mu(d)=\begin{cases}1,&m=1,\\(1-1)^r=0,&m>1\text{ with }r\text{ distinct prime factors}.
\end{cases}
$$

The coefficient calculation uses only the [squarefree integers](../../../number-theory.md#squarefree-integer) dividing $m$. Consequently **the reciprocal identity is an identity of absolutely convergent series**:

$$
\boxed{\zeta(s)\sum_{n=1}^{\infty}\frac{\mu(n)}{n^s}=1\qquad(\Re s>1).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $M(x)=\sum_{n\le x}\mu(n)$ be the [Mertens function](../../../number-theory.md#mertens-function). [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\sum_{n\le X}\frac{\mu(n)}{n^s}=M(X)X^{-s}+s\int_1^X M(x)x^{-s-1}\,dx.
$$

For any $\Re s>0.9$, choose a sufficiently small $\epsilon>0$ with $0.9+\epsilon<\Re s$. The assumed bound makes the boundary term tend to zero and makes the integral absolutely convergent. Moreover, on each [compact set](../../../topology.md#compact-space) of this half-plane, one can choose the same $\epsilon$, so the integral has [locally uniform convergence](../../../real-analysis.md#locally-uniform-convergence). Hence

$$
F(s)=s\int_1^\infty M(x)x^{-s-1}\,dx
$$

is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) on $\Re s>0.9$, agreeing with the reciprocal [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) from part (b) on $\Re s>1$.

The [identity theorem](../../../complex-analysis.md#identity-theorem) applied to the [holomorphic functions](../../../complex-analysis.md#holomorphic-function) $(s-1)\zeta(s)F(s)$ and $s-1$ extends their equality throughout $\Re s>0.9$; the assumed simple [pole](../../../isolated-singularity.md#pole) makes the first function holomorphic at $1$. Thus $\zeta(s)F(s)=1$ away from $1$, proving **a zero-free half-plane**:

$$
\boxed{\zeta(s)\ne0\quad\text{if }\Re s>0.9,\ s\ne1.}
$$

To obtain the strongest symmetric conclusion, use the following basic facts explicitly: the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) gives the [entire function](../../../complex-analysis.md#entire-function) $\xi(s)=\tfrac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)$ with $\xi(s)=\xi(1-s)$, and the [trivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#trivial-zero-of-the-riemann-zeta-function) are the negative even integers. Every [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) is therefore accompanied by its reflection $1-s$. A [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) with real part below $0.1$ would reflect to one above $0.9$, which is impossible. Consequently **all nontrivial zeros lie in the closed strip**

$$
\boxed{0.1\le\Re\rho\le0.9.}
$$

The $\epsilon$ in the hypothesis prevents this argument from excluding either boundary line; the [trivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#trivial-zero-of-the-riemann-zeta-function) remain present.

## 2

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The event that infinitely many $A_n$ occur is $\limsup_n A_n=\bigcap_{m\ge1}\bigcup_{n\ge m}A_n$. For every $m$, the [union bound](../../../probability-inequality.md#boole-s-inequality) and monotonicity of a [probability measure](../../../probability-theory.md#probability-measure) give

$$
0\le\mathbb P(\limsup_n A_n)\le\mathbb P\left(\bigcup_{n\ge m}A_n\right)\le\sum_{n\ge m}\mathbb P(A_n).
$$

The right-hand side tends to zero as the tail of a convergent series. Therefore **the first Borel-Cantelli conclusion** is

$$
\boxed{\mathbb P(\limsup_n A_n)=0.}
$$

This proves the [Borel-Cantelli first lemma](../../../probability-theory.md#borel-cantelli-first-lemma) without any [independence](../../../random-variable.md#independent-random-variables) assumption.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

First, the [Cramér model](../../../analytic-number-theory.md#cramer-model) has infinitely many successes [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), so every $P_n$ is finite. Indeed, for each fixed $K\ge3$, [independence](../../../random-variable.md#independent-random-variables) of the [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) gives

$$
\mathbb P(U_j=0\text{ for all }K\le j\le M)=\prod_{j=K}^M\left(1-\frac1{\log j}\right)\le\exp\left(-\sum_{j=K}^M\frac1{\log j}\right)\longrightarrow0.
$$

The sum diverges, for example because $1/\log j\ge1/j$ for $j\ge3$. [Continuity from above of a measure](../../../measure-theory.md#continuity-from-above-of-a-measure) and a countable [union bound](../../../probability-inequality.md#boole-s-inequality) exclude a final success.

Fix $\epsilon>0$ and put $L_k=\lceil(1+\epsilon)(\log k)^2\rceil$. Let $A_k$ be the event that the whole interval $k+1,\ldots,k+L_k$ consists of failures. By [independence](../../../random-variable.md#independent-random-variables) and $1-v\le e^{-v}$,

$$
\mathbb P(A_k)\le\exp\left(-\sum_{j=k+1}^{k+L_k}\frac1{\log j}\right)\le\exp\left(-\frac{L_k}{\log(k+L_k)}\right).
$$

Since $L_k=o(k)$, the exponent divided by $\log k$ tends to $-(1+\epsilon)$. Thus $\mathbb P(A_k)\le k^{-1-\epsilon/2}$ for all sufficiently large $k$. The [Borel-Cantelli first lemma](../../../probability-theory.md#borel-cantelli-first-lemma) shows that [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) every sufficiently large such interval contains a success. Taking $k=P_n$ then gives $P_{n+1}-P_n\le L_{P_n}$ for all sufficiently large $n$.

For each fixed $\epsilon$, the [limit superior](../../../real-analysis.md#limit-superior) of the normalized gap is therefore at most $1+\epsilon$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Intersect the probability-one events for $\epsilon=1/r$, $r\in\mathbb N$, to obtain **the [Cramér model prime-gap upper bound](../../../analytic-number-theory.md#cramer-model-prime-gap-upper-bound)**:

$$
\boxed{\mathbb P\left(\limsup_{n\to\infty}\frac{P_{n+1}-P_n}{(\log P_n)^2}\le1\right)=1.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk), [independence](../../../random-variable.md#independent-random-variables) and the [Rademacher distribution](../../../probability-theory.md#rademacher-distribution) give the [moment-generating function](../../../probability-theory.md#moment-generating-function)

$$
\mathbb E e^{\theta S_n}=\prod_{i=1}^n\mathbb E e^{\theta X_i}=\left(\frac{e^\theta+e^{-\theta}}2\right)^n=(\cosh\theta)^n.
$$

The function $\theta^2/2-\log\cosh\theta$ is even; for $\theta\ge0$ its derivative is $\theta-\tanh\theta\ge0$, since the derivative of $\tanh\theta$ is at most one and $\tanh0=0$. Here $\cosh$ and $\tanh$ are the [hyperbolic cosine](../../../calculus.md#hyperbolic-cosine) and [hyperbolic tangent](../../../calculus.md#hyperbolic-tangent). Hence **the exponential-moment estimate** is

$$
\boxed{\mathbb E e^{\theta S_n}\le e^{n\theta^2/2}\quad(\theta\in\mathbb R).}
$$

The supplied [exponential maximal bound for a symmetric random walk](../../../probability-theory.md#exponential-maximal-bound-for-a-symmetric-random-walk) now gives $\mathbb P(\max_{k\le n}S_k\ge t\sqrt n)\le\exp(-\theta t\sqrt n+n\theta^2/2)$. For $t>0$, choose $\theta=t/\sqrt n$; for $t=0$, use the elementary bound by one. Thus

$$
\boxed{\mathbb P(\max_{k\le n}S_k\ge t\sqrt n)\le e^{-t^2/2}\quad(t\ge0).}
$$

Fix $a>1$, choose $0<\delta<a^2-1$, and set $n_m=\lfloor(1+\delta)^m\rfloor$. For large $m$ these form an increasing sequence. Apply the preceding [exponential maximal bound for a symmetric random walk](../../../probability-theory.md#exponential-maximal-bound-for-a-symmetric-random-walk) at $n_{m+1}$ with threshold $a\sqrt{2n_m\log\log n_m}$. The resulting probability is at most

$$
\exp\left(-a^2\frac{n_m}{n_{m+1}}\log\log n_m\right).
$$

We have $n_m/n_{m+1}\to(1+\delta)^{-1}$ and $\log\log n_m=\log m+O(1)$. Choose $b$ strictly between $1$ and $a^2/(1+\delta)$; the displayed probabilities are $O(m^{-b})$. By the [Borel-Cantelli first lemma](../../../probability-theory.md#borel-cantelli-first-lemma), [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), eventually $\max_{k\le n_{m+1}}S_k<a\sqrt{2n_m\log\log n_m}$. For every $n_m\le n\le n_{m+1}$, monotonicity of $n\log\log n$ for large $n$ therefore gives

$$
\frac{S_n}{\sqrt{2n\log\log n}}\le a.
$$

Intersect the probability-one events for $a=1+1/r$ to obtain **the [upper law of the iterated logarithm](../../../convergence-of-random-variables.md#upper-law-of-the-iterated-logarithm)**:

$$
\boxed{\mathbb P\left(\limsup_{n\to\infty}\frac{S_n}{\sqrt{2n\log\log n}}\le1\right)=1.}
$$

## 3

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the convention that a [z-sieved number](../../../analytic-number-theory.md#rough-number) is a positive integer with no [prime factor](../../../number-theory.md#prime-factor) strictly below $z$; $1$ is included. Such integers are also called [rough numbers](../../../analytic-number-theory.md#rough-number). Using instead exclusion of [primes](../../../number-theory.md#prime-number) at most $z$ changes an endpoint convention, not the following fixed-$u$ asymptotic.

The [Buchstab function](../../../analytic-number-theory.md#buchstab-function) is the [continuous function](../../../calculus.md#continuous-function) $w:[1,\infty)\to\mathbb R$ determined by

$$
\boxed{w(u)=\frac1u\quad(1\le u\le2),\qquad\frac{d}{du}(u w(u))=w(u-1)\quad(u>2).}
$$

Successive integration over intervals of length one determines the [Buchstab function](../../../analytic-number-theory.md#buchstab-function) uniquely from its initial values.

A standard fixed-$u$ form of [Buchstab theorem](../../../analytic-number-theory.md#buchstab-theorem) states that, for each fixed $u>1$, as $z\to\infty$,

$$
\boxed{\Phi(z^u,z)\sim\frac{z^u}{\log z}\,w(u).}
$$

For $1<u\le2$, this agrees with the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem), since apart from an immaterial endpoint the [z-sieved numbers](../../../analytic-number-theory.md#rough-number) in this range are $1$ and the [primes](../../../number-theory.md#prime-number) from $z$ to $z^u$. The restriction $u>1$ matters: at $u=1$ the count is bounded, so the displayed asymptotic does not hold there.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $c=e^{-\gamma}$, where $\gamma$ is the [Euler--Mascheroni constant](../../../complex-analysis.md#euler-s-constant), and let $f(u)=w(u)-c$. The [Buchstab function](../../../analytic-number-theory.md#buchstab-function) equation becomes

$$
\frac{d}{du}(u f(u))=f(u-1)\qquad(u>2).
$$

The given [Gamma function](../../../complex-analysis.md#gamma-function) bound implies $u f(u)\to0$. Indeed,

$$
\Gamma(u+1)=\int_0^\infty e^{-x}x^u\,dx\ge\int_u^{u+1}e^{-x}x^u\,dx\ge e^{-u-1}u^u,
$$

so $u/\Gamma(u+1)\to0$.

Suppose first that $f\ge0$ throughout an interval $[u,u+1]$, with $u\ge1$. The [delay differential equation](../../../differential-equation.md#delay-differential-equation) and integration successively on $[u+1,u+2]$, $[u+2,u+3]$, and so on propagate nonnegativity to the entire tail $[u,\infty)$. In particular, $v f(v)$ is nonnegative and nondecreasing for $v\ge u+1$. Its limit is zero, so it is identically zero there. Thus $f=0$ on that tail.

The [delay differential equation](../../../differential-equation.md#delay-differential-equation) then propagates this equality backwards: if $f=0$ for $v\ge a$, then $f(v-1)=0$ for $v>\max(a,2)$. Repeating finitely many times would give $f=0$ on $(1,2)$, contradicting $f(v)=1/v-c$ there. Hence every interval $[u,u+1]$ contains a point where $f<0$.

If instead $f\le0$ on $[u,u+1]$, the same propagation makes $v f(v)$ nonpositive and nonincreasing on the tail. Its limit zero again forces it to vanish, giving the same contradiction. Thus every such interval also contains a point where $f>0$. **The oscillation of the Buchstab function is therefore strict on every unit interval**:

$$
\boxed{\exists u^+,u^-\in[u,u+1]:\quad w(u^+)>e^{-\gamma},\quad w(u^-)<e^{-\gamma}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For an [additive arithmetic function](../../../number-theory.md#additive-function-number-theory) $f$, one standard form of the [Turán-Kubilius inequality](../../../analytic-number-theory.md#turan-kubilius-inequality) uses

$$
A_f(N)=\sum_{p^k\le N}\frac{f(p^k)}{p^k}\left(1-\frac1p\right),\qquad B_f(N)^2=\sum_{p^k\le N}\frac{|f(p^k)|^2}{p^k}.
$$

It states, with an absolute constant,

$$
\frac1N\sum_{n\le N}|f(n)-A_f(N)|^2\ll B_f(N)^2.
$$

For real $f$, this also bounds the [variance](../../../variance.md) under the [discrete uniform distribution](../../../discrete-probability-distribution.md#discrete-uniform-distribution), because centering at the actual [expectation](../../../probability-theory.md#expected-value) minimizes the mean square.

For the [prime omega function](../../../number-theory.md#prime-omega-function), $f(p^k)=1$. The [Mertens theorem for reciprocal primes](../../../analytic-number-theory.md#mertens-second-theorem) states $\sum_{p\le N}1/p=\log\log N+O(1)$. The contribution of higher [prime powers](../../../number-theory.md#prime-power) is bounded by $\sum_p1/(p(p-1))\le1$, as proved in 1(a). It follows that $A_\omega(N)=\log\log N+O(1)$ and $B_\omega(N)^2\ll\log\log N$. Writing $L=\log\log N$, the [Turán-Kubilius inequality](../../../analytic-number-theory.md#turan-kubilius-inequality) and [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) therefore yield

$$
\boxed{\mathbb P_N(|\omega-L|\ge0.01L)\ll L^{-1}.}
$$

The bounded error in $A_\omega-L$ is absorbed by, for example, using the threshold $0.005L$ around $A_\omega$ for sufficiently large $N$.

For the [multiplication table problem](../../../analytic-number-theory.md#multiplication-table-problem), call a pair $(a,b)\in[N]^2$ good when $\omega(a),\omega(b)\ge0.99L$ and $\omega(\gcd(a,b))\le0.1L$. The preceding [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) excludes only $O(N^2/L)$ pairs by either of the first two conditions. For the [greatest common divisor](../../../number-theory.md#greatest-common-divisor) condition, [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) under uniform sampling of the two coordinates gives

$$
\frac1{N^2}\sum_{a,b\le N}\omega(\gcd(a,b))=\sum_{p\le N}\left(\frac{\lfloor N/p\rfloor}{N}\right)^2\le\sum_{m=2}^\infty\frac1{m^2}<\infty.
$$

[Markov inequality](../../../probability-inequality.md#markov-inequality) therefore excludes only another $O(N^2/L)$ pairs.

The [prime factors](../../../number-theory.md#prime-factor) of a product form the union of those of its factors. Consequently, for every good pair,

$$
\omega(ab)=\omega(a)+\omega(b)-\omega(\gcd(a,b))\ge1.88L.
$$

On the other hand, apply the proved concentration estimate at $N^2$. Since $\log\log(N^2)=L+\log2$, for large $N$ every integer $m\le N^2$ with $\omega(m)\ge1.88L$ is exceptional there. There are only $O(N^2/L)$ such integers. Products of good pairs lie in this exceptional set; products having only bad representations are at most as numerous as the bad pairs. This proves **the multiplication-table upper bound, using distinct prime factors alone**:

$$
\boxed{\#\{ab:1\le a,b\le N\}\ll\frac{N^2}{\log\log N}=o(N^2).}
$$

## 4

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Expand the two [Dirichlet polynomials](../../../analytic-number-theory.md#dirichlet-polynomial), keeping the [complex conjugate](../../../complex-analysis.md#complex-conjugate) on $B$. The diagonal $m=n$ contributes exactly $T\sum_{n\le X}a_n\overline{b_n}/n^{2\sigma}$. If $m\ne n$, the exponential integral is

$$
\int_T^{2T}e^{it\log(m/n)}\,dt=\frac{e^{2iT\log(m/n)}-e^{iT\log(m/n)}}{i\log(m/n)},
$$

whose absolute value is at most $2/|\log(m/n)|$. Thus **the mean-value formula** is

$$
\boxed{\int_T^{2T}A(\sigma+it)\overline{B(\sigma+it)}\,dt=T\sum_{n\le X}\frac{a_n\overline{b_n}}{n^{2\sigma}}+O\left(\sum_{\substack{m,n\le X\\m\ne n}}\frac{|a_n||b_m|}{n^\sigma m^\sigma|\log(m/n)|}\right).}
$$

This also covers $T=0$.

For $m>n$, integration of $1/x$ over $[n,m]$ gives $\log(m/n)\ge(m-n)/m$; the analogous inequality holds with $m,n$ exchanged. Hence $|\log(m/n)|^{-1}\le\max(m,n)/|m-n|\le X$. This gives the requested first bound $O\bigl(X\sum_{m\ne n}|a_n||b_m|/(n^\sigma m^\sigma)\bigr)$.

For the weighted bound, put $\alpha_n=|a_n|n^{-\sigma}$ and $\beta_m=|b_m|m^{-\sigma}$. The inequality

$$
2\alpha_n\beta_m\le\frac nm\alpha_n^2+\frac mn\beta_m^2
$$

reduces the estimate to a row sum and its symmetric counterpart. For a fixed $n$, the preceding logarithm bounds give

$$
\sum_{\substack{m\le X\\m\ne n}}\frac{n/m}{|\log(m/n)|}\le\sum_{m>n}\frac n{m-n}+\sum_{m<n}\frac{n^2}{m(n-m)}\ll n\log(2X).
$$

Here $n^2/(m(n-m))=n(1/m+1/(n-m))$, and each resulting [harmonic sum](../../../real-analysis.md#harmonic-sum) is $O(\log(2X))$. The symmetric row sum is bounded by $O(m\log(2X))$. Therefore **the second error bound** is

$$
\boxed{O\left(\sum_{n\le X}\frac{|a_n|^2n\log(2X)}{n^{2\sigma}}+\sum_{m\le X}\frac{|b_m|^2m\log(2X)}{m^{2\sigma}}\right).}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $D(s)=\sum_{p\le X}p^{-s}$, a [Dirichlet polynomial](../../../analytic-number-theory.md#dirichlet-polynomial) supported on [primes](../../../number-theory.md#prime-number). The cosine sum is $(D(\sigma+it)+\overline{D(\sigma+it)})/2$, so its $j$th power is a finite linear combination of $D(\sigma+it)^k\overline{D(\sigma+it)^{j-k}}$, $0\le k\le j$.

The [Dirichlet polynomial](../../../analytic-number-theory.md#dirichlet-polynomial) $D(s)^k$ is supported on integers that are products of exactly $k$ [primes](../../../number-theory.md#prime-number), counted with multiplicity. Each coefficient is at most $k!$ by [unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic); for $k=0$ the only coefficient is the one at $1$. As $j$ is odd, $k\ne j-k$, so no integer can appear in both supports. Thus **every diagonal term vanishes** in the [mean value of Dirichlet polynomials](../../../analytic-number-theory.md#mean-value-of-dirichlet-polynomials) from part (a).

Both supports lie in $[1,X^j]$. The first error bound in part (a), with that common length, now gives for each term

$$
\left|\int_T^{2T}D(\sigma+it)^k\overline{D(\sigma+it)^{j-k}}\,dt\right|\ll_j X^j\left(\sum_{n\le X^j}n^{-\sigma}\right)^2.
$$

Summing the finitely many terms proves **the [odd moment of a prime cosine sum](../../../analytic-number-theory.md#odd-moment-of-a-prime-cosine-sum) estimate**:

$$
\boxed{\left|\int_T^{2T}\left(\sum_{p\le X}\frac{\cos(t\log p)}{p^\sigma}\right)^j\,dt\right|\ll_j X^j\left(\sum_{n\le X^j}\frac1{n^\sigma}\right)^2.}
$$

The argument holds for all real $\sigma$ and all $T\ge0$; no cancellation estimate involving $T$ is needed once the diagonal is absent.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $P(t)=\sum_{n\le\sqrt{t/(2\pi)}}n^{-1/2-it}$. The given bound for the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function), together with $(a+b)^4\le8(a^4+b^4)$ for $a,b\ge0$, gives

$$
\int_1^T|\zeta(1/2+it)|^4\,dt\ll\int_1^T|P(t)|^4\,dt+\log T.
$$

The integral over $[0,1]$ is bounded, since the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) has no [pole](../../../isolated-singularity.md#pole) on this compact segment. It remains to estimate the [fourth moment of the Riemann zeta function](../../../analytic-number-theory.md#fourth-moment-of-the-riemann-zeta-function) through this moving [Dirichlet polynomial](../../../analytic-number-theory.md#dirichlet-polynomial) cutoff.

Let $L=\lfloor\sqrt{T/(2\pi)}\rfloor$ and $Y=L^2$. In the expansion of $|P(t)|^4$, a quadruple $n_1,n_2,n_3,n_4\le L$ occurs precisely for

$$
t\ge t_0=\max\bigl(1,2\pi n_1^2,2\pi n_2^2,2\pi n_3^2,2\pi n_4^2\bigr).
$$

Its oscillatory factor is $e^{it\log(n_3n_4/(n_1n_2))}$, and its weight is $(n_1n_2n_3n_4)^{-1/2}$. When $n_1n_2=n_3n_4$, its integral has length at most $T$. When these products differ, its integral over $[t_0,T]$ has absolute value at most $2/|\log(n_3n_4/(n_1n_2))|$. Thus the moving cutoff affects the lower endpoint but preserves the off-diagonal bound from part (a).

Write $r_L(m)=\#\{(a,b):a,b\le L,\ ab=m\}$. The [divisor function](../../../number-theory.md#divisor-function) $d(m)$ bounds $r_L(m)$. Grouping the off-diagonal majorant by the two products and using the weighted row-sum argument in part (a), with coefficient $r_L(m)$ and $\sigma=1/2$, bounds it by

$$
O\left(\log(2Y)\sum_{m\le Y}r_L(m)^2\right)\ll\log(2Y)\sum_{m\le Y}d(m)^2\ll Y\log^4(2Y)\ll T(\log T)^4.
$$

This uses only the given [divisor-square summatory bound](../../../number-theory.md#divisor-square-summatory-bound). For bounded $T$, the desired conclusions follow by boundedness on compact segments, so these estimates may be read for large $T$ with $Y\ge2$. We have proved **the requested diagonal-plus-error estimate**:

$$
\boxed{\int_0^T|\zeta(1/2+it)|^4\,dt\ll T\sum_{\substack{n_1,n_2,n_3,n_4\le\sqrt{T/(2\pi)}\\n_1n_2=n_3n_4}}\frac1{\sqrt{n_1n_2n_3n_4}}+T(\log T)^4.}
$$

The diagonal sum equals $\sum_{m\le Y}r_L(m)^2/m\le\sum_{m\le Y}d(m)^2/m$. If $D(x)=\sum_{m\le x}d(m)^2\ll x\log^3(2x)$, then [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\sum_{m\le Y}\frac{d(m)^2}{m}=\frac{D(Y)}Y+\int_1^Y\frac{D(x)}{x^2}\,dx\ll\log^4(2Y).
$$

Consequently **the full fourth-moment bound** is

$$
\boxed{\int_0^T|\zeta(1/2+it)|^4\,dt\ll T(\log T)^4\qquad(T\ge2).}
$$

## 5

↑ **Parent:** [Paper 124](paper-124.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

One general form of the [Erdős-Kac theorem](../../../analytic-number-theory.md#erdos-kac-theorem) is the following. Let $f$ be a real [strongly additive arithmetic function](../../../number-theory.md#strongly-additive-arithmetic-function), with $|f(p)|\le C$ for all [primes](../../../number-theory.md#prime-number), and define

$$
A(x)=\sum_{p\le x}\frac{f(p)}p,\qquad B(x)^2=\sum_{p\le x}\frac{f(p)^2}p.
$$

If $B(x)\to\infty$, then under the [discrete uniform distribution](../../../discrete-probability-distribution.md#discrete-uniform-distribution) on $[N]$,

$$
\boxed{\frac{f(n)-A(N)}{B(N)}\ \xrightarrow{\mathrm d}\ \mathcal N(0,1).}
$$

Here the arrow denotes [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) and $\mathcal N(0,1)$ is the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). Equivalently, the probability of being at most $z$ tends to the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function) $\Phi(z)$ for every real $z$. Replacing $B(x)^2$ by $\sum_{p\le x}f(p)^2(1-1/p)/p$ is equivalent, because the difference is bounded by $C^2\sum_p p^{-2}$.

This is a general bounded-prime-weight form, not just the special case $f=\omega$. In that case the [Mertens theorem for reciprocal primes](../../../analytic-number-theory.md#mertens-second-theorem) gives $A(N)=\log\log N+O(1)$ and $B(N)^2=\log\log N+O(1)$, so **the classical prime-factor central limit theorem** is

$$
\boxed{\frac{\omega(n)-\log\log N}{\sqrt{\log\log N}}\ \xrightarrow{\mathrm d}\ \mathcal N(0,1).}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Write $y=N^{1/\varphi(N)}$, $L=\sum_{p\le y}|g(p)|$, and $A=\sum_{p\le y}g(p)/p$. Put $I_p(n)=\mathbf1_{p\mid n}$ and $Y_p=I_p-1/p$. The [strongly additive arithmetic function](../../../number-theory.md#strongly-additive-arithmetic-function) identity is $g-A=\sum_{p\le y}g(p)Y_p$.

For any tuple $p_1,\ldots,p_j$, expand $\prod_{r=1}^j(I_{p_r}-1/p_r)$ by choosing an indicator in some positions and the constant in the others. If the selected positions contain distinct [primes](../../../number-theory.md#prime-number) whose product is $d$, then

$$
\mathbb E_N\prod_{r\text{ selected}}I_{p_r}=\frac{\lfloor N/d\rfloor}N=\frac1d+O(N^{-1}).
$$

For the corresponding product of the independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) $X_p$, the [expectation](../../../probability-theory.md#expected-value) is exactly $1/d$. This includes repeated [primes](../../../number-theory.md#prime-number), since their [indicator functions](../../../measure-theory.md#indicator-function) are idempotent, and the empty selection has zero error. Summing absolute values of all expansion coefficients bounds the difference by

$$
\frac1N\prod_{r=1}^j\left(1+\frac1{p_r}\right)\le\frac{2^j}{N}\le\frac{y^j}{N}
$$

when $y\ge2$. Expanding the $j$th power and summing the absolute coefficient weights gives

$$
\mathbb E_N(g-A)^j=\mathbb E\left(\sum_{p\le y}g(p)(X_p-1/p)\right)^j+O\left(\frac{y^jL^j}{N}\right).
$$

It remains to center at the actual [expectation](../../../probability-theory.md#expected-value). Since $\mathbb E_N I_p=\lfloor N/p\rfloor/N$, we have $|\mathbb E_Ng-A|\le L/N$. For each $n$, both $g(n)-A$ and $g(n)-\mathbb E_Ng$ have absolute value at most $L$, because all their indicator coefficients have absolute value at most one. The identity $u^j-v^j=(u-v)\sum_{r=0}^{j-1}u^{j-1-r}v^r$ therefore bounds the change in the [central moment](../../../probability-theory.md#central-moment) by $jL^j/N$.

Finally, [independence](../../../random-variable.md#independent-random-variables) factors each term of the independent [central moment](../../../probability-theory.md#central-moment). If $q_1,\ldots,q_w$ are the distinct [primes](../../../number-theory.md#prime-number) of the tuple and $a_i$ their multiplicities, **the desired comparison** becomes

$$
\boxed{\mathbb E_N(g-\mathbb E_Ng)^j=\sum_{p_1,\ldots,p_j\le y}\prod_{i=1}^w g(q_i)^{a_i}\mathbb E(X_{q_i}-1/q_i)^{a_i}+O\left(\frac{j y^j}{N}L^j\right).}
$$

If $y<2$, then $g=0$ and both sides vanish, so the formula remains valid. The argument also covers complex coefficients $g(p)$; a real-valued assumption is needed for the later [normal distribution](../../../probability-theory.md#normal-distribution) conclusion, not for this [centered moment comparison for additive arithmetic functions](../../../analytic-number-theory.md#centered-moment-comparison-for-additive-arithmetic-functions).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

A useful [method of moments in probability](../../../convergence-of-random-variables.md#method-of-moments-probability-theory) states that if real [random variables](../../../random-variable.md) $Z_N$ have all moments, $\mathbb E Z_N^j\to m_j$ for every integer $j\ge1$, and $(m_j)$ is the moment sequence of a [moment-determinate probability distribution](../../../probability-theory.md#moment-determinacy), then $Z_N$ converges to that distribution in the sense of [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution). In particular, convergence to the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) follows from limiting odd moments zero and limiting even moments $(2k-1)!!$. The [moment-generating function of a standard normal variable](../../../probability-theory.md#moment-generating-function-of-a-standard-normal-variable), finite in a neighbourhood of zero, ensures [moment determinacy](../../../probability-theory.md#moment-determinacy).

For the classical [Erdős-Kac theorem](../../../analytic-number-theory.md#erdos-kac-theorem), put $L=\log\log N$ and choose, for example, $\varphi(N)=L^{1/4}$, with a harmless modification for small $N$. Truncate the [prime omega function](../../../number-theory.md#prime-omega-function) to [primes](../../../number-theory.md#prime-number) $p\le y=N^{1/\varphi(N)}$. The omitted number of distinct [prime factors](../../../number-theory.md#prime-factor) of any $n\le N$ is at most $\varphi(N)$, since a product of $r$ omitted [primes](../../../number-theory.md#prime-number) exceeds $N^{r/\varphi(N)}$. Thus this truncation changes the normalized variable by $o(1)$ uniformly. Also, the [Mertens theorem for reciprocal primes](../../../analytic-number-theory.md#mertens-second-theorem) gives

$$
\sum_{p\le y}\frac1p=L-\log\varphi(N)+O(1)=L+o(\sqrt L).
$$

Part (b) transfers every fixed normalized [central moment](../../../probability-theory.md#central-moment) of the truncated [prime omega function](../../../number-theory.md#prime-omega-function) to the independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) model. Indeed, its unnormalized error is at most $O_j(N^{2j/\varphi(N)-1})$, using $\sum_{p\le y}1\le y$, and this tends to zero for each fixed $j$. In the independent expansion, any singleton index has zero [expectation](../../../probability-theory.md#expected-value); the leading contributions are pairings, giving exactly the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) moments, while blocks of size at least three are negligible after normalization. The [method of moments in probability](../../../convergence-of-random-variables.md#method-of-moments-probability-theory), followed by the uniformly negligible truncation and centering errors, proves the [Erdős-Kac theorem](../../../analytic-number-theory.md#erdos-kac-theorem).

The same strategy proves the bounded-prime-weight form in part (a). Choose $\varphi(N)\to\infty$ slowly enough that $\varphi(N)=o(B(N))$. The omitted weighted contribution is $O(\varphi(N))$; its mean is likewise $O(\varphi(N))$, and its independent [variance](../../../variance.md) is $O(\log\varphi(N)+1)=o(B(N)^2)$ by the [Mertens theorem for reciprocal primes](../../../analytic-number-theory.md#mertens-second-theorem). Hence the truncated model has the same normalization, and part (b) again transfers each fixed [central moment](../../../probability-theory.md#central-moment).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Let $L=\log\log N$, $h=L^{-1/2}$, and let $F_N$ be the [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) of $(\omega-L)/\sqrt L$. Since the [prime omega function](../../../number-theory.md#prime-omega-function) is integer-valued, $F_N$ is constant on every half-open interval between consecutive points of the lattice $(\mathbb Z-L)/\sqrt L$.

Choose $k=\lfloor L\rfloor$ and put $\alpha=(k-L)/\sqrt L$, $\beta=(k+1-L)/\sqrt L$. Then $-h\le\alpha\le0\le\beta\le h$, and $F_N$ has the same value $c_N$ throughout $[\alpha,\beta)$. The [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function) $\Phi$ is continuous, so the definition of the [Kolmogorov distance](../../../probability-theory.md#kolmogorov-distance) gives

$$
E(N)\ge|c_N-\Phi(\alpha)|,\qquad E(N)\ge|c_N-\Phi(\beta)|,
$$

where the second inequality follows by taking a limit from below at $\beta$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) therefore yields

$$
2E(N)\ge\Phi(\beta)-\Phi(\alpha)=\int_\alpha^\beta\frac{e^{-t^2/2}}{\sqrt{2\pi}}\,dt\ge\frac{h e^{-h^2/2}}{\sqrt{2\pi}}.
$$

Thus **the integer lattice forces the lower bound**:

$$
\boxed{E(N)\ge\frac{e^{-1/(2\log\log N)}}{2\sqrt{2\pi\log\log N}}\gg\frac1{\sqrt{\log\log N}}.}
$$

This [lattice obstruction to normal approximation](../../../probability-theory.md#lattice-obstruction-to-normal-approximation) does not require a quantitative [Erdős-Kac theorem](../../../analytic-number-theory.md#erdos-kac-theorem); it follows directly from discreteness and the positive [standard normal density](../../../probability-theory.md#standard-normal-density) near zero.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
