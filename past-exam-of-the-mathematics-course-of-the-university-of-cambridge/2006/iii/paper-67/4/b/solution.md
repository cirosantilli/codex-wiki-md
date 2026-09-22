<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $|T_j(x)|\leq1$ on $[-1,1]$ and the [coefficients](../../../../../../coefficient.md) are summable, the [Weierstrass M-test](../../../../../../weierstrass-m-test.md) gives [uniform convergence](../../../../../../uniform-convergence.md) of this [positive lacunary Chebyshev series](../../../../../../positive-lacunary-chebyshev-series.md) and makes its sum continuous.

Let $r$ be the largest integer with $3^r\leq n$, and set $r=-1$ when $n=0$. The candidate and its tail size are

$$
\boxed{p_n(x)=\sum_{k=0}^ra_kT_{3^k}(x),\qquad E_n(f)=\sum_{k=r+1}^\infty a_k.}
$$

The empty sum for $n=0$ is zero. The candidate has degree at most $n$. The [triangle inequality](../../../../../../triangle-inequality.md) bounds its error by the proposed tail sum, and equality holds at $x=1$, since every [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) has $T_j(1)=1$ and all tail [coefficients](../../../../../../coefficient.md) are positive. It remains to prove that another [polynomial](../../../../../../polynomial-split.md) cannot improve this error.

Put $L=3^{r+1}$, the first omitted degree, so $L>n$. At the points $y_j=\cos(j\pi/L)$ for $j=0,\ldots,L$, every omitted term has

$$
T_{3^k}(y_j)=\cos\left(3^{k-r-1}j\pi\right)=(-1)^j,\qquad k\geq r+1,
$$

because $3^{k-r-1}$ is odd. Uniform convergence therefore gives

$$
f(y_j)-p_n(y_j)=(-1)^j\sum_{k=r+1}^\infty a_k.
$$

These $L+1$ distinct points run in decreasing order; reversing their order still gives alternating signs. Since $L+1\geq n+2$, select $n+2$ consecutive ones and apply the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md). It proves both optimality and uniqueness of the displayed candidate. Thus the best [polynomial](../../../../../../polynomial-split.md) and the error stay unchanged between successive powers of three; this exact truncation property depends on the synchronized tail signs, not on a general rule that truncating a Chebyshev expansion is optimal.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
