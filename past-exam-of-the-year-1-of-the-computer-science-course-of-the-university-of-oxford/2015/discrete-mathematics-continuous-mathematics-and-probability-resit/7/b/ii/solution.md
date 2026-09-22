<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $D=1-(1-p)(1-q)=p+q-pq$. By the [law of total probability](../../../../../../law-of-total-probability.md),

$$
\begin{aligned}
\mathbb P(Y=k)
&=\sum_{n=k}^{\infty}p(1-p)^n\binom nkq^k(1-q)^{n-k}\\
&=p[(1-p)q]^k\sum_{n=k}^{\infty}\binom nk[(1-p)(1-q)]^{n-k}.
\end{aligned}
$$

For $0\leq t<1$, termwise differentiation of the [geometric series](../../../../../../geometric-series.md), valid inside its [radius of convergence](../../../../../../radius-of-convergence.md), gives

$$
\sum_{n=k}^{\infty}\binom nk t^{n-k}
=\frac1{k!}\frac{d^k}{dt^k}\frac1{1-t}
=\frac1{(1-t)^{k+1}}.
$$

Taking $t=(1-p)(1-q)$ therefore yields

$$
\boxed{\mathbb P(Y=k)=\frac pD\left(\frac{(1-p)q}{D}\right)^k,\qquad k\geq0.}
$$

Since $D-p=(1-p)q$, this is the zero-based [geometric distribution](../../../../../../geometric-distribution.md) with parameter

$$
\boxed{p_* =\frac{p}{p+q-pq},\qquad \mathbb P(Y=k)=p_*(1-p_*)^k.}
$$

This illustrates [Bernoulli thinning of a geometric count](../../../../../../geometric-count-under-bernoulli-thinning.md). Here $0<p_*<1$, as $0<p,q<1$.

For the reverse [conditional distribution](../../../../../../conditional-distribution.md), [Bayes' theorem](../../../../../../bayes-theorem.md) gives, for $n\geq k$,

$$
\begin{aligned}
\mathbb P(X=n\mid Y=k)
&=\frac{p(1-p)^n\binom nkq^k(1-q)^{n-k}}
{p[(1-p)q]^k/D^{k+1}}\\
&=\binom nk[(1-p)(1-q)]^{n-k}D^{k+1}.
\end{aligned}
$$

Thus

$$
\boxed{\mathbb P(X=n\mid Y=k)=h_{n,k}(r),\qquad r=D=p+q-pq.}
$$

For $n<k$ the [conditional probability](../../../../../../conditional-probability.md) is zero. The [conditional distribution](../../../../../../conditional-distribution.md) of $X-k$ is the failure-count form of a [negative binomial distribution](../../../../../../negative-binomial-distribution.md), with $k+1$ successes and success parameter $r$: the [geometric-binomial posterior is shifted negative binomial](../../../../../../geometric-binomial-posterior-is-shifted-negative-binomial.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
