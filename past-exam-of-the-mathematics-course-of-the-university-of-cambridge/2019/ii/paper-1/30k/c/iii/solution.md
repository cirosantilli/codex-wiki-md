<h1 id="30k/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume (iii). Fix $n\geq0$ and $A\in\mathcal F_n$, and define

$$
T=n\mathbf1_A+(n+1)\mathbf1_{A^c}.
$$

This is a [stopping time](../../../../../../../stopping-time.md): $\{T\leq n\}=A\in\mathcal F_n$. Applying (iii) at time $n+1$ first to $T$ and then to the deterministic stopping time $n+1$ gives

$$
\mathbb E[\mathbf1_AM_n+\mathbf1_{A^c}M_{n+1}]
=\mathbb E[M_0]
=\mathbb E[M_{n+1}].
$$

Subtracting yields

$$
\mathbb E[\mathbf1_A(M_{n+1}-M_n)]=0
\qquad(A\in\mathcal F_n).
$$

By the defining characterization of [conditional expectation](../../../../../../../conditional-expectation.md), this says $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$. Thus $M$ is a martingale, proving (i). Together the three implications establish the [characterization of a martingale by stopped expectations](../../../../../../../characterization-of-a-martingale-by-stopped-expectations.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [30K](../../../30k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
