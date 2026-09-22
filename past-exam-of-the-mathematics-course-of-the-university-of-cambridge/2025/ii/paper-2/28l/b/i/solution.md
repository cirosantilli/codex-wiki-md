<h1 id="28l/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**False.** Let the jump-chain state space be $\mathbb Z_+$, with

$$
p_{0i}=2^{-i}\quad(i\geq1),
\qquad
p_{i0}=1\quad(i\geq1).
$$

It is irreducible and has invariant distribution

$$
\mu_0=\frac12,
\qquad
\mu_i=2^{-(i+1)}\quad(i\geq1),
$$

so it is positive recurrent.

Give the continuous-time chain holding rates

$$
q_0=1,\qquad q_i=2^{-i}quad(i\geq1),
$$

and set $q_{ij}=q_ip_{ij}$. The rates are bounded, so the chain is nonexplosive. A return cycle from zero jumps to $i$ with probability $2^{-i}$ and then has mean holding time $2^i$ there. Consequently its mean return time is at least

$$
\sum_{i\geq1}2^{-i}2^i=\infty.
$$

Thus the continuous-time chain is not positive recurrent.

Equivalently, the jump-chain invariant distribution would induce the continuous-time invariant measure $\mu_i/q_i$, but this has infinite total mass.

## ↑ Ancestors (12)

1. [I](../i.md)
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
