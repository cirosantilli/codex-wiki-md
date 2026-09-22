<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose a numéraire strategy $\eta$ existed and write $N_t=\eta_{t+1}\cdot P_t=\eta_t\cdot P_t>0$, using zero consumption. Since $\eta_{t+1}$ is $\mathcal F_t$-measurable and $M_t=(-1)^tZ_tP_t$ is a martingale,

$$
\mathbb E[\eta_{t+1}\cdot M_{t+1}\mid\mathcal F_t]
=\eta_{t+1}\cdot M_t.
$$

Thus

$$
-(-1)^t\mathbb E[Z_{t+1}N_{t+1}\mid\mathcal F_t]
=(-1)^tZ_tN_t,
$$

or

$$
\mathbb E[Z_{t+1}N_{t+1}\mid\mathcal F_t]
=-Z_tN_t.
$$

The left side is nonnegative and the right side nonpositive, so $Z_tN_t=0$ almost surely. Strict positivity of $N_t$ implies $Z_t=0$ almost surely for every $t$, contradicting

$$
\mathbb P(Z_t=0\text{ for all }t)=0.
$$

Therefore **the market has no numéraire strategy**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
