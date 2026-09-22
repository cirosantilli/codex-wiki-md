<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take sieve level $D=x^{1/3}$ and coefficient cutoff $L=\sqrt D=x^{1/6}$. Let $\mathcal P$ be the finite set of [odd primes](../../../../../../odd-prime.md) at most $L$. Give $n=p+2$ one unit of weight for each [prime](../../../../../../prime-number.md) $p\leq x$. For an [odd](../../../../../../odd-function.md) [squarefree integer](../../../../../../squarefree-integer.md) $d$ on these primes, the [sieve distribution](../../../../../../sieve-distribution.md) is

$$
A_d=\pi(x;d,-2)=Xg(d)+r(d),\qquad X=\operatorname{Li}(x),\quad g(d)=\frac1{\phi(d)},\quad |r(d)|\leq E_d.
$$

The residue $-2$ is [coprime](../../../../../../coprime-integers.md) to every such $d$, and $g(p)=1/(p-1)\in(0,1)$ for all permitted [primes](../../../../../../prime-number.md). Values of $g$ outside the permitted set can be chosen arbitrarily in $(0,1)$ at [primes](../../../../../../prime-number.md) and extended multiplicatively on [squarefree integers](../../../../../../squarefree-integer.md).

For the [Selberg sieve](../../../../../../selberg-sieve.md) normalizing sum, $k(p)=g(p)/(1-g(p))=1/(p-2)$ and

$$
J=\sum_{\substack{d\leq L\\d\text{ squarefree}\\p\mid d\Rightarrow p\in\mathcal P}}\prod_{p\mid d}\frac1{p-2}\gg\log L.
$$

Here is a direct proof of this lower bound. Restrict the [Euler product](../../../../../../euler-product.md) to $3\leq p\leq y=L^{1/4}$. The [Mertens first theorem](../../../../../../mertens-first-theorem.md) gives $\sum_{3\leq p\leq y}\log p/(p-1)=\log y+O(1)$, which is at most $\tfrac12\log L$ for large $L$. The [Mertens second theorem](../../../../../../mertens-second-theorem.md) gives

$$
W=\prod_{3\leq p\leq y}\left(1+\frac1{p-2}\right)\asymp\log y.
$$

The [truncated Euler-product lower bound](../../../../../../truncated-euler-product-lower-bound.md), with $\theta=1/2$, now gives $J\geq W/2\gg\log L$.

Use the minimizing [Selberg sieve weights](../../../../../../selberg-sieve-weights.md) from Question 3. Their [absolute values](../../../../../../absolute-value.md) are at most one, so the [Selberg least-common-multiple weights](../../../../../../selberg-least-common-multiple-weights.md) satisfy $|\lambda_d|\leq3^{\omega(d)}$. Parts (a) and (b) control the remainder:

$$
\sum_{d\leq D}|\lambda_dr(d)|\leq\sum_{q\leq D}3^{\omega(q)}E_q
\ll\left(\frac{x}{\log^Ax}\right)^{1/2}\left(\frac{x}{\log x}\log^9D\right)^{1/2}
\ll x\log^{4-A/2}x.
$$

The first factor uses the [Bombieri–Vinogradov theorem](../../../../../../bombieri-vinogradov-theorem.md); $D=x^{1/3}$ is below $x^{1/2}/\log^Bx$ for all sufficiently large $x$. The second uses the permitted $\sum_{q\leq D}9^{\omega(q)}/\phi(q)\ll\log^9D$. The PDF has the exponent **nine**, which the TeX transcribes incorrectly. Choose $A=14$ to obtain $O(x/\log^3x)$.

Every [twin prime](../../../../../../twin-prime.md) pair with $p+2>L$ survives the finite sieve, while the pairs with $p+2\leq L$ number at most $L$. The [Selberg upper-bound sieve](../../../../../../selberg-upper-bound-sieve.md) thus gives

$$
\#\{p\leq x:p,p+2\text{ prime}\}\leq L+\frac XJ+O\left(\frac{x}{\log^3x}\right)
\ll\frac{x}{\log^2x}.
$$

Therefore **the twin-prime count is $O(x/\log^2x)$**. The finite cutoff on the forbidden [primes](../../../../../../prime-number.md) is essential: sieving by all [odd primes](../../../../../../odd-prime.md) would also discard the large [prime](../../../../../../prime-number.md) values $p+2$ that we are trying to count.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
