<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

A [binary symmetric channel](../../../../../binary-symmetric-channel.md) flips each transmitted bit independently with probability $p$. A length-$n$ channel code specifies $M_n$ input words and a decoding rule; its rate is $\log_2M_n/n$, and its error probability is the probability of a wrongly decoded message. The [channel capacity](../../../../../channel-capacity.md) is the supremum of asymptotically achievable rates with vanishing error. For $0\leq p\leq1$, put $h_2(p)=-p\log_2p-(1-p)\log_2(1-p)$, with $0\log_20=0$. The [Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) here states

$$
\boxed{C=1-h_2(p)\quad\text{bits per channel use}.}
$$

We prove achievability and the converse rather than using the formula as a substitute for a coding argument. Output complementation reduces $p>1/2$ to $1-p$, so first assume $0<p<1/2$.

Fix $R<C$. Choose $\delta>0$ such that $q=p+\delta<1/2$ and $R<1-h_2(q)$. Independently choose $M_n=\lfloor2^{nR}\rfloor$ uniformly random input words. Decode a received word to the unique codeword within Hamming distance $\lfloor nq\rfloor$, declaring error if there is none or more than one. The [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) says the empirical fraction of independent Bernoulli-$p$ errors tends in probability to $p$, so exceeding this distance has probability tending to zero.

For any independently chosen competing codeword, its probability of lying in this ball is $2^{-n}B_n(q)$, where

$$
B_n(q)=\sum_{j\leq nq}\binom nj\leq(n+1)2^{nh_2(q)}.
$$

Indeed $\binom nj\leq2^{nh_2(j/n)}$ follows by bounding the probability of exactly $j$ successes in a binomial experiment with parameter $j/n$ by one, and $h_2$ increases on $[0,1/2]$. A union bound therefore bounds the ensemble-average decoding error by

$$
\mathbb P\{\operatorname{Bin}(n,p)>nq\}+
(n+1)2^{-n(1-h_2(q)-R)}\longrightarrow0.
$$

Some deterministic code is at least as good as this average. Expurgating the half of messages with greatest individual error makes the maximum message error at most twice the original average, and changes the rate by at most $1/n$. This proves achievability even for maximum-error probability.

For the converse, take uniform messages and any deterministic code/decoder. The independent noise word $Z$ has probability $p^{|Z|}(1-p)^{n-|Z|}$. Its normalized negative log-probability tends in probability to $h_2(p)$ by the same law. Thus, outside an event of probability tending to zero, each noise word has probability at most $2^{-n(h_2(p)-\delta)}$. The decoder's disjoint decision regions $D_j$ contain at most $2^n$ received words in total. Hence

$$
P_{\rm success}\leq o(1)+\frac1{M_n}\sum_j|D_j|2^{-n(h_2(p)-\delta)}
\leq o(1)+2^{n(1-R_n-h_2(p)+\delta)}.
$$

At rates bounded above capacity by a positive amount, choose smaller $\delta$ and obtain success probability tending to zero. This establishes the strong converse as well as the ordinary impossibility of reliable transmission above $C$.

When $p=1/2$ the output is independent of the input, so success probability for uniform messages is at most $1/M_n$ and $C=0$. At $p=0$ or $1$ the channel is noiseless or deterministically inverted; all $2^n$ words can be distinguished, so $C=1$. These endpoints complete the theorem.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
