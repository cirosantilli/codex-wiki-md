<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Markov chain](../../../../../../markov-chain.md) is [irreducible](../../../../../../irreducible-representation.md) if every state can reach every other state in finitely many steps with positive probability. It is a [recurrent Markov chain](../../../../../../recurrent-markov-chain.md) if, starting at any state, it returns to that state with probability one; for an irreducible chain this property is shared by all states.

For the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) on $\mathbb Z$, taking $|j-i|$ steps all in the appropriate direction reaches $j$ from $i$ with probability $2^{-|j-i|}>0$. Thus the chain is irreducible. Its return probabilities are

$$
p_{00}^{(2k)}=\binom{2k}{k}2^{-2k},\qquad p_{00}^{(2k+1)}=0.
$$

By [Stirling formula](../../../../../../stirling-formula.md), $p_{00}^{(2k)}\sim1/\sqrt{\pi k}$, so their sum diverges. The standard recurrence criterion $\sum_{n\geq0}p_{00}^{(n)}=\infty$ therefore proves **the walk is recurrent**.

The printed hint's constant is erroneous: the actual limit of $\sqrt{k}\,p_{00}^{(2k)}$ is $1/\sqrt\pi$. Its positivity is what the recurrence argument requires, but the reciprocal is necessary for the correct numerical value.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
