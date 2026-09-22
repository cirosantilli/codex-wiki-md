<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the factorization $p(\theta,\mathcal D)=p(\theta\mid\mathcal D)p(\mathcal D)$ inside the [evidence lower bound](../../../../../evidence-lower-bound.md):

$$
\begin{aligned}
\mathcal L(\phi)&=\mathbb E_q\left[\log p(\mathcal D)+\log\frac{p(\theta\mid\mathcal D)}{q(\theta;\phi^2)}\right]\\
&=\log p(\mathcal D)-\operatorname{KL}\bigl(q(\theta;\phi^2)\Vert p(\theta\mid\mathcal D)\bigr).
\end{aligned}
$$

Hence

$$
\boxed{\log p(\mathcal D)=\mathcal L(\phi)+\mathcal J(\phi)}.
$$

The [marginal likelihood](../../../../../bayesian-model-evidence.md) is independent of the variational parameter $\phi$, so **maximizing the [evidence lower bound](../../../../../evidence-lower-bound.md) is equivalent to minimizing the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md)**. Nonnegativity of the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) also gives $\mathcal L(\phi)\leq\log p(\mathcal D)$.

## ↑ Ancestors (13)

1. [I](../i.md)
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
