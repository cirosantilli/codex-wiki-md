<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The independent coordinates make the logarithm of the [probability density](../../../../../probability-density.md) ratio a sum. For coordinate $i$, its contribution to the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) is

$$
\mathbb E_q\left[\log\frac{\sigma_i}{\phi}-\frac{\theta_i^2}{2\phi^2}+\frac{\theta_i^2}{2\sigma_i^2}\right]=\log\frac{\sigma_i}{\phi}-\frac12+\frac{\phi^2}{2\sigma_i^2},
$$

because $\mathbb E_q\theta_i^2=\phi^2$. Thus, retaining all constants,

$$
\boxed{\mathcal J(\phi)=\frac{\phi^2}{2}\left(\frac1{\sigma_1^2}+\frac1{\sigma_2^2}\right)-1+\log\frac{\sigma_1\sigma_2}{\phi^2}}.
$$

Here $\sigma_1,\sigma_2>0$ and $\phi>0$, so both [normal densities](../../../../../normal-density.md) are nondegenerate.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
