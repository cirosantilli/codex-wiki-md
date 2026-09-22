<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An irreducible continuous-time chain is recurrent when, after leaving any state, it returns there almost surely. Non-explosion ensures that returns of $X$ correspond exactly to returns of its embedded jump chain, so one is recurrent precisely when the other is.

The expected total occupation time of zero is

$$
\mathbb E_0\int_0^\infty\mathbf1_{\{X_t=0\}}dt
=\int_0^\infty p_{0,0}(t)dt.
$$

Each visit contributes an independent holding time of mean $1/q_0$. Thus this expectation is $(1/q_0)$ times the expected number of visits. If the integral is infinite, the jump chain has infinitely many expected visits; for an irreducible chain this is equivalent to recurrence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
