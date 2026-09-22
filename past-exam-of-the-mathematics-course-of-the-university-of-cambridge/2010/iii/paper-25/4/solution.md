<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $e(t)=\exp(2\pi it)$ and use $\|t\|$ for [distance to the nearest integer](../../../../../distance-to-the-nearest-integer.md). The [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md), in its pigeonhole form, says that for every real $\alpha$ and integer $Q\ge1$ there are [coprime integers](../../../../../coprime-integers.md) $a,q$ with $1\le q\le Q$ and $|\alpha-a/q|\le1/(qQ)$. Indeed put the $Q+1$ [fractional parts](../../../../../fractional-part.md) of $0,\alpha,\ldots,Q\alpha$ into $Q$ equal intervals; two lie in the same interval. Their difference gives $|q\alpha-a|\le1/Q$, and reducing the fraction preserves the claimed bound. This includes rational $\alpha$.

For $t\ge s$, the [finite geometric series](../../../../../finite-geometric-series.md) has length $L=t-s+1$. When $\theta\notin\mathbb Z$,

$$
\left|\sum_{n=s}^t e(\theta n)\right|
=\left|\frac{e(\theta s)(1-e(L\theta))}{1-e(\theta)}\right|
\le\frac1{|\sin\pi\theta|}\le\frac1{2\|\theta\|}.
$$

The last inequality uses the concavity of sine on $[0,\pi/2]$. The triangle inequality also gives $L$. At integer $\theta$ the sum has absolute value $L$, interpreting the reciprocal as infinity. Thus the precise [exponential geometric sum bound](../../../../../exponential-geometric-sum-bound.md) is

$$
\boxed{\left|\sum_{n=s}^t e(\theta n)\right|\le\min\left(L,\frac1{2\|\theta\|}\right).}
$$

The interval must be nonempty; for $t<s$ its sum is zero and its length should be defined as $\max(0,t-s+1)$, rather than using a potentially negative bound.

For the separated points, assume $Q\ge2$ and $\delta>0$. An arc of length $2r\le1$ contains at most $1+2r/\delta$ of the points, by ordering them along the arc. Points with $\|\theta_i\|\le1/Q$ contribute $O(Q+\delta^{-1})$. In the dyadic annulus $2^j/Q<\|\theta_i\|\le2^{j+1}/Q$, each summand is $O(Q2^{-j})$ and there are at most $1+2^{j+2}/(Q\delta)$ points. There are $O(\log(2Q))$ nonempty annuli, giving the stronger [separated reciprocal-distance sum](../../../../../separated-reciprocal-distance-sum.md)

$$
\boxed{\sum_i\min\left(Q,\frac1{2\|\theta_i\|}\right)
\ll Q+\delta^{-1}\log(2Q)
\ll(Q+\delta^{-1})\log Q.}
$$

If there is only one point the bound is immediate; otherwise $\delta\le1/2$. The printed $\log Q$ requires a lower bound away from $Q=1$; $\log(2Q)$ avoids that endpoint defect.

A useful version of the [quadratic Weyl inequality](../../../../../quadratic-weyl-inequality.md) is the following, with $(a,q)=1$, $1\le q\le Q$ and $|\alpha-a/q|\le1/(qQ)$:

$$
\boxed{\left|\sum_{n=0}^N e(\alpha n^2)\right|
\ll\left((N^2/q+N+q)\log(2N)\right)^{1/2}.}
$$

For $N\ge2$, expand the square of this [quadratic exponential sum](../../../../../quadratic-exponential-sum.md) by $h=n-m$:

$$
|S|^2=N+1+2\Re\sum_{h=1}^N e(\alpha h^2)\sum_{m=0}^{N-h}e(2\alpha hm).
$$

The [exponential geometric sum bound](../../../../../exponential-geometric-sum-bound.md) therefore gives $|S|^2\ll N+\sum_{h\le N}\min(N+1,\|2\alpha h\|^{-1})$. For $q\ge8$, partition these $h$ into blocks of length at most $\lfloor q/4\rfloor$. Two different points in one block have difference $d$ with $0<|d|<q/4$. The reduced denominator of $2a/q$ is at least $q/2$, so $\|2ad/q\|\ge1/q$, while

$$
|2d(\alpha-a/q)|\le\frac1{2Q}\le\frac1{2q}.
$$

Thus the rotations $2\alpha h$ are separated by at least $1/(2q)$ in each block. The [separated reciprocal-distance sum](../../../../../separated-reciprocal-distance-sum.md) bounds each block by $O(N+q\log(2N))$. There are $O(N/q+1)$ blocks, and hence

$$
|S|^2\ll N+(N/q+1)(N+q\log(2N))
\ll(N^2/q+N+q)\log(2N).
$$

For $q<8$ or $N<2$, the trivial bound supplies the same assertion with an absolute constant. The same proof applies to $\sum_{n=1}^N e(\alpha n^2)$, whose difference sums also have interval endpoints.

We finally prove a polynomial rate of [quantitative quadratic recurrence](../../../../../quantitative-quadratic-recurrence.md), without using the optional finite-group assumption. For $0<\varepsilon\le1/2$, use the [periodic triangular bump](../../../../../periodic-triangular-bump.md) $b(t)=(1-\|t\|/\varepsilon)_+$. It is $\varepsilon^{-1}$ times the periodic [convolution](../../../../../convolution.md) of two interval indicators, and therefore has the nonnegative [Fourier coefficients](../../../../../fourier-coefficient.md)

$$
\widehat b(0)=\varepsilon,\qquad
\widehat b(r)=\varepsilon\left(\frac{\sin(\pi r\varepsilon)}{\pi r\varepsilon}\right)^2.
$$

Its [Fourier series](../../../../../fourier-series-split.md) is absolutely convergent, $\sum_r\widehat b(r)=b(0)=1$, and the coefficient tail is $\sum_{|r|>R}\widehat b(r)\ll1/(\varepsilon R)$. Suppose that $\|\alpha n^2\|\ge\varepsilon$ for every $1\le n\le N$. Then $\sum_n b(\alpha n^2)=0$. Choose $R=\lceil C\varepsilon^{-2}\rceil$ with a sufficiently large absolute $C$, so that the contribution of frequencies $|r|>R$ has absolute value at most $N\varepsilon/2$. The zero frequency contributes $N\varepsilon$. Since all coefficients are nonnegative and their sum is one, some $1\le r\le R$ must satisfy

$$
\left|\sum_{n=1}^N e(r\alpha n^2)\right|\ge N\varepsilon/2.
$$

Apply the [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md) to $r\alpha$ with $Q=N$, obtaining a reduced $a/q$, $q\le N$. The [quadratic Weyl inequality](../../../../../quadratic-weyl-inequality.md) then implies

$$
N^2\varepsilon^2\ll(N^2/q+N)\log(2N).
$$

Set $\varepsilon=N^{-1/8}$. For sufficiently large $N$, the $N\log(2N)$ term is absorbed on the left, giving $q\ll\varepsilon^{-2}\log(2N)$. The integer $n=rq$ consequently satisfies

$$
1\le n\ll\varepsilon^{-4}\log(2N)=N^{1/2}\log(2N)<N.
$$

Moreover the approximating integer is $arq$, and

$$
\|\alpha n^2\|
\le|\alpha r^2q^2-arq|
=rq^2|r\alpha-a/q|
\le\frac{rq}N
\ll N^{-1/2}\log(2N)<\varepsilon.
$$

This contradicts the assumed avoidance. Increasing the absolute constant handles the finitely many smaller $N$, uniformly for every real $\alpha$. Thus

$$
\boxed{\min_{1\le n\le N}\|\alpha n^2\|\ll N^{-1/8}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
