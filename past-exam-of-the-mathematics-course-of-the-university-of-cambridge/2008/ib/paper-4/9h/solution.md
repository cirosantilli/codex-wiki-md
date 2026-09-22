<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

The [communicating classes](../../../../../communicating-class.md) are $T=\{1,2\}$, $B=\{3,4\}$ and $C=\{5,6,7\}$. The class $T$ is open: it can reach $B$ or $C$ and cannot be reached from either. To remain in $T$ for two steps has probability $1/6$, so $\mathbb P_i(X_{2k}\in T)=(1/6)^k$ for $i\in T$. Its states are [transient states](../../../../../transient-state.md). All returns within $T$ have even length and a two-step return is possible, so their [period of a state in a Markov chain](../../../../../period-of-a-state-in-a-markov-chain.md) is $2$.

The [closed communicating class](../../../../../closed-communicating-class.md) $B$ alternates deterministically between $3$ and $4$, and therefore consists of [positive recurrent states](../../../../../positive-recurrent-state.md) of period $2$. The class $C$ is finite, closed and irreducible, so its states are also [positive recurrent states](../../../../../positive-recurrent-state.md). The self-loop at $7$ gives period $1$ there, and the [period is constant on a communicating class](../../../../../period-is-constant-on-a-communicating-class.md), so every state of $C$ has period $1$.

For $C$, solve the [stationary distribution](../../../../../stationary-distribution.md) equations:

$$
\pi_5=\tfrac12\pi_7,\qquad \pi_6=\pi_5,\qquad \pi_7=\pi_6+\tfrac12\pi_7,\qquad \pi_5+\pi_6+\pi_7=1.
$$

Hence $(\pi_5,\pi_6,\pi_7)=(1/4,1/4,1/2)$. Finite irreducibility and aperiodicity imply convergence to this [stationary distribution](../../../../../stationary-distribution.md) from any state of $C$. If $h_i$ is the probability of eventually entering $C$, the [Markov property](../../../../../markov-property.md) gives

$$
h_1=\tfrac12h_2+\tfrac14,\qquad h_2=\tfrac13h_1+\tfrac16,
$$

so $h_1=2/5$ and $h_2=3/10$. Conditioning on the finite entrance time and then letting the remaining time tend to infinity proves that the limiting probabilities in $C$ are $h_i\pi_j$. The probability of entrance after a large cutoff tends to zero, which justifies this conditioning limit.

For $B$, convergence depends on the [parity balance on entry to a period-two Markov class](../../../../../parity-balance-on-entry-to-a-period-two-markov-class.md). Entry always occurs at $3$. Starting from $1$, the probabilities of first entry at time $2k+1$ and at time $2k+2$ are both $\frac14(1/6)^k$. Each parity therefore has total probability $3/10$, so both $p_{13}^{(n)}$ and $p_{14}^{(n)}$ tend to $3/10$, despite the recurrent class being periodic. Starting from $2$, the corresponding odd- and even-entry probabilities are $\frac12(1/6)^k$ and $\frac1{12}(1/6)^k$, with totals $3/5$ and $1/10$. Consequently

$$
(p_{23}^{(2k)},p_{24}^{(2k)})\longrightarrow(1/10,3/5),\qquad (p_{23}^{(2k+1)},p_{24}^{(2k+1)})\longrightarrow(3/5,1/10),
$$

so neither limit exists. From $3$ or $4$, the probabilities at $3$ and $4$ alternate between zero and one; from $C$ they are identically zero. Finally every probability of being in $T$ tends to zero, from all starting states.

All $49$ requested conclusions are encoded below, with $\ast$ denoting a nonexistent limit:

$$
\boxed{\left(\lim_{n\to\infty}p_{ij}^{(n)}\right)_{i,j=1}^7=\begin{pmatrix}0&0&3/10&3/10&1/10&1/10&1/5\\0&0&\ast&\ast&3/40&3/40&3/20\\0&0&\ast&\ast&0&0&0\\0&0&\ast&\ast&0&0&0\\0&0&0&0&1/4&1/4&1/2\\0&0&0&0&1/4&1/4&1/2\\0&0&0&0&1/4&1/4&1/2\end{pmatrix}.}
$$

The class classification is **$T$: transient, period $2$; $B$: recurrent, period $2$; $C$: recurrent, period $1$**.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
