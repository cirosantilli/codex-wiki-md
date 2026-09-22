<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each $k$, let $\varepsilon_{n,k}=\binom nkf(k/n)-\lfloor\binom nkf(k/n)\rfloor$. The [floor function](../../../../../../floor-function.md) ensures $0\le\varepsilon_{n,k}<1$, even when the quantity being rounded is negative. The [integer](../../../../../../integer.md) endpoint hypothesis gives $\varepsilon_{n,0}=\varepsilon_{n,n}=0$. Thus the error of the [rounded Bernstein polynomial](../../../../../../rounded-bernstein-polynomial.md) satisfies

$$
0\le B_n(f,x)-B_n^*(f,x)
\le S_n(x):=\sum_{k=1}^{n-1}x^k(1-x)^{n-k}.
$$

It suffices to bound this unnormalized sum uniformly. If $0\le x\le1/4$, put $q=x/(1-x)\le1/3$ and sum a [geometric series](../../../../../../geometric-series.md):

$$
S_n(x)\le(1-x)^n\frac q{1-q}
=\frac{x(1-x)^n}{1-2x}\le2x(1-x)^n\le\frac2{n+1}.
$$

The last inequality follows by maximizing $x(1-x)^n$, whose maximum occurs at $x=1/(n+1)$ and is at most $1/(n+1)$. Reflection gives the same bound for $3/4\le x\le1$. In the middle interval both $x$ and $1-x$ are at most $3/4$, so each summand is at most $(3/4)^n$. Therefore, for $n\ge2$,

$$
\boxed{\|B_n(f)-B_n^*(f)\|_\infty
\le\max\left\{\frac2{n+1},(n-1)\left(\frac34\right)^n\right\}\longrightarrow0.}
$$

Endpoint integrality matters: at zero or one a noninteger value would leave a fixed nonzero rounding error.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
