<h1 id="n/n1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [stationary distribution](../../../../../stationary-distribution.md) is a nonnegative row vector $\pi$ with $\pi P=\pi$ and $\sum_i\pi_i=1$. The balance equations give

$$
\pi_1=\tfrac12\pi_1+\tfrac12\pi_4,\quad
\pi_2=\tfrac12\pi_3+\tfrac14\pi_4,\quad
\pi_3=\pi_2+\tfrac14\pi_4,\quad
\pi_4=\tfrac12\pi_1+\tfrac12\pi_3.
$$

The first yields $\pi_1=\pi_4$. Substitution into the middle pair yields $\pi_2=3\pi_4/4$ and $\pi_3=\pi_4$; the fourth equation is then satisfied. Normalization gives $15\pi_4/4=1$, hence

$$
\boxed{\pi=(4,3,4,4)/15}.
$$

All states communicate, so this is the unique [stationary distribution](../../../../../stationary-distribution.md). The self-loop at state 1 additionally makes this finite [Markov chain](../../../../../markov-chain-split.md) aperiodic, although aperiodicity is not required for the balance calculation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [N1](../../n1.md)
3. [N](../../../n.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
