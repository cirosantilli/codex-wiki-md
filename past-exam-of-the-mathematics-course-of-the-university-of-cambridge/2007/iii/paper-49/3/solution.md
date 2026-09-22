<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A nondegenerate [distribution function](../../../../../cumulative-distribution-function.md) $G$ is a [max-stable distribution](../../../../../max-stable-distribution.md) if, for every integer $r\geq1$, there are $a_r>0$ and $b_r\in\mathbb R$ such that

$$
G(a_rx+b_r)^r=G(x)\qquad(x\in\mathbb R).
$$

Equivalently, the suitably centered and positively scaled [sample maximum](../../../../../sample-maximum.md) of $r$ [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with law $G$ again has law $G$. The [extremal types theorem](../../../../../extremal-types-theorem.md) states that every nondegenerate limiting law of normalized [sample maxima](../../../../../sample-maximum.md) is a [max-stable distribution](../../../../../max-stable-distribution.md). Thus this property identifies all possible limiting types, although a particular starting [distribution function](../../../../../cumulative-distribution-function.md) need not admit any such limiting normalization.

The three standard types are the [Gumbel distribution](../../../../../gumbel-distribution.md)

$$
\Lambda(x)=\exp(-e^{-x}),\qquad x\in\mathbb R,
$$

the [Fréchet distribution](../../../../../frechet-distribution.md), with $\alpha>0$,

$$
\Phi_\alpha(x)=\begin{cases}0,&x\leq0,\\ \exp(-x^{-\alpha}),&x>0,\end{cases}
$$

and the [negative Weibull distribution](../../../../../negative-weibull-distribution.md), with $\alpha>0$,

$$
\Psi_\alpha(x)=\begin{cases}\exp(-(-x)^\alpha),&x<0,\\1,&x\geq0.\end{cases}
$$

They are [max-stable distributions](../../../../../max-stable-distribution.md), as follows respectively by taking $(a_r,b_r)=(1,\log r)$, $(r^{1/\alpha},0)$, and $(r^{-1/\alpha},0)$. The necessary and sufficient classification is: **$G$ is max-stable exactly when $G(x)=H((x-b)/a)$ for $a>0$, $b\in\mathbb R$, and one of these three types $H$**. A positive [affine map](../../../../../affine-map.md) sends a [max-stable distribution](../../../../../max-stable-distribution.md) to another [max-stable distribution](../../../../../max-stable-distribution.md).

For the requested threshold equivalence, set $p_n=1-F(u_n)$. By [independence](../../../../../independent-random-variables.md),

$$
\mathbb P(X_{(n)}\leq u_n)=(1-p_n)^n.
$$

If $np_n\to\tau<\infty$, then $p_n\to0$ and the expansion $\log(1-p)=-p+O(p^2)$ gives $n\log(1-p_n)\to-\tau$, since $np_n^2=(np_n)p_n\to0$. Exponentiation proves the claimed limit. Conversely, if $(1-p_n)^n\to e^{-\tau}>0$, then $p_n\to0$: any subsequence with $p_n\geq\delta>0$ would have its powers tending to zero. Taking [logarithms](../../../../../logarithm.md) now gives $-n\log(1-p_n)\to\tau$. Since $-\log(1-p)/p\to1$, including the continuous extension at $p=0$, it follows that $np_n\to\tau$. Hence

$$
\boxed{\mathbb P(X_{(n)}\leq u_n)\to e^{-\tau}\ \Longleftrightarrow\ n\{1-F(u_n)\}\to\tau.}
$$

The exceedance count $S_n$ has the [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,p_n$. For $\tau>0$ and each fixed nonnegative integer $s$, its [probability mass function](../../../../../probability-mass-function.md) satisfies

$$
\mathbb P(S_n=s)=\frac{(n)_s}{s!}p_n^s(1-p_n)^{n-s}\longrightarrow e^{-\tau}\frac{\tau^s}{s!},
$$

where $(n)_s=n(n-1)\cdots(n-s+1)$ and $(n)_0=1$. Indeed $(n)_s/n^s\to1$, $(np_n)^s\to\tau^s$, and $(1-p_n)^{n-s}\to e^{-\tau}$. If $\tau=0$, the bound $\mathbb P(S_n\geq1)\leq\mathbb ES_n=np_n\to0$ gives the degenerate [Poisson distribution](../../../../../poisson-distribution.md) at zero. Summing the finitely many terms proves, in both cases,

$$
\boxed{\mathbb P(S_n\leq k)\longrightarrow e^{-\tau}\sum_{s=0}^k\frac{\tau^s}{s!},\qquad k=0,1,2,\ldots.}
$$

This derives the needed instance of the [Poisson limit theorem](../../../../../poisson-limit-theorem.md) directly.

Finally fix $x$ with $G(x)>0$ and put $u_n=a_nx+b_n$. The assumed limit for the normalized [sample maximum](../../../../../sample-maximum.md) and the proved equivalence give $np_n\to-\log G(x)$. The second-largest [order statistic](../../../../../order-statistic.md) is at most $u_n$ exactly when at most one observation is strictly greater than $u_n$. This event identity holds even if observations have ties. Apply the preceding [Poisson limit theorem](../../../../../poisson-limit-theorem.md) with $k=1$ to obtain

$$
\boxed{\mathbb P\!\left(\frac{W_n-b_n}{a_n}\leq x\right)\longrightarrow G(x)\{1-\log G(x)\}.}
$$

The endpoint $G(x)=1$ corresponds to $\tau=0$ and is already included. This is the case $r=2$ of the [exceedance count limit for extreme order statistics](../../../../../exceedance-count-limit-for-extreme-order-statistics.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
