<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conditional on $R_k=r$, urn 1 has $r$ red and $n-r$ blue balls, while urn 2 has $n-r$ red and $r$ blue balls. The independent selections therefore give

$$
\boxed{\begin{aligned}
\mathbb P(R_{k+1}=r+1\mid R_k=r)&=(n-r)^2/n^2,\\
\mathbb P(R_{k+1}=r-1\mid R_k=r)&=r^2/n^2,\\
\mathbb P(R_{k+1}=r\mid R_k=r)&=2r(n-r)/n^2.
\end{aligned}}
$$

Every other conditional probability is zero. The out-of-range terms at $r=0$ or $r=n$ already have zero probability. These are the transition probabilities of the [Bernoulli-Laplace diffusion model](../../../../../../../bernoulli-laplace-diffusion-model.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
