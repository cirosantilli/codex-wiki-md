<h1 id="12f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $t$, let $B$ have the [binomial distribution](../../../../../../binomial-distribution.md) with parameters $m,t$. The [Bernstein polynomial](../../../../../../bernstein-polynomial.md) is $f_m(t)=\mathbb E[f(B/m)]$. Continuity on the compact interval gives [uniform continuity](../../../../../../uniform-continuity.md) and a finite bound $M=\|f\|_\infty$.

Given $\epsilon>0$, choose $\delta>0$ so $|f(s)-f(t)|<\epsilon$ whenever $|s-t|<\delta$. Since $\mathbb E[B/m]=t$ and $\operatorname{Var}(B/m)=t(1-t)/m\le1/(4m)$, [Chebyshev's inequality](../../../../../../chebyshev-inequality.md) gives

$$
|f_m(t)-f(t)|\le\epsilon+2M\Pr(|B/m-t|\ge\delta)
\le\epsilon+\frac{M}{2m\delta^2}.
$$

The bound is independent of $t$, including both endpoints. Taking the supremum and then letting $m$ tend to infinity proves **$f_m\to f$ uniformly on $[0,1]$**. This provides the required [polynomial](../../../../../../polynomial-split.md)-approximation theorem with its proof.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
