<h1 id="24k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [birth-death chain](../../../../../../birth-death-chain.md) on $\mathbb N_0$ has generator entries $q_{n,n+1}=\lambda_n$, $q_{n,n-1}=\mu_n$ for $n\geq1$, $\mu_0=0$, $q_{nn}=-(\lambda_n+\mu_n)$, and zero elsewhere. Assume the usual conservative nonexplosive chain. The [detailed balance for a birth-death process](../../../../../../detailed-balance-for-a-birth-death-process.md) are $\pi_n\lambda_n=\pi_{n+1}\mu_{n+1}$.

If they hold, each incoming term cancels an outgoing term, giving $\pi Q=0$ and thus invariance. Conversely the invariance equation at zero gives $\pi_0\lambda_0=\pi_1\mu_1$. At state $n$, write the stationarity equation as equality of the neighbouring probability currents

$$
\pi_{n-1}\lambda_{n-1}-\pi_n\mu_n
=\pi_n\lambda_n-\pi_{n+1}\mu_{n+1}.
$$

Induction from the zero boundary current gives [detailed balance for a birth-death process](../../../../../../detailed-balance-for-a-birth-death-process.md) for every edge. Thus **invariant measures are exactly the detailed-balance measures** in this standard birth–death setting. The argument is the generator characterization; a stationary probability law additionally needs finite normalization. For potentially explosive processes, formal generator balance alone would require additional boundary qualifications.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24K](../../24k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
