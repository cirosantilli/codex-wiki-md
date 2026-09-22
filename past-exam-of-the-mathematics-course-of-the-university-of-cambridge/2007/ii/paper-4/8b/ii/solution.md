<h1 id="8b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $|z|<1$, differentiation under the convergent Euler integral gives

$$
F^{(n)}(a,b;c;0)=K(a)_n\int_0^1t^{b+n-1}(1-t)^{c-b-1}\,dt
=\frac{(a)_n(b)_n}{(c)_n},
$$

where $(a)_n=a(a+1)\cdots(a+n-1)$ and $(a)_0=1$ are [Pochhammer symbols](../../../../../../rising-factorial.md). Thus its [Taylor series](../../../../../../taylor-series.md) is

$$
F(a,b;c;z)=\sum_{n=0}^{\infty}\frac{(a)_n(b)_n}{(c)_n n!}z^n,
$$

which is symmetric in $a,b$. In the common region of parameter convergence for the two Euler integrals, this proves equality near zero. The [identity theorem](../../../../../../identity-theorem.md) extends it throughout their common principal slit domain, and parameter continuation gives the usual identity wherever both sides are defined:

$$
\boxed{F(a,b;c;z)=F(b,a;c;z).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8B](../../8b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
