<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To correct every pattern of $t_N=\lfloor pN\rfloor$ errors by nearest-codeword decoding, it suffices to have [minimum Hamming distance](../../../../../../minimum-distance-of-a-code.md) $\delta_N=2t_N+1$: the corresponding radius-$t_N$ [Hamming balls](../../../../../../hamming-ball.md) are disjoint. For $0<p<1/4$, the relative distance tends to $2p<1/2$, so the [asymptotic Gilbert–Varshamov bound](../../../../../../asymptotic-gilbert-varshamov-bound.md) guarantees [code rate](../../../../../../code-rate.md) at least $1-h_2(2p)$ in the limit. Therefore its immediate strict-rate guarantee is

$$
R<1-h_2(2p).
$$

The [binary entropy](../../../../../../binary-entropy.md) is strictly increasing from zero to one on $[0,1/2]$, since $h_2'(x)=\log_2((1-x)/x)>0$ on $(0,1/2)$. Let $a=h_2^{-1}(1-R)$ denote the inverse on this interval. The asymptotic condition becomes

$$
\boxed{p<\frac12h_2^{-1}(1-R)=\frac a2.}
$$

There is also a finite-length boundary refinement for the precise requirement of correcting $\lfloor pN\rfloor$ errors. If $d/N=\theta\leq1/2$, then each weight $\theta^j(1-\theta)^{N-j}$ for $j\leq d$ is at least $\theta^d(1-\theta)^{N-d}$. Expanding $(\theta+(1-\theta))^N$ gives the [entropy bound for a Hamming ball](../../../../../../entropy-bound-for-a-hamming-ball.md)

$$
1\geq v_N(d)\theta^d(1-\theta)^{N-d},
\qquad v_N(d)\leq2^{Nh_2(d/N)}.
$$

The case $d=0$ follows directly from $v_N(0)=1$. Taking $d=2t_N$ and using [monotonicity](../../../../../../monotonic-function.md) of the [binary entropy](../../../../../../binary-entropy.md), the [Gilbert–Varshamov bound](../../../../../../gilbert-varshamov-bound.md) yields

$$
A_2(N,2t_N+1)\geq\frac{2^N}{v_N(2t_N)}
\geq2^{N(1-h_2(2p))}.
$$

Thus the [worst-case correction guarantee from the Gilbert–Varshamov bound](../../../../../../worst-case-correction-guarantee-from-the-gilbert-varshamov-bound.md) even includes $p=a/2$ for the exact radius $\lfloor pN\rfloor$, with the number of messages rounded to an integer when necessary. No positive-rate guarantee of this form is obtained for $p\geq1/4$; one must not extend the increasing-entropy calculation past $2p=1/2$. Failure of this sufficient bound does not rule out better codes.

By contrast, the [Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md) gives vanishing error probability on the [binary symmetric channel](../../../../../../binary-symmetric-channel.md) whenever

$$
\boxed{R<1-h_2(p),\quad\text{or}\quad p<h_2^{-1}(1-R)=a.}
$$

The factor of two comes from demanding disjoint correction balls for every error pattern of a prescribed weight. This is a worst-case distance requirement, and the [Gilbert–Varshamov bound](../../../../../../gilbert-varshamov-bound.md) is itself only a sufficient existence bound. The [Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md) controls the probability of decoding failure for the random channel; rare bad patterns may remain.

Finally, the number of actual errors has [binomial distribution](../../../../../../binomial-distribution.md) with mean $pN$. Correcting exactly its mean does not itself imply error probability tending to zero. To get that conclusion from the distance construction when $R<1-h_2(2p)$, choose $\varepsilon>0$ with $p+\varepsilon<1/4$ and $R<1-h_2(2(p+\varepsilon))$, and correct $\lfloor(p+\varepsilon)N\rfloor$ errors. The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) then makes the probability of exceeding the correction radius tend to zero.

<a id="3/c/image-binary-symmetric-channel-capacity-and-gilbert-varshamov-worst-case-correction-rate"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30-coding-rates.png)

**[Figure 1](#3/c/image-binary-symmetric-channel-capacity-and-gilbert-varshamov-worst-case-correction-rate). Binary symmetric channel capacity and Gilbert–Varshamov worst-case correction rate**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
