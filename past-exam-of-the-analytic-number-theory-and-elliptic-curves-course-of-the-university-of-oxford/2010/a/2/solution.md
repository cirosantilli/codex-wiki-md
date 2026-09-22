<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the convention $f(1)=1$ in the definition of a [multiplicative arithmetic function](../../../../multiplicative-function.md). For a finite set of primes, multiplying the [absolutely convergent](../../../../absolute-convergence.md) local series gives the Dirichlet sum over integers supported on those primes, by [unique prime factorization](../../../../fundamental-theorem-of-arithmetic.md). If all primes up to $Y$ are included, any missing [integer](../../../../integer-split.md) is larger than $Y$, so the difference from the full series is bounded by $\sum_{n>Y}|f(n)|n^{-\sigma}$, which tends to [zero](../../../../zero-of-a-function.md). This proves the [Euler product](../../../../euler-product.md) in its absolute-convergence half-plane.

For coprime $m,n$, every divisor of $mn$ is uniquely a product of a divisor of $m$ and a divisor of $n$. Hence $\sigma_\alpha(mn)=\sigma_\alpha(m)\sigma_\alpha(n)$. The squared modulus is also multiplicative when $\alpha=i\theta$.

At a prime put $z=p^{-s}$ and $a=p^{i\theta}$, so $|a|=1$. Summing by the two divisor exponents gives

$$
\sum_{k\ge0}\left|\sum_{j=0}^ka^j\right|^2z^k
=\frac{1-z^2}{(1-z)^2(1-az)(1-a^{-1}z)}.
$$

For example, expand the square as $\sum_{j,l\le k}a^{j-l}$ and sum $z^k$ from $k=\max(j,l)$ to obtain this rational expression. It remains valid for $a=1$. [Absolute convergence](../../../../absolute-convergence.md) for $\sigma>1$ follows from $|\sigma_{i\theta}(p^k)|\le k+1$ and convergence of $\sum_p p^{-\sigma}$. Multiplying the factors therefore proves

$$
\boxed{\sum_{n\ge1}\frac{|\sigma_{i\theta}(n)|^2}{n^s}
=\frac{\zeta(s)^2\zeta(s+i\theta)\zeta(s-i\theta)}{\zeta(2s)}.}
$$

Suppose now that $\zeta(1+i\theta)=0$. Necessarily $\theta\ne0$, since $s=1$ is a [pole](../../../../pole.md). [Complex conjugation](../../../../complex-conjugation.md) gives a [zero](../../../../zero-of-a-function.md) also at $1-i\theta$. In the numerator, the [double pole](../../../../double-pole.md) at $s=1$ is canceled by those two zeros in the shifted factors. At $s=1\pm i\theta$, the possible [simple pole](../../../../simple-pole.md) of a shifted factor is canceled by the double [zero](../../../../zero-of-a-function.md) of $\zeta(s)^2$. Thus on $\operatorname{Re}s>0$ the only possible remaining poles come from zeros of $\zeta(2s)$. Since the [Euler product](../../../../euler-product.md) excludes zeros for $\operatorname{Re}(2s)>1$, these possible poles lie in $0<\operatorname{Re}s\le1/2$. In particular $f$ is regular for $\operatorname{Re}s>1/2$.

The assumed nonnegative-series principle now makes its [Dirichlet series](../../../../dirichlet-series.md) converge and equal $f$ there. Its first coefficient is one and all coefficients are nonnegative, so $f(\sigma)\ge1$ for real $\sigma>1/2$. But as $\sigma\downarrow1/2$, the numerator remains finite while $\zeta(2\sigma)\to+\infty$, forcing $f(\sigma)\to0$. This contradiction proves

$$
\boxed{\zeta(s)\text{ has no zero on }\operatorname{Re}s=1.}
$$

At the real point $s=1$ the statement is understood as a [pole](../../../../pole.md) rather than a finite nonzero value. The [pole](../../../../pole.md)-location argument did not assume the [zero](../../../../zero-of-a-function.md)-free boundary before proving it.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
