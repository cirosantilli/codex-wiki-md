<h1 id="30k/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume (i), and let $\tau$ be a [stopping time](../../../../../../../stopping-time.md). The increments of the [stopped process](../../../../../../../stopped-martingale-in-discrete-time.md) satisfy

$$
M_{(n+1)\wedge\tau}-M_{n\wedge\tau}
=\mathbf1_{\{\tau>n\}}(M_{n+1}-M_n).
$$

Because $\{\tau>n\}\in\mathcal F_n$, taking [conditional expectation](../../../../../../../conditional-expectation.md) given $\mathcal F_n$ makes the right-hand side zero. Integrability follows from

$$
M_{n\wedge\tau}=M_0+\sum_{k=1}^n\mathbf1_{\{\tau\geq k\}}(M_k-M_{k-1}),
$$

a finite sum of integrable random variables. Hence $M^\tau$ is a martingale, proving (ii).

## ↑ Ancestors (12)

1. [I](../i.md)
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
