<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $1\leq k\leq n$, the [nearest neighbour distance](../../../../../nearest-neighbour-distance.md) $\rho_{(k)}(x)$ is the $k$th [order statistic](../../../../../order-statistic.md) of $D_i=|X_i-x|$. Each $D_i$ has continuous [distribution function](../../../../../cumulative-distribution-function.md) $p_x(r)$ on $[0,\infty)$. The [probability integral transform](../../../../../probability-integral-transform.md) makes $U_i=p_x(D_i)$ [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$. Monotonicity of $p_x$ gives $P=U_{(k)}$, a [uniform order statistic](../../../../../uniform-order-statistic.md). Strict monotonicity is not needed at this stage.

For $0<s<1$, counting observations below $s$ gives

$$
\mathbb P(P\leq s)=\sum_{j=k}^n\binom nj s^j(1-s)^{n-j}.
$$

Differentiating and cancelling consecutive terms gives the [Beta distribution](../../../../../beta-distribution.md):

$$
\boxed{f_P(s)=\frac{n!}{(k-1)!(n-k)!}s^{k-1}(1-s)^{n-k},\qquad 0<s<1.}
$$

The [Gamma function](../../../../../gamma-function.md) identity $\Gamma(j)=(j-1)!$ identifies this with the stated normalization. Ratios of [Beta function](../../../../../beta-function.md) integrals yield the [moments](../../../../../moment.md)

$$
\boxed{\mathbb EP=\frac{k}{n+1},\qquad \mathbb EP^2=\frac{k(k+1)}{(n+1)(n+2)}.}
$$

This is the [probability content of a nearest neighbour ball](../../../../../probability-content-of-a-nearest-neighbour-ball.md) identity, specialized to intervals on the real line.

Now write $f_0=f(x)>0$. The [Lipschitz bound](../../../../../lipschitz-bound.md) gives

$$
|p_x(r)-2rf_0|
=\left|\int_{-r}^r\{f(x+u)-f_0\}\,du\right|
\leq L\int_{-r}^r|u|\,du=Lr^2.
$$

Thus

$$
\boxed{|p_x(r)-2rf(x)|\leq Lr^2.}
$$

Strict positivity of the [probability density function](../../../../../probability-density-function.md) makes $p_x$ continuous and strictly increasing from zero to one, so its [inverse function](../../../../../inverse-function.md) is defined for every $s\in(0,1)$.

For the requested conditional calculation, suppose $f_0^2\geq L$. At $r_0=s/f_0$ the preceding bound gives

$$
p_x(r_0)\geq2s-\frac{Ls^2}{f_0^2}\geq2s-s^2\geq s.
$$

Therefore $r=p_x^{-1}(s)\leq s/f_0$, and substituting in the approximation proves the [inverse probability content bound for a Lipschitz density](../../../../../inverse-probability-content-bound-for-a-lipschitz-density.md):

$$
\boxed{|2f(x)p_x^{-1}(s)-s|\leq\frac{Ls^2}{f(x)^2}.}
$$

The same argument works, without $f_0^2\geq L$, on the meaningful local range $0<s<1$ with $s\leq f_0^2/L$.

Since the [nearest neighbour density estimator](../../../../../nearest-neighbour-density-estimation.md) obeys $f(x)/\widehat f_{(k)}(x)=2(n+1)f_0p_x^{-1}(P)/k$, its conditional bound follows from the [Beta distribution](../../../../../beta-distribution.md) [moments](../../../../../moment.md):

$$
\begin{aligned}
\left|\mathbb E\left[\frac{f(x)}{\widehat f_{(k)}(x)}\right]-1\right|
&=\frac{n+1}{k}\left|\mathbb E\{2f_0p_x^{-1}(P)-P\}\right|\\
&\leq\frac{n+1}{k}\frac L{f_0^2}\mathbb EP^2
=\frac L{f_0^2}\frac{k+1}{n+2}.
\end{aligned}
$$

Hence, under the printed location condition,

$$
\boxed{\left|\mathbb E\left[\frac{f(x)}{\widehat f_{(k)}(x)}\right]-1\right|\leq\frac{k+1}{n+2}.}
$$

The conditional [inverse function](../../../../../inverse-function.md) bound also bounds $p_x^{-1}(P)$, so the [expected value](../../../../../expected-value.md) in this calculation is finite under those formal hypotheses.

There is, however, a genuine flaw in the original PDF: **the printed condition $f(x)\geq\sqrt L$ has no admissible points when $f$ is strictly positive on all of $\mathbb R$**. A [probability density function](../../../../../probability-density-function.md) on all of $\mathbb R$ cannot have [Lipschitz constant](../../../../../lipschitz-constant.md) zero, so $L>0$. Its [Lipschitz bound](../../../../../lipschitz-bound.md) forces

$$
f(x+u)\geq\max\{f_0-L|u|,0\}.
$$

Integrating this triangular lower envelope gives the [Lipschitz density height bound](../../../../../lipschitz-density-height-bound.md)

$$
1=\int_{\mathbb R}f(y)\,dy>\int_{-f_0/L}^{f_0/L}(f_0-L|u|)\,du=\frac{f_0^2}{L}.
$$

The inequality is strict because the [probability density function](../../../../../probability-density-function.md) has positive mass outside the finite interval. Thus $f(x)<\sqrt L$ everywhere. The last two conditional conclusions above are valid implications but vacuous as printed. Dropping strict positivity gives only $f(x)\leq\sqrt L$, with equality forcing the entire [probability density function](../../../../../probability-density-function.md) to be the normalized triangular envelope. The local inverse bound does not justify replacing the printed condition by its reverse in the final [expected value](../../../../../expected-value.md) bound, since $P$ ranges over all of $(0,1)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
