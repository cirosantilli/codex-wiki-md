<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A radius-$r$ Hamming decoder outputs the unique codeword within distance $r$ of the received word, if there is one. Ambiguous cases and absent candidates can be declared errors, or assigned arbitrarily for an error bound. The average error is the mean of the conditional error probabilities over the equally likely transmitted messages.

Let $V_n(r)=\sum_{j=0}^r\binom nj$ be the size of a [Hamming ball](../../../../hamming-ball.md). For any transmitted random codeword, the channel noise weight is $U\sim\operatorname{Bin}(n,p)$. Decoding can fail only if $U>r$ or another codeword lies within distance $r$ of the output. Conditional on the output, each independently sampled competing codeword is still uniform on the whole word space, so has probability $2^{-n}V_n(r)$ of lying in that ball. A [union bound](../../../../boole-s-inequality.md) yields

$$
\boxed{\mathbb E_{\mathcal A}\bar e(\mathcal A)\le(2M-1)2^{-n}V_n(r)+P(U>r)}.
$$

This is an average over the random code construction as well as over messages and noise. It implies existence of at least one deterministic codebook with average error no greater than this bound, rather than asserting the same inequality for every randomly sampled book.

Choose a target rate $R<1-h(p)$ and a small $\delta>0$ such that $p+\delta<1/2$ and $R<1-h(p+\delta)$. Let $M_n=\lfloor2^{nR}\rfloor$ and $r=\lfloor n(p+\delta)\rfloor$. The standard Hamming-volume estimate is $V_n(r)\le2^{nh(r/n)}$: for $s=r/n\le1/2$, each binomial probability term $s^j(1-s)^{n-j}$ with $j\le r$ is at least $s^r(1-s)^{n-r}$, and summing proves this bound. Thus the union-bound term decays exponentially, while $P(U>r)\to0$ by the [law of large numbers](../../../../law-of-large-numbers.md) or a [Chernoff bound](../../../../chernoff-bound.md).

There exists a $2M_n$-message book with average error $\varepsilon_n\to0$. At least half its messages have individual error at most $2\varepsilon_n$, by [Markov's inequality](../../../../markov-s-inequality.md) on the uniformly chosen message. Keep $M_n$ of these and discard the rest. Restricting the decoder's candidate set cannot spoil a previously unique successful decoding. The retained book therefore has maximum error at most $2\varepsilon_n\to0$. For large $n$ its retained codewords must be distinct: identical words could not both have conditional error below one half. This [expurgation of a codebook](../../../../expurgation-of-a-codebook.md) proves reliable communication at every rate below $1-h(p)$, while converting an average-error estimate into the requested maximum-error conclusion.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
