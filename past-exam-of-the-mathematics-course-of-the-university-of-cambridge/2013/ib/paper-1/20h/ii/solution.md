<h1 id="20h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $T_i$ be the expected time to complete the specified directed transition, starting at $i$. This is a [transition-completion time in a Markov chain](../../../../../../transition-completion-time-in-a-markov-chain.md), rather than merely a first visit to $c$. First-step decomposition gives

$$
T_a=1+\tfrac35T_b+\tfrac25T_c,\qquad
T_b=1+\tfrac34T_a,\qquad
T_c=1+\tfrac23T_a+\tfrac13T_b.
$$

The missing $b\to c$ continuation in the middle equation represents successful completion, but its step is counted by the leading one. Substitution gives

$$
\boxed{T_a=128/11,\qquad T_b=107/11,\qquad T_c=12.}
$$

Thus the requested expectation from $a$ is $128/11$ steps.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
