<h1 id="6/i/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Fix any configurations $s$ and $s'$. List the sites where they differ and update those sites in turn to their target signs. Every specified site has positive probability $1/K^2$ of being selected. At every intermediate configuration, both values of its [full conditional distribution](../../../../../../../full-conditional-distribution.md) have positive probability, since all weights $w_i(\pm1)$ are finite and strictly positive. The finite prescribed sequence therefore has positive probability and reaches $s'$.

Thus **every configuration is accessible from every other configuration**, so the sampler is an [irreducible Markov chain](../../../../../../../irreducible-markov-chain.md), or equivalently [phi-irreducible](../../../../../../../phi-irreducibility.md) with counting measure. If $s=s'$, a single update that keeps its selected spin unchanged also has positive probability. This simultaneously proves positive self-transition probability and [aperiodicity](../../../../../../../aperiodic-markov-chain.md), including $K=1$. The sign of finite $J$ does not alter the accessibility argument.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [I](../../i.md)
3. [6](../../../6.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
