<h1 id="11e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

From $f''=f$, differentiating successively gives $f^{(2r)}=f$ and $f^{(2r+1)}=f'$ whenever those [derivatives](../../../../../../derivative.md) have been constructed. Starting with twice differentiability, this relation supplies the next two [derivatives](../../../../../../derivative.md) at each stage. Thus **$f$ is infinitely differentiable**, and its origin series is

$$
\boxed{A\sum_{r=0}^\infty\frac{x^{2r}}{(2r)!}
+B\sum_{r=0}^\infty\frac{x^{2r+1}}{(2r+1)!}.}
$$

For a fixed $x$, both $f$ and $f'$ are bounded on the compact interval between zero and $x$, say by $M_x$. Every higher [derivative](../../../../../../derivative.md) is one of these two functions. [Taylor's theorem](../../../../../../taylor-theorem.md), with the remainder just proved, therefore bounds the order-$n$ remainder by $M_x|x|^n/n!$, which tends to zero: its consecutive positive-term ratio is $|x|/(n+1)$. Hence **the series converges to $f(x)$ for every real $x$**. It also gives $f(x)=A\cosh x+B\sinh x$ by the usual hyperbolic-function series.

At any other centre $a$, apply the proved origin result to $g(t)=f(a+t)$, which also satisfies $g''=g$. Its even [derivatives](../../../../../../derivative.md) at zero are $f(a)$, and its odd ones are $f'(a)$. Consequently

$$
\boxed{f(a+h)=\sum_{k=0}^\infty\frac{f^{(k)}(a)}{k!}h^k
=f(a)\sum_{r=0}^\infty\frac{h^{2r}}{(2r)!}
+f'(a)\sum_{r=0}^\infty\frac{h^{2r+1}}{(2r+1)!}.}
$$

This proves convergence at every centre without assuming that smoothness alone implies equality to a [Taylor series](../../../../../../taylor-series.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
