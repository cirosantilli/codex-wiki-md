# Inverse transform sampling

↑ **Parent:** [Quantile function](quantile-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_transform_sampling)

If $U$ has a [uniform distribution](continuous-uniform-distribution.md) on $(0,1)$ and $Q$ is the [quantile function](quantile-function.md) of a [cumulative distribution function](cumulative-distribution-function.md) $F$, then $Q(U)$ has the desired [probability distribution](probability-distribution-split.md). Indeed, [right continuity](right-continuous-function.md) gives

$$
Q(p)\leq x\quad\Longleftrightarrow\quad p\leq F(x),\qquad 0<p<1,
$$

so $\mathbb P(Q(U)\leq x)=\mathbb P(U\leq F(x))=F(x)$. This short argument works for both jumps and smooth [cumulative distribution functions](cumulative-distribution-function.md). MIT's continuous-probability notes introduce the inverse-transformation construction. [MIT 9.07, inverse transformation method](https://ocw.mit.edu/courses/9-07-statistics-for-brain-and-cognitive-science-fall-2016/6dcc172f428fbfbded912ca8862ea340_MIT9_07F16_lec3.pdf).

For the three-value example, send $U\leq0.2$ to $0$, $0.2<U\leq0.7$ to $1$, and $U>0.7$ to $3$. These [intervals](interval-mathematics.md) have exactly the desired widths $0.2$, $0.5$, $0.3$. For the density example, output $\sqrt U$: for $0\leq y\leq1$, $\mathbb P(\sqrt U\leq y)=\mathbb P(U\leq y^2)=y^2$. Independent uniform draws give [independent random variables](independent-random-variables.md) after this deterministic transformation. This direction of construction works even when $F$ has jumps; applying the [probability integral transform](probability-integral-transform.md) in the other direction requires its own continuity hypotheses.

**Table of contents**

- [Recycling a uniform random variable after discrete sampling](recycling-a-uniform-random-variable-after-discrete-sampling.md)

## ↑ Ancestors (7)

1. [Quantile function](quantile-function.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Arcsine quantiles and moments](arcsine-quantiles-and-moments.md)
- [Laplace prior for sparse images](laplace-prior-for-sparse-images.md)
- [Pareto tail conditional scaling](pareto-tail-conditional-scaling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/2/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/12f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/3f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/26k/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/28k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/28l/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-207/4/a/solution.md)
- [Probability distribution](probability-distribution-split.md)
- [Probability integral transform](probability-integral-transform.md)
- [Quantile endpoint at probability one](quantile-endpoint-at-probability-one.md)
- [Quantile function](quantile-function.md)
- [Rayleigh radial thresholds and quantiles](rayleigh-radial-thresholds-and-quantiles.md)
- [Sampling a discrete uniform distribution](sampling-a-discrete-uniform-distribution.md)
- [Sign-truncated normal sampling](sign-truncated-normal-sampling.md)
- [Triangular distribution](triangular-distribution.md)
- [Uniform random variable](uniform-random-variable.md)
