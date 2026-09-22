<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

For the natural [filtration](../../../../../filtration-probability-theory.md) $\mathcal F_n=\sigma(X_0,\ldots,X_n)$, a [stopping time](../../../../../stopping-time.md) $T$ takes values in $\{0,1,\ldots\}\cup\{\infty\}$ and satisfies $\{T\le n\}\in\mathcal F_n$ for each $n$. Whether it has occurred by time $n$ can be decided from the observations through that time.

The [Strong Markov property](../../../../../strong-markov-property.md) for a time-homogeneous [Markov chain](../../../../../markov-chain.md) says that, on $\{T<\infty\}$, conditional on $\mathcal F_T$, the process $(X_{T+r})_{r\ge0}$ has the law of a fresh chain started at $X_T$. In particular its future conditional law depends on the past only through $X_T$. For example $\mathbb P(X_{T+r}=j\mid\mathcal F_T)=(P^r)_{X_Tj}$ on that event, and the corresponding statement holds for every finite future path.

Start at $i$ and let $T_0=0$, $T_{r+1}=\inf\{n>T_r:X_n=i\}$, with $\inf\varnothing=\infty$. These are [stopping times](../../../../../stopping-time.md). Put $f=\mathbb P_i(T_1<\infty)$. Each finite return restarts the chain at $i$, so the [Strong Markov property](../../../../../strong-markov-property.md) gives inductively

$$
\mathbb P_i(T_r<\infty)=f^r.
$$

The events decrease as $r$ increases; infinitely many visits occur exactly when every return time is finite. Continuity of probability therefore gives

$$
\boxed{\mathbb P_i(\text{infinitely many visits to }i)=\lim_{r\to\infty}f^r
=\begin{cases}0,&f<1,\\1,&f=1.\end{cases}}
$$

No irreducibility assumption is needed for this zero-one conclusion at the starting state.

Let $N=\sum_{n\ge0}\mathbf1_{\{X_n=i\}}$, counting the initial visit. Summing nonnegative random variables and then using the tail-sum identity gives

$$
\sum_{n\ge0}\mathbb P_i(X_n=i)=\mathbb E_iN
=\sum_{r\ge0}\mathbb P_i(N\ge r+1)=\sum_{r\ge0}f^r.
$$

If $f<1$, this is $1/(1-f)<\infty$. Thus [divergence](../../../../../divergence.md) of the given sum forces $f=1$, and **infinitely many visits then occur with probability one**. This proves the [recurrence criterion by return probabilities](../../../../../recurrence-criterion-by-return-probabilities.md) directly from the regeneration at return times; divergent probability sums alone would not suffice for arbitrary dependent events.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
