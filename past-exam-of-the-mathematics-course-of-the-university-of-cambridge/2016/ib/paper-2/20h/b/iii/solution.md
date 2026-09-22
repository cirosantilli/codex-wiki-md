<h1 id="20h/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The only [closed communicating class](../../../../../../../closed-communicating-class.md) is $\{b,d\}$; the class $\{a,c\}$ is open and transient. Its one-step probability of staying inside is at most $2/3$, so if $\tau$ is the entrance time into $\{b,d\}$, then $\mathbb P(\tau>n)\le(2/3)^n$ for an initial state in $\{a,c\}$. Hence entrance occurs almost surely in finite time.

On $\{b,d\}$ it is an irreducible [aperiodic Markov chain](../../../../../../../aperiodic-markov-chain.md), because both states have positive self-loop probabilities. The finite irreducible aperiodic [countable-state Markov chain convergence theorem](../../../../../../../countable-state-markov-chain-convergence-theorem.md) says that its transition probabilities converge to its unique [stationary distribution](../../../../../../../stationary-distribution.md). The balance equation $\pi_b(3/4)=\pi_d(2/3)$ with $\pi_b+\pi_d=1$ gives $\pi_b=8/17$ and $\pi_d=9/17$.

This limit also holds from $a,c$: condition on the finite entrance time and entrance state. For $\tau\le M$, convergence in the closed class applies to a finite sum; the remaining probability is bounded by $\mathbb P(\tau>M)$, which tends to zero as $M\to\infty$. Thus **in the order $a,b,c,d$**,

$$
\boxed{\lim_{n\to\infty}P^n=
\begin{pmatrix}
0&8/17&0&9/17\\
0&8/17&0&9/17\\
0&8/17&0&9/17\\
0&8/17&0&9/17
\end{pmatrix}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [20H](../../../20h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
