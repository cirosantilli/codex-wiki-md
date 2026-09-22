<h1 id="7a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the exponent $\sigma=m$, the [linear recurrence relation](../../../../../../linear-recurrence-relation.md) reduces to $(m+n)a_n=-a_{n-1}$. The excluded nonpositive integers ensure that no denominator is zero. Normalize $a_0=1$ and iterate:

$$
a_n=\frac{(-1)^n}{(m+1)(m+2)\cdots(m+n)}.
$$

The [ratio test](../../../../../../ratio-test.md) gives an infinite radius of convergence for the [power series](../../../../../../power-series.md) factor. Hence a solution is

$$
\boxed{y_m(x)=x^m\left(1+\sum_{n=1}^{\infty}\frac{(-1)^nx^n}{(m+1)(m+2)\cdots(m+n)}\right).}
$$

For nonintegral $m$, choose instead the exponent $\sigma=0$. Since $n-m\ne0$ for every positive integer $n$, its [linear recurrence relation](../../../../../../linear-recurrence-relation.md) gives $na_n=-a_{n-1}$. Thus

$$
\boxed{y_0(x)=e^{-x}.}
$$

The distinct nonintegral leading exponents establish [linear independence](../../../../../../linear-independence.md). More explicitly, $W(e^{-x},y_m)=m e^{-x}x^{m-1}$ by the [Abel identity](../../../../../../abel-s-identity.md) and the leading coefficient at zero, so the [Wronskian](../../../../../../wronskian.md) is nonzero. The factor $x^m$ uses the real branch on $x>0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7A](../../7a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
