<h1 id="7d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the constant [monomial](../../../../../../monomial.md) $f_0=1$, the [binomial theorem](../../../../../../binomial-theorem.md) gives $B_n(f_0)(x)=(x+1-x)^n=1$. For $f_1$, the [binomial coefficient](../../../../../../binomial-coefficient.md) identity $k\binom nk=n\binom{n-1}{k-1}$ gives

$$
B_n(f_1)(x)=x\sum_{j=0}^{n-1}\binom{n-1}{j}x^j(1-x)^{n-1-j}=x.
$$

Thus $\boxed{B_n(f_0)=1,\quad B_n(f_1)=x}$, including $x=0,1$ by evaluation of the [polynomials](../../../../../../polynomial-split.md).

For $m\ge1$ and $n\ge2$, substitute the preceding coefficient identity into the [Bernstein polynomial](../../../../../../bernstein-polynomial.md) sum and write $j=k-1$. This yields the [Bernstein monomial recurrence](../../../../../../bernstein-monomial-recurrence.md)

$$
B_n(f_m)(x)=x\sum_{\ell=0}^{m-1}a_{n,m,\ell}\,B_{n-1}(f_{m-1-\ell})(x).
$$

The coefficients are nonnegative and sum to $1$; $a_{n,m,0}=((n-1)/n)^{m-1}\to1$ and the others tend to zero. The weights in any [Bernstein polynomial](../../../../../../bernstein-polynomial.md) sum are nonnegative and sum to $1$, so $0\le B_n(f_j)(x)\le1$. Induction on $m$ therefore gives $B_n(f_m)(x)\to x\,x^{m-1}=x^m$: the $\ell=0$ term has that limit and the other finitely many terms vanish. In fact, the same estimate in the [supremum norm](../../../../../../supremum-norm.md) proves [uniform convergence](../../../../../../uniform-convergence.md) on $[0,1]$.

As an independent quantitative bound, take a [binomial distribution](../../../../../../binomial-distribution.md) variable $K$ with parameters $(n,x)$. Then $B_n(f_m)(x)=\mathbb E[(K/n)^m]$. On $[0,1]$, factoring the difference of powers gives $|t^m-x^m|\le m|t-x|$; the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [variance](../../../../../../variance-split.md) of $K/n$ give

$$
\boxed{|B_n(f_m)(x)-x^m|\le m\sqrt{\frac{x(1-x)}n}\le\frac m{2\sqrt n}.}
$$

For $m=0$ the error is exactly zero. Finally the requested sum equals $2^m B_{2n}(f_m)(1/2)$, so

$$
\boxed{\lim_{n\to\infty}\frac1{4^n}\sum_{k=0}^{2n}\left(\frac kn\right)^m\binom{2n}{k}=2^m(1/2)^m=1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7D](../../7d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
