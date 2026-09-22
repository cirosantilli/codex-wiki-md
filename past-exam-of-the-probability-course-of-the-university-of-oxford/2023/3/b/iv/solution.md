<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Every step changes the population by one, so $X_n$ has the parity of $n$ when $X_0=0$. Hence $\mathbb P(X_{2m+1}=0)=0$. A return in two steps has positive [probability](../../../../../probability.md) from every state, and all return times are even, so the [period of a state in a Markov chain](../../../../../period-of-a-state-in-a-markov-chain.md) is exactly two.

Each transition exchanges the even and odd classes. Since $\pi$ is an [invariant distribution](../../../../../stationary-distribution.md), their masses are equal: $\pi(\text{even})=\pi(\text{odd})=1/2$. The chain sampled at times $2m$, restricted to the even states, is irreducible and positive recurrent, and it is aperiodic because its diagonal entries are positive. Its [stationary distribution](../../../../../stationary-distribution.md) is $2\pi_k$ on even $k$. The [countable-state Markov chain convergence theorem](../../../../../countable-state-markov-chain-convergence-theorem.md) applied to this sampled chain yields

$$
\boxed{\mathbb P(X_{2m}=0)\longrightarrow2\pi_0=(1-r)^{a+1},\qquad \mathbb P(X_{2m+1}=0)=0.}
$$

Since $\pi_0>0$, the full sequence has no limit. Its time average nevertheless tends to $\pi_0$ by the [countable-state Markov chain ergodic theorem](../../../../../countable-state-markov-chain-ergodic-theorem.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
