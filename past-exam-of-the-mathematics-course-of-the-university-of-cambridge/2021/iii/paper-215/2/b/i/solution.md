<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\Pi_n(x,y)=\pi_n(y)$. Since $P_n\Pi_n=\Pi_nP_n=\Pi_n$ and $\Pi_n^2=\Pi_n$, the [stationary-reset perturbation of a Markov chain](../../../../../../../stationary-reset-perturbation-of-a-markov-chain.md) satisfies

$$
\widetilde P_n^t
=\Pi_n+(1-a_n)^t(P_n^t-\Pi_n).
$$

Every row difference from stationarity is multiplied by the nonnegative scalar $(1-a_n)^t$, so

$$
\boxed{
\lVert\widetilde P_n^t(x,\mathord\cdot)-\pi_n\rVert_{\mathrm{TV}}
=(1-a_n)^t
\lVert P_n^t(x,\mathord\cdot)-\pi_n\rVert_{\mathrm{TV}}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 215](../../../../paper-215-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
