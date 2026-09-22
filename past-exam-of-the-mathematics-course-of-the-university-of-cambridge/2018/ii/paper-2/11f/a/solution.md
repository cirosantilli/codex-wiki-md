<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $f\in C[0,1]$, define its [Bernstein polynomial](../../../../../../bernstein-polynomial.md)

$$
B_nf(x)=\sum_{k=0}^nf\left(\frac kn\right)\binom nkx^k(1-x)^{n-k}.
$$

If $X_{n,x}\sim\operatorname{Bin}(n,x)$, then

$$
B_nf(x)=\mathbb E f(X_{n,x}/n),
\quad
\mathbb E(X_{n,x}/n)=x,
\quad
\operatorname{Var}(X_{n,x}/n)=\frac{x(1-x)}n\leq\frac1{4n}.
$$

Let $M=\|f\|_\infty$. By [uniform continuity](../../../../../../uniform-continuity.md), for any $\varepsilon>0$ choose $\delta>0$ such that $|f(u)-f(v)|<\varepsilon/2$ whenever $|u-v|<\delta$. Splitting the expectation according to that event and using [Chebyshev's inequality](../../../../../../chebyshev-inequality.md) gives, uniformly in $x$,

$$
|B_nf(x)-f(x)|
\leq\frac\varepsilon2+2M\mathbb P(|X_{n,x}/n-x|\geq\delta)
\leq\frac\varepsilon2+\frac{M}{2n\delta^2}.
$$

For sufficiently large $n$ this is below $\varepsilon$. Thus $B_nf\to f$ uniformly on $[0,1]$. An affine change of variable treats every compact interval, proving the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
