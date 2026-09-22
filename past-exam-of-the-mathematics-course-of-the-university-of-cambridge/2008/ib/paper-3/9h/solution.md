<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

A state of a [Markov chain](../../../../../markov-chain.md) is a [recurrent state](../../../../../recurrent-state.md) if, starting there, the first strictly positive return time is finite with probability one. A [recurrent Markov chain](../../../../../recurrent-markov-chain.md) has every state recurrent; in an [irreducible Markov chain](../../../../../irreducible-markov-chain.md) recurrence is a class property. Use the [recurrence criterion by return probabilities](../../../../../recurrence-criterion-by-return-probabilities.md): a state $i$ is recurrent if and only if $\sum_{n\ge0}p_{ii}^{(n)}=\infty$. To see the criterion, this sum is the expected number of visits including the initial one. If the return probability is $r<1$, the [Strong Markov property](../../../../../strong-markov-property.md) makes the number of successive returns geometric and its expected total is $1/(1-r)$. If $r=1$, every fixed number of returns occurs with probability one, so the expectation is infinite.

For the symmetric [simple random walk](../../../../../simple-random-walk.md) on the integers, odd-time return probabilities vanish, while

$$
p_{00}^{(2n)}=\binom{2n}{n}2^{-2n}.
$$

By [Stirling's formula](../../../../../stirling-formula.md), $\binom{2n}{n}\sim4^n/\sqrt{\pi n}$. Hence $p_{00}^{(2n)}\sim1/\sqrt{\pi n}$, whose sum diverges. The return-probability criterion proves recurrence of zero. Translation invariance gives the same result at every integer, or one can use irreducibility. Thus

$$
\boxed{\text{the symmetric simple random walk on }\mathbb Z\text{ is recurrent}.}
$$

This proof establishes almost-sure return, not a finite expected return time; every state of the walk is in fact a [null recurrent state](../../../../../null-recurrent-state.md).

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
