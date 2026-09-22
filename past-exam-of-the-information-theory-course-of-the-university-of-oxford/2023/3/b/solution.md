<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the standard deterministic [channel encoder](../../../../channel-encoder.md) and [channel decoder](../../../../channel-decoder.md), with $m$ message labels and [code rate](../../../../code-rate.md) $R=(\log m)/n$. The [Fano's inequality](../../../../fano-s-inequality.md) hint printed here replaces $\log(m-1)$ by $\log m-1$, which is false in general: take $X$ uniform on $\{0,1\}$ and $Y=2$ in the common [alphabet](../../../../alphabet.md) $\{0,1,2\}$. The error [probability](../../../../probability.md) is one and its [binary entropy](../../../../binary-entropy.md) is zero, so the proposed bound asserts $1\leq\log3-1<1$. The correct [Fano's inequality](../../../../fano-s-inequality.md) alone gives $(1-P_e)\log m\leq n(1-q)+h_2(P_e)$, which does not immediately give the requested additive $1/n$. The following [erasure-pattern counting bound for maximal decoding error](../../../../erasure-pattern-counting-bound-for-maximal-decoding-error.md) proves the displayed claim directly.

The case $m\leq2$ is immediate because $R\leq1/n$. Suppose $m>2$, put $L=\log m-1>0$, and let $w_0$ be the message that the [channel decoder](../../../../channel-decoder.md) returns on the all-erased output. Choose $W$ uniformly among the other $m-1$ messages. Every one of these messages is decoded correctly with [probability](../../../../probability.md) at least $1-\delta$, by the assumed [maximal decoding error probability](../../../../maximal-decoding-error-probability.md) bound.

Let $S$ be the random set of unerased coordinates and $K=|S|$. For each fixed $S$ with $K=k\geq1$, at most $2^k$ output words are possible. A deterministic [channel decoder](../../../../channel-decoder.md) can correctly identify at most one message per output word, so its conditional success [probability](../../../../probability.md), averaged over these $m-1$ messages, is at most $\min\{1,2^k/(m-1)\}$. When $K=0$, success is zero because $w_0$ was excluded.

For every integer $k\geq1$,

$$
\min\left\{1,\frac{2^k}{m-1}\right\}\leq\frac{k}{L}.
$$

If $k\geq L$, this is immediate. If $k<L$, write $r=m/2^k>2$. The elementary inequality $\log r\leq r-1$ for $r\geq2$ gives

$$
L=k-1+\log r\leq k+r-2\leq k(r-1)<\frac{k(m-1)}{2^k},
$$

where the middle inequality is $(k-1)(r-2)\geq0$. This proves the needed scalar bound.

Taking the [expectation](../../../../expected-value-split.md) over erasure patterns, and using $\mathbb E K=n(1-q)$, yields

$$
1-\delta\leq\Pr(\widehat W=W)\leq\frac{\mathbb E K}{L}
=\frac{n(1-q)}{\log m-1}.
$$

Consequently the requested bound is valid:

$$
\boxed{R=\frac{\log m}{n}\leq\frac{1-q}{1-\delta}+\frac1n.}
$$

The use of [maximal decoding error probability](../../../../maximal-decoding-error-probability.md) matters: excluding one message preserves the lower bound on success. The deterministic [channel decoder](../../../../channel-decoder.md) convention also matters; allowing independent randomized guessing would invalidate this particular finite-length claim at $q=1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
