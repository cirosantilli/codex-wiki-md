<h1 id="12e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K$ be the set where the [indicator function](../../../../../../indicator-function.md) $f$ equals one. Fix a positive integer $N$. Each permitted length-$N$ decimal prefix $w=(w_1,\ldots,w_N)\in\{2,7\}^N$ gives the interval

$$
I_w=[t_w,t_w+10^{-N}],\qquad t_w=\sum_{j=1}^Nw_j10^{-j}.
$$

There are $2^N$ such intervals, each of length $10^{-N}$, and they cover $K$. Every point of $K$ is strictly inside the interval for its prefix, since its remaining tail lies between $2/(9\cdot10^N)$ and $7/(9\cdot10^N)$. Thus none of the interval endpoints belongs to $K$. The intervals are disjoint and separated: their distinct prefix integers cannot be consecutive because their final digits are only $2$ and $7$.

The complement consists of finitely many closed intervals on which $f=0$, of total length $1-2^N10^{-N}=1-5^{-N}$. Part (b) therefore already proves [Riemann integrability](../../../../../../riemann-integrable-function.md), since this length tends to one.

To compute the [Riemann integral](../../../../../../riemann-integral.md) directly, make a [partition of an interval](../../../../../../partition-of-an-interval.md) using $0,1$ and all the endpoints of the $I_w$. On complementary cells the upper [Darboux sum](../../../../../../darboux-sum.md) contribution is zero, and on the $I_w$ it is at most their total length. Moreover every nonempty cell contains a terminating decimal, which is not in $K$: neither its terminating expansion with a zero tail nor its alternative expansion with a nine tail consists entirely of twos and sevens. Such decimals are dense, so every cell has infimum zero. Therefore

$$
0=L(f,P_N)\le\int_0^1f(x)\,dx\le U(f,P_N)\le5^{-N}.
$$

Letting $N\to\infty$ gives **the exact answer**

$$
\boxed{\int_0^1f(x)\,dx=0.}
$$

This is an example of an [indicator of a restricted-digit decimal set](../../../../../../indicator-of-a-restricted-digit-decimal-set.md): infinitely many, indeed uncountably many, points can support an [indicator function](../../../../../../indicator-function.md) whose [Riemann integral](../../../../../../riemann-integral.md) is zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12E](../../12e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
