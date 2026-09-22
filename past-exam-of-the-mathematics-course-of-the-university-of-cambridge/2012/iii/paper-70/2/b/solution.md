<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [integer](../../../../../../integer.md) endpoint hypothesis is important. Let $r_{n,k}=\binom nk f(k/n)-\lfloor\binom nk f(k/n)\rfloor$. The [floor function](../../../../../../floor-function.md) gives $0\le r_{n,k}<1$, while $r_{n,0}=r_{n,n}=0$ because $f(0)$ and $f(1)$ are [integers](../../../../../../integer.md). Therefore the [rounded Bernstein polynomial](../../../../../../rounded-bernstein-polynomial.md) satisfies

$$
0\le B_n(f,x)-B_n^*(f,x)\le S_n(x):=\sum_{k=1}^{n-1}x^k(1-x)^{n-k}.
$$

For $0\le x\le1/4$, the successive terms have ratio $x/(1-x)\le1/3$, so the [geometric series](../../../../../../geometric-series.md) estimate gives

$$
S_n(x)\le\frac32x(1-x)^{n-1}\le\frac{3}{2n}.
$$

The last inequality follows by maximizing $x(1-x)^{n-1}$ at $x=1/n$. The same bound holds on $[3/4,1]$ by reflection. On $[1/4,3/4]$, each factor $x$ and $1-x$ is at most $3/4$, giving $S_n(x)\le(n-1)(3/4)^n$. Thus

$$
\boxed{\|B_n(f)-B_n^*(f)\|_\infty\le\max\left\{\frac{3}{2n},(n-1)(3/4)^n\right\}\longrightarrow0.}
$$

Here $n\ge2$; for $n=1$ the difference vanishes. Without the [integer](../../../../../../integer.md) endpoint hypothesis the claim would fail: at $x=0$ the error is $f(0)-\lfloor f(0)\rfloor$, independently of $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
