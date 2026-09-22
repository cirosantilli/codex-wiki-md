<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An error implies that some $\theta\ne\theta^*$ has likelihood at least that of $\theta^*$. A finite [union bound](../../../../../../boole-s-inequality.md) and part (b) therefore give

$$
\limsup_{n\to\infty}\frac1n\log
\mathbb P(\widehat\theta_n\ne\theta^*)
\leq-C^*(\Theta),
$$

where

$$
C^*(\Theta)=
\min_{\theta\ne\theta^*}
\inf_{R:\,D(R\Vert P_{\theta^*})\geq D(R\Vert P_\theta)}
D_e(R\Vert P_{\theta^*}).
$$

Every inner infimum is strictly positive by the argument in part (b), and the minimum of finitely many positive numbers is positive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
