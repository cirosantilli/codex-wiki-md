<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

It suffices by part a to treat a nondecreasing right-continuous integrator, whose increments define a finite Lebesgue–Stieltjes measure $\mu_f$ on $[0,1]$. Let $\alpha_n$ be the left-endpoint step approximation on the dyadic intervals. The displayed sum is exactly

$$
\int_{(0,1]}\alpha_n\,d\mu_f.
$$

The [continuous function](../../../../../../continuous-function.md) $\alpha$ is uniformly continuous on the compact interval, so $\|\alpha_n-\alpha\|_\infty\to0$. Therefore

$$
\left|\int(\alpha_n-\alpha)\,df\right|
\leq\|\alpha_n-\alpha\|_\infty V(1)\longrightarrow0.
$$

Apply this separately to $g$ and $h$ to obtain the asserted [Lebesgue-Stieltjes integral](../../../../../../lebesgue-stieltjes-integration.md) limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
