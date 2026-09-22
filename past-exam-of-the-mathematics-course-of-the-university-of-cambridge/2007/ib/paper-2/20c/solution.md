<h1 id="20c/solution">Solution</h1>

↑ **Parent:** [20C](../20c.md)

Let $G_0,G_1,\ldots$ be independent with $\Pr(G_n=j)=qp^j$ for $j\ge0$. The transition law is realized by the [geometric-arrival single-service queue](../../../../../geometric-arrival-single-service-queue.md)

$$
X_{n+1}=\max(X_n-1,0)+G_n.
$$

The chain is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md): repeated zero arrivals reach zero from every state, and any state can be reached from zero in one step. It is an [aperiodic Markov chain](../../../../../aperiodic-markov-chain.md) because the zero state has self-transition probability $q>0$.

Starting with one customer, serve one customer per step and regard the arriving customers as that customer's offspring. The number of steps until the queue empties is the total progeny of a [Galton-Watson process](../../../../../galton-watson-process.md) with offspring [probability generating function](../../../../../probability-generating-function.md)

$$
g(s)=\frac q{1-ps},\qquad m=g'(1)=\frac pq.
$$

Here is the extinction argument needed for recurrence. The probability of extinction by generation $n$ is $g^{\circ n}(0)$: condition on the first generation and iterate. These probabilities increase to the smallest fixed point in $[0,1]$. The fixed-point equation $s=q/(1-ps)$ has roots $1$ and $q/p$. Thus the queue started at one hits zero almost surely when $p\le q$, but with probability only $q/p<1$ when $p>q$.

If $p\le q$, every finite initial queue empties almost surely, since it represents finitely many family trees. Starting from zero, the first step gives a finite $G_0$, so the return probability to zero is one. If $p>q$, the first step has positive probability of producing one customer, whose probability of never emptying is positive; thus the return probability is below one. Communication in this [irreducible Markov chain](../../../../../irreducible-markov-chain.md) then makes every state a [transient state](../../../../../transient-state.md).

For $p\le q$, the expected total progeny from one customer is

$$
\sum_{n=0}^\infty E Z_n=\sum_{n=0}^\infty m^n,
$$

since conditioning on a generation gives $E Z_{n+1}=mE Z_n$. Nonnegativity justifies interchanging the expectation and sum. For $p<q$ this equals $1/(1-m)$. After the first step from zero the mean number of initial customers is $E G_0=m$, so the mean return time is

$$
E_0\tau_0^+=1+\frac m{1-m}=\frac q{q-p}<\infty.
$$

The chain is therefore [positive recurrent](../../../../../positive-recurrent-markov-chain.md). At $p=q=1/2$ extinction still occurs almost surely, but the expected progeny, and hence the mean return time, is infinite. The chain is [null recurrent](../../../../../null-recurrent-state.md).

For the [stationary distribution](../../../../../stationary-distribution.md) in the positive recurrent case, let $\Pi(z)=\sum_{j\ge0}\pi_jz^j$. Stationarity and the transition realization imply

$$
\Pi(z)=\frac q{1-pz}\left[\pi_0+\frac{\Pi(z)-\pi_0}{z}\right].
$$

Multiplying through and factoring gives

$$
(z-1)(q-pz)\Pi(z)=q\pi_0(z-1),\qquad
\Pi(z)=\frac{q\pi_0}{q-pz}.
$$

Normalization $\Pi(1)=1$ yields $\pi_0=(q-p)/q$. Expanding the [geometric series](../../../../../geometric-series.md) gives the complete classification and invariant probabilities:

$$
\boxed{\begin{array}{ll}
0<p<1/2:&\text{positive recurrent},\quad
\pi_j=(1-p/q)(p/q)^j,\quad j\ge0;\\
p=1/2:&\text{null recurrent};\\
1/2<p<1:&\text{transient}.
\end{array}}
$$

For $p\ge q$ the ratio $p/q$ cannot define a summable probability distribution, consistently with the absence of a stationary probability law. The displayed recurrence proof distinguishes the critical null recurrent case from the transient case; failure of normalizability alone would not do so.

## ↑ Ancestors (10)

1. [20C](../20c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
