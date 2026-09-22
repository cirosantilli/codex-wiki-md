# Erasure-pattern counting bound for maximal decoding error

↑ **Parent:** [Binary erasure channel](binary-erasure-channel.md)

For a deterministic length-$n$ [channel code](channel-code.md) with $m>2$ messages on a [binary erasure channel](binary-erasure-channel.md) of erasure [probability](probability.md) $q$, exclude the message decoded from the all-erased output. Under a uniform choice of the other $m-1$ messages, success [probability](probability.md) is at least $1-\varepsilon_{\max}$. Conditional on an erasure pattern with $k\geq1$ unerased positions, there are at most $2^k$ output words, so average success is at most $\min\{1,2^k/(m-1)\}$. With no unerased positions it is zero.

Put $L=\log_2m-1$. The scalar bound $\min\{1,2^k/(m-1)\}\leq k/L$ is immediate for $k\geq L$. Otherwise set $r=m/2^k>2$. Since $\log_2r\leq r-1$ for $r\geq2$,

$$
L=k-1+\log_2r\leq k+r-2\leq k(r-1)<k(m-1)/2^k.
$$

The inequality $\log_2r\leq r-1$ follows because equality holds at $r=2$ and the [derivative](derivative.md) of $r-1-\log_2r$ is $1-1/(r\ln2)>0$ for $r\geq2$. Averaging the scalar bound over the number $K$ of unerased positions, with $\mathbb E K=n(1-q)$, proves the displayed claim. Thus $\varepsilon_{\max}\leq\delta<1$ implies [code rate](code-rate.md) $R\leq(1-q)/(1-\delta)+1/n$. The cases $m\leq2$ satisfy this rate bound directly.

Deterministic decoding is essential to this version: on an always-erased [channel](communication-channel.md), a randomized uniform guess has [maximal decoding error probability](maximal-decoding-error-probability.md) $1-1/m$ despite receiving no information. The usual deterministic [channel decoder](channel-decoder.md) has maximal error one when $m>1$ on that channel.

## ↑ Ancestors (7)

1. [Binary erasure channel](binary-erasure-channel.md)
2. [Discrete memoryless channel](discrete-memoryless-channel.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/3/b/solution.md)
