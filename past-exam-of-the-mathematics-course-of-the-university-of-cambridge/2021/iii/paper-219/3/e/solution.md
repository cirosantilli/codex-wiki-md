<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Up to normalization, the joint posterior is

$$
p(M_{1:N},M_0,\tau^2\mid D)
\propto(\tau^2)^k
\prod_{s=1}^N
\exp\left[-\frac{(D_s-M_s)^2}{2\sigma^2}
-\frac{(M_s-M_0)^2}{2\tau^2}\right](\tau^2)^{-N/2}.
$$

A [Gibbs sampler](../../../../../../gibbs-sampler.md) cycle consists of:

- independently draw every $M_s$ from the normal conditional in part a;
- draw $M_0\mid M_{1:N},\tau^2\sim N(\bar M,\tau^2/N)$;
- draw$$
  \tau^2\mid M_{1:N},M_0
  \sim\operatorname{Inv\text{-}Gamma}\left(
  \frac N2-k-1,\frac12\sum_s(M_s-M_0)^2\right).
  $$

Each proposal is the exact full conditional and is therefore accepted. If the cycle begins with density $p(\theta^t\mid D)$, integrating the product of the current posterior and successive conditional kernels over all overwritten coordinates leaves

$$
p(\theta^{t+1}\mid D),
$$

so a full Gibbs sweep preserves the joint posterior.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
