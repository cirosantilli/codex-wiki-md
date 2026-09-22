<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [exponential distribution](../../../../../../../exponential-distribution.md) with rate $\beta>0$ has [moment-generating function](../../../../../../../moment-generating-function.md) $\beta/(\beta-t)$ for $t<\beta$. Shifting it by $\alpha$ multiplies the [moment-generating function](../../../../../../../moment-generating-function.md) by $e^{\alpha t}$. Therefore the [shifted-exponential Poisson mixture](../../../../../../../shifted-exponential-poisson-mixture.md) has [probability generating function](../../../../../../../probability-generating-function.md)

$$
\boxed{G_N(z)=e^{\alpha(z-1)}\frac{\beta}{\beta+1-z}.}
$$

The [probability generating function](../../../../../../../probability-generating-function.md) converges and is analytic for $|z|<\beta+1$, and in particular is finite for real $0\le z<\beta+1$.

Write $p=\beta/(\beta+1)$ and $q=1/(\beta+1)$, so $p+q=1$. The factor $e^{\alpha(z-1)}$ is the [probability generating function](../../../../../../../probability-generating-function.md) of $V\sim\operatorname{Poisson}(\alpha)$, while $p/(1-qz)$ is that of a [geometric distribution](../../../../../../../geometric-distribution.md) on $\{0,1,\ldots\}$, with $\mathbb P(W=j)=pq^j$. Choose $V$ and $W$ independently. The product rule for the [probability generating function](../../../../../../../probability-generating-function.md) of a sum of independent counts then proves $N\overset d=V+W$. The support-zero convention for $W$ is essential here.

The [convolution of independent random variables](../../../../../../../convolution-of-independent-random-variables.md) gives the finite sum

$$
\boxed{p_n=e^{-\alpha}\frac{\beta}{\beta+1}\sum_{k=0}^{n}\frac{\alpha^k}{k!}(\beta+1)^{-(n-k)},\qquad n\ge0.}
$$

Taking the logarithmic derivative of the [probability generating function](../../../../../../../probability-generating-function.md) gives

$$
\frac{G_N'(z)}{G_N(z)}=\alpha+\frac1{\beta+1-z},
\qquad
(\beta+1-z)G_N'(z)=\{1+\alpha(\beta+1)-\alpha z\}G_N(z).
$$

Compare coefficients of $z^{n-1}$, for $n\ge2$. The left side is $(\beta+1)np_n-(n-1)p_{n-1}$, and the right side is $\{1+\alpha(\beta+1)\}p_{n-1}-\alpha p_{n-2}$. Hence the [shifted-exponential Poisson count recursion](../../../../../../../shifted-exponential-poisson-count-recursion.md) is

$$
\boxed{p_n=\frac{n+\alpha(\beta+1)}{n(\beta+1)}p_{n-1}-\frac{\alpha}{n(\beta+1)}p_{n-2},\qquad n\ge2.}
$$

The constant and linear coefficients supply the starting values

$$
p_0=e^{-\alpha}\frac{\beta}{\beta+1},\qquad
p_1=\left(\alpha+\frac1{\beta+1}\right)p_0.
$$

These two values determine every subsequent [probability](../../../../../../../probability.md) by the recursion. The negative second term does not mean that the distribution has negative probabilities: the convolution formula exhibits every $p_n$ as a sum of nonnegative quantities.

At $\alpha=0$ the independent [Poisson distribution](../../../../../../../poisson-distribution.md) component is identically zero and the count has a [geometric distribution](../../../../../../../geometric-distribution.md). Both the finite sum and the recursion reduce to $p_n=q p_{n-1}$. Consequently the [Panjer claim-count class](../../../../../../../panjer-claim-count-class.md) parameters are

$$
\boxed{a=\frac1{\beta+1},\qquad b=0.}
$$

Although the shifted model initially has positive $\alpha$, this zero-shift boundary case is well defined.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
