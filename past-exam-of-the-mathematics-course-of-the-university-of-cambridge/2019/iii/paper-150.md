# Paper 150

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_150.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_150.pdf)

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
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Von Mangoldt divisor identity](../../../number-theory.md#von-mangoldt-divisor-identity) gives

$$
\sum_{n\leq x}\log n
=\sum_{d\leq x}\Lambda(d)\left\lfloor\frac xd\right\rfloor
=x\sum_{d\leq x}\frac{\Lambda(d)}d+O(\psi(x)).
$$

By the [Stirling formula](../../../real-analysis.md#stirling-formula), the left side is $\log(\lfloor x\rfloor!)=x\log x-x+O(\log x)$, while the assumed [Chebyshev estimate](../../../number-theory.md#chebyshev-estimate) gives $\psi(x)=O(x)$. Hence

$$
\sum_{n\leq x}\frac{\Lambda(n)}n=\log x+O(1).
$$

The contribution of proper [prime powers](../../../number-theory.md#prime-power) is bounded uniformly:

$$
\sum_{\substack{p^k\leq x\\k\geq2}}\frac{\log p}{p^k}
\leq\sum_p\frac{\log p}{p(p-1)}<\infty.
$$

Removing it leaves

$$
\boxed{\sum_{p\leq x}\frac{\log p}{p}=\log x+O(1).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put

$$
A(x)=\sum_{p\leq x}\frac{\log p}{p}=\log x+E(x),
\qquad E(x)=O(1).
$$

The [Abel summation formula](../../../analytic-number-theory.md#abel-s-summation-formula) with weight $1/\log t$ gives

$$
\sum_{p\leq x}\frac1p
=\frac{A(x)}{\log x}
+\int_2^x\frac{A(t)}{t(\log t)^2}\,dt.
$$

Substituting $A(t)=\log t+E(t)$ yields

$$
\sum_{p\leq x}\frac1p
=\log\log x+c+\frac{E(x)}{\log x}
-\int_x^\infty\frac{E(t)}{t(\log t)^2}\,dt
$$

for a constant $c$. Both final terms are $O(1/\log x)$, so

$$
\boxed{\sum_{p\leq x}\frac1p
=\log\log x+c+O\left(\frac1{\log x}\right).}
$$

This is the [Mertens second theorem](../../../analytic-number-theory.md#mertens-second-theorem).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The same divisor-identity argument as in part (a) gives

$$
\sum_{n\leq x}\frac{\Lambda(n)}n=\log x+O(1).
$$

On the other hand, the [Abel summation formula](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\sum_{n\leq x}\frac{\Lambda(n)}n
=\frac{\psi(x)}x+\int_1^x\frac{\psi(t)}{t^2}\,dt.
$$

Under the proposed asymptotic, the right side is

$$
a\log x+b\log\log x+o(\log\log x)+O(1).
$$

Dividing first by $\log x$ gives $a=1$. Subtracting $\log x$, dividing by $\log\log x$, and taking the [limit](../../../calculus.md#limit-of-a-function) then gives $b=0$. Therefore

$$
\boxed{a=1,\qquad b=0.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Taking the [natural logarithm](../../../calculus.md#natural-logarithm) of the finite [Euler product](../../../analytic-number-theory.md#euler-product) and using the [Taylor series](../../../calculus.md#taylor-series)

$$
-\log(1-u)=u+\sum_{k\geq2}\frac{u^k}{k}
$$

gives

$$
\log\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
=\sum_{p\leq x}\frac1p
+\sum_{p\leq x}\sum_{k\geq2}\frac1{kp^k}.
$$

The double series converges absolutely, and the [Mertens second theorem](../../../analytic-number-theory.md#mertens-second-theorem) therefore makes the right side

$$
\log\log x+\log C+O\left(\frac1{\log x}\right)
$$

for

$$
C=\exp\left(c+\sum_p\sum_{k\geq2}\frac1{kp^k}\right)>0.
$$

Exponentiating proves

$$
\boxed{\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
=C\log x+O(1).}
$$

This is the [Mertens third theorem](../../../analytic-number-theory.md#mertens-third-theorem).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The prime-factor formula for the [Euler totient function](../../../number-theory.md#euler-totient-function) is

$$
\frac n{\varphi(n)}
=\prod_{p\mid n}\left(1-\frac1p\right)^{-1}.
$$

Let

$$
y=\frac{\log n}{\sqrt{\log\log n}}.
$$

The factors with $p\leq y$ contribute at most

$$
\prod_{p\leq y}\left(1-\frac1p\right)^{-1}
=C\log y+O(1)
=(C+o(1))\log\log n
$$

by the [Mertens third theorem](../../../analytic-number-theory.md#mertens-third-theorem). For $p>y$, the number of distinct prime divisors of $n$ is at most $\log n/\log y$, and hence

$$
\begin{aligned}
\log\prod_{\substack{p\mid n\\p>y}}\left(1-\frac1p\right)^{-1}
&\ll\sum_{\substack{p\mid n\\p>y}}\frac1p\\
&\leq\frac{\log n}{y\log y}
=O\left(\frac1{\sqrt{\log\log n}}\right).
\end{aligned}
$$

Thus the large-prime product is $1+o(1)$, and

$$
\frac n{\varphi(n)}\leq(C+o(1))\log\log n.
$$

Taking reciprocals gives, uniformly as $n\to\infty$,

$$
\boxed{\varphi(n)\geq\left(C^{-1}+o(1)\right)
\frac n{\log\log n}.}
$$

## 2

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\mathcal A=(a_n)$ be a finite nonnegative sequence, let $\mathcal P$ be a set of [prime numbers](../../../number-theory.md#prime-number), and define

$$
P(z)=\prod_{\substack{p<z\\p\in\mathcal P}}p.
$$

The [sifting function](../../../analytic-number-theory.md#sifting-function) is

$$
\boxed{S(\mathcal A,\mathcal P;z)
=\sum_{\gcd(n,P(z))=1}a_n.}
$$

For a finite set $A$ of integers, take $a_n$ to be the number of occurrences of $n$ in $A$; then $S(A,\mathcal P;z)$ counts members divisible by no $p\in\mathcal P$ below $z$. For $d\mid P(z)$, write

$$
|\mathcal A_d|=\sum_{d\mid n}a_n.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Suppose the [sieve distribution](../../../analytic-number-theory.md#sieve-distribution) has the form

$$
|\mathcal A_d|=Xg(d)+r_d\qquad(d\mid P(z)),
$$

where $g$ is a [multiplicative arithmetic function](../../../number-theory.md#multiplicative-function) on squarefree integers and $0\leq g(p)<1$. Define

$$
h(d)=\prod_{p\mid d}\frac{g(p)}{1-g(p)},\qquad
G(D,z)=\sum_{\substack{\ell<D\\\ell\mid P(z)}}h(\ell).
$$

Then the [Selberg upper-bound sieve](../../../analytic-number-theory.md#selberg-upper-bound-sieve) states

$$
\boxed{
S(\mathcal A,\mathcal P;z)
\leq\frac X{G(D,z)}
+\sum_{\substack{m<D^2\\m\mid P(z)}}3^{\omega(m)}|r_m|
}
$$

for $1<D\leq z$, with immaterial endpoint changes under other level conventions.

To construct the weights, put

$$
G_d(y,z)=
\sum_{\substack{\ell<y\\\ell\mid P(z)\\(\ell,d)=1}}h(\ell)
$$

and set

$$
\lambda_d=
\begin{cases}
\displaystyle
\mu(d)\prod_{p\mid d}(1-g(p))^{-1}
\frac{G_d(D/d,z)}{G(D,z)},&
d<D,\ d\mid P(z),\\[6pt]
0,&\text{otherwise}.
\end{cases}
$$

Then $\lambda_1=1$. If $\gcd(n,P(z))=1$, the divisor sum $\sum_{d\mid n}\lambda_d$ equals one, and hence

$$
1_{\gcd(n,P(z))=1}
\leq\left(\sum_{\substack{d\mid n\\d\mid P(z)}}\lambda_d\right)^2.
$$

Summing against $a_n$ and expanding gives

$$
S(\mathcal A,\mathcal P;z)
\leq\sum_{d,e}\lambda_d\lambda_e
\bigl(Xg([d,e])+r_{[d,e]}\bigr).
$$

The Selberg diagonalization of the positive quadratic form gives

$$
\sum_{d,e}\lambda_d\lambda_e g([d,e])=\frac1{G(D,z)}.
$$

Finally, grouping the error by $m=[d,e]$ gives at most $3^{\omega(m)}$ pairs $(d,e)$ for each squarefree $m$; using $|\lambda_d|\leq1$ yields the stated remainder.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let

$$
F(n)=\prod_{i=1}^r(n+h_i)
$$

and let $W$ be the product of the finitely many primes at most $r$ or dividing some nonzero difference $h_i-h_j$. Sieve with the primes $p\nmid W$. For such a prime, the congruence $F(n)\equiv0\pmod p$ has exactly $r$ distinct roots. By the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem), the root-counting function $\rho(d)$ is multiplicative on squarefree $d$ coprime to $W$, and

$$
\#\{n\leq x:d\mid F(n)\}
=x\frac{\rho(d)}d+O(\rho(d)).
$$

Thus the [polynomial root density in a sieve](../../../analytic-number-theory.md#polynomial-root-density-in-a-sieve) applies with

$$
g(p)=\frac rp,\qquad r_d=O(\rho(d)).
$$

Take $z=x^{1/4}$ and $D=z$. For squarefree $d$ coprime to $W$,

$$
h(d)=\prod_{p\mid d}\frac r{p-r}
\geq\frac{r^{\omega(d)}}d.
$$

The supplied mean-value estimate, [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula), and removal of square factors using $r^{\omega(n)}\ll_{r,\epsilon}n^\epsilon$ give

$$
G(z,z)\gg_{r,W}(\log z)^r.
$$

The error in the [Selberg upper-bound sieve](../../../analytic-number-theory.md#selberg-upper-bound-sieve) is

$$
\ll\sum_{d<z^2}(3r)^{\omega(d)}
\ll_{r,\epsilon}z^{2+\epsilon}
=o\left(\frac{x}{(\log x)^r}\right).
$$

Consequently

$$
S(\mathcal A,\mathcal P;z)
\ll_{h_1,\ldots,h_r,r}\frac{x}{(\log x)^r}.
$$

If every $n+h_i$ is prime and all of them exceed $z$, then $F(n)$ has no prime divisor $p<z$ with $p\nmid W$, apart from a fixed finite set of divisibility cases absorbed into the implied constant. The cases with some $n+h_i\leq z$ contribute $O_r(z)$. Therefore

$$
\boxed{
\#\{n\leq x:n+h_1,\ldots,n+h_r\text{ are all prime}\}
\ll_{h_1,\ldots,h_r,r}\frac{x}{(\log x)^r}.
}
$$

## 3

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $\sigma>1$, summation over the intervals $[n,n+1)$ gives

$$
\zeta(s)=s\int_1^\infty\frac{\lfloor u\rfloor}{u^{s+1}}\,du.
$$

Since $\lfloor u\rfloor=u-\{u\}$,

$$
\boxed{\zeta(s)=\frac{s}{s-1}
-s\int_1^\infty\frac{\{u\}}{u^{s+1}}\,du.}
$$

The integral converges absolutely and defines a [holomorphic function](../../../complex-analysis.md#holomorphic-function) for $\sigma>0$. This formula therefore gives the [Meromorphic continuation of the Riemann zeta function to the right half-plane](../../../analytic-number-theory.md#meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane), with only a simple pole at $s=1$ and residue one.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $\sigma>1$, both relevant [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) converge absolutely, so their product may be rearranged:

$$
\zeta(s)\sum_{n=1}^\infty\frac{\mu(n)}{n^s}
=\sum_{n=1}^\infty\frac1{n^s}\sum_{d\mid n}\mu(d).
$$

The inner sum is one when $n=1$ and zero otherwise by [Möbius inversion](../../../number-theory.md#mobius-inversion-formula). Hence

$$
\boxed{\frac1{\zeta(s)}
=\sum_{n=1}^\infty\frac{\mu(n)}{n^s}\qquad(\sigma>1).}
$$

This is also the reciprocal of the absolutely convergent [Euler product](../../../analytic-number-theory.md#euler-product).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $\sigma>1$, the [three-four-one zero-free-region argument](../../../analytic-number-theory.md#three-four-one-zero-free-region-argument) starts from

$$
3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\geq0.
$$

Applying this termwise to

$$
-\frac{\zeta'(s)}{\zeta(s)}
=\sum_{n\geq1}\frac{\Lambda(n)}{n^s}
$$

gives

$$
-3\frac{\zeta'(\sigma)}{\zeta(\sigma)}
-4\Re\frac{\zeta'(\sigma+it)}{\zeta(\sigma+it)}
-\Re\frac{\zeta'(\sigma+2it)}{\zeta(\sigma+2it)}
\geq0.
$$

Suppose $\rho=\beta+i\gamma$ is a zero with $|\gamma|\geq4$. In the supplied [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](../../../analytic-number-theory.md#local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative), every nearby zero contributes a nonnegative real part at $\sigma+i\gamma$ when $\sigma>1$. Keeping the term from $\rho$ gives

$$
\Re\frac{\zeta'(\sigma+i\gamma)}{\zeta(\sigma+i\gamma)}
\geq\frac1{\sigma-\beta}-O(\log|\gamma|).
$$

At height zero the pole at one gives

$$
-\frac{\zeta'(\sigma)}{\zeta(\sigma)}
=\frac1{\sigma-1}+O(1),
$$

and the same local expansion at height $2\gamma$ gives

$$
-\Re\frac{\zeta'(\sigma+2i\gamma)}{\zeta(\sigma+2i\gamma)}
\ll\log|\gamma|.
$$

Substitution yields

$$
\frac4{\sigma-\beta}
\leq\frac3{\sigma-1}+O(\log|\gamma|).
$$

Set $\sigma=1+\eta/\log|\gamma|$, first choosing a sufficiently small absolute $\eta>0$. If $\beta>1-c/\log|\gamma|$, the left side is at least $4\log|\gamma|/(\eta+c)$. Choosing $c>0$ sufficiently small contradicts the last inequality. Therefore

$$
\boxed{\zeta(s)\ne0
\quad\text{for}\quad
\sigma>1-\frac c{\log|t|},\quad |t|\geq4.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The truncated [Perron formula](../../../analytic-number-theory.md#perron-s-formula) says that, for $c>1$ and $T\geq2$,

$$
\sum_{n\leq x}a_n
=\frac1{2\pi i}\int_{c-iT}^{c+iT}
\left(\sum_{n=1}^\infty\frac{a_n}{n^s}\right)\frac{x^s}{s}\,ds
+\text{a truncation error},
$$

where an endpoint has half weight and the error is controlled by

$$
\sum_n|a_n|\left(\frac xn\right)^c
\min\left(1,\frac1{T|\log(x/n)|}\right).
$$

Apply this with $a_n=\mu(n)$, $c=1+1/\log x$, and

$$
T=\exp(\sqrt{\log x}).
$$

Part (b) makes the integrand $x^s/(s\zeta(s))$. Move the contour to

$$
\sigma_0=1-\frac{c_2}{\log T}
=1-\frac{c_2}{\sqrt{\log x}},
$$

using a contour that stays inside the [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function) near small $|t|$. The estimates supplied in the question give $1/\zeta(s)\ll\log(|t|+3)$ on the new contour. Its vertical segment is therefore

$$
\ll x^{\sigma_0}(\log T)^2
\ll x\exp(-c_3\sqrt{\log x}),
$$

after decreasing $c_3$. The horizontal segments and the Perron truncation error are

$$
\ll\frac{x(\log x)^{O(1)}}T
\ll x\exp(-c_4\sqrt{\log x}).
$$

No residue is crossed because $1/\zeta(s)$ has a zero, rather than a pole, at $s=1$. Thus the [Mertens function](../../../number-theory.md#mertens-function) satisfies

$$
\boxed{\sum_{n\leq x}\mu(n)
\ll x\exp(-c\sqrt{\log x})}
$$

for some absolute $c>0$.

## 4

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\widehat G$ be the group of all [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character) modulo $q$, where $G=(\mathbb Z/q\mathbb Z)^\times$, and consider

$$
F(s)=\prod_{\chi\in\widehat G}L(s,\chi).
$$

For $p\nmid q$, let $f_p$ be the order of $p$ in $G$. The values $\chi(p)$ run through the $f_p$th roots of unity, each $|G|/f_p$ times, so the local factor is

$$
\prod_{\chi\in\widehat G}(1-\chi(p)p^{-s})^{-1}
=(1-p^{-f_ps})^{-|G|/f_p}.
$$

For $p\mid q$ the local factor is one. Thus the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) for $F$ has nonnegative coefficients.

The principal-character factor has a simple pole at $s=1$, while every nonprincipal [Dirichlet L-function](../../../algebraic-number-theory.md#dirichlet-l-function) is entire. If some nonprincipal $L(1,\chi)$ vanished, its zero would cancel that pole and make $F$ entire. The [Landau theorem for a Dirichlet series with nonnegative coefficients](../../../analytic-number-theory.md#landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients) would then force the Dirichlet series of $F$ to converge for every real $s$. This is impossible: its coefficient at $m^{|G|}$ is at least one for every $m$ coprime to $q$, as is clear from the local factors. Hence

$$
\boxed{L(1,\chi)\ne0\qquad
\text{for every nonprincipal }\chi.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $\sigma>1$, [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters) gives

$$
\sum_{\substack{n\geq1\\n\equiv a\pmod q}}
\frac{\Lambda(n)}{n^\sigma}
=\frac1{\varphi(q)}
\sum_{\chi\bmod q}\overline{\chi(a)}
\left(-\frac{L'(\sigma,\chi)}{L(\sigma,\chi)}\right).
$$

The principal-character term is

$$
\frac1{\sigma-1}+O_q(1).
$$

Part (a) makes every nonprincipal logarithmic derivative bounded as $\sigma\to1^+$, so

$$
\sum_{\substack{n\geq1\\n\equiv a\pmod q}}
\frac{\Lambda(n)}{n^\sigma}
=\frac1{\varphi(q)(\sigma-1)}+O_q(1)
\longrightarrow\infty.
$$

If the nondecreasing [Chebyshev function in an arithmetic progression](../../../analytic-number-theory.md#chebyshev-function-in-an-arithmetic-progression)

$$
\psi(x;q,a)=\sum_{\substack{n\leq x\\n\equiv a\pmod q}}\Lambda(n)
$$

were bounded, the [Abel summation formula](../../../analytic-number-theory.md#abel-s-summation-formula) would keep the displayed Dirichlet series bounded near $\sigma=1$. Therefore

$$
\boxed{\psi(x;q,a)\longrightarrow\infty.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

There is an absolute $c>0$ such that the product of the [Dirichlet L-functions](../../../algebraic-number-theory.md#dirichlet-l-function) modulo $q$ has no zero in

$$
\boxed{\sigma\geq1-\frac{c}{\log(q(|t|+2))}}
$$

except possibly one zero. If it exists, this [exceptional zero](../../../analytic-number-theory.md#siegel-zero) $\beta$ is real and simple, belongs to a real nonprincipal character $\chi_1$, and lies very close to one. Among the primitive characters whose conductors divide $q$, at most one can have such a zero. This is the [classical zero-free region for Dirichlet L-functions](../../../analytic-number-theory.md#classical-zero-free-region-for-dirichlet-l-functions).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $\chi_1$ be the real character associated with the exceptional zero $\beta$. The [prime number theorem in an arithmetic progression with an exceptional zero](../../../analytic-number-theory.md#prime-number-theorem-in-an-arithmetic-progression-with-an-exceptional-zero) gives, uniformly for $x\geq2$ and $(a,q)=1$,

$$
\boxed{
\psi(x;q,a)
=\frac{x}{\varphi(q)}
-\frac{\chi_1(a)x^\beta}{\beta\varphi(q)}
+O\left(
x(\log q)^2
\exp\left[-\frac{c\log x}{\log q+\sqrt{\log x}}\right]
\right).
}
$$

If no exceptional zero exists, the middle term is omitted. The constant $c>0$ is absolute.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Assume $\beta$ exists and choose a reduced residue class $a$ with $\chi_1(a)=-1$; such a class exists because $\chi_1$ is nonprincipal. Fix a sufficiently large constant $A=A(\epsilon)$ and take

$$
x=\exp(A(\log q)^2).
$$

Then $x\geq q^2$ for large $q$. Multiplying the formula from part (d) by $\varphi(q)/x$ gives

$$
\frac{\varphi(q)}x\psi(x;q,a)
=1+\frac{x^{\beta-1}}{\beta}
+O\left(
\varphi(q)(\log q)^2
\exp\left[-\frac{cA\log q}{1+\sqrt A}\right]
\right).
$$

Choose $A$ so large that the error is at most $\epsilon/4$ for all sufficiently large $q$. The assumed upper bound then implies

$$
\frac{x^{\beta-1}}{\beta}\leq1-\frac{3\epsilon}4.
$$

Since $\beta<1$, this gives

$$
x^{\beta-1}\leq1-\frac{3\epsilon}4.
$$

Taking logarithms,

$$
(1-\beta)A(\log q)^2
\geq-\log\left(1-\frac{3\epsilon}4\right).
$$

Therefore, with a positive constant depending only on $\epsilon$,

$$
\boxed{\beta\leq1-\frac{c}{(\log q)^2}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
