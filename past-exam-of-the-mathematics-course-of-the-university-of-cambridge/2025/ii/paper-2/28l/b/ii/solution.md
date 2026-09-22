<h1 id="28l/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This statement is also false. Let the jump chain be simple symmetric random walk on $\mathbb Z$, which is null recurrent, and choose holding rates

$$
q_i=(1+|i|)^2.
$$

Thus $q_{i,i+1}=q_{i,i-1}=q_i/2$. The counting measure $\mu_i=1$ is invariant for the jump chain, so

$$
\pi_i=\frac{C}{(1+|i|)^2}
$$

is an invariant distribution for the continuous-time chain, where $C$ is the normalizing constant.

The chain is nonexplosive: its jump chain returns to zero infinitely often, and the independent holding times on those visits have rate $q_0=1$, so their sum diverges almost surely. For an irreducible nonexplosive continuous-time chain, existence of an invariant distribution is equivalent to positive recurrence. Hence $X$ is positive recurrent although its jump chain is null recurrent.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [28L](../../../28l.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
