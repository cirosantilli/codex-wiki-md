<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the finite [probability distribution](../../../../../../probability-distribution.md), put $\xi_j=(X_j+1)/2$. These are [independent](../../../../../../independent-random-variables.md) fair zero-one variables, and

$$
Y_n=2\sum_{j=1}^n2^{-j}\xi_j-(1-2^{-n}).
$$

The binary integer $\sum_{j=1}^n2^{n-j}\xi_j$ is uniform on $\{0,\ldots,2^n-1\}$. Hence

$$
\boxed{\mathbb P\!\left(Y_n=-1+\frac{2k+1}{2^n}\right)=2^{-n},\qquad 0\leq k<2^n.}
$$

These are the midpoints of $2^n$ equal subintervals of $[-1,1]$. For every bounded continuous $f$, the [Riemann sums](../../../../../../riemann-sum.md) give

$$
\mathbb E f(Y_n)=2^{-n}\sum_{k=0}^{2^n-1}f\!\left(-1+\frac{2k+1}{2^n}\right)\longrightarrow\frac12\int_{-1}^1f(x)\,dx.
$$

Thus $\boxed{Y_n\Rightarrow\operatorname{Unif}[-1,1]}$ in the sense of [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md).

For the almost-sure and $L^2$ assertions, the [Dyadic Rademacher series](../../../../../../dyadic-rademacher-series.md) $Y=\sum_{j\geq1}2^{-j}X_j$ converges absolutely on every sign sequence, since $|X_j|=1$. Its tail satisfies $|Y-Y_n|\leq2^{-n}$, proving [almost sure convergence](../../../../../../almost-sure-convergence.md) and [convergence in L2](../../../../../../convergence-in-l2.md). More precisely, zero means and [independence](../../../../../../independent-random-variables.md) eliminate the cross terms:

$$
\boxed{\mathbb E[(Y-Y_n)^2]=\sum_{j>n}4^{-j}=\frac{4^{-n}}3.}
$$

This identity follows first for finite tails and then by [dominated convergence](../../../../../../dominated-convergence-theorem.md). Bounded continuous test functions and [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) identify the [probability distribution](../../../../../../probability-distribution.md) of $Y$ with the weak limit above, namely the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[-1,1]$.

For the requested product identity, each [Rademacher random variable](../../../../../../rademacher-distribution.md) has [characteristic function](../../../../../../characteristic-function.md) $\mathbb E e^{itX_j}=\cos t$. The [characteristic function of a sum of independent variables](../../../../../../characteristic-function-of-a-sum-of-independent-variables.md) therefore yields

$$
\varphi_{Y_n}(t)=\prod_{j=1}^n\cos(t/2^j).
$$

By part (a), or directly by [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md), this converges to the [characteristic function of a uniform distribution](../../../../../../characteristic-function-of-a-uniform-distribution.md), $\tfrac12\int_{-1}^1e^{itx}\,dx=\sin t/t$. Consequently the [dyadic cosine product](../../../../../../dyadic-cosine-product.md) is

$$
\boxed{\prod_{j=1}^{\infty}\cos(t/2^j)=\frac{\sin t}{t},\qquad t\in\mathbb R.}
$$

Both sides are one at zero. At zeros of the [sinc function](../../../../../../sinc-function.md) the identity is understood as the limit of the finite products, so no logarithm or division by a vanishing factor is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
