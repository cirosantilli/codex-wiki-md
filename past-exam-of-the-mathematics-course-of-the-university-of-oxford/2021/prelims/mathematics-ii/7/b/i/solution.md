<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set

$$
x_{k,n}=\frac{k^2}{k^2+n}\quad(0\leq k\leq n),\qquad
\xi_{k,n}=\frac{x_{k,n}+x_{k+1,n}}2\quad(0\leq k<n).
$$

The points strictly increase from zero to $x_{n,n}=n/(n+1)$. With $f(t)=\sin t$, the given expression is exactly the midpoint [Riemann sum](../../../../../../../riemann-sum.md)

$$
\boxed{S_n=\sum_{k=0}^{n-1}(x_{k+1,n}-x_{k,n})f(\xi_{k,n})}
$$

for the [partition of an interval](../../../../../../../partition-of-an-interval.md) $\mathcal P_n=(x_{0,n},\ldots,x_{n,n})$ of $[0,n/(n+1)]$. The [sine](../../../../../../../sine.md) argument is precisely the midpoint tag, since it is half the sum of the consecutive endpoints.

For a fixed integration [interval](../../../../../../../interval-mathematics.md) $[0,1]$, append $x_{n+1,n}=1$ and choose the final tag $\xi_{n,n}=1$. The resulting [Riemann sum](../../../../../../../riemann-sum.md) $T_n$ satisfies

$$
\boxed{T_n=S_n+\frac{\sin1}{n+1}.}
$$

This makes explicit the small final [interval](../../../../../../../interval-mathematics.md) that the original sum omits.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
