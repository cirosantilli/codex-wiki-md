<h1 id="27k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here the total holding rate is

$$
q_i=-g_{ii}=3^{|i|+1},
$$

and therefore the [jump chain](../../../../../../jump-chain.md) has state-independent transitions

$$
\mathbb P(Y_{n+1}=i-1\mid Y_n=i)=\frac13,
\qquad
\mathbb P(Y_{n+1}=i+1\mid Y_n=i)=\frac23.
$$

It is an upward [biased random walk](../../../../../../biased-random-walk.md) on $\mathbb Z$. By the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md), $Y_n/n\longrightarrow1/3$ almost surely, so $Y_n\to+\infty$. The jump chain, and hence $X$, is transient.

Counting measure is invariant for this jump chain: for every $j$, its incoming mass is $1/3+2/3=1$. The [invariant-measure transfer between a jump chain and a CTMC](../../../../../../invariant-measure-transfer-between-a-jump-chain-and-a-ctmc.md) therefore gives an invariant measure proportional to $q_i^{-1}=3^{-|i|-1}$. Since

$$
\sum_{i\in\mathbb Z}3^{-|i|-1}
=\frac13+2\sum_{i=1}^{\infty}3^{-i-1}
=\frac23,
$$

the normalized [invariant distribution of a continuous-time Markov chain](../../../../../../invariant-distribution-of-a-continuous-time-markov-chain.md) is

$$
\boxed{\pi_i=\frac12\,3^{-|i|},\qquad i\in\mathbb Z.}
$$

This does not contradict transience because an [invariant distribution of an explosive chain](../../../../../../invariant-distribution-of-an-explosive-chain.md) need not imply positive recurrence.

It remains to verify [explosion](../../../../../../explosion-of-a-continuous-time-markov-chain.md). Starting from zero, the probability that the biased walk ever reaches $-k$ is $2^{-k}$. Once it reaches any state, its probability of returning after departure is

$$
\frac13\cdot1+\frac23\cdot\frac12=\frac23,
$$

so its expected total number of visits to that state, conditional on reaching it, is $1/(1-2/3)=3$. If $V_i$ is the number of visits to $i$, then

$$
\mathbb E_0V_i=
\begin{cases}
3,&i\geq0,\\
3\,2^{\,i},&i<0.
\end{cases}
$$

Consequently the expected sum of all holding times is

$$
\begin{aligned}
\mathbb E_0T_\infty
&=\sum_{i\in\mathbb Z}\frac{\mathbb E_0V_i}{q_i}\\
&=\sum_{i=0}^{\infty}\frac3{3^{i+1}}
+\sum_{k=1}^{\infty}\frac{3\,2^{-k}}{3^{k+1}}\\
&=\frac32+\frac15
=\frac{17}{10}<\infty.
\end{aligned}
$$

The nonnegative random variable $T_\infty$ is therefore finite almost surely. By [explosion by summable holding times](../../../../../../explosion-by-summable-holding-times.md), $X$ makes infinitely many jumps by time $T_\infty$, so it is explosive.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
