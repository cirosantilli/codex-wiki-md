<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [multiplicative arithmetic function](../../../../multiplicative-function.md) has $f(1)=1$ and satisfies $f(mn)=f(m)f(n)$ whenever $m,n$ are coprime. For a [prime](../../../../prime-number-split.md) power $p^e$, the divisors are exactly $1,p,\ldots,p^e$, so there are $e+1$. Multiplicativity therefore gives

$$
\boxed{d(n)=\prod_{j=1}^k(e_j+1).}
$$

Fix $\varepsilon>0$. If $p\ge2^{1/\varepsilon}$, then $(e+1)p^{-\varepsilon e}\le(e+1)2^{-e}\le1$ for every [integer](../../../../integer-split.md) $e\ge0$. There are only finitely many [primes](../../../../prime-number-split.md) below the threshold. For each such [prime](../../../../prime-number-split.md) the sequence $(e+1)p^{-\varepsilon e}$ tends to zero, so its supremum $C_p$ is finite and at least one. Thus

$$
\frac{d(n)}{n^\varepsilon}=\prod_{p^e\parallel n}(e+1)p^{-\varepsilon e}\le\prod_{p<2^{1/\varepsilon}}C_p=:C(\varepsilon).
$$

The product is over a fixed finite set, independent of $n$, proving $\boxed{d(n)\le C(\varepsilon)n^\varepsilon}$.

The change of divisor $k=m/d$ gives $\sigma(m)/m=\sum_{k\mid m}1/k$. List the divisors as $k_1<\cdots<k_{d(m)}$. They are distinct positive [integers](../../../../integer-split.md), so $k_j\ge j$ and $\sigma(m)/m\le\sum_{j\le d(m)}1/j$.

For an [integer](../../../../integer-split.md) $K\ge1$, monotonicity of $1/x$ gives $\sum_{k=2}^K1/k\le\int_1^Kdx/x=\log K$; the same bound for real $K\ge1$ follows by taking its [integer](../../../../integer-split.md) part. Consequently

$$
\frac{\sigma(m)}m\le1+\log d(m)\le\varepsilon\log m+1+\log C(\varepsilon).
$$

Hence the requested bound holds with $\boxed{K(\varepsilon)=1+\log C(\varepsilon)}$, including $m=1$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
