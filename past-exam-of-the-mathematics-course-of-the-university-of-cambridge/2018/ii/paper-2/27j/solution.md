<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

For the finite state space $S$, the generator or [Q-matrix](../../../../../transition-rate-matrix.md) $G=(g_{ij})$ is defined by

$$
g_{ij}=\lim_{h\downarrow0}
\frac{\mathbb P_i(X_h=j)-\mathbf1_{\{i=j\}}}{h}.
$$

Its off-diagonal entries are nonnegative jump rates and $g_{ii}=-\sum_{j\ne i}g_{ij}$. The [transition semigroup of a continuous-time Markov chain](../../../../../transition-semigroup-of-a-continuous-time-markov-chain.md) is $P(t)=e^{tG}$.

An [invariant distribution of a continuous-time Markov chain](../../../../../invariant-distribution-of-a-continuous-time-markov-chain.md) is a probability row vector $\pi$ satisfying $\pi P(t)=\pi$ for every $t\geq0$. Differentiation at zero gives $\pi G=0$; conversely, $\pi G=0$ implies $\pi e^{tG}=\pi$. Thus

$$
\boxed{\pi\text{ is invariant}\Longleftrightarrow\pi G=0.}
$$

Invariant distributions need not be unique: each [closed communicating class](../../../../../closed-communicating-class.md) supports one, and their convex combinations are invariant. A finite irreducible chain has a unique invariant distribution.

Let $0=T_0<T_1<\cdots$ be the arrival times of the independent rate-$\lambda$ [Poisson process](../../../../../poisson-process.md). The increments $T_{n+1}-T_n$ are independent exponential variables of rate $\lambda$. Conditional on $Y_n=X_{T_n}=i$, the [Markov property](../../../../../markov-property.md), time homogeneity, and independence of the next increment give

$$
\begin{aligned}
\mathbb P(Y_{n+1}=j\mid Y_0,\ldots,Y_n)
&=\int_0^\infty\lambda e^{-\lambda t}P_{ij}(t)\,dt\\
&=(P_\lambda)_{ij}.
\end{aligned}
$$

Hence $(Y_n)$ is a discrete-time Markov chain. Its transition matrix is the [Poisson-sampled continuous-time Markov chain](../../../../../poisson-sampled-continuous-time-markov-chain.md) resolvent

$$
\boxed{P_\lambda
=\int_0^\infty\lambda e^{-\lambda t}e^{tG}\,dt
=\lambda(\lambda I-G)^{-1}.}
$$

If $\pi G=0$, then $\pi e^{tG}=\pi$ and integration gives $\pi P_\lambda=\pi$. Conversely, if a probability row vector $\nu$ satisfies $\nu P_\lambda=\nu$, multiplying

$$
\nu\lambda(\lambda I-G)^{-1}=\nu
$$

on the right by $\lambda I-G$ yields $\nu G=0$. Therefore the sampled chain and the original chain have **exactly the same invariant distributions**.

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
