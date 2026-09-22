# Integrated cumulative distribution function on a bounded interval

↑ **Parent:** [Cumulative distribution function](cumulative-distribution-function.md)

If a [random variable](random-variable-split.md) $X$ takes values in $[l,r]$, its [cumulative distribution function](cumulative-distribution-function.md) $F_X$ satisfies

$$
\boxed{\int_l^r F_X(t)\,dt=r-\mathbb E[X].}
$$

Indeed $\int_l^r\mathbf1_{\{X\leq t\}}\,dt=r-X$ for every outcome. Taking [expected values](expected-value-split.md) and using [Tonelli's theorem](tonelli-theorem.md) proves the formula, including when the [probability distribution](probability-distribution-split.md) has atoms. For a [probability density function](probability-density-function.md) $f_X$, the same proof reverses the order in $\int_l^r\int_l^t f_X(x)\,dx\,dt=\int_l^r(r-x)f_X(x)\,dx$. Thus $F_X(t)/(r-\mathbb E[X])$, restricted to $[l,r]$, is a [probability density function](probability-density-function.md) whenever $\mathbb E[X]<r$. The reflected construction using $1-F_X(t)$ has normalising constant $\mathbb E[X]-l$ and is closely related to an [integrated tail distribution](integrated-tail-distribution.md).

## ↑ Ancestors (7)

1. [Cumulative distribution function](cumulative-distribution-function.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/16/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/14/d/solution.md)
