# Asymptotic sequence

↑ **Parent:** [Asymptotic expansion](asymptotic-expansion-split.md)

An [asymptotic sequence](asymptotic-sequence.md) orders the scales against which successive errors are compared. On a specified domain approaching $x_0$, suppose each $\phi_n$ is nonzero sufficiently close to the [limit](limit-of-a-function.md) and

$$
\frac{\phi_{n+1}(x)}{\phi_n(x)}\longrightarrow0.
$$

Equivalently, $\phi_{n+1}=o(\phi_n)$ in [little o notation](little-o-notation.md). The notation

$$
f\sim\sum_{n\geq0}a_n\phi_n
$$

means that for every $N\geq0$,

$$
f-\sum_{n=0}^Na_n\phi_n=o(\phi_N).
$$

Each $N$ stays fixed while the parameter tends to its [limit](limit-of-a-function.md).[NIST Digital Library of Mathematical Functions, §2.1(v), generalized asymptotic scales and expansions](nist-digital-library-of-mathematical-functions/2-1-definitions-and-elementary-properties.md)

As $z\to+\infty$, $1,z^{-1},z^{-2},\ldots$ is an [asymptotic sequence](asymptotic-sequence.md), because each adjacent ratio is $1/z$. Fractional scales $1,z^{-1/2},z^{-1},\ldots$ work too, with ratio $z^{-1/2}$. By contrast, $1,1+z^{-1},z^{-1},\ldots$ fails at its first pair: the second scale is not smaller than the first. Ordering by written position alone does not create a hierarchy of sizes.

Successive division of the remainder by $\phi_N$ uniquely recovers every [coefficient](coefficient.md):

$$
a_N=\lim_{x\to x_0}
\frac{f(x)-\sum_{n=0}^{N-1}a_n\phi_n(x)}{\phi_N(x)}.
$$

If two proposed expansions first differ at order $N$, subtracting them and dividing by $\phi_N$ would give a nonzero constant tending to zero, a contradiction. This is uniqueness of the [coefficients](coefficient.md) in a fixed scale, not uniqueness of the represented [function](function-split.md).

For the factorial [integral](integral-split.md) example, the first three limiting responses are $\lim F(z)=1$, $\lim z(F(z)-1)=-1$, and $\lim z^2(F(z)-1+z^{-1})=2$. They extract exactly the coefficients $1,-1,2!$. Choosing an [asymptotic sequence](asymptotic-sequence.md) therefore turns “the next small correction” into a precise and reusable operation.

**Table of contents**

- [Harmonic-mean refinement of an asymptotic sequence](harmonic-mean-refinement-of-an-asymptotic-sequence.md)
- [Geometric-mean refinement of an asymptotic sequence](geometric-mean-refinement-of-an-asymptotic-sequence.md)
- [Termwise equivalent asymptotic scales need not preserve expansions](termwise-equivalent-asymptotic-scales-need-not-preserve-expansions.md)

## ↑ Ancestors (5)

1. [Asymptotic expansion](asymptotic-expansion-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Asymptotic expansion](asymptotic-expansion-split.md)
- [Asymptotic power series](asymptotic-power-series.md)
- [Asymptotic sequence](asymptotic-sequence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/31d/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/31d/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/32a/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/32e/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/32e/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/32c/a/solution.md)
