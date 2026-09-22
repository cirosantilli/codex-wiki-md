<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the additional copies in $Z_N$ as [independent](../../../../../../independent-random-variables.md) of the initial $T_1,\ldots,T_k$, as well as of one another. Set $r=k\lambda$. The [Cramér theorem](../../../../../../cramer-s-theorem.md) for rate-$r$ [exponential random variables](../../../../../../exponential-distribution.md) gives the [rate function](../../../../../../rate-function.md)

$$
K_r(z)=\begin{cases}rz-1-\log(rz),&z>0,\\+\infty,&z\leq0.\end{cases}
$$

Indeed their [cumulant-generating function](../../../../../../cumulant-generating-function.md) is $\log(r/(r-\theta))$ for $\theta<r$, and the maximizer in its [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) is $\theta=r-1/z$. For $Z_N/N$, replacing $N$ summands by $N-k$ does not change either the speed $N$ or this [rate function](../../../../../../rate-function.md). One can also see this directly from $N^{-1}\log\mathbb E e^{\theta Z_N}\to\log(r/(r-\theta))$ and the [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md).

The [product large-deviation principle](../../../../../../product-large-deviation-principle.md), followed by the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) under addition, now gives

$$
I_k(x)=\inf_{\substack{y\geq0,\ z>0\\y+z=x}}\{\lambda y+K_r(z)\}.
$$

For $x>0$ this is the minimum over $0<z\leq x$ of

$$
\lambda x+(r-\lambda)z-1-\log(rz).
$$

If $k>1$, its derivative with respect to $z$ is $r-\lambda-1/z$. Hence the optimum is $z=\min(x,1/[\lambda(k-1)])$, and

$$
\boxed{I_k(x)=
\begin{cases}
+\infty,&x\leq0,\\
k\lambda x-1-\log(k\lambda x),&0<x\leq\frac1{\lambda(k-1)},\\
\lambda x+\log\frac{k-1}{k},&x\geq\frac1{\lambda(k-1)}.
\end{cases}\qquad\text{speed }N.}
$$

The two expressions agree at the transition and have the same derivative $\lambda$. The minimum rate zero occurs at the typical value $x=1/(k\lambda)$. If $k=1$, the minimand is $\lambda x-1-\log(\lambda z)$, decreasing in $z$, so instead

$$
\boxed{I_1(x)=\lambda x-1-\log(\lambda x)\ (x>0),\qquad I_1(x)=+\infty\ (x\leq0).}
$$

These are [good rate functions](../../../../../../good-rate-function.md). The affine branch for $k>1$ is the [slow exponential plus an exponential sample mean](../../../../../../slow-exponential-plus-an-exponential-sample-mean.md) mechanism: the bulk ceases to carry additional excess, which instead comes from $T_1$. In particular, blindly applying the full [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) to the combined sum would be unjustified. Its limiting [cumulant-generating function](../../../../../../cumulant-generating-function.md) is $\log(r/(r-\theta))$ only for $\theta<\lambda$, with a finite boundary slope when $k>1$; [essential smoothness](../../../../../../essential-smoothness-of-a-convex-function.md) fails. The product and contraction argument proves the missing lower bounds.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
