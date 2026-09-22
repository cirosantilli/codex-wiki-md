<h1 id="28j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<j_1<\cdots<j_n<t$, the probability of one jump in each infinitesimal interval around $j_1,\ldots,j_n$ and no other jump by time $t$ gives the joint density

$$
\lambda^n e^{-\lambda t}
$$

for $(J_1,ldots,J_n)$ together with the event $N_t=n$. Since

$$
\mathbb P(N_t=n)=e^{-\lambda t}\frac{(\lambda t)^n}{n!},
$$

the conditional density is

$$
\frac{\lambda^ne^{-\lambda t}}
{e^{-\lambda t}(\lambda t)^n/n!}
=\frac{n!}{t^n}
$$

on that ordered simplex.

Now $n$ independent [uniform](../../../../../../continuous-uniform-distribution.md) points on $[0,t]$ have joint density $t^{-n}$ on the cube. Each ordered vector has $n!$ permutations, so their [order statistics](../../../../../../order-statistic.md) have density $n!/t^n$ on the same simplex. The densities agree, proving [Poisson process conditional arrival times](../../../../../../poisson-process-conditional-arrival-times.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
