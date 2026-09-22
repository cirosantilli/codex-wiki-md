<h1 id="12f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) states that for a random variable $Y$ with finite variance and every $\delta>0$,

$$
\mathbb P(|Y-\mathbb EY|\geq\delta)
\leq\frac{\operatorname{var}Y}{\delta^2}.
$$

Indeed, [Markov inequality](../../../../../../markov-inequality.md) applied to the nonnegative variable $(Y-\mathbb EY)^2$ gives

$$
\mathbb P((Y-\mathbb EY)^2\geq\delta^2)
\leq\frac{\mathbb E[(Y-\mathbb EY)^2]}{\delta^2}.
$$

The sum $S_n=X_1+\cdots+X_n$ has the [binomial distribution](../../../../../../binomial-distribution.md), so

$$
\boxed{
B_n(p)=
\sum_{k=0}^n f(k/n)\binom nkp^k(1-p)^{n-k}}.
$$

For fixed $n$ this is a finite sum of polynomial functions of $p$, hence is a polynomial.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
